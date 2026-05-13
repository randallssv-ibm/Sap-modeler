# CompanyCode

> Source file: `sap-s4com-CompanyCode-v1.json`


## Entity: `CompanyCode`

- **ABAP Name:** `I_CompanyCode`
- **Label:** Company Code
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `CompanyCode` |  |  |  | `String(4)` | Y | Company Code |  |  | S/4 only entity — no ECC CDC mapping |
| `CompanyCodeName` |  |  |  | `String(25)` |  | Company Name |  |  | S/4 only entity — no ECC CDC mapping |
| `CityName` |  |  |  | `String(25)` |  | City |  |  | S/4 only entity — no ECC CDC mapping |
| `Country` |  |  |  | `String(3)` |  | Country/Region Key |  |  | S/4 only entity — no ECC CDC mapping |
| `Currency` |  |  |  | `String(5)` |  | Currency |  |  | S/4 only entity — no ECC CDC mapping |
| `Language` |  |  |  | `String(2)` |  | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `ChartOfAccounts` |  |  |  | `String(4)` |  | Chart of Accounts |  |  | S/4 only entity — no ECC CDC mapping |
| `FiscalYearVariant` |  |  |  | `String(2)` |  | Fiscal Year Variant |  |  | S/4 only entity — no ECC CDC mapping |
| `Company` |  |  |  | `String(6)` |  | Company |  |  | S/4 only entity — no ECC CDC mapping |
| `CreditControlArea` |  |  |  | `String(4)` |  | Credit Control Area |  |  | S/4 only entity — no ECC CDC mapping |
| `CountryChartOfAccounts` |  |  |  | `String(4)` |  | Alternative COA |  |  | S/4 only entity — no ECC CDC mapping |
| `FinancialManagementArea` |  |  |  | `String(4)` |  | FM Area |  |  | S/4 only entity — no ECC CDC mapping |
| `AddressID` |  |  |  | `String(10)` |  | Address |  |  | S/4 only entity — no ECC CDC mapping |
| `TaxableEntity` |  |  |  | `String(4)` |  | Taxes on Sls/Purc. |  |  | S/4 only entity — no ECC CDC mapping |
| `VATRegistration` |  |  |  | `String(20)` |  | VAT Registration No. |  |  | S/4 only entity — no ECC CDC mapping |
| `ExtendedWhldgTaxIsActive` |  |  |  | `Boolean` |  | Extended WTax Active |  |  | S/4 only entity — no ECC CDC mapping |
| `ControllingArea` |  |  |  | `String(4)` |  | Controlling Area |  |  | S/4 only entity — no ECC CDC mapping |
| `FieldStatusVariant` |  |  |  | `String(4)` |  | Field Status Variant |  |  | S/4 only entity — no ECC CDC mapping |
| `NonTaxableTransactionTaxCode` |  |  |  | `String(2)` |  | Output Tax Code |  |  | S/4 only entity — no ECC CDC mapping |
| `DocDateIsUsedForTaxDetn` |  |  |  | `Boolean` |  | Tax Determ.with Doc.Date |  |  | S/4 only entity — no ECC CDC mapping |
| `TaxRptgDateIsActive` |  |  |  | `Boolean` |  | Tax Date |  |  | S/4 only entity — no ECC CDC mapping |
| `CashDiscountBaseAmtIsNetAmt` |  |  |  | `Boolean` |  | Net Discount Base |  |  | S/4 only entity — no ECC CDC mapping |
| `TransitPlant` |  |  |  | `String(4)` |  | Transit Plant |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `CompanyCodeCurrencyRole`

- **ABAP Name:** `I_Companycodecurrencyrole`
- **Label:** Currency Role of Company Code
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `CompanyCode` |  |  |  | `String(4)` | Y | Company Code |  | _CompanyCode | S/4 only entity — no ECC CDC mapping |
| `CurrencyRole` |  |  |  | `String(2)` | Y | Curr./Val. Type |  | _CurrencyRole | S/4 only entity — no ECC CDC mapping |
| `Currency` |  |  |  | `String(5)` |  | Currency |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `CompanyCodeCurrencyTranslation`

- **ABAP Name:** `I_CoCodeCrcyTranslationBasic`
- **Label:** Currency Translation
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `CompanyCode` |  |  |  | `String(4)` | Y | Company Code |  | _CompanyCode | S/4 only entity — no ECC CDC mapping |
| `TargetCurrencyRole` |  |  |  | `String(2)` | Y | Target Currency Role |  | _TargetCurrencyRole | S/4 only entity — no ECC CDC mapping |
| `TargetCurrency` |  |  |  | `String(5)` |  | To Currency |  |  | S/4 only entity — no ECC CDC mapping |
| `SourceCurrencyRole` |  |  |  | `String(2)` |  | Source Currency Role |  | _SourceCurrencyRole | S/4 only entity — no ECC CDC mapping |
| `ExchangeRateType` |  |  |  | `String(4)` |  | Exchange Rate Type |  |  | S/4 only entity — no ECC CDC mapping |
| `CurrencyTranslationDateType` |  |  |  | `String(1)` |  | Transltn Date Type |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `CompanyCodeHierarchy`

