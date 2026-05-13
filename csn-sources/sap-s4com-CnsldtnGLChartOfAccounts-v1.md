# CnsldtnGLChartOfAccounts

> Source file: `sap-s4com-CnsldtnGLChartOfAccounts-v1.json`

**Technical Name:** `` | **Data Category:** `DIMENSION` | **VDM Type:** `COMPOSITE` | **Size:** `M`


## Entity: `CnsldtnGLChartOfAccounts`

- **ABAP Name:** `I_CnsldtnGLChartOfAccounts`
- **Label:** Cnsldtn Combined G/L Chart Of Accounts
- **VDM Type:** `COMPOSITE` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `ChartOfAccounts` | `FINCS_CHARTOFACCOUNTS` | `FINCS_CHARTOFACCOUNTS` |  | `String(4)` | Y | G/L Chart of Accounts |  |  | S/4 only entity — no ECC CDC mapping |
| `AdditionalMasterDataSource` | `FINCS_MASTERDATASOURCE` | `FINCS_MASTERDATASOURCE` |  | `String(10)` |  | Master Data Source |  |  | S/4 only entity — no ECC CDC mapping |
| `CnsldtnIsAdditionalMasterData` | `FINCS_ISADDITIONALMASTERDATA` | `FINCS_ISADDITIONALMASTERDATA` |  | `Boolean` |  | Is Additional Master Data |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `CnsldtnGLChartOfAccountsText`

- **ABAP Name:** `I_CnsldtnGLChartOfAccountsT`
- **Label:** Cnsldtn Combined G/L Chart Of Accounts - Txt
- **VDM Type:** `COMPOSITE` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Language` | `SPRAS` | `SPRAS` |  | `String(2)` | Y | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `ChartOfAccounts` | `FINCS_CHARTOFACCOUNTS` | `FINCS_CHARTOFACCOUNTS` |  | `String(4)` | Y | G/L Chart of Accounts |  | _ChartOfAccounts | S/4 only entity — no ECC CDC mapping |
| `AdditionalMasterDataSource` | `FINCS_MASTERDATASOURCE` | `FINCS_MASTERDATASOURCE` |  | `String(10)` |  | Master Data Source |  |  | S/4 only entity — no ECC CDC mapping |
| `AdditionalMasterDataText` | `FINCS_DESCRIPTION_TEXT_50` | `FINCS_DESCRIPTION_TEXT_50` |  | `String(50)` |  | Description |  |  | S/4 only entity — no ECC CDC mapping |
| `ChartOfAccountsName` | `FINCS_CHARTOFACCOUNTSNAME` | `FINCS_CHARTOFACCOUNTSNAME` |  | `String(50)` |  | G/L Chart of Accounts Description |  |  | S/4 only entity — no ECC CDC mapping |
| `CnsldtnIsAdditionalMasterData` | `FINCS_ISADDITIONALMASTERDATA` | `FINCS_ISADDITIONALMASTERDATA` |  | `Boolean` |  | Is Additional Master Data |  |  | S/4 only entity — no ECC CDC mapping |
