# CompanyCode

> Source file: `sap-s4com-CompanyCode-v1.json`


## Entity: `CompanyCode`

- **ABAP Name:** `I_CompanyCode`
- **Label:** Company Code
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `CompanyCode` | `CompanyCode` | `String(4)` | Y | Company Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `CompanyCodeName` | `CompanyCodeName` | `String(25)` |  | Company Name |  |  | S/4 only entity (no ECC CDC mapping) |
| `CityName` | `CityName` | `String(25)` |  | City |  |  | S/4 only entity (no ECC CDC mapping) |
| `Country` | `Country` | `String(3)` |  | Country/Region Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `Currency` | `Currency` | `String(5)` |  | Currency |  |  | S/4 only entity (no ECC CDC mapping) |
| `Language` | `Language` | `String(2)` |  | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `ChartOfAccounts` | `ChartOfAccounts` | `String(4)` |  | Chart of Accounts |  |  | S/4 only entity (no ECC CDC mapping) |
| `FiscalYearVariant` | `FiscalYearVariant` | `String(2)` |  | Fiscal Year Variant |  |  | S/4 only entity (no ECC CDC mapping) |
| `Company` | `Company` | `String(6)` |  | Company |  |  | S/4 only entity (no ECC CDC mapping) |
| `CreditControlArea` | `CreditControlArea` | `String(4)` |  | Credit Control Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `CountryChartOfAccounts` | `CountryChartOfAccounts` | `String(4)` |  | Alternative COA |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinancialManagementArea` | `FinancialManagementArea` | `String(4)` |  | FM Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `AddressID` | `AddressID` | `String(10)` |  | Address |  |  | S/4 only entity (no ECC CDC mapping) |
| `TaxableEntity` | `TaxableEntity` | `String(4)` |  | Taxes on Sls/Purc. |  |  | S/4 only entity (no ECC CDC mapping) |
| `VATRegistration` | `VATRegistration` | `String(20)` |  | VAT Registration No. |  |  | S/4 only entity (no ECC CDC mapping) |
| `ExtendedWhldgTaxIsActive` | `ExtendedWhldgTaxIsActive` | `Boolean` |  | Extended WTax Active |  |  | S/4 only entity (no ECC CDC mapping) |
| `ControllingArea` | `ControllingArea` | `String(4)` |  | Controlling Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `FieldStatusVariant` | `FieldStatusVariant` | `String(4)` |  | Field Status Variant |  |  | S/4 only entity (no ECC CDC mapping) |
| `NonTaxableTransactionTaxCode` | `NonTaxableTransactionTaxCode` | `String(2)` |  | Output Tax Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `DocDateIsUsedForTaxDetn` | `DocDateIsUsedForTaxDetn` | `Boolean` |  | Tax Determ.with Doc.Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `TaxRptgDateIsActive` | `TaxRptgDateIsActive` | `Boolean` |  | Tax Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `CashDiscountBaseAmtIsNetAmt` | `CashDiscountBaseAmtIsNetAmt` | `Boolean` |  | Net Discount Base |  |  | S/4 only entity (no ECC CDC mapping) |
| `TransitPlant` | `TransitPlant` | `String(4)` |  | Transit Plant |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `CompanyCodeCurrencyRole`

- **ABAP Name:** `I_Companycodecurrencyrole`
- **Label:** Currency Role of Company Code
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `CompanyCode` | `CompanyCode` | `String(4)` | Y | Company Code |  | _CompanyCode | S/4 only entity (no ECC CDC mapping) |
| `CurrencyRole` | `CurrencyRole` | `String(2)` | Y | Curr./Val. Type |  | _CurrencyRole | S/4 only entity (no ECC CDC mapping) |
| `Currency` | `Currency` | `String(5)` |  | Currency |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `CompanyCodeCurrencyTranslation`

- **ABAP Name:** `I_CoCodeCrcyTranslationBasic`
- **Label:** Currency Translation
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `CompanyCode` | `CompanyCode` | `String(4)` | Y | Company Code |  | _CompanyCode | S/4 only entity (no ECC CDC mapping) |
| `TargetCurrencyRole` | `TargetCurrencyRole` | `String(2)` | Y | Target Currency Role |  | _TargetCurrencyRole | S/4 only entity (no ECC CDC mapping) |
| `TargetCurrency` | `TargetCurrency` | `String(5)` |  | To Currency |  |  | S/4 only entity (no ECC CDC mapping) |
| `SourceCurrencyRole` | `SourceCurrencyRole` | `String(2)` |  | Source Currency Role |  | _SourceCurrencyRole | S/4 only entity (no ECC CDC mapping) |
| `ExchangeRateType` | `ExchangeRateType` | `String(4)` |  | Exchange Rate Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `CurrencyTranslationDateType` | `CurrencyTranslationDateType` | `String(1)` |  | Transltn Date Type |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `CompanyCodeHierarchy`

- **ABAP Name:** `I_CompanyCodeHierarchy`
- **Label:** Company Code Hierarchy
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `CompanyCodeHierarchy` | `CompanyCodeHierarchy` | `String(42)` | Y | Company Code Hierarchy |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityEndDate` | `ValidityEndDate` | `Date` | Y | Validity End Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityStartDate` | `ValidityStartDate` | `Date` |  | Validity Start Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `LastChangedByUser` | `LastChangedByUser` | `String(12)` |  | Last Changed By |  |  | S/4 only entity (no ECC CDC mapping) |
| `LastChangeDateTime` | `LastChangeDateTime` | `DateTime` |  | Updated At |  |  | S/4 only entity (no ECC CDC mapping) |
| `LastChangeTime` | `LastChangeTime` | `DateTime` |  | Updated At |  |  | S/4 only entity (no ECC CDC mapping) |
| `HierarchyShortID` | `HierarchyShortID` | `String(20)` |  | Hierarchy ID |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `CompanyCodeHierarchyNode`

- **ABAP Name:** `I_CompanyCodeHierNode`
- **Label:** Company Code Hierarchy Node
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `CompanyCodeHierarchy` | `CompanyCodeHierarchy` | `String(42)` | Y | Company Code Hierarchy |  | _Hierarchy | S/4 only entity (no ECC CDC mapping) |
| `HierarchyNode` | `HierarchyNode` | `String(50)` | Y | Node |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityEndDate` | `ValidityEndDate` | `Date` | Y | Validity End Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityStartDate` | `ValidityStartDate` | `Date` |  | Validity Start Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `ParentNode` | `ParentNode` | `String(50)` |  | Par. Node |  |  | S/4 only entity (no ECC CDC mapping) |
| `HierarchyVersion` | `HierarchyVersion` | `String(15)` |  | Version |  |  | S/4 only entity (no ECC CDC mapping) |
| `CompanyCode` | `CompanyCode` | `String(4)` |  | Company Code |  | _CompanyCode | S/4 only entity (no ECC CDC mapping) |
| `SequenceNumber` | `SequenceNumber` | `String(56)` |  |  |  |  | S/4 only entity (no ECC CDC mapping) |
| `HierarchyNodeSequence` | `HierarchyNodeSequence` | `String(6)` |  | Sequence Number |  |  | S/4 only entity (no ECC CDC mapping) |
| `HierarchyNodeLevel` | `HierarchyNodeLevel` | `String(6)` |  | Hierarchy Level |  |  | S/4 only entity (no ECC CDC mapping) |
| `NodeType` | `NodeType` | `String(1)` |  | Node Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `HierarchyNodeVal` | `HierarchyNodeVal` | `String(40)` |  | Value |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `CompanyCodeHierarchyNodeText`

- **ABAP Name:** `I_CompanyCodeHierNodeT`
- **Label:** Company Code Hierarchy Node - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `CompanyCodeHierarchy` | `CompanyCodeHierarchy` | `String(42)` | Y | Company Code Hierarchy |  | _Hierarchy | S/4 only entity (no ECC CDC mapping) |
| `HierarchyNode` | `HierarchyNode` | `String(50)` | Y | Node |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityEndDate` | `ValidityEndDate` | `Date` | Y | Validity End Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `HierarchyNodeText` | `HierarchyNodeText` | `String(50)` |  | Description |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityStartDate` | `ValidityStartDate` | `Date` |  | Validity Start Date |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `CompanyCodeHierarchyText`

- **ABAP Name:** `I_CompanyCodeHierarchyT`
- **Label:** Company Code Hierarchy - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `CompanyCodeHierarchy` | `CompanyCodeHierarchy` | `String(42)` | Y | Company Code Hierarchy |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityEndDate` | `ValidityEndDate` | `Date` | Y | Validity End Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityStartDate` | `ValidityStartDate` | `Date` |  | Validity Start Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `CompanyCodeHierarchyName` | `CompanyCodeHierarchyName` | `String(50)` |  | Description |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `CurrencyRole`

- **ABAP Name:** `I_CurrencyRole`
- **Label:** Currency Role
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `CurrencyRole` | `CurrencyRole` | `String(2)` | Y | Curr./Val. Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `LegalCurrencyRole` | `LegalCurrencyRole` | `String(2)` |  | Plain Currency Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `AccountingValuationView` | `AccountingValuationView` | `String(1)` |  | Valuation View |  |  | S/4 only entity (no ECC CDC mapping) |
| `AccountingValuationSubview` | `AccountingValuationSubview` | `String(2)` |  | Subtype Val |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `CurrencyRoleText`

- **ABAP Name:** `I_CurrencyRoleText`
- **Label:** Currency Role - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `CurrencyRole` | `CurrencyRole` | `String(2)` | Y | Curr./Val. Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `CurrencyRoleName` | `CurrencyRoleName` | `String(60)` |  | Crcy. Role Name |  |  | S/4 only entity (no ECC CDC mapping) |
