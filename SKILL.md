---
name: Sap-modeler
description: >
  Data modeler assistant for Databricks architects building a finance domain model from SAP ECC sources,
  designed to migrate cleanly to S/4HANA without reworking the domain layer.
  Use this skill to: map ECC ABAP tables to a Databricks medallion model, resolve ABAP technical field names
  to business labels, design source-agnostic Silver/Gold layers that survive an ECC→S4 migration,
  parse SAP CSN/CDS data product JSON files for S4 readiness planning, identify reporting grain for
  GL, CO, SD, and MM domains, model cost center / profit center hierarchies, handle ledger and
  multi-currency normalization, generate Delta Lake DDL and dbt models, and map FP&A reporting
  requirements to SAP source fields.
  Always trigger when user mentions: SAP, ECC, S/4HANA, BKPF, BSEG, ACDOCA, CSKS, CEPC, SKA1,
  EKKO, EKPO, VBRK, VBRP, CDS, CSN, ABAP, journal entry, GL line item, cost center, profit center,
  controlling area, ledger, FP&A, financial planning, ABAP field names, SAP technical metadata,
  ECC migration, S4 migration.
---

# SAP Data Modeler — ECC-First, S/4HANA-Ready

A domain modeling assistant for Databricks architects ingesting **SAP ECC** data today, while designing for a clean **ECC → S/4HANA migration** tomorrow. The Silver/Gold domain model is source-agnostic: only the Bronze ingestion layer changes when the ERP upgrades.

Primary focus: **FP&A** — GL actuals, cost center/profit center reporting, CO hierarchies, multi-currency normalization.

---

## Design Principle: Source-Agnostic Domain Model

```
TODAY (ECC)                          TOMORROW (S/4HANA)
─────────────────────                ─────────────────────
BKPF + BSEG  ──┐                    ACDOCA / GeneralLedgerAccountLineItem ──┐
CSKS         ──┤  Bronze            CostCenter (CDS)                        ├── Bronze
CEPC         ──┤  (raw, source-     ProfitCenter (CDS)                      │   (raw, source-
SKA1/SKAT    ──┤   specific)        GeneralLedgerAccount (CDS)              │    specific)
EKKO/EKPO    ──┘                    PurchaseOrder (CDS)                     ┘
     │                                       │
     ▼                                       ▼
     ╔═══════════════════════════════════════════╗
     ║         SILVER — Conformed Domain         ║  ← never changes
     ║  gl_line_item, cost_center, profit_center ║
     ║  gl_account, vendor, customer, product    ║
     ╚═══════════════════════════════════════════╝
                        │
                        ▼
     ╔═══════════════════════════════════════════╗
     ║         GOLD — FP&A Layer                 ║  ← never changes
     ║  actuals_by_cost_center, p_and_l,         ║
     ║  variance_actual_vs_plan, ytd_summary     ║
     ╚═══════════════════════════════════════════╝
```

**Rule**: Business logic, joins, hierarchies, and aggregations live in Silver/Gold. Bronze is a thin landing zone. When ECC becomes S/4, only Bronze pipelines are rewritten.

---

## ECC Table Catalog — FP&A Focus

### FI — Financial Accounting

| ABAP Table | Description | Key Fields | Grain | Domain Model Target |
|---|---|---|---|---|
| `BKPF` | Accounting Document Header | MANDT+BUKRS+GJAHR+BELNR | 1 row per document | `silver.journal_entry_header` |
| `BSEG` | Accounting Document Line Item | +BUZEI | 1 row per line | `silver.gl_line_item` |
| `BSIS` | Open Items (GL) | BUKRS+HKONT+GJAHR+BELNR+BUZEI | Open GL items | Subset of `silver.gl_line_item` |
| `BSAS` | Cleared Items (GL) | Same | Cleared GL items | Subset of `silver.gl_line_item` |
| `SKA1` | GL Account Master (chart level) | KTOPL+SAKNR | 1 per GL account | `silver.gl_account` |
| `SKAT` | GL Account Texts | SPRAS+KTOPL+SAKNR | 1 per language | Join to `silver.gl_account` |
| `SKB1` | GL Account Master (company code) | BUKRS+SAKNR | 1 per CC+account | Join to `silver.gl_account` |
| `T001` | Company Codes | BUKRS | 1 per company code | `silver.company_code` |
| `T009` | Fiscal Year Variants | PERIV | 1 per variant | `silver.fiscal_year_variant` |
| `T009B` | Fiscal Year Period Definitions | PERIV+BUMON | 1 per period | `silver.fiscal_period` |

