# CompanyCode

> Source file: `sap-s4com-CompanyCode-v1.json`


## Entity: `CompanyCode`

- **ABAP CDS Name:** `I_CompanyCode`
- **Label:** Company Code
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** T001

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `CompanyCode` |  | `T001` | `BUKRS` |  |  | `String(4)` | Y | Company Code |  |  |
| `CompanyCodeName` |  | `T001` | `BUTXT` |  |  | `String(25)` |  | Company Name |  |  |
| `CityName` |  |  |  |  |  | `String(25)` |  | City |  |  |
| `Country` |  | `T001` | `LAND1` |  |  | `String(3)` |  | Country/Region Key |  |  |
| `Currency` |  | `T001` | `WAERS` |  |  | `String(5)` |  | Currency |  |  |
| `Language` |  | `T001` | `SPRAS` |  |  | `String(2)` |  | Language Key |  |  |
| `ChartOfAccounts` |  | `T001` | `KTOPL` |  |  | `String(4)` |  | Chart of Accounts |  |  |
| `FiscalYearVariant` |  | `T001` | `PERIV` |  |  | `String(2)` |  | Fiscal Year Variant |  |  |
| `Company` |  |  |  |  |  | `String(6)` |  | Company |  |  |
| `CreditControlArea` |  | `T001` | `KKBER` |  |  | `String(4)` |  | Credit Control Area |  |  |
| `CountryChartOfAccounts` |  | `T001` | `LKONT` |  |  | `String(4)` |  | Alternative COA |  |  |
| `FinancialManagementArea` |  |  |  |  |  | `String(4)` |  | FM Area |  |  |
| `AddressID` |  | `T001` | `ADRNR` |  |  | `String(10)` |  | Address |  |  |
| `TaxableEntity` |  |  |  |  |  | `String(4)` |  | Taxes on Sls/Purc. |  |  |
| `VATRegistration` |  |  |  |  |  | `String(20)` |  | VAT Registration No. |  |  |
| `ExtendedWhldgTaxIsActive` |  |  |  |  |  | `Boolean` |  | Extended WTax Active |  |  |
| `ControllingArea` |  | `T001` | `KOKRS` |  |  | `String(4)` |  | Controlling Area |  |  |
| `FieldStatusVariant` |  |  |  |  |  | `String(4)` |  | Field Status Variant |  |  |
| `NonTaxableTransactionTaxCode` |  |  |  |  |  | `String(2)` |  | Output Tax Code |  |  |
| `DocDateIsUsedForTaxDetn` |  |  |  |  |  | `Boolean` |  | Tax Determ.with Doc.Date |  |  |
| `TaxRptgDateIsActive` |  |  |  |  |  | `Boolean` |  | Tax Date |  |  |
| `CashDiscountBaseAmtIsNetAmt` |  |  |  |  |  | `Boolean` |  | Net Discount Base |  |  |
| `TransitPlant` |  |  |  |  |  | `String(4)` |  | Transit Plant |  |  |


## Entity: `CompanyCodeCurrencyRole`

- **ABAP CDS Name:** `I_Companycodecurrencyrole`
- **Label:** Currency Role of Company Code
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** T001

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `CompanyCode` |  |  |  |  |  | `String(4)` | Y | Company Code |  |  |
| `CurrencyRole` |  |  |  |  |  | `String(2)` | Y | Curr./Val. Type |  |  |
| `Currency` |  |  |  |  |  | `String(5)` |  | Currency |  |  |


## Entity: `CompanyCodeCurrencyTranslation`

- **ABAP CDS Name:** `I_CoCodeCrcyTranslationBasic`
- **Label:** Currency Translation
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** T001

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `CompanyCode` |  |  |  |  |  | `String(4)` | Y | Company Code |  |  |
| `TargetCurrencyRole` |  |  |  |  |  | `String(2)` | Y | Target Currency Role |  |  |
| `TargetCurrency` |  |  |  |  |  | `String(5)` |  | To Currency |  |  |
| `SourceCurrencyRole` |  |  |  |  |  | `String(2)` |  | Source Currency Role |  |  |
| `ExchangeRateType` |  |  |  |  |  | `String(4)` |  | Exchange Rate Type |  |  |
| `CurrencyTranslationDateType` |  |  |  |  |  | `String(1)` |  | Transltn Date Type |  |  |


## Entity: `CompanyCodeHierarchy`

- **ABAP CDS Name:** `I_CompanyCodeHierarchy`
- **Label:** Company Code Hierarchy
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `CompanyCodeHierarchy` |  |  |  |  |  | `String(42)` | Y | Company Code Hierarchy |  | S/4 only entity |
| `ValidityEndDate` |  |  |  |  |  | `Date` | Y | Validity End Date |  | S/4 only entity |
| `ValidityStartDate` |  |  |  |  |  | `Date` |  | Validity Start Date |  | S/4 only entity |
| `LastChangedByUser` |  |  |  |  |  | `String(12)` |  | Last Changed By |  | S/4 only entity |
| `LastChangeDateTime` |  |  |  |  |  | `DateTime` |  | Updated At |  | S/4 only entity |
| `LastChangeTime` |  |  |  |  |  | `DateTime` |  | Updated At |  | S/4 only entity |
| `HierarchyShortID` |  |  |  |  |  | `String(20)` |  | Hierarchy ID |  | S/4 only entity |


