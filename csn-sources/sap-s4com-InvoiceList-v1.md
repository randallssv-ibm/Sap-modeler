# InvoiceList

> Source file: `sap-s4com-InvoiceList-v1.json`


## Entity: `InvoiceList`

- **ABAP CDS Name:** `I_InvoiceList`
- **Label:** Invoice List
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `InvoiceList` |  |  |  |  |  | `String(10)` | Y | Invoice List |  | S/4 only entity |
| `SDDocumentCategory` |  |  |  |  |  | `String(4)` |  | SD Document Category |  | S/4 only entity |
| `InvoiceListType` |  |  |  |  |  | `String(4)` |  | Invoice List Type |  | S/4 only entity |
| `CreatedByUser` |  |  |  |  |  | `String(12)` |  | Created By |  | S/4 only entity |
| `CreationDate` |  |  |  |  |  | `Date` |  | Created On |  | S/4 only entity |
| `CreationTime` |  |  |  |  |  | `String(6)` |  | Time |  | S/4 only entity |
| `LastChangeDate` |  |  |  |  |  | `Date` |  | Changed On |  | S/4 only entity |
| `LastChangeDateTime` |  |  |  |  |  | `Timestamp` |  | Time Stamp |  | S/4 only entity |
| `LogicalSystem` |  |  |  |  |  | `String(10)` |  | Logical System |  | S/4 only entity |
| `SalesOrganization` |  |  |  |  |  | `String(4)` |  | Sales Organization |  | S/4 only entity |
| `DistributionChannel` |  |  |  |  |  | `String(2)` |  | Distribution Channel |  | S/4 only entity |
| `Division` |  |  |  |  |  | `String(2)` |  | Division |  | S/4 only entity |
| `InvoiceListBillingDate` |  |  |  |  |  | `Date` |  | Billing Date |  | S/4 only entity |
| `InvoiceListIsCancelled` |  |  |  |  |  | `Boolean` |  | Canceled |  | S/4 only entity |
| `CancelledInvoiceList` |  |  |  |  |  | `String(10)` |  | Cancld Invc. List |  | S/4 only entity |
| `InvoiceListCombinationCriteria` |  |  |  |  |  | `String(40)` |  | Combination Criteria |  | S/4 only entity |
| `TotalNetAmount` |  |  |  |  |  | `Decimal(34,4)` |  | Net Value | TransactionCurrency | S/4 only entity |
| `TransactionCurrency` |  |  |  |  |  | `String(5)` |  | Document Currency |  | S/4 only entity |
| `StatisticsCurrency` |  |  |  |  |  | `String(5)` |  | Statistics Currency |  | S/4 only entity |
| `TotalTaxAmount` |  |  |  |  |  | `Decimal(34,4)` |  | Tax Amount | TransactionCurrency | S/4 only entity |
| `CustomerPriceGroup` |  |  |  |  |  | `String(2)` |  | Customer Price Group |  | S/4 only entity |
| `PriceListType` |  |  |  |  |  | `String(2)` |  | Price List Type |  | S/4 only entity |
| `TaxDepartureCountry` |  |  |  |  |  | `String(3)` |  | Tax Departure C/R |  | S/4 only entity |
| `VATRegistration` |  |  |  |  |  | `String(20)` |  | VAT Registration No. |  | S/4 only entity |
| `VATRegistrationOrigin` |  |  |  |  |  | `String(1)` |  | Origin Sales Tax No. |  | S/4 only entity |
| `VATRegistrationCountry` |  |  |  |  |  | `String(3)` |  | Ctry/Rgn Sls Tax No. |  | S/4 only entity |
| `CustomerTaxClassification1` |  |  |  |  |  | `String(1)` |  | Tax Class.1 Customer |  | S/4 only entity |
| `CustomerTaxClassification2` |  |  |  |  |  | `String(1)` |  | Tax Class.2 Customer |  | S/4 only entity |
| `CustomerTaxClassification3` |  |  |  |  |  | `String(1)` |  | Tax Class.3 Customer |  | S/4 only entity |
| `CustomerTaxClassification4` |  |  |  |  |  | `String(1)` |  | Tax Class.4 Customer |  | S/4 only entity |
| `CustomerTaxClassification5` |  |  |  |  |  | `String(1)` |  | Tax Class.5 Customer |  | S/4 only entity |
| `CustomerTaxClassification6` |  |  |  |  |  | `String(1)` |  | Tax Class.6 Customer |  | S/4 only entity |
| `CustomerTaxClassification7` |  |  |  |  |  | `String(1)` |  | Tax Class.7 Customer |  | S/4 only entity |
| `CustomerTaxClassification8` |  |  |  |  |  | `String(1)` |  | Tax Class.8 Customer |  | S/4 only entity |
| `CustomerTaxClassification9` |  |  |  |  |  | `String(1)` |  | Tax Class.9 Customer |  | S/4 only entity |
| `IsEUTriangularDeal` |  |  |  |  |  | `Boolean` |  | EU Triangular Deal |  | S/4 only entity |
| `SDPricingProcedure` |  |  |  |  |  | `String(6)` |  | Pricing Procedure |  | S/4 only entity |
| `ShippingCondition` |  |  |  |  |  | `String(2)` |  | Shipping Conditions |  | S/4 only entity |
| `IncotermsVersion` |  |  |  |  |  | `String(4)` |  | Incoterms Version |  | S/4 only entity |
| `IncotermsClassification` |  |  |  |  |  | `String(3)` |  | Incoterms |  | S/4 only entity |
| `IncotermsTransferLocation` |  |  |  |  |  | `String(28)` |  | Incoterms (Part 2) |  | S/4 only entity |
| `IncotermsLocation1` |  |  |  |  |  | `String(70)` |  | Incoterms Location 1 |  | S/4 only entity |
| `IncotermsLocation2` |  |  |  |  |  | `String(70)` |  | Incoterms Location 2 |  | S/4 only entity |
| `PayerParty` |  |  |  |  |  | `String(10)` |  | Payer |  | S/4 only entity |
| `ContractAccount` |  |  |  |  |  | `String(12)` |  | Contract Account |  | S/4 only entity |
| `CustomerPaymentTerms` |  |  |  |  |  | `String(4)` |  | Terms of Payment |  | S/4 only entity |
| `PaymentMethod` |  |  |  |  |  | `String(1)` |  | Payment Method |  | S/4 only entity |
| `PaymentReference` |  |  |  |  |  | `String(30)` |  | Payment Reference |  | S/4 only entity |
| `FixedValueDate` |  |  |  |  |  | `Date` |  | Fixed Value Date |  | S/4 only entity |
| `AdditionalValueDays` |  |  |  |  |  | `String(2)` |  | Addit. Value Days |  | S/4 only entity |
| `SEPAMandate` |  |  |  |  |  | `String(35)` |  | Mandate Reference |  | S/4 only entity |
| `CompanyCode` |  |  |  |  |  | `String(4)` |  | Company Code |  | S/4 only entity |
| `FiscalYear` |  |  |  |  |  | `String(4)` |  | Fiscal Year |  | S/4 only entity |
| `AccountingDocument` |  |  |  |  |  | `String(10)` |  | Document Number |  | S/4 only entity |
| `FiscalPeriod` |  |  |  |  |  | `String(3)` |  | Posting Period |  | S/4 only entity |
| `CustomerAccountAssignmentGroup` |  |  |  |  |  | `String(2)` |  | Acct Assmt Grp Cust. |  | S/4 only entity |
| `AccountingExchangeRateIsSet` |  |  |  |  |  | `Boolean` |  | Set Exchange Rate |  | S/4 only entity |
| `AccountingExchangeRate` |  |  |  |  |  | `Decimal(9,5)` |  | Accounting Exchange Rate |  | S/4 only entity |
| `ExchangeRateDate` |  |  |  |  |  | `Date` |  | Translation Date |  | S/4 only entity |
| `ExchangeRateType` |  |  |  |  |  | `String(4)` |  | Exchange Rate Type |  | S/4 only entity |
| `DocumentReferenceID` |  |  |  |  |  | `String(16)` |  | Reference |  | S/4 only entity |
| `AssignmentReference` |  |  |  |  |  | `String(18)` |  | Assignment |  | S/4 only entity |
| `DunningArea` |  |  |  |  |  | `String(2)` |  | Dunning Area |  | S/4 only entity |
| `DunningBlockingReason` |  |  |  |  |  | `String(1)` |  | Dunning Block |  | S/4 only entity |
| `DunningKey` |  |  |  |  |  | `String(1)` |  | Dunning Key |  | S/4 only entity |
| `InternalFinancialDocument` |  |  |  |  |  | `String(10)` |  | Financial Doc. No. |  | S/4 only entity |
| `SoldToParty` |  |  |  |  |  | `String(10)` |  | Sold-to Party |  | S/4 only entity |
| `PartnerCompany` |  |  |  |  |  | `String(6)` |  | Trading Partner No. |  | S/4 only entity |
| `PurchaseOrderByCustomer` |  |  |  |  |  | `String(35)` |  | Customer Reference |  | S/4 only entity |
| `CustomerGroup` |  |  |  |  |  | `String(2)` |  | Customer Group |  | S/4 only entity |
| `Country` |  |  |  |  |  | `String(3)` |  | Dest. Country/Region |  | S/4 only entity |
| `CityCode` |  |  |  |  |  | `String(4)` |  | City Code |  | S/4 only entity |
| `SalesDistrict` |  |  |  |  |  | `String(6)` |  | Sales District |  | S/4 only entity |
| `Region` |  |  |  |  |  | `String(3)` |  | Region |  | S/4 only entity |
| `County` |  |  |  |  |  | `String(3)` |  | County Code |  | S/4 only entity |
| `CreditControlArea` |  |  |  |  |  | `String(4)` |  | Credit Control Area |  | S/4 only entity |
| `PricingDocument` |  |  |  |  |  | `String(10)` |  | Doc. Condition No. |  | S/4 only entity |
| `OverallSDProcessStatus` |  |  |  |  |  | `String(1)` |  | Overall Status |  | S/4 only entity |
| `AccountingPostingStatus` |  |  |  |  |  | `String(1)` |  | Posting Status |  | S/4 only entity |
| `AccountingTransferStatus` |  |  |  |  |  | `String(1)` |  | Posting Status |  | S/4 only entity |
| `OvrlItmGeneralIncompletionSts` |  |  |  |  |  | `String(1)` |  | All Items |  | S/4 only entity |
| `OverallPricingIncompletionSts` |  |  |  |  |  | `String(1)` |  | Pricing – All Items |  | S/4 only entity |


