---
name: sap-data-modeler
description: >
  Use this skill whenever the user wants to work with SAP S/4HANA Cloud data products in CSN (Core Schema Notation) / CDS (Core Data Services) format.
  Triggers: reading/analyzing SAP data product JSON files, designing or extending SAP data models, mapping SAP entities to target schemas,
  generating SQL/DDL, understanding VDM annotations, tracing cross-entity joins, identifying data granularity for GL/CO/finance reporting,
  building cost center / profit center / functional area hierarchies, understanding journal entry fact tables, mapping source tables for ETL pipelines,
  identifying redundant or overlapping fields across data products, comparing SalesOrder vs BillingDocument vs InvoiceList granularity,
  working with PurchaseOrder account assignments, understanding ledger/currency multi-valuation, or any SAP entity/field/key question.
  Always use when user mentions: SAP, S/4HANA, CDS, CSN, VDM, ABAP, journal entry, GL line item, cost center, profit center, controlling area, ledger.
---

# SAP S/4HANA Data Modeler Skill

Expert knowledge of 28 SAP S/4HANA Cloud data products in CSN/CDS format, covering Finance (FI), Controlling (CO), Sales (SD), and Procurement (MM) — with emphasis on reporting grain, cross-domain joins, hierarchy navigation, and data redundancy.

---

## CSN File Format

```json
{
  "definitions": { ... },   // entities (kind:"entity") and reusable types (kind:"type")
  "i18n": { ... },          // label key refs resolved at runtime
  "$version": "2.0"
}
```

Entity anatomy: `kind:"entity"`, annotation keys (`@VDM.*`, `@ObjectModel.*`, `@Analytics.*`, `@ODM.*`), and `elements` (fields + associations). Associations have a `target` property and do not map to columns. Types (ABAP data elements) alias `cds.*` primitives — always resolve through the chain to `cds.String/Decimal/Date/...`.

---

## Data Product Catalog — All 28 Products

### Finance & Accounting (FI)

| Data Product | Core Entity | Key | Fields | Grain |
|---|---|---|---|---|
| **GeneralLedgerAccount** | GeneralLedgerAccountLineItem | SourceLedger + CompanyCode + FiscalYear + AccountingDocument + LedgerGLLineItem | 458 | **Lowest** — one row per ledger posting line |
| **JournalEntryHeader** | JournalEntry | CompanyCode + FiscalYear + AccountingDocument | 102 | One row per accounting document header |
| **GeneralLedgerAccount** | GeneralLedgerAccount | ChartOfAccounts + GLAccount | 26 | GL account master per chart |
| **CnsldtnGLChartOfAccounts** | CnsldtnGLChartOfAccounts | ChartOfAccounts | 4 | Consolidation chart of accounts |
| **JournalEntryItemCodes** | PostingKey, DebitCreditCode, SpecialGeneralLedgerCode + 7 more | Various | 2–8 each | FI classification code tables |
| **JournalEntryCodes** | BusinessTransactionType, FinancialTransactionType, JournalEntryType + 6 more | Various | 3–10 each | Transaction categorization code tables |
| **ARBankStatement** | ARBankStatement | BankStatementShortID | 21 | Bank statement header |
| **CashFlow** | CashFlow | CashFlowID + CshFlwValdtyStrtDteTmeVal | 16 | Cash flow position |
| **FiscalYear** | FiscalYear | FiscalYearVariant + FiscalYear | 5 | Period calendar master |
| **Ledger** | Ledger | Ledger | 10 | Accounting principle / valuation view |
| **FinancialTransaction** | FinancialTransaction | CompanyCode + FinancialTransaction | 109 | Treasury/financial instrument |

### Controlling (CO)

| Data Product | Core Entity | Key | Fields | Notes |
|---|---|---|---|---|
| **CostCenter** | CostCenter | ControllingArea + CostCenter + ValidityEndDate | 88 | Time-dependent master |
| **ProfitCenter** | ProfitCenter | ControllingArea + ProfitCenter + ValidityEndDate | 41 | Time-dependent master |
| **FunctionalArea** | FunctionalArea | FunctionalArea | 5 | Cost-of-sales reporting dimension |
| **CostOriginGroup** | CostOriginGroup | ControllingArea + CostOriginType + CostOriginGroup | 3 | CO cost classification |
| **CostCenterActivityType** | CostCenterActivityType | ControllingArea + CostCtrActivityType + ValidityEndDate | 26 | Activity type master |
| **ControllingArea** | ControllingArea | ControllingArea | 17 | CO org umbrella for CC/PC/AT |

