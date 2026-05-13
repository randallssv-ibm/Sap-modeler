# JournalEntryCodes

> Source file: `sap-s4com-JournalEntryCodes-v1.json`

**Technical Name:** `IBUSTRANCAT` | **Data Category:** `DIMENSION` | **VDM Type:** `BASIC` | **Size:** `M`


## Entity: `BusinessTransactionCategory`

- **ABAP Name:** `I_BusinessTransactionCategory`
- **Technical Name:** `IBUSTRANCAT`
- **Label:** Business Transaction Category
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `BusinessTransactionCategory` | `FIS_BTTYPE` | `BTTYPE` |  | `String(4)` | Y | Business Transaction Category |  |  | S/4 only entity — no ECC CDC mapping |
| `BusTransIsSubjToPerdControl` |  |  |  | `Boolean` |  | Period Control |  |  | S/4 only entity — no ECC CDC mapping |
| `PeriodControlIsLedgerSpecific` |  |  |  | `Boolean` |  | Update by Ledger |  |  | S/4 only entity — no ECC CDC mapping |
| `PeriodIsCheckedByLeadingLedger` |  |  |  | `Boolean` |  | Prd by Leading Ldg |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `BusinessTransactionCategoryText`

- **ABAP Name:** `I_BusTransactionCategoryText`
- **Technical Name:** `IFIBUSTXCATT`
- **Label:** Business Transaction Category - Text
- **VDM Type:** `BASIC` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Language` | `SPRAS` | `SPRAS` |  | `String(2)` | Y | Language Key |  | _Language | S/4 only entity — no ECC CDC mapping |
| `BusinessTransactionCategory` | `FIS_BTTYPE` | `BTTYPE` |  | `String(4)` | Y | Business Transaction Category |  |  | S/4 only entity — no ECC CDC mapping |
| `BusTransactionCategoryName` | `FINS_BTTYPE_TXT` | `BTTYPE_TXT` |  | `String(30)` |  | Business Transaction Category Name |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `BusinessTransactionType`

- **ABAP Name:** `I_BusinessTransactionType`
- **Label:** Business Transaction Type
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `BusinessTransactionType` | `FIS_CUSTBTTYPE` | `CUSTBTTYPE` |  | `String(4)` | Y | Business Transaction Type |  |  | S/4 only entity — no ECC CDC mapping |
| `BusinessTransactionCategory` | `FIS_BTTYPE` | `BTTYPE` |  | `String(4)` |  | Business Transaction Category |  | _BusinessTransactionCategory | S/4 only entity — no ECC CDC mapping |
| `BusTransIsSubjToPerdControl` |  |  |  | `Boolean` |  | Period Control |  |  | S/4 only entity — no ECC CDC mapping |
| `PeriodControlIsLedgerSpecific` |  |  |  | `Boolean` |  | Prd Ctrll By Ledger |  |  | S/4 only entity — no ECC CDC mapping |
| `BusinessTransTypeIsInactive` | `FINS_CBTTYPE_INACTIVE` | `CBTTYPE_INACTIVE` |  | `Boolean` |  | Inactive |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `BusinessTransactionTypeText`

- **ABAP Name:** `I_BusTransactionTypeText`
- **Label:** Business Transaction Type - Text
- **VDM Type:** `BASIC` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Language` | `SPRAS` | `SPRAS` |  | `String(2)` | Y | Language Key |  | _Language | S/4 only entity — no ECC CDC mapping |
| `BusinessTransactionType` | `FIS_CUSTBTTYPE` | `CUSTBTTYPE` |  | `String(4)` | Y | Business Transaction Type |  |  | S/4 only entity — no ECC CDC mapping |
| `BusinessTransactionTypeName` | `FINS_CUSTBTTYPE_TEXT` | `CUSTBTTYPE_TEXT` |  | `String(30)` |  | Business Transaction Type Name |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `FinancialTransactionType`

- **ABAP Name:** `I_FinancialTransactionType`
- **Label:** Financial Transaction Type
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `FinancialTransactionType` | `FIS_RMVCT` | `RMVCT` |  | `String(3)` | Y | Financial Transaction Type |  |  | S/4 only entity — no ECC CDC mapping |
| `FinancialTransactionTypeGroup` | `FIS_RMVCT_GRP` | `RMVCT_GRP` |  | `String(3)` |  | Financial Transaction Type Group |  |  | S/4 only entity — no ECC CDC mapping |
| `CarryForwardTransactionType` | `RMVCT_CFO` | `RMVCT_CFO` |  | `String(3)` |  | Carryfwd trans.type |  |  | S/4 only entity — no ECC CDC mapping |
| `TransactionTypeIsDerived` | `KZ_TOIND` | `KZ_TOIND` |  | `Boolean` |  | Totals trans. type |  |  | S/4 only entity — no ECC CDC mapping |
| `TransacTypeTotalsFormulaText` | `RMVCT_SUM` | `RMVCT_SUM` |  | `String(75)` |  | Totals formula |  |  | S/4 only entity — no ECC CDC mapping |
| `BalanceCarryForwardIsFixed` | `KZ_CFIND` | `KZ_CFIND` |  | `Boolean` |  | No chngs to bal. c/f |  |  | S/4 only entity — no ECC CDC mapping |
| `AcquisitionIsCurrentYearOnly` | `KZ_CYIND` | `KZ_CYIND` |  | `Boolean` |  | Yr of acq./curr. yr |  |  | S/4 only entity — no ECC CDC mapping |
| `BrkdwnByYearsIsNotApplicable` | `KZ_CYDBI` | `KZ_CYDBI` |  | `Boolean` |  | Save AY - no |  |  | S/4 only entity — no ECC CDC mapping |
| `RetirementTransactionType` | `RMVCT_RET` | `RMVCT_RET` |  | `String(3)` |  | TTy: Retirement |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `FinancialTransactionTypeText`