### CO — Controlling

| ABAP Table | Description | Key Fields | Grain | Domain Model Target |
|---|---|---|---|---|
| `CSKS` | Cost Center Master | MANDT+KOKRS+KOSTL+DATBI | Time-dependent | `silver.cost_center` |
| `CSKT` | Cost Center Texts | SPRAS+KOKRS+KOSTL+DATBI | Per language | Join to `silver.cost_center` |
| `CEPC` | Profit Center Master | MANDT+KOKRS+PRCTR+DATBI | Time-dependent | `silver.profit_center` |
| `CEPCT` | Profit Center Texts | SPRAS+KOKRS+PRCTR+DATBI | Per language | Join to `silver.profit_center` |
| `SETHEADER` | Hierarchy Set Header | SETCLASS+SUBCLASS+SETNAME | 1 per hierarchy | `silver.hierarchy` |
| `SETNODE` | Hierarchy Internal Nodes | SETCLASS+SUBCLASS+SETNAME+SUBSETNAME | Parent→child | `silver.hierarchy_node` |
| `SETLEAF` | Hierarchy Leaf Values | SETCLASS+SUBCLASS+SETNAME+FROM_VALUE | Leaf→value range | `silver.hierarchy_leaf` |
| `TKA01` | Controlling Areas | KOKRS | 1 per CO area | `silver.controlling_area` |
| `CSKA` | CO Cost Elements (chart) | KTOPL+KSTAR | 1 per cost element | `silver.cost_element` |
| `CSKB` | CO Cost Elements (CO area) | KOKRS+KSTAR+DATBI | Time-dependent | Join to `silver.cost_element` |

> **Note on ECC CO-PA**: Line-item CO-PA lives in `CE1xxxx` tables (client-specific). In S/4, this is unified into ACDOCA. Design Silver to absorb both.

### SD — Sales & Distribution

| ABAP Table | Description | Key Fields | Grain | Domain Model Target |
|---|---|---|---|---|
| `VBRK` | Billing Document Header | MANDT+VBELN | 1 per billing doc | `silver.billing_header` |
| `VBRP` | Billing Document Item | MANDT+VBELN+POSNR | 1 per item | `silver.billing_item` |
| `VBAK` | Sales Order Header | MANDT+VBELN | 1 per SO | `silver.sales_order_header` |
| `VBAP` | Sales Order Item | MANDT+VBELN+POSNR | 1 per item | `silver.sales_order_item` |
| `VBKD` | Sales Document Business Data | MANDT+VBELN+POSNR | Payment/incoterms per item | Join to `silver.sales_order_header` |
| `VEDA` | Contract Data | MANDT+VBELN+VPOSN | Contract validity/cancel dates | Join to `silver.sales_order_item` |

> **Revenue tracing**: The GL posting chain is VBRK.VBELN → BKPF.AWKEY (when BKPF.AWTYP='VBRK'). Use this join in Bronze to link billing docs to journal entries. VBRP.AUBEL/AUPOS traces back to the originating sales order (VBAK/VBAP).

### MM — Materials Management / Procurement

