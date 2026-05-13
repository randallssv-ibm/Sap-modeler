---
name: sap-data-modeler
description: >
  Data modeler assistant for Databricks architects working with SAP sources (ECC and S/4HANA).
  Use this skill to: parse SAP CSN/CDS data product JSON files and extract technical field metadata,
  resolve ABAP technical names to business-readable labels, map SAP source entities to Databricks
  domain model targets, design FP&A-oriented finance data models (GL, CO, cost center hierarchies,
  profit center reporting, ledger/currency), trace cross-entity joins and key relationships,
  identify reporting grain for journal entries, billing, sales orders, and purchase orders,
  generate Delta Lake DDL or dbt models from SAP source patterns, handle ECC-to-S4 field mapping
  differences, and apply VDM/CDS annotation patterns to understand field semantics.
  Always trigger when user mentions: SAP, ECC, S/4HANA, CDS, CSN, ABAP, BKPF, BSEG, ACDOCA,
  journal entry, GL line item, cost center, profit center, controlling area, ledger, FP&A,
  financial planning, data product JSON, technical field names, SAP metadata.
---

# SAP Data Modeler — Databricks FP&A Assistant

A domain modeling assistant for Databricks architects ingesting SAP ECC or S/4HANA data.
The core workflow: **parse SAP CSN/CDS metadata → resolve technical names → design finance domain model → generate Databricks-ready DDL or dbt models**.

Primary focus: FP&A (Financial Planning & Analysis) — GL actuals, cost center/profit center reporting, ledger/currency handling, and CO hierarchies.

---

## Core Workflow

```
SAP Source (ECC or S4)
  │
  ├─ ECC:  Raw ABAP tables (BKPF, BSEG, EKKO, EKPO, KNA1, LFA1, MARA, ...)
  └─ S4:   CSN/CDS Data Products (JSON) — structured virtual data models
              │
              ▼
        CSN Metadata Parsing
        - Extract entity definitions, field names, data types
        - Resolve ABAP technical names → business labels (via @EndUserText.label)
        - Identify keys, associations, and grain
              │
              ▼
        Finance Domain Model (Databricks / Delta Lake)
        - Bronze: raw SAP fields, technical names preserved
        - Silver: decoded, joined, currency-normalized, hierarchy-enriched
        - Gold:   FP&A-ready aggregates (P&L, cost center actuals, variance)
```

---

## CSN File Anatomy

SAP data products are distributed as `.json` files in CSN (Core Schema Notation) format:

```json
{
  "$version": "2.0",
  "definitions": {
    "EntityName": {
      "kind": "entity",
      "@VDM.viewType": "BASIC",
      "@Analytics.dataCategory": "FACT",
      "elements": {
        "FieldName": {
          "type": "cds.String",
          "length": 4,
          "@EndUserText.label": "Company Code",
          "@ObjectModel.foreignKey.association": "_CompanyCode",
          "key": true
        },
        "_CompanyCode": {
          "type": "cds.Association",
          "target": "CompanyCode",
          "keys": [{ "ref": ["CompanyCode"] }]
        }
      }
    }
  }
}
```

### Parsing Rules
| CSN property | What it tells you |
|---|---|
| `"key": true` | Part of the entity's primary key |
| `"type": "cds.Association"` | Not a column — a navigation path; use `.target` for join target |
| `@EndUserText.label` | Business-readable field label — use for column aliases in domain model |
| `@VDM.viewType` | `BASIC` = source, `COMPOSITE` = joined/enriched, `CONSUMPTION` = report-ready |
| `@Analytics.dataCategory` | `FACT`, `DIMENSION`, `HIERARCHY` — maps to medallion layer role |
| `@ObjectModel.foreignKey.association` | Which association resolves this FK field |
| `@Semantics.amount.currencyCode` | Paired currency field for this amount |
| `@Semantics.quantity.unitOfMeasure` | Paired UoM field for this quantity |

---

## ECC vs S/4HANA Source Mapping

### GL Actuals — The Core FP&A Fact

