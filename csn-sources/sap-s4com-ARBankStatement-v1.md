# ARBankStatement

> Source file: `sap-s4com-ARBankStatement-v1.json`


## Entity: `ARBankStatement`

- **ABAP CDS Name:** `I_BankStatement`
- **Label:** Header of a bank statement
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `BankStatementShortID` |  |  |  |  |  | `String(8)` | Y | Short Key |  | S/4 only entity |
| `CompanyCode` |  |  |  |  |  | `String(4)` |  | Company Code |  | S/4 only entity |
| `HouseBank` |  |  |  |  |  | `String(5)` |  | House Bank |  | S/4 only entity |
| `HouseBankAccount` |  |  |  |  |  | `String(5)` |  | House Bank Acct ID |  | S/4 only entity |
| `BankStatement` |  |  |  |  |  | `String(18)` |  | Bank Statement Number |  | S/4 only entity |
| `BankStatementDate` |  |  |  |  |  | `Date` |  | Bank Statement Date |  | S/4 only entity |
| `BankStatementStatus` |  |  |  |  |  | `String(1)` |  | Statement Status |  | S/4 only entity |
| `BankStatementPageNumber` |  |  |  |  |  | `String(5)` |  | Page No. (5 Digits) |  | S/4 only entity |
| `Currency` |  |  |  |  |  | `String(5)` |  | Currency |  | S/4 only entity |
| `OpeningBalanceIsInterim` |  |  |  |  |  | `Boolean` |  | Interim Opening |  | S/4 only entity |
| `ClosingBalanceIsInterim` |  |  |  |  |  | `Boolean` |  | Interim Closing |  | S/4 only entity |
| `OpeningBalanceAmtInTransCrcy` |  |  |  |  |  | `Decimal(34,4)` |  | Opening Balance | Currency | S/4 only entity |
| `ClosingBalanceAmtInTransCrcy` |  |  |  |  |  | `Decimal(34,4)` |  | Ending Bal.Amount | Currency | S/4 only entity |
| `InterimOpenBalAmtInTransCrcy` |  |  |  |  |  | `Decimal(34,4)` |  | Interim Opening Balance | Currency | S/4 only entity |
| `InterimClsgBalAmtInTransCrcy` |  |  |  |  |  | `Decimal(34,4)` |  | Interim Closing Balance | Currency | S/4 only entity |
| `PaymentTransactionTypeGroup` |  |  |  |  |  | `String(8)` |  | Transaction Type |  | S/4 only entity |
| `CreatedByUser` |  |  |  |  |  | `String(12)` |  | EB User |  | S/4 only entity |
| `BankStatementIsManuallyCreated` |  |  |  |  |  | `Boolean` |  | BS created manually |  | S/4 only entity |
| `BankStatementFormat` |  |  |  |  |  | `String(2)` |  | Statement Format |  | S/4 only entity |
| `BankStatementImportDate` |  |  |  |  |  | `Date` |  | Statement Import Date |  | S/4 only entity |
| `BankStatementImportTime` |  |  |  |  |  | `String(6)` |  | Stmnt. Import Time |  | S/4 only entity |


## Entity: `BankStmntItemReprocessReason`

- **ABAP CDS Name:** `I_BankStmntItemReprocessReason`
- **Label:** Bank Statement Item Reprocessing Reason
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `BankStmntItemReprocessReason` |  |  |  |  |  | `String(2)` | Y | Reproc. Reason Code |  | S/4 only entity |


## Entity: `BankStmntItmReprocessRsnText`

- **ABAP CDS Name:** `I_BankStmntItmReprocessRsnName`
- **Label:** Bank Stmnt Item Reprocessing Reason Name
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `BankStmntItemReprocessReason` |  |  |  |  |  | `String(2)` | Y | Reproc. Reason Code |  | S/4 only entity |
| `Language` |  |  |  |  |  | `String(2)` | Y | Language Key |  | S/4 only entity |
| `BankStmntItemReprocessRsnName` |  |  |  |  |  | `String(60)` |  | Reprocessing Reason |  | S/4 only entity |
