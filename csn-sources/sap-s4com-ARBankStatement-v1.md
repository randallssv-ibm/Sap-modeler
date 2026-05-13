# ARBankStatement

> Source file: `sap-s4com-ARBankStatement-v1.json`


## Entity: `ARBankStatement`

- **ABAP Name:** `I_BankStatement`
- **Label:** Header of a bank statement
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `BankStatementShortID` | `BankStatementShortID` | `String(8)` | Y | Short Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `CompanyCode` | `CompanyCode` | `String(4)` |  | Company Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `HouseBank` | `HouseBank` | `String(5)` |  | House Bank |  |  | S/4 only entity (no ECC CDC mapping) |
| `HouseBankAccount` | `HouseBankAccount` | `String(5)` |  | House Bank Acct ID |  |  | S/4 only entity (no ECC CDC mapping) |
| `BankStatement` | `BankStatement` | `String(18)` |  | Bank Statement Number |  |  | S/4 only entity (no ECC CDC mapping) |
| `BankStatementDate` | `BankStatementDate` | `Date` |  | Bank Statement Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `BankStatementStatus` | `BankStatementStatus` | `String(1)` |  | Statement Status |  |  | S/4 only entity (no ECC CDC mapping) |
| `BankStatementPageNumber` | `BankStatementPageNumber` | `String(5)` |  | Page No. (5 Digits) |  |  | S/4 only entity (no ECC CDC mapping) |
| `Currency` | `Currency` | `String(5)` |  | Currency |  |  | S/4 only entity (no ECC CDC mapping) |
| `OpeningBalanceIsInterim` | `OpeningBalanceIsInterim` | `Boolean` |  | Interim Opening |  |  | S/4 only entity (no ECC CDC mapping) |
| `ClosingBalanceIsInterim` | `ClosingBalanceIsInterim` | `Boolean` |  | Interim Closing |  |  | S/4 only entity (no ECC CDC mapping) |
| `OpeningBalanceAmtInTransCrcy` | `OpeningBalanceAmtInTransCrcy` | `Decimal(34,4)` |  | Opening Balance | Currency |  | S/4 only entity (no ECC CDC mapping) |
| `ClosingBalanceAmtInTransCrcy` | `ClosingBalanceAmtInTransCrcy` | `Decimal(34,4)` |  | Ending Bal.Amount | Currency |  | S/4 only entity (no ECC CDC mapping) |
| `InterimOpenBalAmtInTransCrcy` | `InterimOpenBalAmtInTransCrcy` | `Decimal(34,4)` |  | Interim Opening Balance | Currency |  | S/4 only entity (no ECC CDC mapping) |
| `InterimClsgBalAmtInTransCrcy` | `InterimClsgBalAmtInTransCrcy` | `Decimal(34,4)` |  | Interim Closing Balance | Currency |  | S/4 only entity (no ECC CDC mapping) |
| `PaymentTransactionTypeGroup` | `PaymentTransactionTypeGroup` | `String(8)` |  | Transaction Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `CreatedByUser` | `CreatedByUser` | `String(12)` |  | EB User |  |  | S/4 only entity (no ECC CDC mapping) |
| `BankStatementIsManuallyCreated` | `BankStatementIsManuallyCreated` | `Boolean` |  | BS created manually |  |  | S/4 only entity (no ECC CDC mapping) |
| `BankStatementFormat` | `BankStatementFormat` | `String(2)` |  | Statement Format |  |  | S/4 only entity (no ECC CDC mapping) |
| `BankStatementImportDate` | `BankStatementImportDate` | `Date` |  | Statement Import Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `BankStatementImportTime` | `BankStatementImportTime` | `String(6)` |  | Stmnt. Import Time |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `BankStmntItemReprocessReason`

- **ABAP Name:** `I_BankStmntItemReprocessReason`
- **Label:** Bank Statement Item Reprocessing Reason
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `BankStmntItemReprocessReason` | `BankStmntItemReprocessReason` | `String(2)` | Y | Reproc. Reason Code |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `BankStmntItmReprocessRsnText`

- **ABAP Name:** `I_BankStmntItmReprocessRsnName`
- **Label:** Bank Stmnt Item Reprocessing Reason Name
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `BankStmntItemReprocessReason` | `BankStmntItemReprocessReason` | `String(2)` | Y | Reproc. Reason Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `BankStmntItemReprocessRsnName` | `BankStmntItemReprocessRsnName` | `String(60)` |  | Reprocessing Reason |  |  | S/4 only entity (no ECC CDC mapping) |