| Layer | ECC Table | S/4HANA CDS Entity | Notes |
|---|---|---|---|
| Document header | `BKPF` | `JournalEntry` | CompanyCode + FiscalYear + AccountingDocument |
| Line item | `BSEG` | `GeneralLedgerAccountLineItem` | + SourceLedger + LedgerGLLineItem |
| Universal journal | — | `ACDOCA` (raw) / `GeneralLedgerAccountLineItem` (CDS) | S4 only — replaces BKPF+BSEG |

**Key difference**: In ECC, BKPF+BSEG are separate; in S/4, ACDOCA is the single universal journal. The CDS layer normalizes both into `GeneralLedgerAccountLineItem`.

### Other Key Table Mappings

| Domain | ECC | S/4HANA CDS Entity |
|---|---|---|
| Cost Center master | `CSKS` | `CostCenter` |
| Profit Center master | `CEPC` | `ProfitCenter` |
| GL Account master | `SKA1` / `SKAT` | `GeneralLedgerAccount` |
| Customer | `KNA1` + `KNB1` | `Customer` + `CustomerCompanyCode` |
| Supplier | `LFA1` + `LFB1` | `Supplier` + `SupplierCompanyCode` |
| Material/Product | `MARA` + `MARC` | `Product` + `ProductPlant` |
| Purchase Order | `EKKO` + `EKPO` | `PurchaseOrder` + `PurchaseOrderItem` |
| Sales Order | `VBAK` + `VBAP` | `SalesOrder` + `SalesOrderItem` |
| Billing | `VBRK` + `VBRP` | `BillingDocument` + `BillingDocumentItem` |
| CO-PA line items | `CE1xxxx` / `ACDOCA` | `GeneralLedgerAccountLineItem` (CO fields) |

---

## Finance Domain Model — FP&A Target Design

### Medallion Layer Responsibilities

```
Bronze (raw)
  - 1:1 with SAP source fields; preserve ABAP technical names
  - Add ingestion metadata: _source_system, _extracted_at, _sap_client
  - No transformations; partitioned by FiscalYear

Silver (conformed)
  - Decode technical names using @EndUserText.label aliases
  - Resolve FKs: join master data (CostCenter, ProfitCenter, GLAccount)
  - Normalize amounts to a single reporting currency (AmountInGlobalCurrency)
  - Apply time-dependency joins for master data validity
  - Explode multi-currency fields into canonical structure
  - Partition by FiscalYear + FiscalPeriod

Gold (FP&A-ready)
  - Aggregated by cost center hierarchy node / profit center / GL account group
  - Variance: Actual vs Plan (requires plan data join)
  - Period-to-date and year-to-date measures
  - Conformed dimensions shared across FI and CO
```

### Core FP&A Fact Table — GL Line Item Silver

Minimum field set for an FP&A GL fact table in Databricks:

```sql
CREATE TABLE silver.gl_line_item (
  -- Keys
  source_ledger         STRING,   -- SourceLedger       (0L = leading)
  company_code          STRING,   -- CompanyCode
  fiscal_year           STRING,   -- FiscalYear
  accounting_document   STRING,   -- AccountingDocument
  ledger_gl_line_item   STRING,   -- LedgerGLLineItem

  -- Posting context
  posting_date          DATE,     -- PostingDate
  fiscal_period         STRING,   -- FiscalPeriod (001–016)
  fiscal_year_period    STRING,   -- FiscalYearPeriod (YYYYPPP) — range predicates
  document_type         STRING,   -- AccountingDocumentType
  debit_credit_code     STRING,   -- DebitCreditCode (S=debit, H=credit)

  -- GL dimension
  gl_account            STRING,   -- GLAccount
  chart_of_accounts     STRING,   -- ChartOfAccounts

  -- CO dimensions
  controlling_area      STRING,   -- ControllingArea
  cost_center           STRING,   -- CostCenter
  profit_center         STRING,   -- ProfitCenter
  functional_area       STRING,   -- FunctionalArea
  wbs_element           STRING,   -- WBSElement

  -- SD/MM reference (nullable)
  sales_document        STRING,   -- SalesDocument
  purchasing_document   STRING,   -- PurchasingDocument
  customer              STRING,   -- Customer
  supplier              STRING,   -- Supplier

  -- Amounts — always carry all three; pick one for reporting
  amount_txn_currency   DECIMAL(23,2), -- AmountInTransactionCurrency
  transaction_currency  STRING,        -- TransactionCurrency
  amount_cc_currency    DECIMAL(23,2), -- AmountInCompanyCodeCurrency
  company_code_currency STRING,        -- CompanyCodeCurrency
  amount_global         DECIMAL(23,2), -- AmountInGlobalCurrency
  global_currency       STRING,        -- GlobalCurrency

  -- Metadata
  _source_system        STRING,
  _extracted_at         TIMESTAMP,
  _sap_client           STRING
)
PARTITIONED BY (fiscal_year, company_code);
```

