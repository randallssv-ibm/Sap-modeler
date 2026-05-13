# CnsldtnGLChartOfAccounts

> Source file: `sap-s4com-CnsldtnGLChartOfAccounts-v1.json`

**Technical Name:** `` | **Data Category:** `DIMENSION` | **VDM Type:** `COMPOSITE` | **Size:** `M`


## Entity: `CnsldtnGLChartOfAccounts`

- **ABAP Name:** `I_CnsldtnGLChartOfAccounts`
- **Label:** Cnsldtn Combined G/L Chart Of Accounts
- **VDM Type:** `COMPOSITE` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `ChartOfAccounts` | `T001` | `KTOPL` | `String(4)` | Y | G/L Chart of Accounts |  |  |  |
| `AdditionalMasterDataSource` |  |  | `String(10)` |  | Master Data Source |  |  | S/4 only entity |
| `CnsldtnIsAdditionalMasterData` |  |  | `Boolean` |  | Is Additional Master Data |  |  | S/4 only entity |


## Entity: `CnsldtnGLChartOfAccountsText`

- **ABAP Name:** `I_CnsldtnGLChartOfAccountsT`
- **Label:** Cnsldtn Combined G/L Chart Of Accounts - Txt
- **VDM Type:** `COMPOSITE` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `Language` |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity |
| `ChartOfAccounts` | `T001` | `KTOPL` | `String(4)` | Y | G/L Chart of Accounts |  | _ChartOfAccounts |  |
| `AdditionalMasterDataSource` |  |  | `String(10)` |  | Master Data Source |  |  | S/4 only entity |
| `AdditionalMasterDataText` |  |  | `String(50)` |  | Description |  |  | S/4 only entity |
| `ChartOfAccountsName` |  |  | `String(50)` |  | G/L Chart of Accounts Description |  |  | S/4 only entity |
| `CnsldtnIsAdditionalMasterData` |  |  | `Boolean` |  | Is Additional Master Data |  |  | S/4 only entity |
