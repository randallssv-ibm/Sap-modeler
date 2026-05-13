# JournalEntryCodes

> Source file: `sap-s4com-JournalEntryCodes-v1.json`

**Technical Name:** `IBUSTRANCAT` | **Data Category:** `DIMENSION` | **VDM Type:** `BASIC` | **Size:** `M`


## Entity: `BusinessTransactionCategory`

- **ABAP CDS Name:** `I_BusinessTransactionCategory`
- **Technical Name:** `IBUSTRANCAT`
- **Label:** Business Transaction Category
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `BusinessTransactionCategory` | `FIS_BTTYPE` |  |  |  |  | `String(4)` | Y | Business Transaction Category |  | S/4 only entity |
| `BusTransIsSubjToPerdControl` |  |  |  |  |  | `Boolean` |  | Period Control |  | S/4 only entity |
| `PeriodControlIsLedgerSpecific` |  |  |  |  |  | `Boolean` |  | Update by Ledger |  | S/4 only entity |
| `PeriodIsCheckedByLeadingLedger` |  |  |  |  |  | `Boolean` |  | Prd by Leading Ldg |  | S/4 only entity |


## Entity: `BusinessTransactionCategoryText`

- **ABAP CDS Name:** `I_BusTransactionCategoryText`
- **Technical Name:** `IFIBUSTXCATT`
- **Label:** Business Transaction Category - Text
- **VDM Type:** `BASIC` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Language` | `SPRAS` |  |  |  |  | `String(2)` | Y | Language Key |  | S/4 only entity |
| `BusinessTransactionCategory` | `FIS_BTTYPE` |  |  |  |  | `String(4)` | Y | Business Transaction Category |  | S/4 only entity |
| `BusTransactionCategoryName` | `FINS_BTTYPE_TXT` |  |  |  |  | `String(30)` |  | Business Transaction Category Name |  | S/4 only entity |


## Entity: `BusinessTransactionType`

- **ABAP CDS Name:** `I_BusinessTransactionType`
- **Label:** Business Transaction Type
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `BusinessTransactionType` | `FIS_CUSTBTTYPE` |  |  |  |  | `String(4)` | Y | Business Transaction Type |  | S/4 only entity |
| `BusinessTransactionCategory` | `FIS_BTTYPE` |  |  |  |  | `String(4)` |  | Business Transaction Category |  | S/4 only entity |
| `BusTransIsSubjToPerdControl` |  |  |  |  |  | `Boolean` |  | Period Control |  | S/4 only entity |
| `PeriodControlIsLedgerSpecific` |  |  |  |  |  | `Boolean` |  | Prd Ctrll By Ledger |  | S/4 only entity |
| `BusinessTransTypeIsInactive` | `FINS_CBTTYPE_INACTIVE` |  |  |  |  | `Boolean` |  | Inactive |  | S/4 only entity |


## Entity: `BusinessTransactionTypeText`

- **ABAP CDS Name:** `I_BusTransactionTypeText`
- **Label:** Business Transaction Type - Text
- **VDM Type:** `BASIC` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Language` | `SPRAS` |  |  |  |  | `String(2)` | Y | Language Key |  | S/4 only entity |
| `BusinessTransactionType` | `FIS_CUSTBTTYPE` |  |  |  |  | `String(4)` | Y | Business Transaction Type |  | S/4 only entity |
| `BusinessTransactionTypeName` | `FINS_CUSTBTTYPE_TEXT` |  |  |  |  | `String(30)` |  | Business Transaction Type Name |  | S/4 only entity |


## Entity: `FinancialTransactionType`

- **ABAP CDS Name:** `I_FinancialTransactionType`
- **Label:** Financial Transaction Type
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `FinancialTransactionType` | `FIS_RMVCT` |  |  |  |  | `String(3)` | Y | Financial Transaction Type |  | S/4 only entity |
| `FinancialTransactionTypeGroup` | `FIS_RMVCT_GRP` |  |  |  |  | `String(3)` |  | Financial Transaction Type Group |  | S/4 only entity |
| `CarryForwardTransactionType` | `RMVCT_CFO` |  |  |  |  | `String(3)` |  | Carryfwd trans.type |  | S/4 only entity |
| `TransactionTypeIsDerived` | `KZ_TOIND` |  |  |  |  | `Boolean` |  | Totals trans. type |  | S/4 only entity |
| `TransacTypeTotalsFormulaText` | `RMVCT_SUM` |  |  |  |  | `String(75)` |  | Totals formula |  | S/4 only entity |
| `BalanceCarryForwardIsFixed` | `KZ_CFIND` |  |  |  |  | `Boolean` |  | No chngs to bal. c/f |  | S/4 only entity |
| `AcquisitionIsCurrentYearOnly` | `KZ_CYIND` |  |  |  |  | `Boolean` |  | Yr of acq./curr. yr |  | S/4 only entity |
| `BrkdwnByYearsIsNotApplicable` | `KZ_CYDBI` |  |  |  |  | `Boolean` |  | Save AY - no |  | S/4 only entity |
| `RetirementTransactionType` | `RMVCT_RET` |  |  |  |  | `String(3)` |  | TTy: Retirement |  | S/4 only entity |


