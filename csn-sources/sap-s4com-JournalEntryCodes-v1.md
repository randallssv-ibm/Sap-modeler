# JournalEntryCodes

> Source file: `sap-s4com-JournalEntryCodes-v1.json`

**Technical Name:** `IBUSTRANCAT` | **Data Category:** `DIMENSION` | **VDM Type:** `BASIC` | **Size:** `M`


## Entity: `BusinessTransactionCategory`

- **ABAP Name:** `I_BusinessTransactionCategory`
- **Technical Name:** `IBUSTRANCAT`
- **Label:** Business Transaction Category
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `BusinessTransactionCategory` | `BusinessTransactionCategory` | `String(4)` | Y | Business Transaction Category |  |  | S/4 only entity (no ECC CDC mapping) |
| `BusTransIsSubjToPerdControl` | `BusTransIsSubjToPerdControl` | `Boolean` |  | Period Control |  |  | S/4 only entity (no ECC CDC mapping) |
| `PeriodControlIsLedgerSpecific` | `PeriodControlIsLedgerSpecific` | `Boolean` |  | Update by Ledger |  |  | S/4 only entity (no ECC CDC mapping) |
| `PeriodIsCheckedByLeadingLedger` | `PeriodIsCheckedByLeadingLedger` | `Boolean` |  | Prd by Leading Ldg |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `BusinessTransactionCategoryText`

- **ABAP Name:** `I_BusTransactionCategoryText`
- **Technical Name:** `IFIBUSTXCATT`
- **Label:** Business Transaction Category - Text
- **VDM Type:** `BASIC` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Language` | `Language` | `String(2)` | Y | Language Key |  | _Language | S/4 only entity (no ECC CDC mapping) |
| `BusinessTransactionCategory` | `BusinessTransactionCategory` | `String(4)` | Y | Business Transaction Category |  |  | S/4 only entity (no ECC CDC mapping) |
| `BusTransactionCategoryName` | `BusTransactionCategoryName` | `String(30)` |  | Business Transaction Category Name |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `BusinessTransactionType`

- **ABAP Name:** `I_BusinessTransactionType`
- **Label:** Business Transaction Type
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `BusinessTransactionType` | `BusinessTransactionType` | `String(4)` | Y | Business Transaction Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `BusinessTransactionCategory` | `BusinessTransactionCategory` | `String(4)` |  | Business Transaction Category |  | _BusinessTransactionCategory | S/4 only entity (no ECC CDC mapping) |
| `BusTransIsSubjToPerdControl` | `BusTransIsSubjToPerdControl` | `Boolean` |  | Period Control |  |  | S/4 only entity (no ECC CDC mapping) |
| `PeriodControlIsLedgerSpecific` | `PeriodControlIsLedgerSpecific` | `Boolean` |  | Prd Ctrll By Ledger |  |  | S/4 only entity (no ECC CDC mapping) |
| `BusinessTransTypeIsInactive` | `BusinessTransTypeIsInactive` | `Boolean` |  | Inactive |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `BusinessTransactionTypeText`

- **ABAP Name:** `I_BusTransactionTypeText`
- **Label:** Business Transaction Type - Text
- **VDM Type:** `BASIC` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Language` | `Language` | `String(2)` | Y | Language Key |  | _Language | S/4 only entity (no ECC CDC mapping) |
| `BusinessTransactionType` | `BusinessTransactionType` | `String(4)` | Y | Business Transaction Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `BusinessTransactionTypeName` | `BusinessTransactionTypeName` | `String(30)` |  | Business Transaction Type Name |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `FinancialTransactionType`

