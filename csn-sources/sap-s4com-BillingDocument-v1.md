# BillingDocument

> Source file: `sap-s4com-BillingDocument-v1.json`

**Technical Name:** `` | **Data Category:** `DIMENSION` | **VDM Type:** `BASIC` | **Size:** `L`


## Entity: `BillingDocument`

- **ABAP Name:** `I_BillingDocument`
- **Label:** Billing Document
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** vbrk

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `BillingDocument` | `VBRK` | `VBELN` | `String(10)` | Y | Billing Document |  |  |  |
| `SDDocumentCategory` |  |  | `String(4)` |  | SD Document Category |  |  |  |
| `BillingDocumentCategory` |  |  | `String(1)` |  | Billing Category |  |  |  |
| `BillingDocumentType` | `VBRK` | `FKART` | `String(4)` |  | Billing Type |  |  |  |
| `CreatedByUser` |  |  | `String(12)` |  | Created By |  |  |  |
| `CreationDate` | `VBRK` | `ERDAT` | `Date` |  | Created On |  |  |  |
| `CreationTime` |  |  | `String(6)` |  | Time |  |  |  |
| `LastChangeDate` |  |  | `Date` |  | Changed On |  |  |  |
| `LastChangeDateTime` |  |  | `Timestamp` |  | Time Stamp |  |  |  |
| `LogicalSystem` |  |  | `String(10)` |  | Logical System |  |  |  |
| `SalesOrganization` | `VBRK` | `VKORG` | `String(4)` |  | Sales Organization |  |  |  |
| `DistributionChannel` | `VBRK` | `VTWEG` | `String(2)` |  | Distribution Channel |  |  |  |
| `Division` | `VBRK` | `SPART` | `String(2)` |  | Division |  |  |  |
| `BillingDocumentDate` | `VBRK` | `FKDAT` | `Date` |  | Billing Date |  |  |  |
| `BillingDocumentIsCancelled` |  |  | `Boolean` |  | Canceled |  |  |  |
| `CancelledBillingDocument` |  |  | `String(10)` |  | Canceled Bill. Doc. |  |  |  |
| `BillingDocCombinationCriteria` |  |  | `String(40)` |  | Combination Criteria |  |  |  |
| `ManualInvoiceMaintIsRelevant` |  |  | `Boolean` |  | Man. Invoice Maint. |  |  |  |
| `NmbrOfPages` |  |  | `String(3)` |  | Number of Pages |  |  |  |
| `IsIntrastatReportingRelevant` |  |  | `Boolean` |  | Intrastat Relevance |  |  |  |
| `IsIntrastatReportingExcluded` |  |  | `Boolean` |  | Intrastat Exclusion |  |  |  |
| `BillingDocumentIsTemporary` |  |  | `Boolean` |  | Draft Indicator |  |  |  |
| `TotalNetAmount` |  |  | `Decimal(34,4)` |  | Net Value | TransactionCurrency |  |  |
| `TransactionCurrency` | `VBRK` | `WAERK` | `String(5)` |  | Document Currency |  |  |  |
| `StatisticsCurrency` |  |  | `String(5)` |  | Statistics Currency |  |  |  |
| `TotalTaxAmount` |  |  | `Decimal(34,4)` |  | Tax Amount | TransactionCurrency |  |  |
| `CustomerPriceGroup` |  |  | `String(2)` |  | Customer Price Group |  |  |  |
| `PriceListType` |  |  | `String(2)` |  | Price List Type |  |  |  |
| `TaxDepartureCountry` |  |  | `String(3)` |  | Tax Departure C/R |  |  |  |
| `VATRegistration` |  |  | `String(20)` |  | VAT Registration No. |  |  |  |
| `VATRegistrationOrigin` |  |  | `String(1)` |  | Origin Sales Tax No. |  |  |  |
| `VATRegistrationCountry` |  |  | `String(3)` |  | Ctry/Rgn Sls Tax No. |  |  |  |
| `HierarchyTypePricing` |  |  | `String(1)` |  | HierarchyTypePricing |  |  |  |
| `CustomerTaxClassification1` |  |  | `String(1)` |  | Tax Class.1 Customer |  |  |  |
| `CustomerTaxClassification2` |  |  | `String(1)` |  | Tax Class.2 Customer |  |  |  |
| `CustomerTaxClassification3` |  |  | `String(1)` |  | Tax Class.3 Customer |  |  |  |
| `CustomerTaxClassification4` |  |  | `String(1)` |  | Tax Class.4 Customer |  |  |  |
| `CustomerTaxClassification5` |  |  | `String(1)` |  | Tax Class.5 Customer |  |  |  |
| `CustomerTaxClassification6` |  |  | `String(1)` |  | Tax Class.6 Customer |  |  |  |
| `CustomerTaxClassification7` |  |  | `String(1)` |  | Tax Class.7 Customer |  |  |  |
| `CustomerTaxClassification8` |  |  | `String(1)` |  | Tax Class.8 Customer |  |  |  |
| `CustomerTaxClassification9` |  |  | `String(1)` |  | Tax Class.9 Customer |  |  |  |
| `IsEUTriangularDeal` |  |  | `Boolean` |  | EU Triangular Deal |  |  |  |
| `SDPricingProcedure` |  |  | `String(6)` |  | Pricing Procedure |  |  |  |
| `ShippingCondition` |  |  | `String(2)` |  | Shipping Conditions |  |  |  |
| `PlantSupplier` |  |  | `String(10)` |  | Sppl. No. Plnt |  |  |  |
| `IncotermsVersion` |  |  | `String(4)` |  | Incoterms Version |  |  |  |
| `IncotermsClassification` |  |  | `String(3)` |  | Incoterms |  |  |  |
| `IncotermsTransferLocation` |  |  | `String(28)` |  | Incoterms (Part 2) |  |  |  |
| `IncotermsLocation1` |  |  | `String(70)` |  | Incoterms Location 1 |  |  |  |
| `IncotermsLocation2` |  |  | `String(70)` |  | Incoterms Location 2 |  |  |  |
| `PayerParty` | `VBRK` | `KUNRG` | `String(10)` |  | Payer |  |  |  |
| `ContractAccount` |  |  | `String(12)` |  | Contract Account |  |  |  |
| `CustomerPaymentTerms` |  |  | `String(4)` |  | Terms of Payment |  |  |  |
| `PaymentMethod` |  |  | `String(1)` |  | Payment Method |  |  |  |
| `PaymentReference` |  |  | `String(30)` |  | Payment Reference |  |  |  |
| `FixedValueDate` |  |  | `Date` |  | Fixed Value Date |  |  |  |
| `AdditionalValueDays` |  |  | `String(2)` |  | Addit. Value Days |  |  |  |
| `SEPAMandate` |  |  | `String(35)` |  | Mandate Reference |  |  |  |
| `CompanyCode` | `VBRK` | `BUKRS` | `String(4)` |  | Company Code |  |  |  |
| `FiscalYear` | `VBRK` | `GJAHR` | `String(4)` |  | Fiscal Year |  |  |  |
| `AccountingDocument` | `VBRK` | `BELNR` | `String(10)` |  | Document Number |  |  |  |
| `FiscalPeriod` |  |  | `String(3)` |  | Posting Period |  |  | ECC BKPF.MONAT unpadded ('3'); S/4 zero-padded ('003') |
| `CustomerAccountAssignmentGroup` |  |  | `String(2)` |  | Acct Assmt Grp Cust. |  |  |  |
| `AccountingExchangeRateIsSet` |  |  | `Boolean` |  | Set Exchange Rate |  |  |  |
| `AccountingExchangeRate` |  |  | `Decimal(9,5)` |  | Accounting Exchange Rate |  |  |  |
| `ExchangeRateDate` |  |  | `Date` |  | Translation Date |  |  |  |
| `ExchangeRateType` |  |  | `String(4)` |  | Exchange Rate Type |  |  |  |
| `DocumentReferenceID` |  |  | `String(16)` |  | Reference |  |  |  |
| `AssignmentReference` |  |  | `String(18)` |  | Assignment |  |  |  |
| `ReversalReason` |  |  | `String(2)` |  | Reversal Reason |  |  |  |
| `DunningArea` |  |  | `String(2)` |  | Dunning Area |  |  |  |
| `DunningBlockingReason` |  |  | `String(1)` |  | Dunning Block |  |  |  |
| `DunningKey` |  |  | `String(1)` |  | Dunning Key |  |  |  |
| `InternalFinancialDocument` |  |  | `String(10)` |  | Financial Doc. No. |  |  |  |
| `IsRelevantForAccrual` |  |  | `Boolean` |  | Relevant for Accrual |  |  |  |
| `SoldToParty` |  |  | `String(10)` |  | Sold-to Party |  |  |  |
| `PartnerCompany` |  |  | `String(6)` |  | Trading Partner No. |  |  |  |
| `PurchaseOrderByCustomer` |  |  | `String(35)` |  | Customer Reference |  |  |  |
| `CustomerGroup` |  |  | `String(2)` |  | Customer Group |  |  |  |
| `Country` |  |  | `String(3)` |  | Dest. Country/Region |  |  |  |
| `CityCode` |  |  | `String(4)` |  | City Code |  |  |  |
| `SalesDistrict` |  |  | `String(6)` |  | Sales District |  |  |  |
| `Region` |  |  | `String(3)` |  | Region |  |  |  |
| `County` |  |  | `String(3)` |  | County Code |  |  |  |
| `CreditControlArea` |  |  | `String(4)` |  | Credit Control Area |  |  |  |
| `CustomerRebateAgreement` |  |  | `String(10)` |  | Agreement |  |  |  |
| `PricingDocument` |  |  | `String(10)` |  | Doc. Condition No. |  |  |  |
| `OverallSDProcessStatus` |  |  | `String(1)` |  | Overall Status |  |  |  |
| `OverallBillingStatus` |  |  | `String(1)` |  | Status |  |  |  |
| `AccountingPostingStatus` |  |  | `String(1)` |  | Posting Status |  |  |  |
| `AccountingTransferStatus` |  |  | `String(1)` |  | Posting Status |  |  |  |
| `BillingIssueType` |  |  | `String(1)` |  | Issue Type |  |  |  |
| `InvoiceListStatus` |  |  | `String(1)` |  | Invoice List Status |  |  |  |
| `OvrlItmGeneralIncompletionSts` |  |  | `String(1)` |  | All Items |  |  |  |
| `OverallPricingIncompletionSts` |  |  | `String(1)` |  | Pricing – All Items |  |  |  |
| `InvoiceClearingStatus` |  |  | `String(1)` |  | Clearing Status |  |  |  |
| `InvoiceListType` |  |  | `String(4)` |  | Invoice List Type |  |  |  |
| `InvoiceListBillingDate` |  |  | `Date` |  | Inv. List Bill. Date |  |  |  |
| `ForeignTradeStstclCurrency` |  |  | `String(5)` |  | Currency |  |  |  |