| ABAP Table | Description | Key Fields | Grain | Domain Model Target |
|---|---|---|---|---|
| `EKKO` | Purchase Order Header | MANDT+EBELN | 1 per PO | `silver.po_header` |
| `EKPO` | Purchase Order Item | MANDT+EBELN+EBELP | 1 per item | `silver.po_item` |
| `EKKN` | PO Account Assignment | MANDT+EBELN+EBELP+ZEKKN | Cost distribution | `silver.po_account_assignment` |

### Master Data

| ABAP Table | Description | Key Fields | Domain Model Target |
|---|---|---|---|
| `KNA1` | Customer Master (general) | MANDT+KUNNR | `silver.customer` |
| `KNB1` | Customer Master (company code) | MANDT+KUNNR+BUKRS | Join to `silver.customer` |
| `LFA1` | Vendor Master (general) | MANDT+LIFNR | `silver.supplier` |
| `LFB1` | Vendor Master (company code) | MANDT+LIFNR+BUKRS | Join to `silver.supplier` |
| `MARA` | Material Master (general) | MANDT+MATNR | `silver.product` |
| `MARC` | Material Master (plant) | MANDT+MATNR+WERKS | Join to `silver.product` |
| `MAKT` | Material Descriptions | MANDT+MATNR+SPRAS | Join to `silver.product` |

---

## ABAP Technical Name Reference — FP&A Fields

### BKPF — Document Header

| ABAP Field | Type | Business Name | Silver Column | Notes |
|---|---|---|---|---|
| `MANDT` | CLNT(3) | Client | _(filter, not stored)_ | Always filter = '100' or configured client |
| `BUKRS` | CHAR(4) | Company Code | `company_code` | FK → T001 |
| `GJAHR` | NUMC(4) | Fiscal Year | `fiscal_year` | |
| `BELNR` | CHAR(10) | Accounting Document Number | `accounting_document` | |
| `BLART` | CHAR(2) | Document Type | `document_type` | SA=GL, KR=vendor inv, DR=customer inv |
| `BUDAT` | DATS | Posting Date | `posting_date` | Use for period filtering |
| `BLDAT` | DATS | Document Date | `document_date` | Invoice date |
| `CPUDT` | DATS | Entry Date | `entry_date` | |
| `WAERS` | CUKY(5) | Currency Key | `transaction_currency` | |
| `KURSF` | DEC | Exchange Rate | `exchange_rate` | |
| `BKTXT` | CHAR(25) | Document Header Text | `document_text` | |
| `TCODE` | CHAR(20) | Transaction Code | `transaction_code` | FB01, F-02, VF01, etc. |
| `STBLG` | CHAR(10) | Reverse Document Number | `reversal_document` | Populated if reversed |
| `XBLNR` | CHAR(16) | Reference Document Number | `reference_document` | External reference |

### BSEG — Line Item

| ABAP Field | Type | Business Name | Silver Column | Notes |
|---|---|---|---|---|
| `BUZEI` | NUMC(3) | Line Item Number | `line_item` | |
| `HKONT` | CHAR(10) | GL Account | `gl_account` | FK → SKA1 |
| `KOSTL` | CHAR(10) | Cost Center | `cost_center` | FK → CSKS |
| `PRCTR` | CHAR(18) | Profit Center | `profit_center` | FK → CEPC |
| `FKBER` | CHAR(16) | Functional Area | `functional_area` | |
| `GSBER` | CHAR(4) | Business Area | `business_area` | |
| `KOKRS` | CHAR(4) | Controlling Area | `controlling_area` | FK → TKA01 |
| `DMBTR` | CURR | Amount in Company Code Currency | `amount_cc_currency` | Always populated |
| `WRBTR` | CURR | Amount in Transaction Currency | `amount_txn_currency` | |
| `SHKZG` | CHAR(1) | Debit/Credit Indicator | `debit_credit_code` | S=debit, H=credit |
| `MWSKZ` | CHAR(2) | Tax Code | `tax_code` | |
| `LIFNR` | CHAR(10) | Vendor | `supplier` | FK → LFA1 |
| `KUNNR` | CHAR(10) | Customer | `customer` | FK → KNA1 |
| `MATNR` | CHAR(18) | Material Number | `product` | FK → MARA |
| `WERKS` | CHAR(4) | Plant | `plant` | |
| `VBELN` | CHAR(10) | Sales/Billing Document | `sales_document` | |
| `AUBEL` | CHAR(10) | Sales Order | `sales_order` | |
| `EBELN` | CHAR(10) | Purchase Order | `purchasing_document` | |
| `EBELP` | NUMC(5) | PO Line Item | `purchasing_document_item` | |
| `ANLN1` | CHAR(12) | Main Asset Number | `asset_number` | |
| `AUFNR` | CHAR(12) | Internal Order | `internal_order` | |
| `PS_PSP_PNR` | NUMC(8) | WBS Element | `wbs_element` | |
| `ZUONR` | CHAR(18) | Assignment Field | `assignment` | Often used as reference |
| `SGTXT` | CHAR(50) | Item Text | `item_text` | |

