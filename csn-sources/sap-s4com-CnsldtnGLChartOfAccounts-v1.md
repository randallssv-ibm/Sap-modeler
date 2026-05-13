# CnsldtnGLChartOfAccounts

> Source file: `sap-s4com-CnsldtnGLChartOfAccounts-v1.json`

**Technical Name:** `` | **Data Category:** `DIMENSION` | **VDM Type:** `COMPOSITE` | **Size:** `M`


## Entity: `CnsldtnGLChartOfAccounts`

- **ABAP Name:** `I_CnsldtnGLChartOfAccounts`
- **Label:** Cnsldtn Combined G/L Chart Of Accounts
- **VDM Type:** `COMPOSITE` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `ChartOfAccounts` | `ChartOfAccounts` | `String(4)` | Y | G/L Chart of Accounts |  |  | S/4 only entity (no ECC CDC mapping) |
| `AdditionalMasterDataSource` | `AdditionalMasterDataSource` | `String(10)` |  | Master Data Source |  |  | S/4 only entity (no ECC CDC mapping) |
| `CnsldtnIsAdditionalMasterData` | `CnsldtnIsAdditionalMasterData` | `Boolean` |  | Is Additional Master Data |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `CnsldtnGLChartOfAccountsText`

- **ABAP Name:** `I_CnsldtnGLChartOfAccountsT`
- **Label:** Cnsldtn Combined G/L Chart Of Accounts - Txt
- **VDM Type:** `COMPOSITE` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `ChartOfAccounts` | `ChartOfAccounts` | `String(4)` | Y | G/L Chart of Accounts |  | _ChartOfAccounts | S/4 only entity (no ECC CDC mapping) |
| `AdditionalMasterDataSource` | `AdditionalMasterDataSource` | `String(10)` |  | Master Data Source |  |  | S/4 only entity (no ECC CDC mapping) |
| `AdditionalMasterDataText` | `AdditionalMasterDataText` | `String(50)` |  | Description |  |  | S/4 only entity (no ECC CDC mapping) |
| `ChartOfAccountsName` | `ChartOfAccountsName` | `String(50)` |  | G/L Chart of Accounts Description |  |  | S/4 only entity (no ECC CDC mapping) |
| `CnsldtnIsAdditionalMasterData` | `CnsldtnIsAdditionalMasterData` | `Boolean` |  | Is Additional Master Data |  |  | S/4 only entity (no ECC CDC mapping) |
