# BillingDocument

> Source file: `sap-s4com-BillingDocument-v1.json`

**Technical Name:** `` | **Data Category:** `DIMENSION` | **VDM Type:** `BASIC` | **Size:** `L`


## Entity: `BillingDocument`

- **ABAP Name:** `I_BillingDocument`
- **Label:** Billing Document
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** vbrk

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `BillingDocument` | `BillingDocument` | `String(10)` | Y | Billing Document |  |  |  |
| `SDDocumentCategory` | `SDDocumentCategory` | `String(4)` |  | SD Document Category |  |  |  |
| `BillingDocumentCategory` | `BillingDocumentCategory` | `String(1)` |  | Billing Category |  |  |  |
| `BillingDocumentType` | `BillingDocumentType` | `String(4)` |  | Billing Type |  |  |  |
| `CreatedByUser` | `CreatedByUser` | `String(12)` |  | Created By |  |  |  |
| `CreationDate` | `CreationDate` | `Date` |  | Created On |  |  |  |
| `CreationTime` | `CreationTime` | `String(6)` |  | Time |  |  |  |
| `LastChangeDate` | `LastChangeDate` | `Date` |  | Changed On |  |  |  |
| `LastChangeDateTime` | `LastChangeDateTime` | `Timestamp` |  | Time Stamp |  |  |  |
| `LogicalSystem` | `LogicalSystem` | `String(10)` |  | Logical System |  |  |  |
| `SalesOrganization` | `SalesOrganization` | `String(4)` |  | Sales Organization |  |  |  |
| `DistributionChannel` | `DistributionChannel` | `String(2)` |  | Distribution Channel |  |  |  |
| `Division` | `Division` | `String(2)` |  | Division |  |  |  |
| `BillingDocumentDate` | `BillingDocumentDate` | `Date` |  | Billing Date |  |  |  |
| `BillingDocumentIsCancelled` | `BillingDocumentIsCancelled` | `Boolean` |  | Canceled |  |  |  |
| `CancelledBillingDocument` | `CancelledBillingDocument` | `String(10)` |  | Canceled Bill. Doc. |  |  |  |
| `BillingDocCombinationCriteria` | `BillingDocCombinationCriteria` | `String(40)` |  | Combination Criteria |  |  |  |
| `ManualInvoiceMaintIsRelevant` | `ManualInvoiceMaintIsRelevant` | `Boolean` |  | Man. Invoice Maint. |  |  |  |
| `NmbrOfPages` | `NmbrOfPages` | `String(3)` |  | Number of Pages |  |  |  |
| `IsIntrastatReportingRelevant` | `IsIntrastatReportingRelevant` | `Boolean` |  | Intrastat Relevance |  |  |  |
| `IsIntrastatReportingExcluded` | `IsIntrastatReportingExcluded` | `Boolean` |  | Intrastat Exclusion |  |  |  |
| `BillingDocumentIsTemporary` | `BillingDocumentIsTemporary` | `Boolean` |  | Draft Indicator |  |  |  |
| `TotalNetAmount` | `TotalNetAmount` | `Decimal(34,4)` |  | Net Value | TransactionCurrency |  |  |
| `TransactionCurrency` | `TransactionCurrency` | `String(5)` |  | Document Currency |  |  |  |
| `StatisticsCurrency` | `StatisticsCurrency` | `String(5)` |  | Statistics Currency |  |  |  |
| `TotalTaxAmount` | `TotalTaxAmount` | `Decimal(34,4)` |  | Tax Amount | TransactionCurrency |  |  |
| `CustomerPriceGroup` | `CustomerPriceGroup` | `String(2)` |  | Customer Price Group |  |  |  |
| `PriceListType` | `PriceListType` | `String(2)` |  | Price List Type |  |  |  |
| `TaxDepartureCountry` | `TaxDepartureCountry` | `String(3)` |  | Tax Departure C/R |  |  |  |
| `VATRegistration` | `VATRegistration` | `String(20)` |  | VAT Registration No. |  |  |  |
| `VATRegistrationOrigin` | `VATRegistrationOrigin` | `String(1)` |  | Origin Sales Tax No. |  |  |  |
| `VATRegistrationCountry` | `VATRegistrationCountry` | `String(3)` |  | Ctry/Rgn Sls Tax No. |  |  |  |
| `HierarchyTypePricing` | `HierarchyTypePricing` | `String(1)` |  | HierarchyTypePricing |  |  |  |
| `CustomerTaxClassification1` | `CustomerTaxClassification1` | `String(1)` |  | Tax Class.1 Customer |  |  |  |
| `CustomerTaxClassification2` | `CustomerTaxClassification2` | `String(1)` |  | Tax Class.2 Customer |  |  |  |
| `CustomerTaxClassification3` | `CustomerTaxClassification3` | `String(1)` |  | Tax Class.3 Customer |  |  |  |
| `CustomerTaxClassification4` | `CustomerTaxClassification4` | `String(1)` |  | Tax Class.4 Customer |  |  |  |
| `CustomerTaxClassification5` | `CustomerTaxClassification5` | `String(1)` |  | Tax Class.5 Customer |  |  |  |
| `CustomerTaxClassification6` | `CustomerTaxClassification6` | `String(1)` |  | Tax Class.6 Customer |  |  |  |
| `CustomerTaxClassification7` | `CustomerTaxClassification7` | `String(1)` |  | Tax Class.7 Customer |  |  |  |
| `CustomerTaxClassification8` | `CustomerTaxClassification8` | `String(1)` |  | Tax Class.8 Customer |  |  |  |
| `CustomerTaxClassification9` | `CustomerTaxClassification9` | `String(1)` |  | Tax Class.9 Customer |  |  |  |
| `IsEUTriangularDeal` | `IsEUTriangularDeal` | `Boolean` |  | EU Triangular Deal |  |  |  |
| `SDPricingProcedure` | `SDPricingProcedure` | `String(6)` |  | Pricing Procedure |  |  |  |
| `ShippingCondition` | `ShippingCondition` | `String(2)` |  | Shipping Conditions |  |  |  |
| `PlantSupplier` | `PlantSupplier` | `String(10)` |  | Sppl. No. Plnt |  |  |  |
| `IncotermsVersion` | `IncotermsVersion` | `String(4)` |  | Incoterms Version |  |  |  |
| `IncotermsClassification` | `IncotermsClassification` | `String(3)` |  | Incoterms |  |  |  |
| `IncotermsTransferLocation` | `IncotermsTransferLocation` | `String(28)` |  | Incoterms (Part 2) |  |  |  |
| `IncotermsLocation1` | `IncotermsLocation1` | `String(70)` |  | Incoterms Location 1 |  |  |  |
| `IncotermsLocation2` | `IncotermsLocation2` | `String(70)` |  | Incoterms Location 2 |  |  |  |
| `PayerParty` | `PayerParty` | `String(10)` |  | Payer |  |  |  |
| `ContractAccount` | `ContractAccount` | `String(12)` |  | Contract Account |  |  |  |
| `CustomerPaymentTerms` | `CustomerPaymentTerms` | `String(4)` |  | Terms of Payment |  |  |  |
| `PaymentMethod` | `PaymentMethod` | `String(1)` |  | Payment Method |  |  |  |
| `PaymentReference` | `PaymentReference` | `String(30)` |  | Payment Reference |  |  |  |
| `FixedValueDate` | `FixedValueDate` | `Date` |  | Fixed Value Date |  |  |  |
| `AdditionalValueDays` | `AdditionalValueDays` | `String(2)` |  | Addit. Value Days |  |  |  |
| `SEPAMandate` | `SEPAMandate` | `String(35)` |  | Mandate Reference |  |  |  |
| `CompanyCode` | `CompanyCode` | `String(4)` |  | Company Code |  |  |  |
| `FiscalYear` | `FiscalYear` | `String(4)` |  | Fiscal Year |  |  |  |
| `AccountingDocument` | `AccountingDocument` | `String(10)` |  | Document Number |  |  |  |
| `FiscalPeriod` | `FiscalPeriod` | `String(3)` |  | Posting Period |  |  | ECC: BKPF.MONAT (unpadded '3'); S/4: zero-padded '003' |
| `CustomerAccountAssignmentGroup` | `CustomerAccountAssignmentGroup` | `String(2)` |  | Acct Assmt Grp Cust. |  |  |  |
| `AccountingExchangeRateIsSet` | `AccountingExchangeRateIsSet` | `Boolean` |  | Set Exchange Rate |  |  |  |
| `AccountingExchangeRate` | `AccountingExchangeRate` | `Decimal(9,5)` |  | Accounting Exchange Rate |  |  |  |
| `ExchangeRateDate` | `ExchangeRateDate` | `Date` |  | Translation Date |  |  |  |
| `ExchangeRateType` | `ExchangeRateType` | `String(4)` |  | Exchange Rate Type |  |  |  |
| `DocumentReferenceID` | `DocumentReferenceID` | `String(16)` |  | Reference |  |  |  |
| `AssignmentReference` | `AssignmentReference` | `String(18)` |  | Assignment |  |  |  |
| `ReversalReason` | `ReversalReason` | `String(2)` |  | Reversal Reason |  |  |  |
| `DunningArea` | `DunningArea` | `String(2)` |  | Dunning Area |  |  |  |
| `DunningBlockingReason` | `DunningBlockingReason` | `String(1)` |  | Dunning Block |  |  |  |
| `DunningKey` | `DunningKey` | `String(1)` |  | Dunning Key |  |  |  |
| `InternalFinancialDocument` | `InternalFinancialDocument` | `String(10)` |  | Financial Doc. No. |  |  |  |
| `IsRelevantForAccrual` | `IsRelevantForAccrual` | `Boolean` |  | Relevant for Accrual |  |  |  |
| `SoldToParty` | `SoldToParty` | `String(10)` |  | Sold-to Party |  |  |  |
| `PartnerCompany` | `PartnerCompany` | `String(6)` |  | Trading Partner No. |  |  |  |
| `PurchaseOrderByCustomer` | `PurchaseOrderByCustomer` | `String(35)` |  | Customer Reference |  |  |  |
| `CustomerGroup` | `CustomerGroup` | `String(2)` |  | Customer Group |  |  |  |
| `Country` | `Country` | `String(3)` |  | Dest. Country/Region |  |  |  |
| `CityCode` | `CityCode` | `String(4)` |  | City Code |  |  |  |
| `SalesDistrict` | `SalesDistrict` | `String(6)` |  | Sales District |  |  |  |
| `Region` | `Region` | `String(3)` |  | Region |  |  |  |
| `County` | `County` | `String(3)` |  | County Code |  |  |  |
| `CreditControlArea` | `CreditControlArea` | `String(4)` |  | Credit Control Area |  |  |  |
| `CustomerRebateAgreement` | `CustomerRebateAgreement` | `String(10)` |  | Agreement |  |  |  |
| `PricingDocument` | `PricingDocument` | `String(10)` |  | Doc. Condition No. |  |  |  |
| `OverallSDProcessStatus` | `OverallSDProcessStatus` | `String(1)` |  | Overall Status |  |  |  |
| `OverallBillingStatus` | `OverallBillingStatus` | `String(1)` |  | Status |  |  |  |
| `AccountingPostingStatus` | `AccountingPostingStatus` | `String(1)` |  | Posting Status |  |  |  |
| `AccountingTransferStatus` | `AccountingTransferStatus` | `String(1)` |  | Posting Status |  |  |  |
| `BillingIssueType` | `BillingIssueType` | `String(1)` |  | Issue Type |  |  |  |
| `InvoiceListStatus` | `InvoiceListStatus` | `String(1)` |  | Invoice List Status |  |  |  |
| `OvrlItmGeneralIncompletionSts` | `OvrlItmGeneralIncompletionSts` | `String(1)` |  | All Items |  |  |  |
| `OverallPricingIncompletionSts` | `OverallPricingIncompletionSts` | `String(1)` |  | Pricing – All Items |  |  |  |
| `InvoiceClearingStatus` | `InvoiceClearingStatus` | `String(1)` |  | Clearing Status |  |  |  |
| `InvoiceListType` | `InvoiceListType` | `String(4)` |  | Invoice List Type |  |  |  |
| `InvoiceListBillingDate` | `InvoiceListBillingDate` | `Date` |  | Inv. List Bill. Date |  |  |  |
| `ForeignTradeStstclCurrency` | `ForeignTradeStstclCurrency` | `String(5)` |  | Currency |  |  |  |


