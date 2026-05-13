# JournalEntryCodes

> Source file: `sap-s4com-JournalEntryCodes-v1.json`

**Technical Name:** `IBUSTRANCAT` | **Data Category:** `DIMENSION` | **VDM Type:** `BASIC` | **Size:** `M`


## Entity: `BusinessTransactionCategory`

- **ABAP Name:** `I_BusinessTransactionCategory`
- **Technical Name:** `IBUSTRANCAT`
- **Label:** Business Transaction Category
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `BusinessTransactionCategory` |  |  | `String(4)` | Y | Business Transaction Category |  |  | S/4 only entity |
| `BusTransIsSubjToPerdControl` |  |  | `Boolean` |  | Period Control |  |  | S/4 only entity |
| `PeriodControlIsLedgerSpecific` |  |  | `Boolean` |  | Update by Ledger |  |  | S/4 only entity |
| `PeriodIsCheckedByLeadingLedger` |  |  | `Boolean` |  | Prd by Leading Ldg |  |  | S/4 only entity |


## Entity: `BusinessTransactionCategoryText`

- **ABAP Name:** `I_BusTransactionCategoryText`
- **Technical Name:** `IFIBUSTXCATT`
- **Label:** Business Transaction Category - Text
- **VDM Type:** `BASIC` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `Language` |  |  | `String(2)` | Y | Language Key |  | _Language | S/4 only entity |
| `BusinessTransactionCategory` |  |  | `String(4)` | Y | Business Transaction Category |  |  | S/4 only entity |
| `BusTransactionCategoryName` |  |  | `String(30)` |  | Business Transaction Category Name |  |  | S/4 only entity |


## Entity: `BusinessTransactionType`

- **ABAP Name:** `I_BusinessTransactionType`
- **Label:** Business Transaction Type
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `BusinessTransactionType` |  |  | `String(4)` | Y | Business Transaction Type |  |  | S/4 only entity |
| `BusinessTransactionCategory` |  |  | `String(4)` |  | Business Transaction Category |  | _BusinessTransactionCategory | S/4 only entity |
| `BusTransIsSubjToPerdControl` |  |  | `Boolean` |  | Period Control |  |  | S/4 only entity |
| `PeriodControlIsLedgerSpecific` |  |  | `Boolean` |  | Prd Ctrll By Ledger |  |  | S/4 only entity |
| `BusinessTransTypeIsInactive` |  |  | `Boolean` |  | Inactive |  |  | S/4 only entity |


## Entity: `BusinessTransactionTypeText`

- **ABAP Name:** `I_BusTransactionTypeText`
- **Label:** Business Transaction Type - Text
- **VDM Type:** `BASIC` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `Language` |  |  | `String(2)` | Y | Language Key |  | _Language | S/4 only entity |
| `BusinessTransactionType` |  |  | `String(4)` | Y | Business Transaction Type |  |  | S/4 only entity |
| `BusinessTransactionTypeName` |  |  | `String(30)` |  | Business Transaction Type Name |  |  | S/4 only entity |


## Entity: `FinancialTransactionType`

- **ABAP Name:** `I_FinancialTransactionType`
- **Label:** Financial Transaction Type
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `FinancialTransactionType` |  |  | `String(3)` | Y | Financial Transaction Type |  |  | S/4 only entity |
| `FinancialTransactionTypeGroup` |  |  | `String(3)` |  | Financial Transaction Type Group |  |  | S/4 only entity |
| `CarryForwardTransactionType` |  |  | `String(3)` |  | Carryfwd trans.type |  |  | S/4 only entity |
| `TransactionTypeIsDerived` |  |  | `Boolean` |  | Totals trans. type |  |  | S/4 only entity |
| `TransacTypeTotalsFormulaText` |  |  | `String(75)` |  | Totals formula |  |  | S/4 only entity |
| `BalanceCarryForwardIsFixed` |  |  | `Boolean` |  | No chngs to bal. c/f |  |  | S/4 only entity |
| `AcquisitionIsCurrentYearOnly` |  |  | `Boolean` |  | Yr of acq./curr. yr |  |  | S/4 only entity |
| `BrkdwnByYearsIsNotApplicable` |  |  | `Boolean` |  | Save AY - no |  |  | S/4 only entity |
| `RetirementTransactionType` |  |  | `String(3)` |  | TTy: Retirement |  |  | S/4 only entity |


