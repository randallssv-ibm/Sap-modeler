# InvoiceList

> Source file: `sap-s4com-InvoiceList-v1.json`


## Entity: `InvoiceList`

- **ABAP Name:** `I_InvoiceList`
- **Label:** Invoice List
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `InvoiceList` | `InvoiceList` | `String(10)` | Y | Invoice List |  |  | S/4 only entity (no ECC CDC mapping) |
| `SDDocumentCategory` | `SDDocumentCategory` | `String(4)` |  | SD Document Category |  |  | S/4 only entity (no ECC CDC mapping) |
| `InvoiceListType` | `InvoiceListType` | `String(4)` |  | Invoice List Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `CreatedByUser` | `CreatedByUser` | `String(12)` |  | Created By |  |  | S/4 only entity (no ECC CDC mapping) |
| `CreationDate` | `CreationDate` | `Date` |  | Created On |  |  | S/4 only entity (no ECC CDC mapping) |
| `CreationTime` | `CreationTime` | `String(6)` |  | Time |  |  | S/4 only entity (no ECC CDC mapping) |
| `LastChangeDate` | `LastChangeDate` | `Date` |  | Changed On |  |  | S/4 only entity (no ECC CDC mapping) |
| `LastChangeDateTime` | `LastChangeDateTime` | `Timestamp` |  | Time Stamp |  |  | S/4 only entity (no ECC CDC mapping) |
| `LogicalSystem` | `LogicalSystem` | `String(10)` |  | Logical System |  |  | S/4 only entity (no ECC CDC mapping) |
| `SalesOrganization` | `SalesOrganization` | `String(4)` |  | Sales Organization |  |  | S/4 only entity (no ECC CDC mapping) |
| `DistributionChannel` | `DistributionChannel` | `String(2)` |  | Distribution Channel |  |  | S/4 only entity (no ECC CDC mapping) |
| `Division` | `Division` | `String(2)` |  | Division |  |  | S/4 only entity (no ECC CDC mapping) |
| `InvoiceListBillingDate` | `InvoiceListBillingDate` | `Date` |  | Billing Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `InvoiceListIsCancelled` | `InvoiceListIsCancelled` | `Boolean` |  | Canceled |  |  | S/4 only entity (no ECC CDC mapping) |
| `CancelledInvoiceList` | `CancelledInvoiceList` | `String(10)` |  | Cancld Invc. List |  |  | S/4 only entity (no ECC CDC mapping) |
| `InvoiceListCombinationCriteria` | `InvoiceListCombinationCriteria` | `String(40)` |  | Combination Criteria |  |  | S/4 only entity (no ECC CDC mapping) |
| `TotalNetAmount` | `TotalNetAmount` | `Decimal(34,4)` |  | Net Value | TransactionCurrency |  | S/4 only entity (no ECC CDC mapping) |
| `TransactionCurrency` | `TransactionCurrency` | `String(5)` |  | Document Currency |  |  | S/4 only entity (no ECC CDC mapping) |
| `StatisticsCurrency` | `StatisticsCurrency` | `String(5)` |  | Statistics Currency |  |  | S/4 only entity (no ECC CDC mapping) |
| `TotalTaxAmount` | `TotalTaxAmount` | `Decimal(34,4)` |  | Tax Amount | TransactionCurrency |  | S/4 only entity (no ECC CDC mapping) |
| `CustomerPriceGroup` | `CustomerPriceGroup` | `String(2)` |  | Customer Price Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `PriceListType` | `PriceListType` | `String(2)` |  | Price List Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `TaxDepartureCountry` | `TaxDepartureCountry` | `String(3)` |  | Tax Departure C/R |  |  | S/4 only entity (no ECC CDC mapping) |
| `VATRegistration` | `VATRegistration` | `String(20)` |  | VAT Registration No. |  |  | S/4 only entity (no ECC CDC mapping) |
| `VATRegistrationOrigin` | `VATRegistrationOrigin` | `String(1)` |  | Origin Sales Tax No. |  |  | S/4 only entity (no ECC CDC mapping) |
| `VATRegistrationCountry` | `VATRegistrationCountry` | `String(3)` |  | Ctry/Rgn Sls Tax No. |  |  | S/4 only entity (no ECC CDC mapping) |
| `CustomerTaxClassification1` | `CustomerTaxClassification1` | `String(1)` |  | Tax Class.1 Customer |  |  | S/4 only entity (no ECC CDC mapping) |
| `CustomerTaxClassification2` | `CustomerTaxClassification2` | `String(1)` |  | Tax Class.2 Customer |  |  | S/4 only entity (no ECC CDC mapping) |
| `CustomerTaxClassification3` | `CustomerTaxClassification3` | `String(1)` |  | Tax Class.3 Customer |  |  | S/4 only entity (no ECC CDC mapping) |
| `CustomerTaxClassification4` | `CustomerTaxClassification4` | `String(1)` |  | Tax Class.4 Customer |  |  | S/4 only entity (no ECC CDC mapping) |
| `CustomerTaxClassification5` | `CustomerTaxClassification5` | `String(1)` |  | Tax Class.5 Customer |  |  | S/4 only entity (no ECC CDC mapping) |
| `CustomerTaxClassification6` | `CustomerTaxClassification6` | `String(1)` |  | Tax Class.6 Customer |  |  | S/4 only entity (no ECC CDC mapping) |
| `CustomerTaxClassification7` | `CustomerTaxClassification7` | `String(1)` |  | Tax Class.7 Customer |  |  | S/4 only entity (no ECC CDC mapping) |
| `CustomerTaxClassification8` | `CustomerTaxClassification8` | `String(1)` |  | Tax Class.8 Customer |  |  | S/4 only entity (no ECC CDC mapping) |
| `CustomerTaxClassification9` | `CustomerTaxClassification9` | `String(1)` |  | Tax Class.9 Customer |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsEUTriangularDeal` | `IsEUTriangularDeal` | `Boolean` |  | EU Triangular Deal |  |  | S/4 only entity (no ECC CDC mapping) |
| `SDPricingProcedure` | `SDPricingProcedure` | `String(6)` |  | Pricing Procedure |  |  | S/4 only entity (no ECC CDC mapping) |
| `ShippingCondition` | `ShippingCondition` | `String(2)` |  | Shipping Conditions |  |  | S/4 only entity (no ECC CDC mapping) |
| `IncotermsVersion` | `IncotermsVersion` | `String(4)` |  | Incoterms Version |  |  | S/4 only entity (no ECC CDC mapping) |
| `IncotermsClassification` | `IncotermsClassification` | `String(3)` |  | Incoterms |  |  | S/4 only entity (no ECC CDC mapping) |
| `IncotermsTransferLocation` | `IncotermsTransferLocation` | `String(28)` |  | Incoterms (Part 2) |  |  | S/4 only entity (no ECC CDC mapping) |
| `IncotermsLocation1` | `IncotermsLocation1` | `String(70)` |  | Incoterms Location 1 |  |  | S/4 only entity (no ECC CDC mapping) |
| `IncotermsLocation2` | `IncotermsLocation2` | `String(70)` |  | Incoterms Location 2 |  |  | S/4 only entity (no ECC CDC mapping) |
| `PayerParty` | `PayerParty` | `String(10)` |  | Payer |  |  | S/4 only entity (no ECC CDC mapping) |
| `ContractAccount` | `ContractAccount` | `String(12)` |  | Contract Account |  |  | S/4 only entity (no ECC CDC mapping) |
| `CustomerPaymentTerms` | `CustomerPaymentTerms` | `String(4)` |  | Terms of Payment |  |  | S/4 only entity (no ECC CDC mapping) |
| `PaymentMethod` | `PaymentMethod` | `String(1)` |  | Payment Method |  |  | S/4 only entity (no ECC CDC mapping) |
| `PaymentReference` | `PaymentReference` | `String(30)` |  | Payment Reference |  |  | S/4 only entity (no ECC CDC mapping) |
| `FixedValueDate` | `FixedValueDate` | `Date` |  | Fixed Value Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `AdditionalValueDays` | `AdditionalValueDays` | `String(2)` |  | Addit. Value Days |  |  | S/4 only entity (no ECC CDC mapping) |
| `SEPAMandate` | `SEPAMandate` | `String(35)` |  | Mandate Reference |  |  | S/4 only entity (no ECC CDC mapping) |
| `CompanyCode` | `CompanyCode` | `String(4)` |  | Company Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `FiscalYear` | `FiscalYear` | `String(4)` |  | Fiscal Year |  |  | S/4 only entity (no ECC CDC mapping) |
| `AccountingDocument` | `AccountingDocument` | `String(10)` |  | Document Number |  |  | S/4 only entity (no ECC CDC mapping) |
| `FiscalPeriod` | `FiscalPeriod` | `String(3)` |  | Posting Period |  |  | S/4 only entity (no ECC CDC mapping); ECC: BKPF.MONAT (unpadded '3'); S/4: zero-padded '003' |
| `CustomerAccountAssignmentGroup` | `CustomerAccountAssignmentGroup` | `String(2)` |  | Acct Assmt Grp Cust. |  |  | S/4 only entity (no ECC CDC mapping) |
| `AccountingExchangeRateIsSet` | `AccountingExchangeRateIsSet` | `Boolean` |  | Set Exchange Rate |  |  | S/4 only entity (no ECC CDC mapping) |
| `AccountingExchangeRate` | `AccountingExchangeRate` | `Decimal(9,5)` |  | Accounting Exchange Rate |  |  | S/4 only entity (no ECC CDC mapping) |
| `ExchangeRateDate` | `ExchangeRateDate` | `Date` |  | Translation Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `ExchangeRateType` | `ExchangeRateType` | `String(4)` |  | Exchange Rate Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `DocumentReferenceID` | `DocumentReferenceID` | `String(16)` |  | Reference |  |  | S/4 only entity (no ECC CDC mapping) |
| `AssignmentReference` | `AssignmentReference` | `String(18)` |  | Assignment |  |  | S/4 only entity (no ECC CDC mapping) |
| `DunningArea` | `DunningArea` | `String(2)` |  | Dunning Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `DunningBlockingReason` | `DunningBlockingReason` | `String(1)` |  | Dunning Block |  |  | S/4 only entity (no ECC CDC mapping) |
| `DunningKey` | `DunningKey` | `String(1)` |  | Dunning Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `InternalFinancialDocument` | `InternalFinancialDocument` | `String(10)` |  | Financial Doc. No. |  |  | S/4 only entity (no ECC CDC mapping) |
| `SoldToParty` | `SoldToParty` | `String(10)` |  | Sold-to Party |  |  | S/4 only entity (no ECC CDC mapping) |
| `PartnerCompany` | `PartnerCompany` | `String(6)` |  | Trading Partner No. |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchaseOrderByCustomer` | `PurchaseOrderByCustomer` | `String(35)` |  | Customer Reference |  |  | S/4 only entity (no ECC CDC mapping) |
| `CustomerGroup` | `CustomerGroup` | `String(2)` |  | Customer Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `Country` | `Country` | `String(3)` |  | Dest. Country/Region |  |  | S/4 only entity (no ECC CDC mapping) |
| `CityCode` | `CityCode` | `String(4)` |  | City Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `SalesDistrict` | `SalesDistrict` | `String(6)` |  | Sales District |  |  | S/4 only entity (no ECC CDC mapping) |
| `Region` | `Region` | `String(3)` |  | Region |  |  | S/4 only entity (no ECC CDC mapping) |
| `County` | `County` | `String(3)` |  | County Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `CreditControlArea` | `CreditControlArea` | `String(4)` |  | Credit Control Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `PricingDocument` | `PricingDocument` | `String(10)` |  | Doc. Condition No. |  |  | S/4 only entity (no ECC CDC mapping) |
| `OverallSDProcessStatus` | `OverallSDProcessStatus` | `String(1)` |  | Overall Status |  |  | S/4 only entity (no ECC CDC mapping) |
| `AccountingPostingStatus` | `AccountingPostingStatus` | `String(1)` |  | Posting Status |  |  | S/4 only entity (no ECC CDC mapping) |
| `AccountingTransferStatus` | `AccountingTransferStatus` | `String(1)` |  | Posting Status |  |  | S/4 only entity (no ECC CDC mapping) |
| `OvrlItmGeneralIncompletionSts` | `OvrlItmGeneralIncompletionSts` | `String(1)` |  | All Items |  |  | S/4 only entity (no ECC CDC mapping) |
| `OverallPricingIncompletionSts` | `OverallPricingIncompletionSts` | `String(1)` |  | Pricing – All Items |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `InvoiceListItem`