## Entity: `BillingDocumentItem`

- **ABAP Name:** `I_BillingDocumentItem`
- **Label:** Billing Document Item
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** vbrp

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `BillingDocument` | `VBRK` | `VBELN` | `String(10)` | Y | Billing Document |  | _BillingDocument |  |
| `BillingDocumentItem` | `VBRP` | `POSNR` | `String(6)` | Y | Item |  |  |  |
| `SalesDocumentItemCategory` |  |  | `String(4)` |  | Sales Doc. Item Cat. |  |  |  |
| `SalesDocumentItemType` |  |  | `String(1)` |  | Item Type |  |  |  |
| `ReturnItemProcessingType` |  |  | `String(1)` |  | Returns |  |  |  |
| `CreatedByUser` |  |  | `String(12)` |  | Created By |  |  |  |
| `CreationDate` | `VBRK` | `ERDAT` | `Date` |  | Created On |  |  |  |
| `CreationTime` |  |  | `String(6)` |  | Time |  |  |  |
| `ReferenceLogicalSystem` |  |  | `String(10)` |  | Logical System |  |  |  |
| `OrganizationDivision` |  |  | `String(2)` |  | Division of Order |  |  |  |
| `Division` | `VBRK` | `SPART` | `String(2)` |  | Division |  |  |  |
| `SalesOffice` |  |  | `String(4)` |  | Sales Office |  |  |  |
| `Material` | `VBRP` | `MATNR` | `String(40)` |  | Material |  |  |  |
| `Product` |  |  | `String(40)` |  | Product |  |  |  |
| `OriginallyRequestedMaterial` |  |  | `String(40)` |  | Material Entered |  |  |  |
| `InternationalArticleNumber` |  |  | `String(18)` |  | EAN/UPC |  |  |  |
| `PricingReferenceMaterial` |  |  | `String(40)` |  | Pricing Ref. Matl |  |  |  |
| `Batch` |  |  | `String(10)` |  | Batch |  |  |  |
| `ProductHierarchyNode` |  |  | `String(18)` |  | Product Hierarchy |  |  |  |
| `MaterialGroup` |  |  | `String(9)` |  | Material Group |  |  |  |
| `ProductGroup` |  |  | `String(9)` |  | Product Group |  |  |  |
| `AdditionalMaterialGroup1` |  |  | `String(3)` |  | Material Group 1 |  |  |  |
| `AdditionalMaterialGroup2` |  |  | `String(3)` |  | Material Group 2 |  |  |  |
| `AdditionalMaterialGroup3` |  |  | `String(3)` |  | Material Group 3 |  |  |  |
| `AdditionalMaterialGroup4` |  |  | `String(3)` |  | Material Group 4 |  |  |  |
| `AdditionalMaterialGroup5` |  |  | `String(3)` |  | Material Group 5 |  |  |  |
| `ProductConfiguration` |  |  | `String(18)` |  | Configuration |  |  |  |
| `MaterialCommissionGroup` |  |  | `String(2)` |  | Commission Group |  |  |  |
| `Plant` | `VBRP` | `WERKS` | `String(4)` |  | Plant |  |  |  |
| `StorageLocation` |  |  | `String(4)` |  | Storage Location |  |  |  |
| `ReplacementPartType` |  |  | `String(1)` |  | Replacement Part |  |  |  |
| `MaterialGroupHierarchy1` |  |  | `String(18)` |  | Material Group 1 |  |  |  |
| `MaterialGroupHierarchy2` |  |  | `String(18)` |  | Material Group 2 |  |  |  |
| `PlantRegion` |  |  | `String(3)` |  | Region of Dlv. Plant |  |  |  |
| `PlantCounty` |  |  | `String(3)` |  | County of Dlv.Plant |  |  |  |
| `PlantCity` |  |  | `String(4)` |  | City of Deliv. Plant |  |  |  |
| `TransitPlant` |  |  | `String(4)` |  | Transit Plant |  |  |  |
| `ValueChainCategory` |  |  | `String(4)` |  | Value Chain Category |  |  |  |
| `BOMExplosion` |  |  | `String(8)` |  | BOM Explosion Number |  |  |  |
| `MaterialDeterminationType` |  |  | `String(1)` |  | Mat.Determ.Active |  |  |  |
| `SoldProduct` |  |  | `String(40)` |  | Product Sold |  |  |  |
| `BillingDocumentItemText` |  |  | `String(40)` |  | Item Description |  |  |  |
| `ServicesRenderedDate` |  |  | `Date` |  | Serv. Rendered Date |  |  |  |
| `BillingQuantity` | `VBRP` | `FKIMG` | `Decimal(13,3)` |  | Invoiced Quantity | BillingQuantityUnit |  |  |
| `BillingQuantityUnit` |  |  | `String(3)` |  | Sales Unit |  |  |  |
| `BillingQuantityInBaseUnit` |  |  | `Decimal(13,3)` |  | Billing Qty in SKU | BaseUnit |  |  |
| `BaseUnit` |  |  | `String(3)` |  | Base Unit of Measure |  |  |  |
| `MRPRequiredQuantityInBaseUnit` |  |  | `Decimal(13,3)` |  | Required Quantity | BaseUnit |  |  |
| `BillingToBaseQuantityDnmntr` |  |  | `Decimal(5,0)` |  | Denominator |  |  |  |
| `BillingToBaseQuantityNmrtr` |  |  | `Decimal(5,0)` |  | Numerator |  |  |  |
| `ItemGrossWeight` |  |  | `Decimal(15,3)` |  | Gross Weight | ItemWeightUnit |  |  |
| `ItemNetWeight` |  |  | `Decimal(15,3)` |  | Net Weight | ItemWeightUnit |  |  |
| `ItemWeightUnit` |  |  | `String(3)` |  | Unit of Weight |  |  |  |
| `ItemVolume` |  |  | `Decimal(15,3)` |  | Volume | ItemVolumeUnit |  |  |
| `ItemVolumeUnit` |  |  | `String(3)` |  | Volume Unit |  |  |  |
| `BillToPartyCountry` |  |  | `String(3)` |  | Dest. Ctry/Reg. Ord. |  |  |  |
| `BillToPartyRegion` |  |  | `String(3)` |  | Region Order |  |  |  |
| `BillingPlanRule` |  |  | `String(1)` |  | Billing Rule |  |  |  |
| `BillingPlan` |  |  | `String(10)` |  | Bill. Plan No. |  |  |  |
| `BillingPlanItem` |  |  | `String(6)` |  | Item |  |  |  |
| `DownPaymentProcessingVariant` |  |  | `String(1)` |  | Down Payment Variant |  |  |  |
| `NetAmount` | `VBRP` | `NETWR` | `Decimal(34,4)` |  | Net Value | TransactionCurrency |  |  |
| `TransactionCurrency` | `VBRK` | `WAERK` | `String(5)` |  | Document Currency |  |  |  |
| `GrossAmount` |  |  | `Decimal(34,4)` |  | Gross Value | TransactionCurrency |  |  |
| `PricingDate` |  |  | `Date` |  | Pricing Date |  |  |  |
| `PriceDetnExchangeRate` |  |  | `Decimal(9,5)` |  | Exchange Rate |  |  |  |
| `PricingScaleQuantityInBaseUnit` |  |  | `Decimal(13,3)` |  | Scale Quantity | BaseUnit |  |  |
| `TaxAmount` | `VBRK` | `MWSBK` | `Decimal(34,4)` |  | Tax Amount | TransactionCurrency |  |  |
| `CostAmount` |  |  | `Decimal(34,4)` |  | Cost | TransactionCurrency |  |  |
| `Subtotal1Amount` |  |  | `Decimal(34,4)` |  | Subtotal 1 | TransactionCurrency |  |  |
| `Subtotal2Amount` |  |  | `Decimal(34,4)` |  | Subtotal 2 | TransactionCurrency |  |  |
| `Subtotal3Amount` |  |  | `Decimal(34,4)` |  | Subtotal 3 | TransactionCurrency |  |  |
| `Subtotal4Amount` |  |  | `Decimal(34,4)` |  | Subtotal 4 | TransactionCurrency |  |  |
| `Subtotal5Amount` |  |  | `Decimal(34,4)` |  | Subtotal 5 | TransactionCurrency |  |  |
| `Subtotal6Amount` |  |  | `Decimal(34,4)` |  | Subtotal 6 | TransactionCurrency |  |  |
| `StatisticalValueControl` |  |  | `String(1)` |  | Statistical Value |  |  |  |
| `CashDiscountIsDeductible` |  |  | `Boolean` |  | Cash Discount |  |  |  |
| `CustomerConditionGroup1` |  |  | `String(2)` |  | Condition Group 1 |  |  |  |
| `CustomerConditionGroup2` |  |  | `String(2)` |  | Condition Group 2 |  |  |  |
| `CustomerConditionGroup3` |  |  | `String(2)` |  | Condition Group 3 |  |  |  |
| `CustomerConditionGroup4` |  |  | `String(2)` |  | Condition Group 4 |  |  |  |
| `CustomerConditionGroup5` |  |  | `String(2)` |  | Condition Group 5 |  |  |  |
| `ManualPriceChangeType` |  |  | `String(1)` |  | Manual Price |  |  |  |
| `MaterialPricingGroup` |  |  | `String(2)` |  | Material Price Grp |  |  |  |
| `StatisticsExchangeRate` |  |  | `Decimal(9,5)` |  | Exchange Rate Stats. |  |  |  |
| `MainItemPricingRefMaterial` |  |  | `String(40)` |  | Pricing Ref.Material |  |  |  |
| `MainItemMaterialPricingGroup` |  |  | `String(2)` |  | MnItem MatPricingGrp |  |  |  |
| `TimeSheetOvertimeCategory` |  |  | `String(4)` |  | Overtime Category |  |  |  |
| `PricingRelevance` |  |  | `String(1)` |  | Pricing Relevance |  |  |  |
| `DepartureCountry` |  |  | `String(3)` |  | Departure Ctry/Reg. |  |  |  |
| `TaxJurisdiction` |  |  | `String(15)` |  | Tax Jurisdiction |  |  |  |
| `ProductTaxClassification1` |  |  | `String(1)` |  | Product Tax Classification 1 |  |  |  |
| `ProductTaxClassification2` |  |  | `String(1)` |  | Product Tax Classification 2 |  |  |  |
| `ProductTaxClassification3` |  |  | `String(1)` |  | Product Tax Classification 3 |  |  |  |
| `ProductTaxClassification4` |  |  | `String(1)` |  | Product Tax Classification 4 |  |  |  |
| `ProductTaxClassification5` |  |  | `String(1)` |  | Product Tax Classification 5 |  |  |  |
| `ProductTaxClassification6` |  |  | `String(1)` |  | Product Tax Classification 6 |  |  |  |
| `ProductTaxClassification7` |  |  | `String(1)` |  | Product Tax Classification 7 |  |  |  |
| `ProductTaxClassification8` |  |  | `String(1)` |  | Product Tax Classification 8 |  |  |  |
| `ProductTaxClassification9` |  |  | `String(1)` |  | Product Tax Classification 9 |  |  |  |
| `ZeroVATRsn` |  |  | `String(1)` |  | Reason 0 VAT |  |  |  |
| `TaxCode` |  |  | `String(2)` |  | Tax Code |  |  |  |
| `TaxRateValidityStartDate` |  |  | `Date` |  | Tax Rate Valid-From |  |  |  |
| `CountryOfOrigin` |  |  | `String(3)` |  | Cntry/Reg of Origin |  |  |  |
| `RegionOfOrigin` |  |  | `String(3)` |  | Region of Origin |  |  |  |
| `CommodityCode` |  |  | `String(30)` |  | Commodity Code |  |  |  |
| `EligibleAmountForCashDiscount` |  |  | `Decimal(34,4)` |  | Cash Disc. Bas. | TransactionCurrency |  |  |
| `BusinessArea` |  |  | `String(4)` |  | Business Area |  |  |  |
| `ProfitCenter` |  |  | `String(10)` |  | Profit Center |  |  |  |
| `OrderID` |  |  | `String(12)` |  | Order |  |  |  |
| `WBSElement` |  |  | `String(8)` |  | WBS Element |  |  |  |
| `WBSElementInternalID` |  |  | `String(8)` |  | WBS Internal ID |  |  |  |
| `ProviderContract` |  |  | `String(20)` |  | Provider Contract |  |  |  |
| `ProviderContractItem` |  |  | `String(6)` |  | Provider Contract Item |  |  |  |
| `BillingPerformancePeriodStrDte` |  |  | `Date` |  | Per. of Perf. Start |  |  |  |
| `BillingPeriodOfPerfStartDate` |  |  | `Date` |  | Per. of Perf. Start |  |  |  |
| `BillingPerformancePeriodEndDte` |  |  | `Date` |  | Per. of Perf. End |  |  |  |
| `BillingPeriodOfPerfEndDate` |  |  | `Date` |  | Per. of Perf. End |  |  |  |
| `ControllingArea` | `TKA01` | `KOKRS` | `String(4)` |  | Controlling Area |  |  |  |
| `ProfitabilitySegment` |  |  | `String(10)` |  | Profitability Segment (Deprecated) |  |  |  |
| `ProfitabilitySegment_2` |  |  | `String(10)` |  | Profitability Segment |  |  |  |
| `CostCenter` |  |  | `String(10)` |  | Cost Center |  |  |  |
| `OriginSDDocument` |  |  | `String(10)` |  | Originating Document |  |  |  |
| `OriginSDDocumentItem` |  |  | `String(6)` |  | Originating Item |  |  |  |
| `PriceDetnExchangeRateDate` |  |  | `Date` |  | Translation Date |  |  |  |
| `MatlAccountAssignmentGroup` |  |  | `String(2)` |  | Acct Assmt Grp Mat. |  |  |  |
| `ReferenceSDDocument` |  |  | `String(10)` |  | Reference Document |  |  |  |
| `ReferenceSDDocumentItem` |  |  | `String(6)` |  | Reference Item |  |  |  |
| `ReferenceSDDocumentCategory` |  |  | `String(4)` |  | Ref. Doc. Category |  |  |  |
| `SalesDocument` | `VBRP` | `AUBEL` | `String(10)` |  | Sales Document |  |  |  |
| `SalesDocumentItem` | `VBRP` | `AUPOS` | `String(6)` |  | Sales Document Item |  |  |  |
| `SalesSDDocumentCategory` |  |  | `String(4)` |  | Sales Doc. Category |  |  |  |
| `HigherLevelItem` |  |  | `String(6)` |  | Higher-Level Item |  |  |  |
| `HigherLvlItmOfBatSpltItm` |  |  | `String(6)` |  | HigherLevelItemBatch |  |  |  |
| `BillingDocumentItemInPartSgmt` |  |  | `String(6)` |  | Partner Item |  |  |  |
| `ExternalReferenceDocument` |  |  | `String(10)` |  | Ext. Reference Document |  |  |  |
| `ExternalReferenceDocumentItem` |  |  | `String(6)` |  | Ext. Ref. Document Item |  |  |  |
| `BillingDocExtReferenceDocItem` |  |  | `String(6)` |  | Ext. Reference Doc. Item |  |  |  |
| `PrelimBillingDocument` |  |  | `String(10)` |  | Prelimin. Bill. Doc. |  |  |  |
| `PrelimBillingDocumentItem` |  |  | `String(6)` |  | Prelimin. Doc. Item |  |  |  |
| `SalesGroup` |  |  | `String(3)` |  | Sales Group |  |  |  |
| `AdditionalCustomerGroup1` |  |  | `String(3)` |  | Customer Group 1 |  |  |  |
| `AdditionalCustomerGroup2` |  |  | `String(3)` |  | Customer Group 2 |  |  |  |
| `AdditionalCustomerGroup3` |  |  | `String(3)` |  | Customer Group 3 |  |  |  |
| `AdditionalCustomerGroup4` |  |  | `String(3)` |  | Customer Group 4 |  |  |  |
| `AdditionalCustomerGroup5` |  |  | `String(3)` |  | Customer Group 5 |  |  |  |
| `SDDocumentReason` |  |  | `String(3)` |  | Order Reason |  |  |  |
| `RetailPromotion` |  |  | `String(10)` |  | Retail Promotion |  |  |  |
| `RebateBasisAmount` |  |  | `Decimal(34,4)` |  | Rebate Basis | TransactionCurrency |  |  |
| `VolumeRebateGroup` |  |  | `String(2)` |  | Volume Rebate Group |  |  |  |
| `ItemIsRelevantForCredit` |  |  | `Boolean` |  | Credit Funct. Active |  |  |  |
| `CreditRelatedPrice` |  |  | `Decimal(34,4)` |  | Credit Price | TransactionCurrency |  |  |
| `SalesDeal` |  |  | `String(10)` |  | Sales Deal |  |  |  |
| `SalesPromotion` |  |  | `String(10)` |  | Promotion |  |  |  |
| `SalesOrderSalesDistrict` |  |  | `String(6)` |  | Sales Distr. Order |  |  |  |
| `SalesOrderCustomerGroup` |  |  | `String(2)` |  | Customer Grp Order |  |  |  |
| `SalesOrderCustomerPriceGroup` |  |  | `String(2)` |  | Price Group of Order |  |  |  |
| `SalesOrderPriceListType` |  |  | `String(2)` |  | Price List Order |  |  |  |
| `SalesOrderSalesOrganization` |  |  | `String(4)` |  | Sales Org. of Order |  |  |  |
| `SalesOrderDistributionChannel` |  |  | `String(2)` |  | Distr. Channel Order |  |  |  |
| `SalesDocIsCreatedFromReference` |  |  | `Boolean` |  | SalesDocumentRefer |  |  |  |
| `ShippingPoint` |  |  | `String(4)` |  | Shipping Point |  |  |  |
| `ServiceDocumentType` |  |  | `String(4)` |  | Service Doc. Type |  |  |  |
| `ServiceDocument` |  |  | `String(10)` |  | Service Document |  |  |  |
| `ServiceDocumentItem` |  |  | `String(6)` |  | Service Doc. Item |  |  |  |
| `BusinessSolutionOrder` |  |  | `String(10)` |  | Solution Order |  |  |  |
| `BusinessSolutionOrderItem` |  |  | `String(6)` |  | Solution Order Item |  |  |  |
| `HigherLevelItemUsage` |  |  | `String(1)` |  | Usage of HL Item |  |  |  |
| `BillingDocumentIsTemporary` |  |  | `Boolean` |  | Draft Indicator |  |  |  |
| `SDDocumentCategory` |  |  | `String(4)` |  | SD Document Category |  |  |  |
| `BillingDocumentType` | `VBRK` | `FKART` | `String(4)` |  | Billing Type |  |  |  |
| `SalesOrganization` | `VBRK` | `VKORG` | `String(4)` |  | Sales Organization |  |  |  |
| `DistributionChannel` | `VBRK` | `VTWEG` | `String(2)` |  | Distribution Channel |  |  |  |
| `CustomerPriceGroup` |  |  | `String(2)` |  | Customer Price Group |  |  |  |
| `CustomerGroup` |  |  | `String(2)` |  | Customer Group |  |  |  |
| `Country` |  |  | `String(3)` |  | Dest. Country/Region |  |  |  |
| `Region` |  |  | `String(3)` |  | Region |  |  |  |
| `CityCode` |  |  | `String(4)` |  | City Code |  |  |  |
| `SalesDistrict` |  |  | `String(6)` |  | Sales District |  |  |  |
| `OverallSDProcessStatus` |  |  | `String(1)` |  | Overall Status |  |  |  |
| `OverallBillingStatus` |  |  | `String(1)` |  | Status |  |  |  |
| `SoldToParty` |  |  | `String(10)` |  | Sold-to Party |  |  |  |
| `PayerParty` | `VBRK` | `KUNRG` | `String(10)` |  | Payer |  |  |  |
| `BillingDocumentDate` | `VBRK` | `FKDAT` | `Date` |  | Billing Date |  |  |  |
| `CompanyCode` | `VBRK` | `BUKRS` | `String(4)` |  | Company Code |  |  |  |
| `County` |  |  | `String(3)` |  | County Code |  |  |  |
| `CustomerRebateAgreement` |  |  | `String(10)` |  | Agreement |  |  |  |
| `BillingDocumentCategory` |  |  | `String(1)` |  | Billing Category |  |  |  |
| `PricingDocument` |  |  | `String(10)` |  | Doc. Condition No. |  |  |  |
| `CancelledBillingDocument` |  |  | `String(10)` |  | Canceled Bill. Doc. |  | _CancelledBillingDocument |  |
| `ShipToParty` |  |  | `String(10)` |  | Ship-to Party |  |  |  |
| `BillToParty` |  |  | `String(10)` |  | Bill-to Party |  |  |  |
| `SalesEmployee` |  |  | `String(8)` |  | Sales Employee |  |  |  |
| `ResponsibleEmployee` |  |  | `String(8)` |  | Employee Responsible |  |  |  |
