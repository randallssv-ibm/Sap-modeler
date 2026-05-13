# CnsldtnGLChartOfAccounts

> Source file: `sap-s4com-CnsldtnGLChartOfAccounts-v1.json`

**Technical Name:** `` | **Data Category:** `DIMENSION` | **VDM Type:** `COMPOSITE` | **Size:** `M`


## Entity: `CnsldtnGLChartOfAccounts`

- **ABAP CDS Name:** `I_CnsldtnGLChartOfAccounts`
- **Label:** Cnsldtn Combined G/L Chart Of Accounts
- **VDM Type:** `COMPOSITE` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** GLPCA, GLPCT

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `ChartOfAccounts` | `FINCS_CHARTOFACCOUNTS` |  |  |  |  | `String(4)` | Y | G/L Chart of Accounts |  |  |
| `AdditionalMasterDataSource` | `FINCS_MASTERDATASOURCE` |  |  |  |  | `String(10)` |  | Master Data Source |  |  |
| `CnsldtnIsAdditionalMasterData` | `FINCS_ISADDITIONALMASTERDATA` |  |  |  |  | `Boolean` |  | Is Additional Master Data |  |  |


## Entity: `CnsldtnGLChartOfAccountsText`

- **ABAP CDS Name:** `I_CnsldtnGLChartOfAccountsT`
- **Label:** Cnsldtn Combined G/L Chart Of Accounts - Txt
- **VDM Type:** `COMPOSITE` | **Data Category:** ``
- **ECC Source Tables:** GLPCT

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Language` | `SPRAS` |  |  |  |  | `String(2)` | Y | Language Key |  |  |
| `ChartOfAccounts` | `FINCS_CHARTOFACCOUNTS` |  |  |  |  | `String(4)` | Y | G/L Chart of Accounts |  |  |
| `AdditionalMasterDataSource` | `FINCS_MASTERDATASOURCE` |  |  |  |  | `String(10)` |  | Master Data Source |  |  |
| `AdditionalMasterDataText` | `FINCS_DESCRIPTION_TEXT_50` |  |  |  |  | `String(50)` |  | Description |  |  |
| `ChartOfAccountsName` | `FINCS_CHARTOFACCOUNTSNAME` |  |  |  |  | `String(50)` |  | G/L Chart of Accounts Description |  |  |
| `CnsldtnIsAdditionalMasterData` | `FINCS_ISADDITIONALMASTERDATA` |  |  |  |  | `Boolean` |  | Is Additional Master Data |  |  |