- **ABAP Name:** `I_InvoiceListItem`
- **Label:** Invoice List Item
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `InvoiceList` | `InvoiceList` | `String(10)` | Y | Invoice List |  | _InvoiceList | S/4 only entity (no ECC CDC mapping) |
| `InvoiceListItem` | `InvoiceListItem` | `String(6)` | Y | Item |  |  | S/4 only entity (no ECC CDC mapping) |
| `BillingDocument` | `BillingDocument` | `String(10)` |  | Billing Document |  |  | S/4 only entity (no ECC CDC mapping) |
| `NetAmount` | `NetAmount` | `Decimal(34,4)` |  | Net Value | TransactionCurrency |  | S/4 only entity (no ECC CDC mapping) |
| `TaxAmount` | `TaxAmount` | `Decimal(34,4)` |  | Tax Amount | TransactionCurrency |  | S/4 only entity (no ECC CDC mapping) |
| `GrossAmount` | `GrossAmount` | `Decimal(34,4)` |  | Gross Amount | TransactionCurrency |  | S/4 only entity (no ECC CDC mapping) |
| `RemunerationNetAmount` | `RemunerationNetAmount` | `Decimal(34,4)` |  | Factoring Discount | TransactionCurrency |  | S/4 only entity (no ECC CDC mapping) |
| `RemunerationTaxAmount` | `RemunerationTaxAmount` | `Decimal(34,4)` |  | Fact. Discount Tax | TransactionCurrency |  | S/4 only entity (no ECC CDC mapping) |
| `TransactionCurrency` | `TransactionCurrency` | `String(5)` |  | Document Currency |  |  | S/4 only entity (no ECC CDC mapping) |
| `PricingIsIncomplete` | `PricingIsIncomplete` | `Boolean` |  | Pricing |  |  | S/4 only entity (no ECC CDC mapping) |
| `SoldToParty` | `SoldToParty` | `String(10)` |  | Sold-to Party |  |  | S/4 only entity (no ECC CDC mapping) |
| `LogicalSystem` | `LogicalSystem` | `String(10)` |  | Logical System |  |  | S/4 only entity (no ECC CDC mapping) |