- **ABAP Name:** `I_FinancialTransactionTypeT`
- **Label:** Financial Transaction Type - Text
- **VDM Type:** `BASIC` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Language` | `SPRAS` | `SPRAS` |  | `String(2)` | Y | Language Key |  | _Language | S/4 only entity — no ECC CDC mapping |
| `FinancialTransactionType` | `FIS_RMVCT` | `RMVCT` |  | `String(3)` | Y | Financial Transaction Type |  |  | S/4 only entity — no ECC CDC mapping |
| `FinancialTransactionTypeName` | `RMVCT_TXT` | `RMVCT_TXT` |  | `String(20)` |  | Description |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `JournalEntryCategory`

- **ABAP Name:** `I_AccountingDocumentCategory`
- **Label:** Accounting Document Category
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `AccountingDocumentCategory` | `FARP_BSTAT_D` | `BSTAT` |  | `String(1)` | Y | Document Status |  |  | S/4 only entity — no ECC CDC mapping |
| `DomainValue` | `DOMVALUE_L` | `DOMVALUE_L` |  | `String(10)` |  | Lower Value |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `JournalEntryCategoryText`

- **ABAP Name:** `I_AccountingDocumentCategoryT`
- **Label:** Accounting Document Category - Text
- **VDM Type:** `BASIC` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `AccountingDocumentCategory` | `FARP_BSTAT_D` | `BSTAT` |  | `String(1)` | Y | Document Status |  |  | S/4 only entity — no ECC CDC mapping |
| `Language` | `SPRAS` | `SPRAS` |  | `String(2)` | Y | Language Key |  | _Language | S/4 only entity — no ECC CDC mapping |
| `AccountingDocumentCategoryName` | `FIS_VAL_TEXT` | `VAL_TEXT` |  | `String(60)` |  | Name |  |  | S/4 only entity — no ECC CDC mapping |
| `DomainValue` | `DOMVALUE_L` | `DOMVALUE_L` |  | `String(10)` |  | Lower Value |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `JournalEntryType`

- **ABAP Name:** `I_AccountingDocumentType`
- **Label:** Journal Entry Type
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `AccountingDocumentType` | `FARP_BLART` | `BLART` |  | `String(2)` | Y | Journal Entry Type |  |  | S/4 only entity — no ECC CDC mapping |
| `AccountingDocumentNumberRange` | `NUMKR` | `NUMKR` |  | `String(2)` |  | Number Range |  |  | S/4 only entity — no ECC CDC mapping |
| `AuthorizationGroup` | `BRGRU` | `BRGRU` |  | `String(4)` |  | Authorization |  |  | S/4 only entity — no ECC CDC mapping |
| `ExchangeRateType` | `KURST_003` | `KURST_003` |  | `String(4)` |  | Exchange Rate Type for FC Documents |  |  | S/4 only entity — no ECC CDC mapping |
| `AllowedFinancialAccountTypes` | `KOARS_003` | `KOARS_003` |  | `String(5)` |  | Account Types |  |  | S/4 only entity — no ECC CDC mapping |
| `CustomerPostingIsAllowed` | `FIS_XKOAD` | `XKOAD` |  | `Boolean` |  | Customer Posting Is Allowed |  |  | S/4 only entity — no ECC CDC mapping |
| `SupplierPostingIsAllowed` | `FIS_XKOAK` | `XKOAK` |  | `Boolean` |  | Supplier Posting Is Allowed |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `JournalEntryTypeText`

- **ABAP Name:** `I_AccountingDocumentTypeText`
- **Label:** Accounting Document Type - Text
- **VDM Type:** `BASIC` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `AccountingDocumentType` | `FARP_BLART` | `BLART` |  | `String(2)` | Y | Journal Entry Type |  |  | S/4 only entity — no ECC CDC mapping |
| `Language` | `SPRAS` | `SPRAS` |  | `String(2)` | Y | Language Key |  | _Language | S/4 only entity — no ECC CDC mapping |
| `AccountingDocumentTypeName` | `FARP_LTEXT_003T` | `LTEXT_003T` |  | `String(20)` |  | Journal Entry Type Name |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `ReferenceDocumentType`

- **ABAP Name:** `I_ReferenceDocumentType`
- **Label:** Reference Document Type
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `ReferenceDocumentType` | `FIS_AWTYP` | `AWTYP` |  | `String(5)` | Y | Reference Document Type |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `ReferenceDocumentTypeText`

- **ABAP Name:** `I_ReferenceDocumentTypeText`
- **Label:** Reference Document Type - Text
- **VDM Type:** `BASIC` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `ReferenceDocumentType` | `FIS_AWTYP` | `AWTYP` |  | `String(5)` | Y | Reference Document Type |  |  | S/4 only entity — no ECC CDC mapping |
| `Language` | `SPRAS` | `SPRAS` |  | `String(2)` | Y | Language Key |  | _Language | S/4 only entity — no ECC CDC mapping |
| `ReferenceDocumentTypeName` | `TEXT_TYP` | `TEXT_TYP` |  | `String(20)` |  | Object Type Name |  |  | S/4 only entity — no ECC CDC mapping |