### Org Structure

| Data Product | Core Entity | Key | Fields | Notes |
|---|---|---|---|---|
| **CompanyCode** | CompanyCode | CompanyCode | 24 | FI legal entity |
| **Plant** | Plant | Plant | 16 | Logistics/manufacturing unit |

### Sales & Billing (SD)

| Data Product | Core Entity | Key | Fields | Grain |
|---|---|---|---|---|
| **SalesOrder** | SalesOrder / SalesOrderItem | SalesOrder (+ SalesOrderItem) | 159 / 231 | Order header / line |
| **BillingDocument** | BillingDocument / BillingDocumentItem | BillingDocument (+ BillingDocumentItem) | 101 / 196 | Billing header / line — posts to GL |
| **InvoiceList** | InvoiceList / InvoiceListItem | InvoiceList (+ InvoiceListItem) | 83 / 13 | Invoice grouping header / line |
| **SalesMasterDataConfiguration** | 36 code entities | Various | 2–4 each | Sales config/code tables |

### Procurement (MM)

| Data Product | Core Entity | Key | Fields | Grain |
|---|---|---|---|---|
| **PurchaseOrder** | PurchaseOrder | PurchaseOrder | 58 | PO header |
| **PurchaseOrder** | PurchaseOrderItem | PurchaseOrder + PurchaseOrderItem | 75 | PO line |
| **PurchaseOrder** | PurchaseOrderAccountAssignment | PurchaseOrder + PurchaseOrderItem + AccountAssignmentNumber | 83 | Account assignment / cost object distribution |
| **PurchaseOrder** | PurchaseOrderScheduleLine | PurchaseOrder + PurchaseOrderItem + PurchaseOrderScheduleLine | 80 | Delivery schedule line |

### Master Data

| Data Product | Root Entity | Key | Fields | Child Entities |
|---|---|---|---|---|
| **Customer** | Customer | Customer | 117 | CustomerCompanyCode, CustomerSalesArea, CustomerSalesAreaTax, CustomerDunning, CustomerWithHoldingTax, CustomerUnloadingPoint |
| **Supplier** | Supplier | Supplier | 135 | SupplierCompanyCode, SupplierPurchasingOrganization, SupplierWithHoldingTax |
| **Product** | Product | Product | 156 | ProductPlant, ProductDescription, ProductSales, ProductSalesDelivery, ProductValuation + 15 more |

---

## Reporting Granularity

### The GL Fact Table Stack

```
JournalEntry (header)
  Keys: CompanyCode + FiscalYear + AccountingDocument   [102 fields]
  → 1:N join on same 3 keys
GeneralLedgerAccountLineItem (line item)   ← PRIMARY FACT TABLE
  Keys: SourceLedger + CompanyCode + FiscalYear + AccountingDocument + LedgerGLLineItem   [458 fields]
```

`GeneralLedgerAccountLineItem` is the universal fact table. It embeds **all** account assignment dimensions directly — no sub-joins needed for basic CO/SD/MM lookups:

- **GL**: GLAccount, ChartOfAccounts, GLAccountType, AlternativeGLAccount, DebitCreditCode, PostingKey
- **CO**: CostCenter, ProfitCenter, FunctionalArea, BusinessArea, Segment, CostCtrActivityType, OrderID, WBSElement, ControllingArea, CostOriginGroup
- **Partner/intercompany**: PartnerCostCenter, PartnerProfitCenter, PartnerFunctionalArea, PartnerBusinessArea, PartnerCompanyCode, PartnerCompany
- **SD reference**: SalesDocument, SalesDocumentItem, SalesOrganization, DistributionChannel, Customer, Product, Plant, BillingDocumentType, SoldProduct, BillToParty
- **MM reference**: PurchasingDocument, PurchasingDocumentItem, AccountAssignmentNumber, Supplier
- **Multi-currency**: AmountInTransactionCurrency, AmountInCompanyCodeCurrency, AmountInGlobalCurrency, AmountInFunctionalCurrency + 8 free-defined currencies
- **Asset accounting**: MasterFixedAsset, FixedAsset, AssetTransactionType, AssetClass, DepreciationFiscalPeriod
- **Public sector / FM**: Fund, Grant, BudgetPeriod, CommitmentItem, FundsCenter, FundedProgram
- **Consolidation**: Company, ConsolidationUnit, CnsldtnFinancialStatementItem, PartnerConsolidationUnit