### CSKS — Cost Center Master

| ABAP Field | Business Name | Silver Column | Notes |
|---|---|---|---|
| `KOKRS` | Controlling Area | `controlling_area` | |
| `KOSTL` | Cost Center | `cost_center` | |
| `DATBI` | Valid To Date | `validity_end_date` | Time-dependency key |
| `DATAB` | Valid From Date | `validity_start_date` | |
| `BUKRS` | Company Code | `company_code` | |
| `PRCTR` | Default Profit Center | `default_profit_center` | Not authoritative for postings |
| `KHINR` | Cost Center Hierarchy Area | `hierarchy_area` | Links to SETHEADER |
| `KOSAR` | Cost Center Category | `cost_center_category` | E=expense, I=investment |
| `VERAK` | Person Responsible | `responsible_person` | |
| `ABTEI` | Department | `department` | |

---

## ECC Hierarchy Model (SET Framework)

ECC cost center and profit center hierarchies use the SET framework — three tables:

```
SETHEADER (SETCLASS='0101' for CC, '0106' for PC)
  SETNAME = hierarchy name (= TKA01.KHINR for CC standard hierarchy)
  │
  ├── SETNODE (internal nodes — groups)
  │     SUBSETNAME = child set name
  │     Recursive: a SETNODE.SUBSETNAME → another SETHEADER.SETNAME
  │
  └── SETLEAF (leaf nodes — actual CC/PC values)
        FROM_VALUE, TO_VALUE = cost center range (often FROM=TO for single values)
```

### Flattening to Bridge Table (Silver)

```sql
-- Recursive CTE to flatten ECC SET hierarchy into ancestor bridge
WITH RECURSIVE hier AS (
  -- Anchor: top-level set
  SELECT
    h.SETNAME   AS root_node,
    h.SETNAME   AS node_name,
    h.SETNAME   AS ancestor_node,
    0           AS depth
  FROM SETHEADER h
  WHERE h.SETCLASS = '0101'
    AND h.SUBCLASS = :controlling_area
    AND h.SETNAME  = :root_hierarchy

  UNION ALL

  -- Internal nodes
  SELECT
    hier.root_node,
    n.SUBSETNAME  AS node_name,
    hier.node_name AS ancestor_node,
    hier.depth + 1
  FROM SETNODE n
  JOIN hier ON n.SETNAME = hier.node_name
    AND n.SETCLASS = '0101'
    AND n.SUBCLASS = :controlling_area
)
-- Join leaves to get cost center ranges
SELECT
  hier.root_node,
  hier.ancestor_node,
  hier.depth,
  l.FROM_VALUE AS cost_center_from,
  l.TO_VALUE   AS cost_center_to
FROM hier
JOIN SETLEAF l
  ON l.SETNAME   = hier.node_name
  AND l.SETCLASS = '0101'
  AND l.SUBCLASS = :controlling_area
```