## Entity: `InvoiceListItem`

- **ABAP CDS Name:** `I_InvoiceListItem`
- **Label:** Invoice List Item
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `InvoiceList` |  |  |  |  |  | `String(10)` | Y | Invoice List |  | S/4 only entity |
| `InvoiceListItem` |  |  |  |  |  | `String(6)` | Y | Item |  | S/4 only entity |
| `BillingDocument` |  |  |  |  |  | `String(10)` |  | Billing Document |  | S/4 only entity |
| `NetAmount` |  |  |  |  |  | `Decimal(34,4)` |  | Net Value | TransactionCurrency | S/4 only entity |
| `TaxAmount` |  |  |  |  |  | `Decimal(34,4)` |  | Tax Amount | TransactionCurrency | S/4 only entity |
| `GrossAmount` |  |  |  |  |  | `Decimal(34,4)` |  | Gross Amount | TransactionCurrency | S/4 only entity |
| `RemunerationNetAmount` |  |  |  |  |  | `Decimal(34,4)` |  | Factoring Discount | TransactionCurrency | S/4 only entity |
| `RemunerationTaxAmount` |  |  |  |  |  | `Decimal(34,4)` |  | Fact. Discount Tax | TransactionCurrency | S/4 only entity |
| `TransactionCurrency` |  |  |  |  |  | `String(5)` |  | Document Currency |  | S/4 only entity |
| `PricingIsIncomplete` |  |  |  |  |  | `Boolean` |  | Pricing |  | S/4 only entity |
| `SoldToParty` |  |  |  |  |  | `String(10)` |  | Sold-to Party |  | S/4 only entity |
| `LogicalSystem` |  |  |  |  |  | `String(10)` |  | Logical System |  | S/4 only entity |