### Grain Comparison: SD Pipeline

```
SalesOrderItem (231 fields)     ← requested, not financial; has Order qty, pricing conditions
  → goods delivery / billing
BillingDocumentItem (196 fields) ← revenue recognition point; finalized price + tax; 1 item → N GL lines
  → accounting interface
GeneralLedgerAccountLineItem (458 fields) ← actual debit/credit; multi-currency; full CO assignment
```

For revenue reporting: use `BillingDocumentItem` (operational) or `GeneralLedgerAccountLineItem` (accounting). Never mix both in a single fact without deduplication logic.

### Grain Comparison: PO / Commitment

```
PurchaseOrderItem (75 fields)              ← what was ordered
PurchaseOrderAccountAssignment (83 fields) ← how cost is distributed (CostCenter, GLAccount, etc.)
PurchaseOrderScheduleLine (80 fields)      ← when it's expected
  → goods receipt / invoice
GeneralLedgerAccountLineItem              ← actuals (filter: PurchasingDocument IS NOT NULL)
```

---

## Organizational Hierarchy

```
ControllingArea   (keys: ControllingArea)
  .CostCenterStandardHierarchy → CostCenterHierarchy root
  .ProfitCenterStandardHierarchy → ProfitCenterHierarchy root
  .ChartOfAccounts → links CO to FI
  .ControllingAreaCurrency → CO object currency

  ├── CostCenter  (keys: ControllingArea + CostCenter + ValidityEndDate)
  │     .CompanyCode, .ProfitCenter (default PC), .CostCenterCategory, .BusinessArea
  │     → CostCenterHierarchyNode (ControllingArea + CostCenterHierarchy + HierarchyNode + ValidityEndDate)
  │         .ParentNode, .HierarchyNodeLevel, .NodeType, .CostCenter (leaf value)
  │
  ├── ProfitCenter  (keys: ControllingArea + ProfitCenter + ValidityEndDate)
  │     .Segment, .CompanyCode, .ProfitCenterStandardHierarchy
  │     → ProfitCenterHierarchyNode (ControllingArea + ProfitCenterHierarchy + HierarchyNode + ValidityEndDate)
  │     → PrftCtrCompanyCodeAssignment (ControllingArea + ProfitCenter + CompanyCode)
  │
  ├── CostCenterActivityType  (keys: ControllingArea + CostCtrActivityType + ValidityEndDate)
  │     → CostCtrActivityTypeHierNode
  │
  └── CostOriginGroup  (keys: ControllingArea + CostOriginType + CostOriginGroup)

CompanyCode  (keys: CompanyCode)
  .ControllingArea, .ChartOfAccounts, .FiscalYearVariant, .Currency, .Country
  .Company (consolidation unit)
  → CompanyCodeHierarchyNode (for legal entity rollup)
  → CompanyCodeCurrencyRole (Ledger + CompanyCode → currency role mapping)
  → CompanyCodeCurrencyTranslation (exchange rate rules)

Ledger  (keys: Ledger)
  .IsLeadingLedger (true/false)
  → LedgerCompanyCodeCurrencyRoles (Ledger + CompanyCode: maps FreeDefinedCurrency1–8 roles)
```

**One ControllingArea spans multiple CompanyCodes.** Cross-company postings appear in GL line items via PartnerCostCenter / PartnerCompanyCode.

**Time-dependency join rule**: CostCenter, ProfitCenter, CostCenterActivityType all have ValidityEndDate in their key. To join a GL line item (PostingDate) to its master data: `ValidityStartDate <= PostingDate AND PostingDate <= ValidityEndDate`.

---

## Hierarchy Navigation Pattern

All CO/FI hierarchies share the same node table structure:

```sql
-- Hierarchy entities follow this pattern:
<Object>Hierarchy:      [ControllingArea +] <Hierarchy> + ValidityEndDate
<Object>HierarchyNode:  [ControllingArea +] <Hierarchy> + HierarchyNode + ValidityEndDate
  fields: ParentNode, HierarchyNodeLevel, NodeType, HierarchyNodeVal, <Object> (leaf FK)
<Object>HierarchyNodeText: same keys + Language
```

Available hierarchy objects: CostCenter, ProfitCenter, CostCenterActivityType, FunctionalArea, CompanyCode, GLAccount, GeneralLedgerAccount, FinancialStatement

Recursive rollup (standard SQL):
```sql
WITH RECURSIVE rollup AS (
  SELECT HierarchyNode, ParentNode, CostCenter, HierarchyNodeLevel, 0 AS depth
  FROM CostCenterHierarchyNode
  WHERE ControllingArea = :ca
    AND CostCenterHierarchy = :hier_id
    AND ValidityEndDate >= CURRENT_DATE
    AND HierarchyNode = :root_node
  UNION ALL
  SELECT c.HierarchyNode, c.ParentNode, c.CostCenter, c.HierarchyNodeLevel, r.depth + 1
  FROM CostCenterHierarchyNode c
  JOIN rollup r ON c.ParentNode = r.HierarchyNode
    AND c.ControllingArea = :ca
    AND c.CostCenterHierarchy = :hier_id
    AND c.ValidityEndDate >= CURRENT_DATE
)
SELECT SUM(gl.AmountInCompanyCodeCurrency)
FROM GeneralLedgerAccountLineItem gl
JOIN rollup h ON gl.CostCenter = h.CostCenter AND h.CostCenter IS NOT NULL
WHERE gl.CompanyCode = :company_code
  AND gl.FiscalYear = :year
  AND gl.FiscalPeriod BETWEEN :p_from AND :p_to
```

---

## Cross-Domain Join Map

### GL Line Item — All Dimensions

| GL Field(s) | Joins To | Target Data Product | Notes |
|---|---|---|---|
| CompanyCode | CompanyCode.CompanyCode | CompanyCode | Direct |
| SourceLedger | Ledger.Ledger | Ledger | Filter IsLeadingLedger for group reporting |
| ChartOfAccounts + GLAccount | GeneralLedgerAccount | GeneralLedgerAccount | |
| ControllingArea + CostCenter | CostCenter (+ date filter) | CostCenter | |
| ControllingArea + ProfitCenter | ProfitCenter (+ date filter) | ProfitCenter | |
| FunctionalArea | FunctionalArea.FunctionalArea | FunctionalArea | |
| FiscalYearVariant + FiscalYear | FiscalYear | FiscalYear | |
| AccountingDocumentType | JournalEntryType.AccountingDocumentType | JournalEntryCodes | |
| BusinessTransactionType | BusinessTransactionType | JournalEntryCodes | |
| BusinessTransactionCategory | BusinessTransactionCategory | JournalEntryCodes | |
| FinancialTransactionType | FinancialTransactionType | JournalEntryCodes + JournalEntryItemCodes | |
| Customer | Customer.Customer | Customer | |
| Supplier | Supplier.Supplier | Supplier | |
| Product | Product.Product | Product | |
| Plant | Plant.Plant | Plant | |
| ControllingArea + CostOriginGroup (+ CostOriginType) | CostOriginGroup | CostOriginGroup | 3-part key |
| PostingKey | PostingKey.PostingKey | JournalEntryItemCodes | |
| DebitCreditCode | DebitCreditCode | JournalEntryItemCodes | S=debit, H=credit |
| PurchasingDocument + PurchasingDocumentItem | PurchaseOrderItem | PurchaseOrder | |

### JournalEntry → GL Line Items
```
JournalEntry.{CompanyCode, FiscalYear, AccountingDocument}
  = GeneralLedgerAccountLineItem.{CompanyCode, FiscalYear, AccountingDocument}
```

### SD → GL Reference
```
BillingDocument posts to GL with:
  GL.ReferenceDocumentType IN ('VBRK','VBRP')  -- billing doc category
  GL.ReferenceDocument = BillingDocument.BillingDocument
  GL.SalesDocument = SalesOrder header reference
```

### PO → GL Actuals
```
GL.PurchasingDocument = PurchaseOrder.PurchaseOrder
GL.PurchasingDocumentItem = PurchaseOrderItem.PurchaseOrderItem
```