Store the flattened result as `silver.cost_center_hierarchy_bridge` with columns:
`(controlling_area, hierarchy_name, ancestor_node, cost_center, depth)`

---

## Silver Layer DDL — Core FP&A Tables

### gl_line_item

```sql
CREATE TABLE silver.gl_line_item (
  -- Source metadata
  _source_system        STRING NOT NULL,   -- 'ECC' or 'S4'
  _sap_client           STRING NOT NULL,
  _extracted_at         TIMESTAMP NOT NULL,

  -- Document key (maps to BKPF+BSEG / ACDOCA)
  company_code          STRING NOT NULL,   -- BUKRS / CompanyCode
  fiscal_year           STRING NOT NULL,   -- GJAHR / FiscalYear
  accounting_document   STRING NOT NULL,   -- BELNR / AccountingDocument
  line_item             STRING NOT NULL,   -- BUZEI / LedgerGLLineItem
  source_ledger         STRING,            -- ECC: null/derived; S4: SourceLedger

  -- Posting context
  posting_date          DATE NOT NULL,     -- BUDAT / PostingDate
  document_date         DATE,             -- BLDAT / DocumentDate
  fiscal_period         STRING,           -- MONAT / FiscalPeriod (001–016)
  fiscal_year_period    STRING,           -- YYYYPPP — derived, for range predicates
  document_type         STRING,           -- BLART / AccountingDocumentType
  debit_credit_code     STRING,           -- SHKZG / DebitCreditCode (S/H)
  reference_document    STRING,           -- XBLNR / ReferenceDocument

  -- GL dimension
  gl_account            STRING,           -- HKONT / GLAccount
  chart_of_accounts     STRING,           -- derived from T001 / ChartOfAccounts

  -- CO dimensions
  controlling_area      STRING,           -- KOKRS / ControllingArea
  cost_center           STRING,           -- KOSTL / CostCenter
  profit_center         STRING,           -- PRCTR / ProfitCenter
  functional_area       STRING,           -- FKBER / FunctionalArea
  business_area         STRING,           -- GSBER / BusinessArea
  internal_order        STRING,           -- AUFNR / OrderID
  wbs_element           STRING,           -- PS_PSP_PNR / WBSElement

  -- Counterparty
  supplier              STRING,           -- LIFNR / Supplier
  customer              STRING,           -- KUNNR / Customer

  -- SD/MM reference (nullable)
  sales_document        STRING,           -- VBELN/AUBEL / SalesDocument
  purchasing_document   STRING,           -- EBELN / PurchasingDocument
  purchasing_doc_item   STRING,           -- EBELP / PurchasingDocumentItem

  -- Amounts — carry all; pick one for reporting
  amount_txn_currency   DECIMAL(23,2),   -- WRBTR / AmountInTransactionCurrency
  transaction_currency  STRING,          -- WAERS / TransactionCurrency
  amount_cc_currency    DECIMAL(23,2),   -- DMBTR / AmountInCompanyCodeCurrency
  company_code_currency STRING,          -- derived from T001

  -- ECC only (null in S4 — global currency handled differently)
  amount_global         DECIMAL(23,2),   -- derived or null until S4
  global_currency       STRING,

  -- Item detail
  item_text             STRING,          -- SGTXT / ItemText
  assignment            STRING           -- ZUONR / Assignment
)
USING DELTA
PARTITIONED BY (fiscal_year, company_code)
TBLPROPERTIES ('delta.autoOptimize.optimizeWrite' = 'true');
```

### cost_center