- **ABAP Name:** `I_CompanyCodeHierarchy`
- **Label:** Company Code Hierarchy
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `CompanyCodeHierarchy` |  |  |  | `String(42)` | Y | Company Code Hierarchy |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityEndDate` |  |  |  | `Date` | Y | Validity End Date |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityStartDate` |  |  |  | `Date` |  | Validity Start Date |  |  | S/4 only entity — no ECC CDC mapping |
| `LastChangedByUser` |  |  |  | `String(12)` |  | Last Changed By |  |  | S/4 only entity — no ECC CDC mapping |
| `LastChangeDateTime` |  |  |  | `DateTime` |  | Updated At |  |  | S/4 only entity — no ECC CDC mapping |
| `LastChangeTime` |  |  |  | `DateTime` |  | Updated At |  |  | S/4 only entity — no ECC CDC mapping |
| `HierarchyShortID` |  |  |  | `String(20)` |  | Hierarchy ID |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `CompanyCodeHierarchyNode`

- **ABAP Name:** `I_CompanyCodeHierNode`
- **Label:** Company Code Hierarchy Node
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `CompanyCodeHierarchy` |  |  |  | `String(42)` | Y | Company Code Hierarchy |  | _Hierarchy | S/4 only entity — no ECC CDC mapping |
| `HierarchyNode` |  |  |  | `String(50)` | Y | Node |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityEndDate` |  |  |  | `Date` | Y | Validity End Date |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityStartDate` |  |  |  | `Date` |  | Validity Start Date |  |  | S/4 only entity — no ECC CDC mapping |
| `ParentNode` |  |  |  | `String(50)` |  | Par. Node |  |  | S/4 only entity — no ECC CDC mapping |
| `HierarchyVersion` |  |  |  | `String(15)` |  | Version |  |  | S/4 only entity — no ECC CDC mapping |
| `CompanyCode` |  |  |  | `String(4)` |  | Company Code |  | _CompanyCode | S/4 only entity — no ECC CDC mapping |
| `SequenceNumber` |  |  |  | `String(56)` |  |  |  |  | S/4 only entity — no ECC CDC mapping |
| `HierarchyNodeSequence` |  |  |  | `String(6)` |  | Sequence Number |  |  | S/4 only entity — no ECC CDC mapping |
| `HierarchyNodeLevel` |  |  |  | `String(6)` |  | Hierarchy Level |  |  | S/4 only entity — no ECC CDC mapping |
| `NodeType` |  |  |  | `String(1)` |  | Node Type |  |  | S/4 only entity — no ECC CDC mapping |
| `HierarchyNodeVal` |  |  |  | `String(40)` |  | Value |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `CompanyCodeHierarchyNodeText`

- **ABAP Name:** `I_CompanyCodeHierNodeT`
- **Label:** Company Code Hierarchy Node - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `CompanyCodeHierarchy` |  |  |  | `String(42)` | Y | Company Code Hierarchy |  | _Hierarchy | S/4 only entity — no ECC CDC mapping |
| `HierarchyNode` |  |  |  | `String(50)` | Y | Node |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityEndDate` |  |  |  | `Date` | Y | Validity End Date |  |  | S/4 only entity — no ECC CDC mapping |
| `Language` |  |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `HierarchyNodeText` |  |  |  | `String(50)` |  | Description |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityStartDate` |  |  |  | `Date` |  | Validity Start Date |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `CompanyCodeHierarchyText`

- **ABAP Name:** `I_CompanyCodeHierarchyT`
- **Label:** Company Code Hierarchy - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `CompanyCodeHierarchy` |  |  |  | `String(42)` | Y | Company Code Hierarchy |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityEndDate` |  |  |  | `Date` | Y | Validity End Date |  |  | S/4 only entity — no ECC CDC mapping |
| `Language` |  |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityStartDate` |  |  |  | `Date` |  | Validity Start Date |  |  | S/4 only entity — no ECC CDC mapping |
| `CompanyCodeHierarchyName` |  |  |  | `String(50)` |  | Description |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `CurrencyRole`

- **ABAP Name:** `I_CurrencyRole`
- **Label:** Currency Role
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `CurrencyRole` |  |  |  | `String(2)` | Y | Curr./Val. Type |  |  | S/4 only entity — no ECC CDC mapping |
| `LegalCurrencyRole` |  |  |  | `String(2)` |  | Plain Currency Type |  |  | S/4 only entity — no ECC CDC mapping |
| `AccountingValuationView` |  |  |  | `String(1)` |  | Valuation View |  |  | S/4 only entity — no ECC CDC mapping |
| `AccountingValuationSubview` |  |  |  | `String(2)` |  | Subtype Val |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `CurrencyRoleText`

- **ABAP Name:** `I_CurrencyRoleText`
- **Label:** Currency Role - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `CurrencyRole` |  |  |  | `String(2)` | Y | Curr./Val. Type |  |  | S/4 only entity — no ECC CDC mapping |
| `Language` |  |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `CurrencyRoleName` |  |  |  | `String(60)` |  | Crcy. Role Name |  |  | S/4 only entity — no ECC CDC mapping |