## Entity: `FinancialTransactionTypeText`

- **ABAP CDS Name:** `I_FinancialTransactionTypeT`
- **Label:** Financial Transaction Type - Text
- **VDM Type:** `BASIC` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Language` | `SPRAS` |  |  |  |  | `String(2)` | Y | Language Key |  | S/4 only entity |
| `FinancialTransactionType` | `FIS_RMVCT` |  |  |  |  | `String(3)` | Y | Financial Transaction Type |  | S/4 only entity |
| `FinancialTransactionTypeName` | `RMVCT_TXT` |  |  |  |  | `String(20)` |  | Description |  | S/4 only entity |


## Entity: `JournalEntryCategory`

- **ABAP CDS Name:** `I_AccountingDocumentCategory`
- **Label:** Accounting Document Category
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `AccountingDocumentCategory` | `FARP_BSTAT_D` |  |  |  |  | `String(1)` | Y | Document Status |  | S/4 only entity |
| `DomainValue` | `DOMVALUE_L` |  |  |  |  | `String(10)` |  | Lower Value |  | S/4 only entity |


## Entity: `JournalEntryCategoryText`

- **ABAP CDS Name:** `I_AccountingDocumentCategoryT`
- **Label:** Accounting Document Category - Text
- **VDM Type:** `BASIC` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `AccountingDocumentCategory` | `FARP_BSTAT_D` |  |  |  |  | `String(1)` | Y | Document Status |  | S/4 only entity |
| `Language` | `SPRAS` |  |  |  |  | `String(2)` | Y | Language Key |  | S/4 only entity |
| `AccountingDocumentCategoryName` | `FIS_VAL_TEXT` |  |  |  |  | `String(60)` |  | Name |  | S/4 only entity |
| `DomainValue` | `DOMVALUE_L` |  |  |  |  | `String(10)` |  | Lower Value |  | S/4 only entity |


## Entity: `JournalEntryType`

- **ABAP CDS Name:** `I_AccountingDocumentType`
- **Label:** Journal Entry Type
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** T003, T003T

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `AccountingDocumentType` | `FARP_BLART` |  |  |  |  | `String(2)` | Y | Journal Entry Type |  |  |
| `AccountingDocumentNumberRange` | `NUMKR` |  |  |  |  | `String(2)` |  | Number Range |  |  |
| `AuthorizationGroup` | `BRGRU` |  |  |  |  | `String(4)` |  | Authorization |  |  |
| `ExchangeRateType` | `KURST_003` |  |  |  |  | `String(4)` |  | Exchange Rate Type for FC Documents |  |  |
| `AllowedFinancialAccountTypes` | `KOARS_003` |  |  |  |  | `String(5)` |  | Account Types |  |  |
| `CustomerPostingIsAllowed` | `FIS_XKOAD` |  |  |  |  | `Boolean` |  | Customer Posting Is Allowed |  |  |
| `SupplierPostingIsAllowed` | `FIS_XKOAK` |  |  |  |  | `Boolean` |  | Supplier Posting Is Allowed |  |  |


## Entity: `JournalEntryTypeText`

- **ABAP CDS Name:** `I_AccountingDocumentTypeText`
- **Label:** Accounting Document Type - Text
- **VDM Type:** `BASIC` | **Data Category:** ``
- **ECC Source Tables:** T003T

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `AccountingDocumentType` | `FARP_BLART` |  |  |  |  | `String(2)` | Y | Journal Entry Type |  |  |
| `Language` | `SPRAS` |  |  |  |  | `String(2)` | Y | Language Key |  |  |
| `AccountingDocumentTypeName` | `FARP_LTEXT_003T` |  |  |  |  | `String(20)` |  | Journal Entry Type Name |  |  |


## Entity: `ReferenceDocumentType`

- **ABAP CDS Name:** `I_ReferenceDocumentType`
- **Label:** Reference Document Type
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `ReferenceDocumentType` | `FIS_AWTYP` |  |  |  |  | `String(5)` | Y | Reference Document Type |  | S/4 only entity |


## Entity: `ReferenceDocumentTypeText`

- **ABAP CDS Name:** `I_ReferenceDocumentTypeText`
- **Label:** Reference Document Type - Text
- **VDM Type:** `BASIC` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `ReferenceDocumentType` | `FIS_AWTYP` |  |  |  |  | `String(5)` | Y | Reference Document Type |  | S/4 only entity |
| `Language` | `SPRAS` |  |  |  |  | `String(2)` | Y | Language Key |  | S/4 only entity |
| `ReferenceDocumentTypeName` | `TEXT_TYP` |  |  |  |  | `String(20)` |  | Object Type Name |  | S/4 only entity |
