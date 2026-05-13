# ControllingArea

> Source file: `sap-s4com-ControllingArea-v1.json`


## Entity: `ControllingArea`

- **ABAP Name:** `I_ControllingArea`
- **Label:** Controlling Area
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `ControllingArea` | `TKA01` | `KOKRS` | `String(4)` | Y | Controlling Area |  |  |  |
| `FiscalYearVariant` | `TKA01` | `PERIV` | `String(2)` |  | Fiscal Year Variant |  |  |  |
| `ControllingAreaName` | `TKA01` | `BEZEI` | `String(25)` |  | Controlling Area Name |  |  |  |
| `ControllingAreaCurrency` |  |  | `String(5)` |  | Controlling Area Currency |  |  | S/4 only entity |
| `ChartOfAccounts` | `TKA01` | `KTOPL` | `String(4)` |  | Chart of Accounts |  |  |  |
| `CostCenterStandardHierarchy` | `TKA01` | `KHINR` | `String(12)` |  | Cost Center Standard Hierarchy |  |  |  |
| `OperatingConcern` |  |  | `String(4)` |  | Operating Concern |  |  | S/4 only entity |
| `ProfitCenterStandardHierarchy` |  |  | `String(12)` |  | Profit Center Standard Hierarchy |  |  | S/4 only entity |
| `BusinessProcessStandardHier` |  |  | `String(12)` |  | Business Process Standard Hierarchy Area |  |  | S/4 only entity |
| `CreditDownPaymentDefaultGLAcct` |  |  | `String(10)` |  | G/L Account for Supplier Down Payments |  |  | S/4 only entity |
| `DebitDownPaymentDefaultGLAcct` |  |  | `String(10)` |  | G/L Account for Customer Down Payments |  |  | S/4 only entity |
| `ControllingAreaCurrencyRole` |  |  | `String(2)` |  | Currency Type for Controlling Area |  |  | S/4 only entity |
| `FinancialManagementArea` |  |  | `String(4)` |  | FM Area |  |  | S/4 only entity |
| `ControllingAreaResponsibleUser` |  |  | `String(12)` |  | Responsible User of Controlling Area |  |  | S/4 only entity |
| `DefaultProfitCenter` |  |  | `String(10)` |  | Default Profit Center |  |  | S/4 only entity |
| `CtrlgStdFinStatementVersion` |  |  | `String(42)` |  | Leading Ctrlg Financial Stmnt Version |  |  | S/4 only entity |
| `ProfitCenterAccountingCurrency` |  |  | `String(5)` |  | Profit Center Local Currency |  |  | S/4 only entity |