### CompanyCode → CO/FI
```
CompanyCode.ControllingArea → ControllingArea
CompanyCode.ChartOfAccounts → GeneralLedgerAccount (ChartOfAccounts)
CompanyCode.FiscalYearVariant → FiscalYear (FiscalYearVariant)
CostCenter.CompanyCode → CompanyCode
PrftCtrCompanyCodeAssignment.CompanyCode → CompanyCode
```

---

## Redundancies & Known Overlaps

### Duplicate Amount Dimensions on GL Line Item
The 12+ currency amount fields are **not redundant** — each is a different valuation view. `LedgerCompanyCodeCurrencyRoles` defines which `FreeDefinedCurrencyNRole` maps to which accounting principle/currency. For simple reporting: use `AmountInCompanyCodeCurrency` (local) or `AmountInGlobalCurrency` (group).

### Material vs Product field names
Both `Material` and `Product` fields appear on SalesOrderItem, BillingDocumentItem, and GL line items — they hold the same value. `Product` is the current CDS name; `Material` is the ABAP legacy name. Always join on `Product` for cross-data-product consistency.

### CostCenter.ProfitCenter (default) vs ProfitCenter master
`CostCenter.ProfitCenter` is the default profit center assignment for that cost center. It is **not** the authoritative source for actual posting assignments. In GL postings, `GeneralLedgerAccountLineItem.ProfitCenter` is derived at posting time and may differ (e.g., manual override). Use `PrftCtrCompanyCodeAssignment` for organizational mapping queries.

### PostingDate on both JournalEntry and GL Line Item
`JournalEntry.PostingDate` = authoritative header date. `GeneralLedgerAccountLineItem.PostingDate` = denormalized copy. Use GL.PostingDate for filtering line items directly; join to JournalEntry header only for header-level attributes (e.g., AccountingDocumentHeaderText, TransactionCode).

### BillingDocument vs InvoiceList
`InvoiceList` groups multiple `BillingDocument`s into a consolidated invoice for a customer. `InvoiceListItem` links back to individual billing docs. For revenue analysis, work at BillingDocument grain; use InvoiceList only for customer invoice presentation logic.

### SalesOrderItem vs BillingDocumentItem
`SalesOrderItem` carries order quantity and pricing — not posted to accounting. `BillingDocumentItem` is the actual revenue event. Never aggregate both for revenue figures without deduplication.

---

## Multi-Ledger & Currency Architecture

```
Ledger.IsLeadingLedger = true → standard (IFRS/local GAAP) ledger, typically code '0L'
Ledger.ExtensionLedgerType → parallel accounting ledger (e.g., US GAAP, USGAAP)

LedgerCompanyCodeCurrencyRoles (Ledger + CompanyCode):
  CompanyCodeCurrencyRole → which role is local currency
  GlobalCurrencyRole → which role is group currency
  FreeDefinedCurrency1–8Role → custom currency assignments

GL line item carries all currency values in parallel — same posting, multiple valuations.
```

**For group/consolidation reporting**: Filter `SourceLedger = '0L'` (or join `Ledger.IsLeadingLedger = true`) then use `AmountInGlobalCurrency`.

**For legal entity reporting**: Use `AmountInCompanyCodeCurrency` — always populated regardless of ledger.

---

## FiscalYear / Period Reference

```
FiscalYearVariant → defines calendar (K4=calendar year, V3=Apr-Mar, etc.)
FiscalYear.FiscalYearStartDate / FiscalYearEndDate → actual date bounds
FiscalYear.NumberOfFiscalPeriods → 12 or 16 (special periods for year-end)
```

GL line item period fields:
- `FiscalYear` + `FiscalPeriod` = standard (period 001–016)
- `FiscalYearPeriod` = YYYYPPP concatenated (good for range predicates)
- Special periods 013–016 = year-end adjustment periods (exclude from operational reporting unless needed)

---

## Reference Files

Load these only when field-level detail is needed for a specific entity:

- **`references/entity-field-catalog.md`** — Complete field listing for all major entities (SalesOrder, Customer, Product, Supplier, GeneralLedgerAccount, GL Line Item, etc.)
- **`references/type-primitives.md`** — ABAP type → CDS primitive resolution table (~700 types)
