# InvoiceList

> Source file: `sap-s4com-InvoiceList-v1.json`


## Entity: `InvoiceList`

- **ABAP CDS Name:** `I_InvoiceList`
- **Label:** Invoice List
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** VFRK

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `InvoiceList` |  |  |  |  |  | `String(10)` | Y | Invoice List |  |  |
| `SDDocumentCategory` |  |  |  |  |  | `String(4)` |  | SD Document Category |  |  |
| `InvoiceListType` |  |  |  |  |  | `String(4)` |  | Invoice List Type |  |  |
| `CreatedByUser` |  |  |  |  |  | `String(12)` |  | Created By |  |  |
| `CreationDate` |  |  |  |  |  | `Date` |  | Created On |  |  |
| `CreationTime` |  |  |  |  |  | `String(6)` |  | Time |  |  |
| `LastChangeDate` |  |  |  |  |  | `Date` |  | Changed On |  |  |
| `LastChangeDateTime` |  |  |  |  |  | `Timestamp` |  | Time Stamp |  |  |
| `LogicalSystem` |  |  |  |  |  | `String(10)` |  | Logical System |  |  |
| `SalesOrganization` |  |  |  |  |  | `String(4)` |  | Sales Organization |  |  |
| `DistributionChannel` |  |  |  |  |  | `String(2)` |  | Distribution Channel |  |  |
| `Division` |  |  |  |  |  | `String(2)` |  | Division |  |  |
| `InvoiceListBillingDate` |  |  |  |  |  | `Date` |  | Billing Date |  |  |
| `InvoiceListIsCancelled` |  |  |  |  |  | `Boolean` |  | Canceled |  |  |
| `CancelledInvoiceList` |  |  |  |  |  | `String(10)` |  | Cancld Invc. List |  |  |
| `InvoiceListCombinationCriteria` |  |  |  |  |  | `String(40)` |  | Combination Criteria |  |  |
| `TotalNetAmount` |  |  |  |  |  | `Decimal(34,4)` |  | Net Value | TransactionCurrency |  |
| `TransactionCurrency` |  |  |  |  |  | `String(5)` |  | Document Currency |  |  |
| `StatisticsCurrency` |  |  |  |  |  | `String(5)` |  | Statistics Currency |  |  |
| `TotalTaxAmount` |  |  |  |  |  | `Decimal(34,4)` |  | Tax Amount | TransactionCurrency |  |
| `CustomerPriceGroup` |  |  |  |  |  | `String(2)` |  | Customer Price Group |  |  |
| `PriceListType` |  |  |  |  |  | `String(2)` |  | Price List Type |  |  |
| `TaxDepartureCountry` |  |  |  |  |  | `String(3)` |  | Tax Departure C/R |  |  |
| `VATRegistration` |  |  |  |  |  | `String(20)` |  | VAT Registration No. |  |  |
| `VATRegistrationOrigin` |  |  |  |  |  | `String(1)` |  | Origin Sales Tax No. |  |  |
| `VATRegistrationCountry` |  |  |  |  |  | `String(3)` |  | Ctry/Rgn Sls Tax No. |  |  |
| `CustomerTaxClassification1` |  |  |  |  |  | `String(1)` |  | Tax Class.1 Customer |  |  |
| `CustomerTaxClassification2` |  |  |  |  |  | `String(1)` |  | Tax Class.2 Customer |  |  |
| `CustomerTaxClassification3` |  |  |  |  |  | `String(1)` |  | Tax Class.3 Customer |  |  |
| `CustomerTaxClassification4` |  |  |  |  |  | `String(1)` |  | Tax Class.4 Customer |  |  |
| `CustomerTaxClassification5` |  |  |  |  |  | `String(1)` |  | Tax Class.5 Customer |  |  |
| `CustomerTaxClassification6` |  |  |  |  |  | `String(1)` |  | Tax Class.6 Customer |  |  |
| `CustomerTaxClassification7` |  |  |  |  |  | `String(1)` |  | Tax Class.7 Customer |  |  |
| `CustomerTaxClassification8` |  |  |  |  |  | `String(1)` |  | Tax Class.8 Customer |  |  |
| `CustomerTaxClassification9` |  |  |  |  |  | `String(1)` |  | Tax Class.9 Customer |  |  |
| `IsEUTriangularDeal` |  |  |  |  |  | `Boolean` |  | EU Triangular Deal |  |  |
| `SDPricingProcedure` |  |  |  |  |  | `String(6)` |  | Pricing Procedure |  |  |
| `ShippingCondition` |  |  |  |  |  | `String(2)` |  | Shipping Conditions |  |  |
| `IncotermsVersion` |  |  |  |  |  | `String(4)` |  | Incoterms Version |  |  |
| `IncotermsClassification` |  |  |  |  |  | `String(3)` |  | Incoterms |  |  |
| `IncotermsTransferLocation` |  |  |  |  |  | `String(28)` |  | Incoterms (Part 2) |  |  |
| `IncotermsLocation1` |  |  |  |  |  | `String(70)` |  | Incoterms Location 1 |  |  |
| `IncotermsLocation2` |  |  |  |  |  | `String(70)` |  | Incoterms Location 2 |  |  |
| `PayerParty` |  |  |  |  |  | `String(10)` |  | Payer |  |  |
| `ContractAccount` |  |  |  |  |  | `String(12)` |  | Contract Account |  |  |
| `CustomerPaymentTerms` |  |  |  |  |  | `String(4)` |  | Terms of Payment |  |  |
| `PaymentMethod` |  |  |  |  |  | `String(1)` |  | Payment Method |  |  |
| `PaymentReference` |  |  |  |  |  | `String(30)` |  | Payment Reference |  |  |
| `FixedValueDate` |  |  |  |  |  | `Date` |  | Fixed Value Date |  |  |
| `AdditionalValueDays` |  |  |  |  |  | `String(2)` |  | Addit. Value Days |  |  |
| `SEPAMandate` |  |  |  |  |  | `String(35)` |  | Mandate Reference |  |  |
| `CompanyCode` |  |  |  |  |  | `String(4)` |  | Company Code |  |  |
| `FiscalYear` |  |  |  |  |  | `String(4)` |  | Fiscal Year |  |  |
| `AccountingDocument` |  |  |  |  |  | `String(10)` |  | Document Number |  |  |
| `FiscalPeriod` |  |  |  |  |  | `String(3)` |  | Posting Period |  |  |
| `CustomerAccountAssignmentGroup` |  |  |  |  |  | `String(2)` |  | Acct Assmt Grp Cust. |  |  |
| `AccountingExchangeRateIsSet` |  |  |  |  |  | `Boolean` |  | Set Exchange Rate |  |  |
| `AccountingExchangeRate` |  |  |  |  |  | `Decimal(9,5)` |  | Accounting Exchange Rate |  |  |
| `ExchangeRateDate` |  |  |  |  |  | `Date` |  | Translation Date |  |  |
| `ExchangeRateType` |  |  |  |  |  | `String(4)` |  | Exchange Rate Type |  |  |
| `DocumentReferenceID` |  |  |  |  |  | `String(16)` |  | Reference |  |  |
| `AssignmentReference` |  |  |  |  |  | `String(18)` |  | Assignment |  |  |
| `DunningArea` |  |  |  |  |  | `String(2)` |  | Dunning Area |  |  |
| `DunningBlockingReason` |  |  |  |  |  | `String(1)` |  | Dunning Block |  |  |
| `DunningKey` |  |  |  |  |  | `String(1)` |  | Dunning Key |  |  |
| `InternalFinancialDocument` |  |  |  |  |  | `String(10)` |  | Financial Doc. No. |  |  |
| `SoldToParty` |  |  |  |  |  | `String(10)` |  | Sold-to Party |  |  |
| `PartnerCompany` |  |  |  |  |  | `String(6)` |  | Trading Partner No. |  |  |
| `PurchaseOrderByCustomer` |  |  |  |  |  | `String(35)` |  | Customer Reference |  |  |
| `CustomerGroup` |  |  |  |  |  | `String(2)` |  | Customer Group |  |  |
| `Country` |  |  |  |  |  | `String(3)` |  | Dest. Country/Region |  |  |
| `CityCode` |  |  |  |  |  | `String(4)` |  | City Code |  |  |
| `SalesDistrict` |  |  |  |  |  | `String(6)` |  | Sales District |  |  |
| `Region` |  |  |  |  |  | `String(3)` |  | Region |  |  |
| `County` |  |  |  |  |  | `String(3)` |  | County Code |  |  |
| `CreditControlArea` |  |  |  |  |  | `String(4)` |  | Credit Control Area |  |  |
| `PricingDocument` |  |  |  |  |  | `String(10)` |  | Doc. Condition No. |  |  |
| `OverallSDProcessStatus` |  |  |  |  |  | `String(1)` |  | Overall Status |  |  |
| `AccountingPostingStatus` |  |  |  |  |  | `String(1)` |  | Posting Status |  |  |
| `AccountingTransferStatus` |  |  |  |  |  | `String(1)` |  | Posting Status |  |  |
| `OvrlItmGeneralIncompletionSts` |  |  |  |  |  | `String(1)` |  | All Items |  |  |
| `OverallPricingIncompletionSts` |  |  |  |  |  | `String(1)` |  | Pricing – All Items |  |  |