## Entity: `BillingDocumentItem`

- **ABAP Name:** `I_BillingDocumentItem`
- **Label:** Billing Document Item
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** vbrp

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `BillingDocument` | `BillingDocument` | `String(10)` | Y | Billing Document |  | _BillingDocument |  |
| `BillingDocumentItem` | `BillingDocumentItem` | `String(6)` | Y | Item |  |  |  |
| `SalesDocumentItemCategory` | `SalesDocumentItemCategory` | `String(4)` |  | Sales Doc. Item Cat. |  |  |  |
| `SalesDocumentItemType` | `SalesDocumentItemType` | `String(1)` |  | Item Type |  |  |  |
| `ReturnItemProcessingType` | `ReturnItemProcessingType` | `String(1)` |  | Returns |  |  |  |
| `CreatedByUser` | `CreatedByUser` | `String(12)` |  | Created By |  |  |  |
| `CreationDate` | `CreationDate` | `Date` |  | Created On |  |  |  |
| `CreationTime` | `CreationTime` | `String(6)` |  | Time |  |  |  |
| `ReferenceLogicalSystem` | `ReferenceLogicalSystem` | `String(10)` |  | Logical System |  |  |  |
| `OrganizationDivision` | `OrganizationDivision` | `String(2)` |  | Division of Order |  |  |  |
| `Division` | `Division` | `String(2)` |  | Division |  |  |  |
| `SalesOffice` | `SalesOffice` | `String(4)` |  | Sales Office |  |  |  |
| `Material` | `Material` | `String(40)` |  | Material |  |  |  |
| `Product` | `Product` | `String(40)` |  | Product |  |  |  |
| `OriginallyRequestedMaterial` | `OriginallyRequestedMaterial` | `String(40)` |  | Material Entered |  |  |  |
| `InternationalArticleNumber` | `InternationalArticleNumber` | `String(18)` |  | EAN/UPC |  |  |  |
| `PricingReferenceMaterial` | `PricingReferenceMaterial` | `String(40)` |  | Pricing Ref. Matl |  |  |  |
| `Batch` | `Batch` | `String(10)` |  | Batch |  |  |  |
| `ProductHierarchyNode` | `ProductHierarchyNode` | `String(18)` |  | Product Hierarchy |  |  |  |
| `MaterialGroup` | `MaterialGroup` | `String(9)` |  | Material Group |  |  |  |
| `ProductGroup` | `ProductGroup` | `String(9)` |  | Product Group |  |  |  |
| `AdditionalMaterialGroup1` | `AdditionalMaterialGroup1` | `String(3)` |  | Material Group 1 |  |  |  |
| `AdditionalMaterialGroup2` | `AdditionalMaterialGroup2` | `String(3)` |  | Material Group 2 |  |  |  |
| `AdditionalMaterialGroup3` | `AdditionalMaterialGroup3` | `String(3)` |  | Material Group 3 |  |  |  |
| `AdditionalMaterialGroup4` | `AdditionalMaterialGroup4` | `String(3)` |  | Material Group 4 |  |  |  |
| `AdditionalMaterialGroup5` | `AdditionalMaterialGroup5` | `String(3)` |  | Material Group 5 |  |  |  |
| `ProductConfiguration` | `ProductConfiguration` | `String(18)` |  | Configuration |  |  |  |
| `MaterialCommissionGroup` | `MaterialCommissionGroup` | `String(2)` |  | Commission Group |  |  |  |
| `Plant` | `Plant` | `String(4)` |  | Plant |  |  |  |
| `StorageLocation` | `StorageLocation` | `String(4)` |  | Storage Location |  |  |  |
| `ReplacementPartType` | `ReplacementPartType` | `String(1)` |  | Replacement Part |  |  |  |
| `MaterialGroupHierarchy1` | `MaterialGroupHierarchy1` | `String(18)` |  | Material Group 1 |  |  |  |
| `MaterialGroupHierarchy2` | `MaterialGroupHierarchy2` | `String(18)` |  | Material Group 2 |  |  |  |
| `PlantRegion` | `PlantRegion` | `String(3)` |  | Region of Dlv. Plant |  |  |  |
| `PlantCounty` | `PlantCounty` | `String(3)` |  | County of Dlv.Plant |  |  |  |
| `PlantCity` | `PlantCity` | `String(4)` |  | City of Deliv. Plant |  |  |  |
| `TransitPlant` | `TransitPlant` | `String(4)` |  | Transit Plant |  |  |  |
| `ValueChainCategory` | `ValueChainCategory` | `String(4)` |  | Value Chain Category |  |  |  |
| `BOMExplosion` | `BOMExplosion` | `String(8)` |  | BOM Explosion Number |  |  |  |
| `MaterialDeterminationType` | `MaterialDeterminationType` | `String(1)` |  | Mat.Determ.Active |  |  |  |
| `SoldProduct` | `SoldProduct` | `String(40)` |  | Product Sold |  |  |  |
| `BillingDocumentItemText` | `BillingDocumentItemText` | `String(40)` |  | Item Description |  |  |  |
| `ServicesRenderedDate` | `ServicesRenderedDate` | `Date` |  | Serv. Rendered Date |  |  |  |
| `BillingQuantity` | `BillingQuantity` | `Decimal(13,3)` |  | Invoiced Quantity | BillingQuantityUnit |  |  |
| `BillingQuantityUnit` | `BillingQuantityUnit` | `String(3)` |  | Sales Unit |  |  |  |
| `BillingQuantityInBaseUnit` | `BillingQuantityInBaseUnit` | `Decimal(13,3)` |  | Billing Qty in SKU | BaseUnit |  |  |
| `BaseUnit` | `BaseUnit` | `String(3)` |  | Base Unit of Measure |  |  |  |
| `MRPRequiredQuantityInBaseUnit` | `MRPRequiredQuantityInBaseUnit` | `Decimal(13,3)` |  | Required Quantity | BaseUnit |  |  |
| `BillingToBaseQuantityDnmntr` | `BillingToBaseQuantityDnmntr` | `Decimal(5,0)` |  | Denominator |  |  |  |
| `BillingToBaseQuantityNmrtr` | `BillingToBaseQuantityNmrtr` | `Decimal(5,0)` |  | Numerator |  |  |  |
| `ItemGrossWeight` | `ItemGrossWeight` | `Decimal(15,3)` |  | Gross Weight | ItemWeightUnit |  |  |
| `ItemNetWeight` | `ItemNetWeight` | `Decimal(15,3)` |  | Net Weight | ItemWeightUnit |  |  |
| `ItemWeightUnit` | `ItemWeightUnit` | `String(3)` |  | Unit of Weight |  |  |  |
| `ItemVolume` | `ItemVolume` | `Decimal(15,3)` |  | Volume | ItemVolumeUnit |  |  |
| `ItemVolumeUnit` | `ItemVolumeUnit` | `String(3)` |  | Volume Unit |  |  |  |
| `BillToPartyCountry` | `BillToPartyCountry` | `String(3)` |  | Dest. Ctry/Reg. Ord. |  |  |  |
| `BillToPartyRegion` | `BillToPartyRegion` | `String(3)` |  | Region Order |  |  |  |
| `BillingPlanRule` | `BillingPlanRule` | `String(1)` |  | Billing Rule |  |  |  |
| `BillingPlan` | `BillingPlan` | `String(10)` |  | Bill. Plan No. |  |  |  |
| `BillingPlanItem` | `BillingPlanItem` | `String(6)` |  | Item |  |  |  |
| `DownPaymentProcessingVariant` | `DownPaymentProcessingVariant` | `String(1)` |  | Down Payment Variant |  |  |  |
| `NetAmount` | `NetAmount` | `Decimal(34,4)` |  | Net Value | TransactionCurrency |  |  |
| `TransactionCurrency` | `TransactionCurrency` | `String(5)` |  | Document Currency |  |  |  |
| `GrossAmount` | `GrossAmount` | `Decimal(34,4)` |  | Gross Value | TransactionCurrency |  |  |
| `PricingDate` | `PricingDate` | `Date` |  | Pricing Date |  |  |  |
| `PriceDetnExchangeRate` | `PriceDetnExchangeRate` | `Decimal(9,5)` |  | Exchange Rate |  |  |  |
| `PricingScaleQuantityInBaseUnit` | `PricingScaleQuantityInBaseUnit` | `Decimal(13,3)` |  | Scale Quantity | BaseUnit |  |  |
| `TaxAmount` | `TaxAmount` | `Decimal(34,4)` |  | Tax Amount | TransactionCurrency |  |  |
| `CostAmount` | `CostAmount` | `Decimal(34,4)` |  | Cost | TransactionCurrency |  |  |
| `Subtotal1Amount` | `Subtotal1Amount` | `Decimal(34,4)` |  | Subtotal 1 | TransactionCurrency |  |  |
| `Subtotal2Amount` | `Subtotal2Amount` | `Decimal(34,4)` |  | Subtotal 2 | TransactionCurrency |  |  |
| `Subtotal3Amount` | `Subtotal3Amount` | `Decimal(34,4)` |  | Subtotal 3 | TransactionCurrency |  |  |
| `Subtotal4Amount` | `Subtotal4Amount` | `Decimal(34,4)` |  | Subtotal 4 | TransactionCurrency |  |  |
| `Subtotal5Amount` | `Subtotal5Amount` | `Decimal(34,4)` |  | Subtotal 5 | TransactionCurrency |  |  |
| `Subtotal6Amount` | `Subtotal6Amount` | `Decimal(34,4)` |  | Subtotal 6 | TransactionCurrency |  |  |
| `StatisticalValueControl` | `StatisticalValueControl` | `String(1)` |  | Statistical Value |  |  |  |
| `CashDiscountIsDeductible` | `CashDiscountIsDeductible` | `Boolean` |  | Cash Discount |  |  |  |
| `CustomerConditionGroup1` | `CustomerConditionGroup1` | `String(2)` |  | Condition Group 1 |  |  |  |
| `CustomerConditionGroup2` | `CustomerConditionGroup2` | `String(2)` |  | Condition Group 2 |  |  |  |
| `CustomerConditionGroup3` | `CustomerConditionGroup3` | `String(2)` |  | Condition Group 3 |  |  |  |
| `CustomerConditionGroup4` | `CustomerConditionGroup4` | `String(2)` |  | Condition Group 4 |  |  |  |
| `CustomerConditionGroup5` | `CustomerConditionGroup5` | `String(2)` |  | Condition Group 5 |  |  |  |
| `ManualPriceChangeType` | `ManualPriceChangeType` | `String(1)` |  | Manual Price |  |  |  |
| `MaterialPricingGroup` | `MaterialPricingGroup` | `String(2)` |  | Material Price Grp |  |  |  |
| `StatisticsExchangeRate` | `StatisticsExchangeRate` | `Decimal(9,5)` |  | Exchange Rate Stats. |  |  |  |
| `MainItemPricingRefMaterial` | `MainItemPricingRefMaterial` | `String(40)` |  | Pricing Ref.Material |  |  |  |
| `MainItemMaterialPricingGroup` | `MainItemMaterialPricingGroup` | `String(2)` |  | MnItem MatPricingGrp |  |  |  |
| `TimeSheetOvertimeCategory` | `TimeSheetOvertimeCategory` | `String(4)` |  | Overtime Category |  |  |  |
| `PricingRelevance` | `PricingRelevance` | `String(1)` |  | Pricing Relevance |  |  |  |
| `DepartureCountry` | `DepartureCountry` | `String(3)` |  | Departure Ctry/Reg. |  |  |  |
| `TaxJurisdiction` | `TaxJurisdiction` | `String(15)` |  | Tax Jurisdiction |  |  |  |
| `ProductTaxClassification1` | `ProductTaxClassification1` | `String(1)` |  | Product Tax Classification 1 |  |  |  |
| `ProductTaxClassification2` | `ProductTaxClassification2` | `String(1)` |  | Product Tax Classification 2 |  |  |  |
| `ProductTaxClassification3` | `ProductTaxClassification3` | `String(1)` |  | Product Tax Classification 3 |  |  |  |
| `ProductTaxClassification4` | `ProductTaxClassification4` | `String(1)` |  | Product Tax Classification 4 |  |  |  |
| `ProductTaxClassification5` | `ProductTaxClassification5` | `String(1)` |  | Product Tax Classification 5 |  |  |  |
| `ProductTaxClassification6` | `ProductTaxClassification6` | `String(1)` |  | Product Tax Classification 6 |  |  |  |
| `ProductTaxClassification7` | `ProductTaxClassification7` | `String(1)` |  | Product Tax Classification 7 |  |  |  |
| `ProductTaxClassification8` | `ProductTaxClassification8` | `String(1)` |  | Product Tax Classification 8 |  |  |  |
| `ProductTaxClassification9` | `ProductTaxClassification9` | `String(1)` |  | Product Tax Classification 9 |  |  |  |
| `ZeroVATRsn` | `ZeroVATRsn` | `String(1)` |  | Reason 0 VAT |  |  |  |
| `TaxCode` | `TaxCode` | `String(2)` |  | Tax Code |  |  |  |
| `TaxRateValidityStartDate` | `TaxRateValidityStartDate` | `Date` |  | Tax Rate Valid-From |  |  |  |
| `CountryOfOrigin` | `CountryOfOrigin` | `String(3)` |  | Cntry/Reg of Origin |  |  |  |
| `RegionOfOrigin` | `RegionOfOrigin` | `String(3)` |  | Region of Origin |  |  |  |
| `CommodityCode` | `CommodityCode` | `String(30)` |  | Commodity Code |  |  |  |
| `EligibleAmountForCashDiscount` | `EligibleAmountForCashDiscount` | `Decimal(34,4)` |  | Cash Disc. Bas. | TransactionCurrency |  |  |
| `BusinessArea` | `BusinessArea` | `String(4)` |  | Business Area |  |  |  |
| `ProfitCenter` | `ProfitCenter` | `String(10)` |  | Profit Center |  |  |  |
| `OrderID` | `OrderID` | `String(12)` |  | Order |  |  |  |
| `WBSElement` | `WBSElement` | `String(8)` |  | WBS Element |  |  |  |
| `WBSElementInternalID` | `WBSElementInternalID` | `String(8)` |  | WBS Internal ID |  |  |  |
| `ProviderContract` | `ProviderContract` | `String(20)` |  | Provider Contract |  |  |  |
| `ProviderContractItem` | `ProviderContractItem` | `String(6)` |  | Provider Contract Item |  |  |  |
| `BillingPerformancePeriodStrDte` | `BillingPerformancePeriodStrDte` | `Date` |  | Per. of Perf. Start |  |  |  |
| `BillingPeriodOfPerfStartDate` | `BillingPeriodOfPerfStartDate` | `Date` |  | Per. of Perf. Start |  |  |  |
| `BillingPerformancePeriodEndDte` | `BillingPerformancePeriodEndDte` | `Date` |  | Per. of Perf. End |  |  |  |
| `BillingPeriodOfPerfEndDate` | `BillingPeriodOfPerfEndDate` | `Date` |  | Per. of Perf. End |  |  |  |
| `ControllingArea` | `ControllingArea` | `String(4)` |  | Controlling Area |  |  |  |
| `ProfitabilitySegment` | `ProfitabilitySegment` | `String(10)` |  | Profitability Segment (Deprecated) |  |  |  |
| `ProfitabilitySegment_2` | `ProfitabilitySegment_2` | `String(10)` |  | Profitability Segment |  |  |  |
| `CostCenter` | `CostCenter` | `String(10)` |  | Cost Center |  |  |  |
| `OriginSDDocument` | `OriginSDDocument` | `String(10)` |  | Originating Document |  |  |  |
| `OriginSDDocumentItem` | `OriginSDDocumentItem` | `String(6)` |  | Originating Item |  |  |  |
| `PriceDetnExchangeRateDate` | `PriceDetnExchangeRateDate` | `Date` |  | Translation Date |  |  |  |
| `MatlAccountAssignmentGroup` | `MatlAccountAssignmentGroup` | `String(2)` |  | Acct Assmt Grp Mat. |  |  |  |
| `ReferenceSDDocument` | `ReferenceSDDocument` | `String(10)` |  | Reference Document |  |  |  |
| `ReferenceSDDocumentItem` | `ReferenceSDDocumentItem` | `String(6)` |  | Reference Item |  |  |  |
| `ReferenceSDDocumentCategory` | `ReferenceSDDocumentCategory` | `String(4)` |  | Ref. Doc. Category |  |  |  |
| `SalesDocument` | `SalesDocument` | `String(10)` |  | Sales Document |  |  |  |
| `SalesDocumentItem` | `SalesDocumentItem` | `String(6)` |  | Sales Document Item |  |  |  |
| `SalesSDDocumentCategory` | `SalesSDDocumentCategory` | `String(4)` |  | Sales Doc. Category |  |  |  |
| `HigherLevelItem` | `HigherLevelItem` | `String(6)` |  | Higher-Level Item |  |  |  |
| `HigherLvlItmOfBatSpltItm` | `HigherLvlItmOfBatSpltItm` | `String(6)` |  | HigherLevelItemBatch |  |  |  |
| `BillingDocumentItemInPartSgmt` | `BillingDocumentItemInPartSgmt` | `String(6)` |  | Partner Item |  |  |  |
| `ExternalReferenceDocument` | `ExternalReferenceDocument` | `String(10)` |  | Ext. Reference Document |  |  |  |
| `ExternalReferenceDocumentItem` | `ExternalReferenceDocumentItem` | `String(6)` |  | Ext. Ref. Document Item |  |  |  |
| `BillingDocExtReferenceDocItem` | `BillingDocExtReferenceDocItem` | `String(6)` |  | Ext. Reference Doc. Item |  |  |  |
| `PrelimBillingDocument` | `PrelimBillingDocument` | `String(10)` |  | Prelimin. Bill. Doc. |  |  |  |
| `PrelimBillingDocumentItem` | `PrelimBillingDocumentItem` | `String(6)` |  | Prelimin. Doc. Item |  |  |  |
| `SalesGroup` | `SalesGroup` | `String(3)` |  | Sales Group |  |  |  |
| `AdditionalCustomerGroup1` | `AdditionalCustomerGroup1` | `String(3)` |  | Customer Group 1 |  |  |  |
| `AdditionalCustomerGroup2` | `AdditionalCustomerGroup2` | `String(3)` |  | Customer Group 2 |  |  |  |
| `AdditionalCustomerGroup3` | `AdditionalCustomerGroup3` | `String(3)` |  | Customer Group 3 |  |  |  |
| `AdditionalCustomerGroup4` | `AdditionalCustomerGroup4` | `String(3)` |  | Customer Group 4 |  |  |  |
| `AdditionalCustomerGroup5` | `AdditionalCustomerGroup5` | `String(3)` |  | Customer Group 5 |  |  |  |
| `SDDocumentReason` | `SDDocumentReason` | `String(3)` |  | Order Reason |  |  |  |
| `RetailPromotion` | `RetailPromotion` | `String(10)` |  | Retail Promotion |  |  |  |
| `RebateBasisAmount` | `RebateBasisAmount` | `Decimal(34,4)` |  | Rebate Basis | TransactionCurrency |  |  |
| `VolumeRebateGroup` | `VolumeRebateGroup` | `String(2)` |  | Volume Rebate Group |  |  |  |
| `ItemIsRelevantForCredit` | `ItemIsRelevantForCredit` | `Boolean` |  | Credit Funct. Active |  |  |  |
| `CreditRelatedPrice` | `CreditRelatedPrice` | `Decimal(34,4)` |  | Credit Price | TransactionCurrency |  |  |
| `SalesDeal` | `SalesDeal` | `String(10)` |  | Sales Deal |  |  |  |
| `SalesPromotion` | `SalesPromotion` | `String(10)` |  | Promotion |  |  |  |
| `SalesOrderSalesDistrict` | `SalesOrderSalesDistrict` | `String(6)` |  | Sales Distr. Order |  |  |  |
| `SalesOrderCustomerGroup` | `SalesOrderCustomerGroup` | `String(2)` |  | Customer Grp Order |  |  |  |
| `SalesOrderCustomerPriceGroup` | `SalesOrderCustomerPriceGroup` | `String(2)` |  | Price Group of Order |  |  |  |
| `SalesOrderPriceListType` | `SalesOrderPriceListType` | `String(2)` |  | Price List Order |  |  |  |
| `SalesOrderSalesOrganization` | `SalesOrderSalesOrganization` | `String(4)` |  | Sales Org. of Order |  |  |  |
| `SalesOrderDistributionChannel` | `SalesOrderDistributionChannel` | `String(2)` |  | Distr. Channel Order |  |  |  |
| `SalesDocIsCreatedFromReference` | `SalesDocIsCreatedFromReference` | `Boolean` |  | SalesDocumentRefer |  |  |  |
| `ShippingPoint` | `ShippingPoint` | `String(4)` |  | Shipping Point |  |  |  |
| `ServiceDocumentType` | `ServiceDocumentType` | `String(4)` |  | Service Doc. Type |  |  |  |
| `ServiceDocument` | `ServiceDocument` | `String(10)` |  | Service Document |  |  |  |
| `ServiceDocumentItem` | `ServiceDocumentItem` | `String(6)` |  | Service Doc. Item |  |  |  |
| `BusinessSolutionOrder` | `BusinessSolutionOrder` | `String(10)` |  | Solution Order |  |  |  |
| `BusinessSolutionOrderItem` | `BusinessSolutionOrderItem` | `String(6)` |  | Solution Order Item |  |  |  |
| `HigherLevelItemUsage` | `HigherLevelItemUsage` | `String(1)` |  | Usage of HL Item |  |  |  |
| `BillingDocumentIsTemporary` | `BillingDocumentIsTemporary` | `Boolean` |  | Draft Indicator |  |  |  |
| `SDDocumentCategory` | `SDDocumentCategory` | `String(4)` |  | SD Document Category |  |  |  |
| `BillingDocumentType` | `BillingDocumentType` | `String(4)` |  | Billing Type |  |  |  |
| `SalesOrganization` | `SalesOrganization` | `String(4)` |  | Sales Organization |  |  |  |
| `DistributionChannel` | `DistributionChannel` | `String(2)` |  | Distribution Channel |  |  |  |
| `CustomerPriceGroup` | `CustomerPriceGroup` | `String(2)` |  | Customer Price Group |  |  |  |
| `CustomerGroup` | `CustomerGroup` | `String(2)` |  | Customer Group |  |  |  |
| `Country` | `Country` | `String(3)` |  | Dest. Country/Region |  |  |  |
| `Region` | `Region` | `String(3)` |  | Region |  |  |  |
| `CityCode` | `CityCode` | `String(4)` |  | City Code |  |  |  |
| `SalesDistrict` | `SalesDistrict` | `String(6)` |  | Sales District |  |  |  |
| `OverallSDProcessStatus` | `OverallSDProcessStatus` | `String(1)` |  | Overall Status |  |  |  |
| `OverallBillingStatus` | `OverallBillingStatus` | `String(1)` |  | Status |  |  |  |
| `SoldToParty` | `SoldToParty` | `String(10)` |  | Sold-to Party |  |  |  |
| `PayerParty` | `PayerParty` | `String(10)` |  | Payer |  |  |  |
| `BillingDocumentDate` | `BillingDocumentDate` | `Date` |  | Billing Date |  |  |  |
| `CompanyCode` | `CompanyCode` | `String(4)` |  | Company Code |  |  |  |
| `County` | `County` | `String(3)` |  | County Code |  |  |  |
| `CustomerRebateAgreement` | `CustomerRebateAgreement` | `String(10)` |  | Agreement |  |  |  |
| `BillingDocumentCategory` | `BillingDocumentCategory` | `String(1)` |  | Billing Category |  |  |  |
| `PricingDocument` | `PricingDocument` | `String(10)` |  | Doc. Condition No. |  |  |  |
| `CancelledBillingDocument` | `CancelledBillingDocument` | `String(10)` |  | Canceled Bill. Doc. |  | _CancelledBillingDocument |  |
| `ShipToParty` | `ShipToParty` | `String(10)` |  | Ship-to Party |  |  |  |
| `BillToParty` | `BillToParty` | `String(10)` |  | Bill-to Party |  |  |  |
| `SalesEmployee` | `SalesEmployee` | `String(8)` |  | Sales Employee |  |  |  |
| `ResponsibleEmployee` | `ResponsibleEmployee` | `String(8)` |  | Employee Responsible |  |  |  |