```sql
CREATE TABLE silver.cost_center (
  _source_system        STRING NOT NULL,
  controlling_area      STRING NOT NULL,   -- KOKRS / ControllingArea
  cost_center           STRING NOT NULL,   -- KOSTL / CostCenter
  validity_start_date   DATE NOT NULL,     -- DATAB / ValidityStartDate
  validity_end_date     DATE NOT NULL,     -- DATBI / ValidityEndDate
  company_code          STRING,            -- BUKRS / CompanyCode
  default_profit_center STRING,            -- PRCTR (default only — not authoritative for GL)
  cost_center_category  STRING,            -- KOSAR
  hierarchy_area        STRING,            -- KHINR → links to SET hierarchy
  department            STRING,            -- ABTEI
  responsible_person    STRING,            -- VERAK
  cost_center_name      STRING,            -- from CSKT
  _extracted_at         TIMESTAMP NOT NULL
)
USING DELTA;
```

---

## Key Modeling Patterns

### 1. Time-Dependent Master Data Join

```sql
-- Always join CC/PC on posting date, not latest record
LEFT JOIN silver.cost_center cc
  ON gl.controlling_area  = cc.controlling_area
 AND gl.cost_center       = cc.cost_center
 AND gl.posting_date BETWEEN cc.validity_start_date AND cc.validity_end_date
```

### 2. Debit/Credit Sign Normalization

SAP stores amounts as absolute values. Apply sign in Silver:

```sql
CASE debit_credit_code
  WHEN 'S' THEN  amount_cc_currency   -- debit  = positive
  WHEN 'H' THEN -amount_cc_currency   -- credit = negative
END AS signed_amount
```

For P&L: revenue GL accounts (credit-normal) flip sign again at Gold layer per account type.

### 3. Special Period Exclusion

Periods 013–016 are year-end adjustments. Exclude for operational FP&A:

```sql
WHERE CAST(fiscal_period AS INT) BETWEEN 1 AND 12
```

### 4. Client Filter

Always filter `MANDT = :client` in Bronze. Never store MANDT in Silver — it's infrastructure, not a business key.

### 5. Fiscal Period Derivation (ECC)

ECC stores fiscal period in `MONAT` (BKPF). Derive `fiscal_year_period` for range predicates:

```sql
CONCAT(gjahr, LPAD(monat, 3, '0')) AS fiscal_year_period  -- e.g. '2024003'
```

### 6. ECC Currency Gap

ECC BSEG carries only transaction currency (`WRBTR`) and company code currency (`DMBTR`). Global/group currency is **not** in BSEG — it requires a separate currency translation step or the `FAGLFLEXT` totals table. Design Silver with `amount_global` as nullable; populate via FX rate join or leave for S/4 migration.

---

## ECC → S/4HANA Migration Map

When the ERP upgrades, only Bronze changes. Silver column names are already aligned to S/4 CDS names:

| Silver Column | ECC Source (Bronze) | S/4 CDS Source (Bronze) |
|---|---|---|
| `company_code` | `BKPF.BUKRS` | `GeneralLedgerAccountLineItem.CompanyCode` |
| `fiscal_year` | `BKPF.GJAHR` | `.FiscalYear` |
| `accounting_document` | `BKPF.BELNR` | `.AccountingDocument` |
| `line_item` | `BSEG.BUZEI` | `.LedgerGLLineItem` |
| `source_ledger` | _(null / derived)_ | `.SourceLedger` |
| `posting_date` | `BKPF.BUDAT` | `.PostingDate` |
| `fiscal_period` | `BKPF.MONAT` | `.FiscalPeriod` |
| `document_type` | `BKPF.BLART` | `.AccountingDocumentType` |
| `debit_credit_code` | `BSEG.SHKZG` | `.DebitCreditCode` |
| `gl_account` | `BSEG.HKONT` | `.GLAccount` |
| `controlling_area` | `BSEG.KOKRS` | `.ControllingArea` |
| `cost_center` | `BSEG.KOSTL` | `.CostCenter` |
| `profit_center` | `BSEG.PRCTR` | `.ProfitCenter` |
| `functional_area` | `BSEG.FKBER` | `.FunctionalArea` |
| `supplier` | `BSEG.LIFNR` | `.Supplier` |
| `customer` | `BSEG.KUNNR` | `.Customer` |
| `amount_txn_currency` | `BSEG.WRBTR` | `.AmountInTransactionCurrency` |
| `transaction_currency` | `BKPF.WAERS` | `.TransactionCurrency` |
| `amount_cc_currency` | `BSEG.DMBTR` | `.AmountInCompanyCodeCurrency` |
| `amount_global` | _(FX-derived)_ | `.AmountInGlobalCurrency` |
| `cost_center` (master) | `CSKS.KOSTL` | `CostCenter.CostCenter` |
| `validity_start_date` | `CSKS.DATAB` | `CostCenter.ValidityStartDate` |
| `validity_end_date` | `CSKS.DATBI` | `CostCenter.ValidityEndDate` |
| `hierarchy_area` | `CSKS.KHINR` → SETHEADER | `CostCenterHierarchyNode` |