## Entity: `InvoiceListItem`

- **ABAP CDS Name:** `I_InvoiceListItem`
- **Label:** Invoice List Item
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** VFRP

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `InvoiceList` |  |  |  |  |  | `String(10)` | Y | Invoice List |  |  |
| `InvoiceListItem` |  |  |  |  |  | `String(6)` | Y | Item |  |  |
| `BillingDocument` |  |  |  |  |  | `String(10)` |  | Billing Document |  |  |
| `NetAmount` |  |  |  |  |  | `Decimal(34,4)` |  | Net Value | TransactionCurrency |  |
| `TaxAmount` |  |  |  |  |  | `Decimal(34,4)` |  | Tax Amount | TransactionCurrency |  |
| `GrossAmount` |  |  |  |  |  | `Decimal(34,4)` |  | Gross Amount | TransactionCurrency |  |
| `RemunerationNetAmount` |  |  |  |  |  | `Decimal(34,4)` |  | Factoring Discount | TransactionCurrency |  |
| `RemunerationTaxAmount` |  |  |  |  |  | `Decimal(34,4)` |  | Fact. Discount Tax | TransactionCurrency |  |
| `TransactionCurrency` |  |  |  |  |  | `String(5)` |  | Document Currency |  |  |
| `PricingIsIncomplete` |  |  |  |  |  | `Boolean` |  | Pricing |  |  |
| `SoldToParty` |  |  |  |  |  | `String(10)` |  | Sold-to Party |  |  |
| `LogicalSystem` |  |  |  |  |  | `String(10)` |  | Logical System |  |  |