## Entity: `FinancialTransactionTypeText`

- **ABAP Name:** `I_FinancialTransactionTypeT`
- **Label:** Financial Transaction Type - Text
- **VDM Type:** `BASIC` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `Language` |  |  | `String(2)` | Y | Language Key |  | _Language | S/4 only entity |
| `FinancialTransactionType` |  |  | `String(3)` | Y | Financial Transaction Type |  |  | S/4 only entity |
| `FinancialTransactionTypeName` |  |  | `String(20)` |  | Description |  |  | S/4 only entity |


## Entity: `JournalEntryCategory`

- **ABAP Name:** `I_AccountingDocumentCategory`
- **Label:** Accounting Document Category
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `AccountingDocumentCategory` |  |  | `String(1)` | Y | Document Status |  |  | S/4 only entity |
| `DomainValue` |  |  | `String(10)` |  | Lower Value |  |  | S/4 only entity |


## Entity: `JournalEntryCategoryText`

- **ABAP Name:** `I_AccountingDocumentCategoryT`
- **Label:** Accounting Document Category - Text
- **VDM Type:** `BASIC` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `AccountingDocumentCategory` |  |  | `String(1)` | Y | Document Status |  |  | S/4 only entity |
| `Language` |  |  | `String(2)` | Y | Language Key |  | _Language | S/4 only entity |
| `AccountingDocumentCategoryName` |  |  | `String(60)` |  | Name |  |  | S/4 only entity |
| `DomainValue` |  |  | `String(10)` |  | Lower Value |  |  | S/4 only entity |


## Entity: `JournalEntryType`

- **ABAP Name:** `I_AccountingDocumentType`
- **Label:** Journal Entry Type
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `AccountingDocumentType` |  |  | `String(2)` | Y | Journal Entry Type |  |  | S/4 only entity |
| `AccountingDocumentNumberRange` |  |  | `String(2)` |  | Number Range |  |  | S/4 only entity |
| `AuthorizationGroup` |  |  | `String(4)` |  | Authorization |  |  | S/4 only entity |
| `ExchangeRateType` |  |  | `String(4)` |  | Exchange Rate Type for FC Documents |  |  | S/4 only entity |
| `AllowedFinancialAccountTypes` |  |  | `String(5)` |  | Account Types |  |  | S/4 only entity |
| `CustomerPostingIsAllowed` |  |  | `Boolean` |  | Customer Posting Is Allowed |  |  | S/4 only entity |
| `SupplierPostingIsAllowed` |  |  | `Boolean` |  | Supplier Posting Is Allowed |  |  | S/4 only entity |


## Entity: `JournalEntryTypeText`

- **ABAP Name:** `I_AccountingDocumentTypeText`
- **Label:** Accounting Document Type - Text
- **VDM Type:** `BASIC` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `AccountingDocumentType` |  |  | `String(2)` | Y | Journal Entry Type |  |  | S/4 only entity |
| `Language` |  |  | `String(2)` | Y | Language Key |  | _Language | S/4 only entity |
| `AccountingDocumentTypeName` |  |  | `String(20)` |  | Journal Entry Type Name |  |  | S/4 only entity |


## Entity: `ReferenceDocumentType`

- **ABAP Name:** `I_ReferenceDocumentType`
- **Label:** Reference Document Type
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `ReferenceDocumentType` |  |  | `String(5)` | Y | Reference Document Type |  |  | S/4 only entity |


## Entity: `ReferenceDocumentTypeText`

- **ABAP Name:** `I_ReferenceDocumentTypeText`
- **Label:** Reference Document Type - Text
- **VDM Type:** `BASIC` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `ReferenceDocumentType` |  |  | `String(5)` | Y | Reference Document Type |  |  | S/4 only entity |
| `Language` |  |  | `String(2)` | Y | Language Key |  | _Language | S/4 only entity |
| `ReferenceDocumentTypeName` |  |  | `String(20)` |  | Object Type Name |  |  | S/4 only entity |
