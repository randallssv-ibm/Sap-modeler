# ARBankStatement

> Source file: `sap-s4com-ARBankStatement-v1.json`


## Entity: `ARBankStatement`

- **ABAP Name:** `I_BankStatement`
- **Label:** Header of a bank statement
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `BankStatementShortID` |  |  |  | `String(8)` | Y | Short Key |  |  | S/4 only entity — no ECC CDC mapping |
| `CompanyCode` |  |  |  | `String(4)` |  | Company Code |  |  | S/4 only entity — no ECC CDC mapping |
| `HouseBank` |  |  |  | `String(5)` |  | House Bank |  |  | S/4 only entity — no ECC CDC mapping |
| `HouseBankAccount` |  |  |  | `String(5)` |  | House Bank Acct ID |  |  | S/4 only entity — no ECC CDC mapping |
| `BankStatement` |  |  |  | `String(18)` |  | Bank Statement Number |  |  | S/4 only entity — no ECC CDC mapping |
| `BankStatementDate` |  |  |  | `Date` |  | Bank Statement Date |  |  | S/4 only entity — no ECC CDC mapping |
| `BankStatementStatus` |  |  |  | `String(1)` |  | Statement Status |  |  | S/4 only entity — no ECC CDC mapping |
| `BankStatementPageNumber` |  |  |  | `String(5)` |  | Page No. (5 Digits) |  |  | S/4 only entity — no ECC CDC mapping |
| `Currency` |  |  |  | `String(5)` |  | Currency |  |  | S/4 only entity — no ECC CDC mapping |
| `OpeningBalanceIsInterim` |  |  |  | `Boolean` |  | Interim Opening |  |  | S/4 only entity — no ECC CDC mapping |
| `ClosingBalanceIsInterim` |  |  |  | `Boolean` |  | Interim Closing |  |  | S/4 only entity — no ECC CDC mapping |
| `OpeningBalanceAmtInTransCrcy` |  |  |  | `Decimal(34,4)` |  | Opening Balance | Currency |  | S/4 only entity — no ECC CDC mapping |
| `ClosingBalanceAmtInTransCrcy` |  |  |  | `Decimal(34,4)` |  | Ending Bal.Amount | Currency |  | S/4 only entity — no ECC CDC mapping |
| `InterimOpenBalAmtInTransCrcy` |  |  |  | `Decimal(34,4)` |  | Interim Opening Balance | Currency |  | S/4 only entity — no ECC CDC mapping |
| `InterimClsgBalAmtInTransCrcy` |  |  |  | `Decimal(34,4)` |  | Interim Closing Balance | Currency |  | S/4 only entity — no ECC CDC mapping |
| `PaymentTransactionTypeGroup` |  |  |  | `String(8)` |  | Transaction Type |  |  | S/4 only entity — no ECC CDC mapping |
| `CreatedByUser` |  |  |  | `String(12)` |  | EB User |  |  | S/4 only entity — no ECC CDC mapping |
| `BankStatementIsManuallyCreated` |  |  |  | `Boolean` |  | BS created manually |  |  | S/4 only entity — no ECC CDC mapping |
| `BankStatementFormat` |  |  |  | `String(2)` |  | Statement Format |  |  | S/4 only entity — no ECC CDC mapping |
| `BankStatementImportDate` |  |  |  | `Date` |  | Statement Import Date |  |  | S/4 only entity — no ECC CDC mapping |
| `BankStatementImportTime` |  |  |  | `String(6)` |  | Stmnt. Import Time |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `BankStmntItemReprocessReason`

- **ABAP Name:** `I_BankStmntItemReprocessReason`
- **Label:** Bank Statement Item Reprocessing Reason
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `BankStmntItemReprocessReason` |  |  |  | `String(2)` | Y | Reproc. Reason Code |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `BankStmntItmReprocessRsnText`

- **ABAP Name:** `I_BankStmntItmReprocessRsnName`
- **Label:** Bank Stmnt Item Reprocessing Reason Name
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `BankStmntItemReprocessReason` |  |  |  | `String(2)` | Y | Reproc. Reason Code |  |  | S/4 only entity — no ECC CDC mapping |
| `Language` |  |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `BankStmntItemReprocessRsnName` |  |  |  | `String(60)` |  | Reprocessing Reason |  |  | S/4 only entity — no ECC CDC mapping |
