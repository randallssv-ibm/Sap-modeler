# ControllingArea

> Source file: `sap-s4com-ControllingArea-v1.json`


## Entity: `ControllingArea`

- **ABAP Name:** `I_ControllingArea`
- **Label:** Controlling Area
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `ControllingArea` | `FIS_KOKRS` | `KOKRS` |  | `String(4)` | Y | Controlling Area |  |  | S/4 only entity — no ECC CDC mapping |
| `FiscalYearVariant` | `FIS_PERIV` | `PERIV` |  | `String(2)` |  | Fiscal Year Variant |  |  | S/4 only entity — no ECC CDC mapping |
| `ControllingAreaName` | `FIS_KOKRS_NAME` | `KOKRS_NAME` |  | `String(25)` |  | Controlling Area Name |  |  | S/4 only entity — no ECC CDC mapping |
| `ControllingAreaCurrency` | `FIS_KWAER` | `KWAER` |  | `String(5)` |  | Controlling Area Currency |  |  | S/4 only entity — no ECC CDC mapping |
| `ChartOfAccounts` | `FIS_KTOPL` | `KTOPL` |  | `String(4)` |  | Chart of Accounts |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCenterStandardHierarchy` | `FIS_KSTHI` | `KSTHI` |  | `String(12)` |  | Cost Center Standard Hierarchy |  |  | S/4 only entity — no ECC CDC mapping |
| `OperatingConcern` | `ERKRS` | `ERKRS` |  | `String(4)` |  | Operating Concern |  |  | S/4 only entity — no ECC CDC mapping |
| `ProfitCenterStandardHierarchy` | `FIS_PRCTR_STD_HIER` | `PRCTR_STD_HIER` |  | `String(12)` |  | Profit Center Standard Hierarchy |  |  | S/4 only entity — no ECC CDC mapping |
| `BusinessProcessStandardHier` | `FIS_CO_BPHINR` | `CO_BPHINR` |  | `String(12)` |  | Business Process Standard Hierarchy Area |  |  | S/4 only entity — no ECC CDC mapping |
| `CreditDownPaymentDefaultGLAcct` | `FIS_KSTAR_FIN` | `KSTAR_FIN` |  | `String(10)` |  | G/L Account for Supplier Down Payments |  |  | S/4 only entity — no ECC CDC mapping |
| `DebitDownPaymentDefaultGLAcct` | `FIS_KSTAR_FID` | `KSTAR_FID` |  | `String(10)` |  | G/L Account for Customer Down Payments |  |  | S/4 only entity — no ECC CDC mapping |
| `ControllingAreaCurrencyRole` | `FIS_CO_CTYP` | `CO_CTYP` |  | `String(2)` |  | Currency Type for Controlling Area |  |  | S/4 only entity — no ECC CDC mapping |
| `FinancialManagementArea` | `FIKRS` | `FIKRS` |  | `String(4)` |  | FM Area |  |  | S/4 only entity — no ECC CDC mapping |
| `ControllingAreaResponsibleUser` | `FIS_CO_VNAME` | `CO_VNAME` |  | `String(12)` |  | Responsible User of Controlling Area |  |  | S/4 only entity — no ECC CDC mapping |
| `DefaultProfitCenter` | `FIS_DEFPRCTR` | `DEFPRCTR` |  | `String(10)` |  | Default Profit Center |  |  | S/4 only entity — no ECC CDC mapping |
| `CtrlgStdFinStatementVersion` | `FIS_LEADING_FSV` | `LEADING_FSV` |  | `String(42)` |  | Leading Ctrlg Financial Stmnt Version |  |  | S/4 only entity — no ECC CDC mapping |
| `ProfitCenterAccountingCurrency` | `FIS_PCACUR` | `PCACUR` |  | `String(5)` |  | Profit Center Local Currency |  |  | S/4 only entity — no ECC CDC mapping |
