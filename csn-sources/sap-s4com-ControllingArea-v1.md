# ControllingArea

> Source file: `sap-s4com-ControllingArea-v1.json`


## Entity: `ControllingArea`

- **ABAP Name:** `I_ControllingArea`
- **Label:** Controlling Area
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `ControllingArea` | `ControllingArea` | `String(4)` | Y | Controlling Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `FiscalYearVariant` | `FiscalYearVariant` | `String(2)` |  | Fiscal Year Variant |  |  | S/4 only entity (no ECC CDC mapping) |
| `ControllingAreaName` | `ControllingAreaName` | `String(25)` |  | Controlling Area Name |  |  | S/4 only entity (no ECC CDC mapping) |
| `ControllingAreaCurrency` | `ControllingAreaCurrency` | `String(5)` |  | Controlling Area Currency |  |  | S/4 only entity (no ECC CDC mapping) |
| `ChartOfAccounts` | `ChartOfAccounts` | `String(4)` |  | Chart of Accounts |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCenterStandardHierarchy` | `CostCenterStandardHierarchy` | `String(12)` |  | Cost Center Standard Hierarchy |  |  | S/4 only entity (no ECC CDC mapping) |
| `OperatingConcern` | `OperatingConcern` | `String(4)` |  | Operating Concern |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProfitCenterStandardHierarchy` | `ProfitCenterStandardHierarchy` | `String(12)` |  | Profit Center Standard Hierarchy |  |  | S/4 only — no ECC equivalent; S/4 only entity (no ECC CDC mapping) |
| `BusinessProcessStandardHier` | `BusinessProcessStandardHier` | `String(12)` |  | Business Process Standard Hierarchy Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `CreditDownPaymentDefaultGLAcct` | `CreditDownPaymentDefaultGLAcct` | `String(10)` |  | G/L Account for Supplier Down Payments |  |  | S/4 only entity (no ECC CDC mapping) |
| `DebitDownPaymentDefaultGLAcct` | `DebitDownPaymentDefaultGLAcct` | `String(10)` |  | G/L Account for Customer Down Payments |  |  | S/4 only entity (no ECC CDC mapping) |
| `ControllingAreaCurrencyRole` | `ControllingAreaCurrencyRole` | `String(2)` |  | Currency Type for Controlling Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinancialManagementArea` | `FinancialManagementArea` | `String(4)` |  | FM Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `ControllingAreaResponsibleUser` | `ControllingAreaResponsibleUser` | `String(12)` |  | Responsible User of Controlling Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `DefaultProfitCenter` | `DefaultProfitCenter` | `String(10)` |  | Default Profit Center |  |  | S/4 only entity (no ECC CDC mapping) |
| `CtrlgStdFinStatementVersion` | `CtrlgStdFinStatementVersion` | `String(42)` |  | Leading Ctrlg Financial Stmnt Version |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProfitCenterAccountingCurrency` | `ProfitCenterAccountingCurrency` | `String(5)` |  | Profit Center Local Currency |  |  | S/4 only entity (no ECC CDC mapping) |