---

## Key Modeling Patterns

### 1. Time-Dependent Master Data Join

CostCenter, ProfitCenter, and CostCenterActivityType are time-dependent (ValidityEndDate in key). Always join on posting date:

```sql
LEFT JOIN silver.cost_center cc
  ON gl.controlling_area = cc.controlling_area
  AND gl.cost_center = cc.cost_center
  AND gl.posting_date BETWEEN cc.validity_start_date AND cc.validity_end_date
```

### 2. Ledger Filter for FP&A

For standard FP&A reporting, always filter to the leading ledger:

```sql
WHERE source_ledger = '0L'   -- leading ledger (IFRS/local GAAP)
-- or join: AND ledger.is_leading_ledger = true
```

### 3. Hierarchy Rollup (Cost Center / Profit Center)

```sql
-- In Databricks, use recursive CTE or pre-expanded hierarchy table
WITH RECURSIVE hier AS (
  SELECT hierarchy_node, parent_node, cost_center, node_level, 0 AS depth
  FROM silver.cost_center_hierarchy_node
  WHERE controlling_area = :ca
    AND hierarchy_node = :root_node
  UNION ALL
  SELECT c.hierarchy_node, c.parent_node, c.cost_center, c.node_level, h.depth + 1
  FROM silver.cost_center_hierarchy_node c
  JOIN hier h ON c.parent_node = h.hierarchy_node
    AND c.controlling_area = :ca
)
SELECT h.hierarchy_node, SUM(gl.amount_global) AS total_amount
FROM gold.gl_actuals gl
JOIN hier h ON gl.cost_center = h.cost_center
GROUP BY h.hierarchy_node
```

For Databricks at scale: pre-explode hierarchies into an `ancestor_node` bridge table at Silver layer to avoid recursive CTEs on large fact tables.

### 4. Debit/Credit Sign Convention

SAP stores amounts as absolute values with a separate `DebitCreditCode` (S=debit, H=credit). For P&L reporting, apply sign:

```sql
CASE debit_credit_code
  WHEN 'S' THEN  amount_global         -- debit = positive expense
  WHEN 'H' THEN -amount_global         -- credit = negative / revenue
END AS signed_amount
```

### 5. Special Period Exclusion

Periods 013–016 are year-end adjustment periods. Exclude for operational FP&A:

```sql
WHERE CAST(fiscal_period AS INT) <= 12
```

### 6. ECC Field Name Alignment

When ingesting ECC tables directly (not via CDS), map ABAP technical names:

| ABAP Field | ABAP Table | CDS Name | Business Label |
|---|---|---|---|
| `BUKRS` | BKPF/BSEG | CompanyCode | Company Code |
| `GJAHR` | BKPF/BSEG | FiscalYear | Fiscal Year |
| `BELNR` | BKPF/BSEG | AccountingDocument | Accounting Document |
| `BUZEI` | BSEG | LedgerGLLineItem | Line Item |
| `BUDAT` | BKPF | PostingDate | Posting Date |
| `MONAT` | BKPF | FiscalPeriod | Fiscal Period |
| `HKONT` | BSEG | GLAccount | GL Account |
| `KOSTL` | BSEG | CostCenter | Cost Center |
| `PRCTR` | BSEG | ProfitCenter | Profit Center |
| `FKBER` | BSEG | FunctionalArea | Functional Area |
| `DMBTR` | BSEG | AmountInCompanyCodeCurrency | Amount (CC Curr) |
| `WRBTR` | BSEG | AmountInTransactionCurrency | Amount (Txn Curr) |
| `WAERS` | BKPF | TransactionCurrency | Currency |
| `SHKZG` | BSEG | DebitCreditCode | D/C Indicator |
| `LIFNR` | BSEG | Supplier | Vendor |
| `KUNNR` | BSEG | Customer | Customer |