- **ABAP Name:** `I_FinancialTransactionType`
- **Label:** Financial Transaction Type
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `FinancialTransactionType` | `FinancialTransactionType` | `String(3)` | Y | Financial Transaction Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinancialTransactionTypeGroup` | `FinancialTransactionTypeGroup` | `String(3)` |  | Financial Transaction Type Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `CarryForwardTransactionType` | `CarryForwardTransactionType` | `String(3)` |  | Carryfwd trans.type |  |  | S/4 only entity (no ECC CDC mapping) |
| `TransactionTypeIsDerived` | `TransactionTypeIsDerived` | `Boolean` |  | Totals trans. type |  |  | S/4 only entity (no ECC CDC mapping) |
| `TransacTypeTotalsFormulaText` | `TransacTypeTotalsFormulaText` | `String(75)` |  | Totals formula |  |  | S/4 only entity (no ECC CDC mapping) |
| `BalanceCarryForwardIsFixed` | `BalanceCarryForwardIsFixed` | `Boolean` |  | No chngs to bal. c/f |  |  | S/4 only entity (no ECC CDC mapping) |
| `AcquisitionIsCurrentYearOnly` | `AcquisitionIsCurrentYearOnly` | `Boolean` |  | Yr of acq./curr. yr |  |  | S/4 only entity (no ECC CDC mapping) |
| `BrkdwnByYearsIsNotApplicable` | `BrkdwnByYearsIsNotApplicable` | `Boolean` |  | Save AY - no |  |  | S/4 only entity (no ECC CDC mapping) |
| `RetirementTransactionType` | `RetirementTransactionType` | `String(3)` |  | TTy: Retirement |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `FinancialTransactionTypeText`

- **ABAP Name:** `I_FinancialTransactionTypeT`
- **Label:** Financial Transaction Type - Text
- **VDM Type:** `BASIC` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Language` | `Language` | `String(2)` | Y | Language Key |  | _Language | S/4 only entity (no ECC CDC mapping) |
| `FinancialTransactionType` | `FinancialTransactionType` | `String(3)` | Y | Financial Transaction Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinancialTransactionTypeName` | `FinancialTransactionTypeName` | `String(20)` |  | Description |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `JournalEntryCategory`

- **ABAP Name:** `I_AccountingDocumentCategory`
- **Label:** Accounting Document Category
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `AccountingDocumentCategory` | `AccountingDocumentCategory` | `String(1)` | Y | Document Status |  |  | S/4 only entity (no ECC CDC mapping) |
| `DomainValue` | `DomainValue` | `String(10)` |  | Lower Value |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `JournalEntryCategoryText`

- **ABAP Name:** `I_AccountingDocumentCategoryT`
- **Label:** Accounting Document Category - Text
- **VDM Type:** `BASIC` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `AccountingDocumentCategory` | `AccountingDocumentCategory` | `String(1)` | Y | Document Status |  |  | S/4 only entity (no ECC CDC mapping) |
| `Language` | `Language` | `String(2)` | Y | Language Key |  | _Language | S/4 only entity (no ECC CDC mapping) |
| `AccountingDocumentCategoryName` | `AccountingDocumentCategoryName` | `String(60)` |  | Name |  |  | S/4 only entity (no ECC CDC mapping) |
| `DomainValue` | `DomainValue` | `String(10)` |  | Lower Value |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `JournalEntryType`

- **ABAP Name:** `I_AccountingDocumentType`
- **Label:** Journal Entry Type
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `AccountingDocumentType` | `AccountingDocumentType` | `String(2)` | Y | Journal Entry Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `AccountingDocumentNumberRange` | `AccountingDocumentNumberRange` | `String(2)` |  | Number Range |  |  | S/4 only entity (no ECC CDC mapping) |
| `AuthorizationGroup` | `AuthorizationGroup` | `String(4)` |  | Authorization |  |  | S/4 only entity (no ECC CDC mapping) |
| `ExchangeRateType` | `ExchangeRateType` | `String(4)` |  | Exchange Rate Type for FC Documents |  |  | S/4 only entity (no ECC CDC mapping) |
| `AllowedFinancialAccountTypes` | `AllowedFinancialAccountTypes` | `String(5)` |  | Account Types |  |  | S/4 only entity (no ECC CDC mapping) |
| `CustomerPostingIsAllowed` | `CustomerPostingIsAllowed` | `Boolean` |  | Customer Posting Is Allowed |  |  | S/4 only entity (no ECC CDC mapping) |
| `SupplierPostingIsAllowed` | `SupplierPostingIsAllowed` | `Boolean` |  | Supplier Posting Is Allowed |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `JournalEntryTypeText`

- **ABAP Name:** `I_AccountingDocumentTypeText`
- **Label:** Accounting Document Type - Text
- **VDM Type:** `BASIC` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `AccountingDocumentType` | `AccountingDocumentType` | `String(2)` | Y | Journal Entry Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `Language` | `Language` | `String(2)` | Y | Language Key |  | _Language | S/4 only entity (no ECC CDC mapping) |
| `AccountingDocumentTypeName` | `AccountingDocumentTypeName` | `String(20)` |  | Journal Entry Type Name |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `ReferenceDocumentType`

- **ABAP Name:** `I_ReferenceDocumentType`
- **Label:** Reference Document Type
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `ReferenceDocumentType` | `ReferenceDocumentType` | `String(5)` | Y | Reference Document Type |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `ReferenceDocumentTypeText`

- **ABAP Name:** `I_ReferenceDocumentTypeText`
- **Label:** Reference Document Type - Text
- **VDM Type:** `BASIC` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `ReferenceDocumentType` | `ReferenceDocumentType` | `String(5)` | Y | Reference Document Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `Language` | `Language` | `String(2)` | Y | Language Key |  | _Language | S/4 only entity (no ECC CDC mapping) |
| `ReferenceDocumentTypeName` | `ReferenceDocumentTypeName` | `String(20)` |  | Object Type Name |  |  | S/4 only entity (no ECC CDC mapping) |