**Migration checklist for Silver**:
- [ ] Add `source_ledger` filter logic (S/4 requires `WHERE source_ledger = '0L'` for leading ledger)
- [ ] Populate `amount_global` natively (no FX derivation needed in S/4)
- [ ] Replace SET hierarchy tables with `CostCenterHierarchyNode` CDS entity
- [ ] Remove `MANDT` client filter (handled differently in CDS)
- [ ] Validate `fiscal_period` padding format matches (ECC: `MONAT` = '3', S/4: `FiscalPeriod` = '003')
- [ ] SD domain: GL link changes from BKPF.AWTYP='VBRK' / AWKEY lookup → `BillingDocument.AccountingDocument` field directly on the CDS entity
- [ ] SD domain: `VBRK.BELNR` (accounting document) is embedded in `BillingDocument` CDS — no separate GL join needed in S/4

---

## CSN/CDS Parsing — S/4 Readiness Planning

### Pre-parsed Reference — Use This First

The `csn-sources/` directory contains pre-parsed markdown for all 26 SAP data products. Each file provides the full ECC↔S/4 field mapping in a unified table:

```
| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC/S4 Diff |
```

**How to use csn-sources files**:
- **ECC Table + ECC Field** columns = the physical ABAP table.field to read from in ECC Bronze
- **ABAP Data Element** = the semantic type (use for field-level documentation and data dictionary lookup)
- **CDS Field** = the column name to use in Silver (pre-aligned to S/4 CDS field name)
- **ECC/S4 Diff** = flag rows needing special handling (padding, S/4-only fields, ledger filters)
- Rows where ECC Table/Field are blank = S/4-only fields; mark as `NULL` in ECC Bronze

Navigate by data product:

| Domain | File |
|---|---|
| GL — Line Item | [sap-s4com-GeneralLedgerAccount-v1.md](csn-sources/sap-s4com-GeneralLedgerAccount-v1.md) |
| GL — Journal Header | [sap-s4com-JournalEntryHeader-v1.md](csn-sources/sap-s4com-JournalEntryHeader-v1.md) |
| Cost Center | [sap-s4com-CostCenter-v1.md](csn-sources/sap-s4com-CostCenter-v1.md) |
| Profit Center | [sap-s4com-ProfitCenter-v1.md](csn-sources/sap-s4com-ProfitCenter-v1.md) |
| Billing | [sap-s4com-BillingDocument-v1.md](csn-sources/sap-s4com-BillingDocument-v1.md) |
| Sales Order | [sap-s4com-SalesOrder-v1.md](csn-sources/sap-s4com-SalesOrder-v1.md) |
| Purchase Order | [sap-s4com-PurchaseOrder-v1.md](csn-sources/sap-s4com-PurchaseOrder-v1.md) |
| Customer | [sap-s4com-Customer-v1.md](csn-sources/sap-s4com-Customer-v1.md) |
| Supplier | [sap-s4com-Supplier-v1.md](csn-sources/sap-s4com-Supplier-v1.md) |
| GL Account | [sap-s4com-GeneralLedgerAccount-v1.md](csn-sources/sap-s4com-GeneralLedgerAccount-v1.md) |