---

## Reporting Grain Reference

| Entity / Table | Key | Grain | FP&A Use |
|---|---|---|---|
| `GeneralLedgerAccountLineItem` / BSEG+ACDOCA | Ledger+CC+FY+Doc+LineItem | One posting line | **Primary FP&A fact** |
| `JournalEntry` / BKPF | CC+FY+Doc | Document header | Header text, transaction type |
| `CostCenter` / CSKS | CA+CC+ValidityEnd | CC master per period | Cost center attributes |
| `ProfitCenter` / CEPC | CA+PC+ValidityEnd | PC master per period | Profit center attributes |
| `BillingDocumentItem` / VBRP | BillingDoc+Item | Revenue line | Operational revenue |
| `PurchaseOrderAccountAssignment` / EKKN | PO+Item+AcctAssign | Cost distribution | Commitment reporting |

---

## Data Product Catalog — 28 SAP S/4HANA Cloud Products

### Finance & Accounting (FI)
| Data Product | Core Entity | Key Fields | Grain |
|---|---|---|---|
| GeneralLedgerAccount | GeneralLedgerAccountLineItem | SourceLedger+CompanyCode+FiscalYear+AccountingDocument+LedgerGLLineItem | Lowest — one row per posting line |
| JournalEntryHeader | JournalEntry | CompanyCode+FiscalYear+AccountingDocument | Document header |
| GeneralLedgerAccount | GeneralLedgerAccount | ChartOfAccounts+GLAccount | GL master |
| ARBankStatement | ARBankStatement | BankStatementShortID | Bank statement |
| CashFlow | CashFlow | CashFlowID+ValidityStart | Cash position |
| FiscalYear | FiscalYear | FiscalYearVariant+FiscalYear | Period calendar |
| Ledger | Ledger | Ledger | Valuation view |
| FinancialTransaction | FinancialTransaction | CompanyCode+FinancialTransaction | Treasury instrument |

### Controlling (CO)
| Data Product | Core Entity | Key Fields | Notes |
|---|---|---|---|
| CostCenter | CostCenter | ControllingArea+CostCenter+ValidityEndDate | Time-dependent |
| ProfitCenter | ProfitCenter | ControllingArea+ProfitCenter+ValidityEndDate | Time-dependent |
| FunctionalArea | FunctionalArea | FunctionalArea | Cost-of-sales dim |
| CostCenterActivityType | CostCenterActivityType | ControllingArea+CostCtrActivityType+ValidityEndDate | Activity type |
| ControllingArea | ControllingArea | ControllingArea | CO org unit |
| CostOriginGroup | CostOriginGroup | ControllingArea+CostOriginType+CostOriginGroup | CO classification |

### Org Structure
| CompanyCode | CompanyCode | CompanyCode | Legal entity |
| Plant | Plant | Plant | Logistics unit |

### Sales & Billing (SD)
| SalesOrder | SalesOrder / SalesOrderItem | SalesOrder(+Item) | Order line |
| BillingDocument | BillingDocument / BillingDocumentItem | BillingDocument(+Item) | Revenue event |
| InvoiceList | InvoiceList / InvoiceListItem | InvoiceList(+Item) | Invoice grouping |

### Procurement (MM)
| PurchaseOrder | PurchaseOrder | PurchaseOrder | PO header |
| PurchaseOrder | PurchaseOrderItem | PO+Item | PO line |
| PurchaseOrder | PurchaseOrderAccountAssignment | PO+Item+AcctAssign | Cost distribution |

### Master Data
| Customer | Customer | Customer | 117 fields + children |
| Supplier | Supplier | Supplier | 135 fields + children |
| Product | Product | Product | 156 fields + children |

---

## Reference Files

Load these when field-level detail is needed:

- **`references/entity-field-catalog.md`** — Full field listing for all major entities
- **`references/type-primitives.md`** — ABAP type → CDS primitive resolution (~700 types)
- **`references/ecc-to-s4-field-map.md`** — ABAP technical name → CDS field name mapping
