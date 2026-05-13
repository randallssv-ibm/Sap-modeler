# ARBankStatement

> Source file: `sap-s4com-ARBankStatement-v1.json`


## Entity: `ARBankStatement`

- **ABAP CDS Name:** `I_BankStatement`
- **Label:** Header of a bank statement
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** FEBKO, FEBEP

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `BankStatementShortID` |  |  |  |  |  | `String(8)` | Y | Short Key |  |  |
| `CompanyCode` |  |  |  |  |  | `String(4)` |  | Company Code |  |  |
| `HouseBank` |  |  |  |  |  | `String(5)` |  | House Bank |  |  |
| `HouseBankAccount` |  |  |  |  |  | `String(5)` |  | House Bank Acct ID |  |  |
| `BankStatement` |  |  |  |  |  | `String(18)` |  | Bank Statement Number |  |  |
| `BankStatementDate` |  |  |  |  |  | `Date` |  | Bank Statement Date |  |  |
| `BankStatementStatus` |  |  |  |  |  | `String(1)` |  | Statement Status |  |  |
| `BankStatementPageNumber` |  |  |  |  |  | `String(5)` |  | Page No. (5 Digits) |  |  |
| `Currency` |  |  |  |  |  | `String(5)` |  | Currency |  |  |
| `OpeningBalanceIsInterim` |  |  |  |  |  | `Boolean` |  | Interim Opening |  |  |
| `ClosingBalanceIsInterim` |  |  |  |  |  | `Boolean` |  | Interim Closing |  |  |
| `OpeningBalanceAmtInTransCrcy` |  |  |  |  |  | `Decimal(34,4)` |  | Opening Balance | Currency |  |
| `ClosingBalanceAmtInTransCrcy` |  |  |  |  |  | `Decimal(34,4)` |  | Ending Bal.Amount | Currency |  |
| `InterimOpenBalAmtInTransCrcy` |  |  |  |  |  | `Decimal(34,4)` |  | Interim Opening Balance | Currency |  |
| `InterimClsgBalAmtInTransCrcy` |  |  |  |  |  | `Decimal(34,4)` |  | Interim Closing Balance | Currency |  |
| `PaymentTransactionTypeGroup` |  |  |  |  |  | `String(8)` |  | Transaction Type |  |  |
| `CreatedByUser` |  |  |  |  |  | `String(12)` |  | EB User |  |  |
| `BankStatementIsManuallyCreated` |  |  |  |  |  | `Boolean` |  | BS created manually |  |  |
| `BankStatementFormat` |  |  |  |  |  | `String(2)` |  | Statement Format |  |  |
| `BankStatementImportDate` |  |  |  |  |  | `Date` |  | Statement Import Date |  |  |
| `BankStatementImportTime` |  |  |  |  |  | `String(6)` |  | Stmnt. Import Time |  |  |


## Entity: `BankStmntItemReprocessReason`

- **ABAP CDS Name:** `I_BankStmntItemReprocessReason`
- **Label:** Bank Statement Item Reprocessing Reason
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `BankStmntItemReprocessReason` |  |  |  |  |  | `String(2)` | Y | Reproc. Reason Code |  | S/4 only entity |


## Entity: `BankStmntItmReprocessRsnText`

- **ABAP CDS Name:** `I_BankStmntItmReprocessRsnName`
- **Label:** Bank Stmnt Item Reprocessing Reason Name
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `BankStmntItemReprocessReason` |  |  |  |  |  | `String(2)` | Y | Reproc. Reason Code |  | S/4 only entity |
| `Language` |  |  |  |  |  | `String(2)` | Y | Language Key |  | S/4 only entity |
| `BankStmntItemReprocessRsnName` |  |  |  |  |  | `String(60)` |  | Reprocessing Reason |  | S/4 only entity |