### Parsing Raw CSN JSON

When working directly with the JSON files (e.g. evaluating a new data product not yet in `csn-sources/`):

```python
import json

def parse_csn_entity(csn_path, entity_name):
    with open(csn_path) as f:
        csn = json.load(f)

    entity = csn["definitions"][entity_name]
    fields = []
    for fname, fdef in entity["elements"].items():
        if fdef.get("type") == "cds.Association":
            continue  # skip associations — not columns
        # The 'type' field is the ABAP data element name (semantic type)
        abap_data_element = fdef.get("type", "")
        fields.append({
            "cds_name":      fname,
            "abap_data_element": abap_data_element,  # e.g. FIS_BUKRS, FARP_BELNR_D
            "cds_type":      fdef.get("type"),
            "is_key":        fdef.get("key", False),
            "label":         fdef.get("@EndUserText.label", ""),
            "currency_ref":  fdef.get("@Semantics.amount.currencyCode", {}).get("="),
            "uom_ref":       fdef.get("@Semantics.quantity.unitOfMeasure", {}).get("="),
            "fk_assoc":      fdef.get("@ObjectModel.foreignKey.association", ""),
        })
    return fields
```

> **ABAP data element → physical field**: The `type` field in CSN is the ABAP data element (semantic name), **not** the physical table.field. To get the physical name: strip namespace prefixes (`FIS_`, `FARP_`, `FAC_`, `FINS_`, `FAGL_`) and suffixes (`_D`, `_ALPHA`, `_NO_CONV`). Then cross-reference with `references/ecc-to-s4-field-map.md` or the relevant `csn-sources/` file.

Key annotations to extract for domain modeling:

| Annotation | Meaning | Action |
|---|---|---|
| `@EndUserText.label` | Business field name | Use as Silver column alias |
| `"key": true` | Primary key field | Include in uniqueness check |
| `@Semantics.amount.currencyCode` | Paired currency field | Always carry currency alongside amount |
| `@Semantics.quantity.unitOfMeasure` | Paired UoM field | Always carry UoM alongside quantity |
| `@Analytics.dataCategory: "FACT"` | Fact entity | Maps to Silver fact table |
| `@Analytics.dataCategory: "DIMENSION"` | Dimension entity | Maps to Silver dimension table |
| `@VDM.viewType: "BASIC"` | Closest to source tables | Prefer for Bronze→Silver mapping |
| `@Analytics.dataExtraction.delta.changeDataCapture.mapping` | CDC source table | ECC table used for delta extraction (key fields only) |

---

## Reference Files

- **`csn-sources/`** — Pre-parsed S/4 data product field reference (26 files). Each file: full ECC Table.Field ↔ CDS Field mapping, ABAP data element, type, key flag, currency/UoM pairs, and ECC/S4 diff notes. **Start here when mapping a specific CDS entity to ECC Bronze.**
- **`references/ecc-table-field-catalog.md`** — Full field listing for BKPF, BSEG, CSKS, CEPC, SKA1, EKKO, EKPO, VBRK, VBRP, VBAK, VBAP, LFA1, KNA1
- **`references/ecc-to-s4-field-map.md`** — FP&A-focused ECC Table.Field → S/4 CDS field mapping with Bronze query patterns for GL, Cost Center, Profit Center, GL Account, Customer, Supplier, PO, Billing, and Sales Order
- **`references/gl-account-type-classification.md`** — GL account type codes (XBILK, GVTYP) and P&L sign convention for FP&A reporting
- **`references/document-type-reference.md`** — BLART document types, FP&A grouping logic, reversal detection, and origin tracing via AWTYP/AWKEY