## Entity: `CompanyCodeHierarchyNode`

- **ABAP CDS Name:** `I_CompanyCodeHierNode`
- **Label:** Company Code Hierarchy Node
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `CompanyCodeHierarchy` |  |  |  |  |  | `String(42)` | Y | Company Code Hierarchy |  | S/4 only entity |
| `HierarchyNode` |  |  |  |  |  | `String(50)` | Y | Node |  | S/4 only entity |
| `ValidityEndDate` |  |  |  |  |  | `Date` | Y | Validity End Date |  | S/4 only entity |
| `ValidityStartDate` |  |  |  |  |  | `Date` |  | Validity Start Date |  | S/4 only entity |
| `ParentNode` |  |  |  |  |  | `String(50)` |  | Par. Node |  | S/4 only entity |
| `HierarchyVersion` |  |  |  |  |  | `String(15)` |  | Version |  | S/4 only entity |
| `CompanyCode` |  |  |  |  |  | `String(4)` |  | Company Code |  | S/4 only entity |
| `SequenceNumber` |  |  |  |  |  | `String(56)` |  |  |  | S/4 only entity |
| `HierarchyNodeSequence` |  |  |  |  |  | `String(6)` |  | Sequence Number |  | S/4 only entity |
| `HierarchyNodeLevel` |  |  |  |  |  | `String(6)` |  | Hierarchy Level |  | S/4 only entity |
| `NodeType` |  |  |  |  |  | `String(1)` |  | Node Type |  | S/4 only entity |
| `HierarchyNodeVal` |  |  |  |  |  | `String(40)` |  | Value |  | S/4 only entity |


## Entity: `CompanyCodeHierarchyNodeText`

- **ABAP CDS Name:** `I_CompanyCodeHierNodeT`
- **Label:** Company Code Hierarchy Node - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `CompanyCodeHierarchy` |  |  |  |  |  | `String(42)` | Y | Company Code Hierarchy |  | S/4 only entity |
| `HierarchyNode` |  |  |  |  |  | `String(50)` | Y | Node |  | S/4 only entity |
| `ValidityEndDate` |  |  |  |  |  | `Date` | Y | Validity End Date |  | S/4 only entity |
| `Language` |  |  |  |  |  | `String(2)` | Y | Language Key |  | S/4 only entity |
| `HierarchyNodeText` |  |  |  |  |  | `String(50)` |  | Description |  | S/4 only entity |
| `ValidityStartDate` |  |  |  |  |  | `Date` |  | Validity Start Date |  | S/4 only entity |


## Entity: `CompanyCodeHierarchyText`

- **ABAP CDS Name:** `I_CompanyCodeHierarchyT`
- **Label:** Company Code Hierarchy - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `CompanyCodeHierarchy` |  |  |  |  |  | `String(42)` | Y | Company Code Hierarchy |  | S/4 only entity |
| `ValidityEndDate` |  |  |  |  |  | `Date` | Y | Validity End Date |  | S/4 only entity |
| `Language` |  |  |  |  |  | `String(2)` | Y | Language Key |  | S/4 only entity |
| `ValidityStartDate` |  |  |  |  |  | `Date` |  | Validity Start Date |  | S/4 only entity |
| `CompanyCodeHierarchyName` |  |  |  |  |  | `String(50)` |  | Description |  | S/4 only entity |


## Entity: `CurrencyRole`

- **ABAP CDS Name:** `I_CurrencyRole`
- **Label:** Currency Role
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `CurrencyRole` |  |  |  |  |  | `String(2)` | Y | Curr./Val. Type |  | S/4 only entity |
| `LegalCurrencyRole` |  |  |  |  |  | `String(2)` |  | Plain Currency Type |  | S/4 only entity |
| `AccountingValuationView` |  |  |  |  |  | `String(1)` |  | Valuation View |  | S/4 only entity |
| `AccountingValuationSubview` |  |  |  |  |  | `String(2)` |  | Subtype Val |  | S/4 only entity |


## Entity: `CurrencyRoleText`

- **ABAP CDS Name:** `I_CurrencyRoleText`
- **Label:** Currency Role - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `CurrencyRole` |  |  |  |  |  | `String(2)` | Y | Curr./Val. Type |  | S/4 only entity |
| `Language` |  |  |  |  |  | `String(2)` | Y | Language Key |  | S/4 only entity |
| `CurrencyRoleName` |  |  |  |  |  | `String(60)` |  | Crcy. Role Name |  | S/4 only entity |
