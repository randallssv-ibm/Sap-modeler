# ControllingArea

> Source file: `sap-s4com-ControllingArea-v1.json`


## Entity: `ControllingArea`

- **ABAP CDS Name:** `I_ControllingArea`
- **Label:** Controlling Area
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** TKA01

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `ControllingArea` | `FIS_KOKRS` | `TKA01` | `KOKRS` |  |  | `String(4)` | Y | Controlling Area |  |  |
| `FiscalYearVariant` | `FIS_PERIV` | `TKA01` | `PERIV` |  |  | `String(2)` |  | Fiscal Year Variant |  |  |
| `ControllingAreaName` | `FIS_KOKRS_NAME` | `TKA01` | `BEZEI` |  |  | `String(25)` |  | Controlling Area Name |  |  |
| `ControllingAreaCurrency` | `FIS_KWAER` |  |  |  |  | `String(5)` |  | Controlling Area Currency |  |  |
| `ChartOfAccounts` | `FIS_KTOPL` | `TKA01` | `KTOPL` |  |  | `String(4)` |  | Chart of Accounts |  |  |
| `CostCenterStandardHierarchy` | `FIS_KSTHI` | `TKA01` | `KHINR` |  |  | `String(12)` |  | Cost Center Standard Hierarchy |  |  |
| `OperatingConcern` | `ERKRS` |  |  |  |  | `String(4)` |  | Operating Concern |  |  |
| `ProfitCenterStandardHierarchy` | `FIS_PRCTR_STD_HIER` |  |  |  |  | `String(12)` |  | Profit Center Standard Hierarchy |  |  |
| `BusinessProcessStandardHier` | `FIS_CO_BPHINR` |  |  |  |  | `String(12)` |  | Business Process Standard Hierarchy Area |  |  |
| `CreditDownPaymentDefaultGLAcct` | `FIS_KSTAR_FIN` |  |  |  |  | `String(10)` |  | G/L Account for Supplier Down Payments |  |  |
| `DebitDownPaymentDefaultGLAcct` | `FIS_KSTAR_FID` |  |  |  |  | `String(10)` |  | G/L Account for Customer Down Payments |  |  |
| `ControllingAreaCurrencyRole` | `FIS_CO_CTYP` |  |  |  |  | `String(2)` |  | Currency Type for Controlling Area |  |  |
| `FinancialManagementArea` | `FIKRS` |  |  |  |  | `String(4)` |  | FM Area |  |  |
| `ControllingAreaResponsibleUser` | `FIS_CO_VNAME` |  |  |  |  | `String(12)` |  | Responsible User of Controlling Area |  |  |
| `DefaultProfitCenter` | `FIS_DEFPRCTR` |  |  |  |  | `String(10)` |  | Default Profit Center |  |  |
| `CtrlgStdFinStatementVersion` | `FIS_LEADING_FSV` |  |  |  |  | `String(42)` |  | Leading Ctrlg Financial Stmnt Version |  |  |
| `ProfitCenterAccountingCurrency` | `FIS_PCACUR` |  |  |  |  | `String(5)` |  | Profit Center Local Currency |  |  |
