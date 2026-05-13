# BillingDocument

> Source file: `sap-s4com-BillingDocument-v1.json`

**Technical Name:** `` | **Data Category:** `DIMENSION` | **VDM Type:** `BASIC` | **Size:** `L`


## Entity: `BillingDocument`

- **ABAP CDS Name:** `I_BillingDocument`
- **Label:** Billing Document
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** VBRK

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `BillingDocument` | `VBELN_VF` | `VBRK` | `VBELN` |  |  | `String(10)` | Y | Billing Document |  |  |
| `SDDocumentCategory` | `VBTYPL` |  |  |  |  | `String(4)` |  | SD Document Category |  |  |
| `BillingDocumentCategory` | `FKTYP` |  |  |  |  | `String(1)` |  | Billing Category |  |  |
| `BillingDocumentType` | `FKART` | `VBRK` | `FKART` |  |  | `String(4)` |  | Billing Type |  |  |
| `CreatedByUser` | `ERNAM` |  |  |  |  | `String(12)` |  | Created By |  |  |
| `CreationDate` | `ERDAT` | `VBRK` | `ERDAT` |  |  | `Date` |  | Created On |  |  |
| `CreationTime` | `ERZET` |  |  |  |  | `String(6)` |  | Time |  |  |
| `LastChangeDate` | `AEDAT` |  |  |  |  | `Date` |  | Changed On |  |  |
| `LastChangeDateTime` | `TIMESTAMPL` |  |  |  |  | `Timestamp` |  | Time Stamp |  |  |
| `LogicalSystem` | `LOGSYS` |  |  |  |  | `String(10)` |  | Logical System |  |  |
| `SalesOrganization` | `VKORG` | `VBRK` | `VKORG` |  |  | `String(4)` |  | Sales Organization |  |  |
| `DistributionChannel` | `VTWEG` | `VBRK` | `VTWEG` |  |  | `String(2)` |  | Distribution Channel |  |  |
| `Division` | `SPART` | `VBRK` | `SPART` |  |  | `String(2)` |  | Division |  |  |
| `BillingDocumentDate` | `FKDAT` | `VBRK` | `FKDAT` |  |  | `Date` |  | Billing Date |  |  |
| `BillingDocumentIsCancelled` | `FKSTO` |  |  |  |  | `Boolean` |  | Canceled |  |  |
| `CancelledBillingDocument` | `SFAKN` |  |  |  |  | `String(10)` |  | Canceled Bill. Doc. |  |  |
| `BillingDocCombinationCriteria` | `DZUKRI` |  |  |  |  | `String(40)` |  | Combination Criteria |  |  |
| `ManualInvoiceMaintIsRelevant` | `MRNKZ` |  |  |  |  | `Boolean` |  | Man. Invoice Maint. |  |  |
| `NmbrOfPages` | `J_1ANOPG` |  |  |  |  | `String(3)` |  | Number of Pages |  |  |
| `IsIntrastatReportingRelevant` | `INTRA_REL` |  |  |  |  | `Boolean` |  | Intrastat Relevance |  |  |
| `IsIntrastatReportingExcluded` | `INTRA_EXCL` |  |  |  |  | `Boolean` |  | Intrastat Exclusion |  |  |
| `BillingDocumentIsTemporary` | `VF_DRAFT_INDICATOR` |  |  |  |  | `Boolean` |  | Draft Indicator |  |  |
| `TotalNetAmount` | `NETWR` |  |  |  |  | `Decimal(34,4)` |  | Net Value | TransactionCurrency |  |
| `TransactionCurrency` | `WAERK` | `VBRK` | `WAERK` |  |  | `String(5)` |  | Document Currency |  |  |
| `StatisticsCurrency` | `STWAE` |  |  |  |  | `String(5)` |  | Statistics Currency |  |  |
| `TotalTaxAmount` | `MWSBP` |  |  |  |  | `Decimal(34,4)` |  | Tax Amount | TransactionCurrency |  |
| `CustomerPriceGroup` | `KONDA` |  |  |  |  | `String(2)` |  | Customer Price Group |  |  |
| `PriceListType` | `PLTYP` |  |  |  |  | `String(2)` |  | Price List Type |  |  |
| `TaxDepartureCountry` | `LANDTX` |  |  |  |  | `String(3)` |  | Tax Departure C/R |  |  |
| `VATRegistration` | `STCEG` |  |  |  |  | `String(20)` |  | VAT Registration No. |  |  |
| `VATRegistrationOrigin` | `STCEG_H` |  |  |  |  | `String(1)` |  | Origin Sales Tax No. |  |  |
| `VATRegistrationCountry` | `STCEG_L` |  |  |  |  | `String(3)` |  | Ctry/Rgn Sls Tax No. |  |  |
| `HierarchyTypePricing` | `HITYP_PR` |  |  |  |  | `String(1)` |  | HierarchyTypePricing |  |  |
| `CustomerTaxClassification1` | `TAXK1` |  |  |  |  | `String(1)` |  | Tax Class.1 Customer |  |  |
| `CustomerTaxClassification2` | `TAXK2` |  |  |  |  | `String(1)` |  | Tax Class.2 Customer |  |  |
| `CustomerTaxClassification3` | `TAXK3` |  |  |  |  | `String(1)` |  | Tax Class.3 Customer |  |  |
| `CustomerTaxClassification4` | `TAXK4` |  |  |  |  | `String(1)` |  | Tax Class.4 Customer |  |  |
| `CustomerTaxClassification5` | `TAXK5` |  |  |  |  | `String(1)` |  | Tax Class.5 Customer |  |  |
| `CustomerTaxClassification6` | `TAXK6` |  |  |  |  | `String(1)` |  | Tax Class.6 Customer |  |  |
| `CustomerTaxClassification7` | `TAXK7` |  |  |  |  | `String(1)` |  | Tax Class.7 Customer |  |  |
| `CustomerTaxClassification8` | `TAXK8` |  |  |  |  | `String(1)` |  | Tax Class.8 Customer |  |  |
| `CustomerTaxClassification9` | `TAXK9` |  |  |  |  | `String(1)` |  | Tax Class.9 Customer |  |  |
| `IsEUTriangularDeal` | `XEGDR` |  |  |  |  | `Boolean` |  | EU Triangular Deal |  |  |
| `SDPricingProcedure` | `KALSMASD` |  |  |  |  | `String(6)` |  | Pricing Procedure |  |  |
| `ShippingCondition` | `VSBED` |  |  |  |  | `String(2)` |  | Shipping Conditions |  |  |
| `PlantSupplier` | `LIFNR_WK` |  |  |  |  | `String(10)` |  | Sppl. No. Plnt |  |  |
| `IncotermsVersion` | `INCOV` |  |  |  |  | `String(4)` |  | Incoterms Version |  |  |
| `IncotermsClassification` | `INCO1` |  |  |  |  | `String(3)` |  | Incoterms |  |  |
| `IncotermsTransferLocation` | `INCO2` |  |  |  |  | `String(28)` |  | Incoterms (Part 2) |  |  |
| `IncotermsLocation1` | `INCO2_L` |  |  |  |  | `String(70)` |  | Incoterms Location 1 |  |  |
| `IncotermsLocation2` | `INCO3_L` |  |  |  |  | `String(70)` |  | Incoterms Location 2 |  |  |
| `PayerParty` | `KUNRG` | `VBRK` | `KUNRG` |  |  | `String(10)` |  | Payer |  |  |
| `ContractAccount` | `CORR_VKONT_KK` |  |  |  |  | `String(12)` |  | Contract Account |  |  |
| `CustomerPaymentTerms` | `DZTERM` |  |  |  |  | `String(4)` |  | Terms of Payment |  |  |
| `PaymentMethod` | `SCHZW_BSEG` |  |  |  |  | `String(1)` |  | Payment Method |  |  |
| `PaymentReference` | `KIDNO` |  |  |  |  | `String(30)` |  | Payment Reference |  |  |
| `FixedValueDate` | `VALDT` |  |  |  |  | `Date` |  | Fixed Value Date |  |  |
| `AdditionalValueDays` | `VALTG` |  |  |  |  | `String(2)` |  | Addit. Value Days |  |  |
| `SEPAMandate` | `SEPA_MNDID` |  |  |  |  | `String(35)` |  | Mandate Reference |  |  |
| `CompanyCode` | `BUKRS` | `VBRK` | `BUKRS` |  |  | `String(4)` |  | Company Code |  |  |
| `FiscalYear` | `GJAHR` | `VBRK` | `GJAHR` |  |  | `String(4)` |  | Fiscal Year |  |  |
| `AccountingDocument` | `BELNR_D` | `VBRK` | `BELNR` |  |  | `String(10)` |  | Document Number |  |  |
| `FiscalPeriod` | `POPER` |  |  |  |  | `String(3)` |  | Posting Period |  |  |
| `CustomerAccountAssignmentGroup` | `KTGRD` |  |  |  |  | `String(2)` |  | Acct Assmt Grp Cust. |  |  |
| `AccountingExchangeRateIsSet` | `CPKUR` |  |  |  |  | `Boolean` |  | Set Exchange Rate |  |  |
| `AccountingExchangeRate` | `KURRF_NOT_CONVERTED` |  |  |  |  | `Decimal(9,5)` |  | Accounting Exchange Rate |  |  |
| `ExchangeRateDate` | `WWERT_D` |  |  |  |  | `Date` |  | Translation Date |  |  |
| `ExchangeRateType` | `KURST` |  |  |  |  | `String(4)` |  | Exchange Rate Type |  |  |
| `DocumentReferenceID` | `XBLNR_V1` |  |  |  |  | `String(16)` |  | Reference |  |  |
| `AssignmentReference` | `ORDNR_V` |  |  |  |  | `String(18)` |  | Assignment |  |  |
| `ReversalReason` | `STGRD` |  |  |  |  | `String(2)` |  | Reversal Reason |  |  |
| `DunningArea` | `MABER` |  |  |  |  | `String(2)` |  | Dunning Area |  |  |
| `DunningBlockingReason` | `MANSP` |  |  |  |  | `String(1)` |  | Dunning Block |  |  |
| `DunningKey` | `MSCHL` |  |  |  |  | `String(1)` |  | Dunning Key |  |  |
| `InternalFinancialDocument` | `LCNUM` |  |  |  |  | `String(10)` |  | Financial Doc. No. |  |  |
| `IsRelevantForAccrual` | `ISACCRUALRELEVANT` |  |  |  |  | `Boolean` |  | Relevant for Accrual |  |  |
| `SoldToParty` | `KUNAG` |  |  |  |  | `String(10)` |  | Sold-to Party |  |  |
| `PartnerCompany` | `RASSC` |  |  |  |  | `String(6)` |  | Trading Partner No. |  |  |
| `PurchaseOrderByCustomer` | `BSTKD` |  |  |  |  | `String(35)` |  | Customer Reference |  |  |
| `CustomerGroup` | `KDGRP` |  |  |  |  | `String(2)` |  | Customer Group |  |  |
| `Country` | `LLAND` |  |  |  |  | `String(3)` |  | Dest. Country/Region |  |  |
| `CityCode` | `CITYC` |  |  |  |  | `String(4)` |  | City Code |  |  |
| `SalesDistrict` | `BZIRK` |  |  |  |  | `String(6)` |  | Sales District |  |  |
| `Region` | `REGIO` |  |  |  |  | `String(3)` |  | Region |  |  |
| `County` | `COUNC` |  |  |  |  | `String(3)` |  | County Code |  |  |
| `CreditControlArea` | `KKBER` |  |  |  |  | `String(4)` |  | Credit Control Area |  |  |
| `CustomerRebateAgreement` | `KNUMA` |  |  |  |  | `String(10)` |  | Agreement |  |  |
| `PricingDocument` | `KNUMV` |  |  |  |  | `String(10)` |  | Doc. Condition No. |  |  |
| `OverallSDProcessStatus` | `GBSTK` |  |  |  |  | `String(1)` |  | Overall Status |  |  |
| `OverallBillingStatus` | `VF_STATUS` |  |  |  |  | `String(1)` |  | Status |  |  |
| `AccountingPostingStatus` | `BUCHK` |  |  |  |  | `String(1)` |  | Posting Status |  |  |
| `AccountingTransferStatus` | `RFBSK` |  |  |  |  | `String(1)` |  | Posting Status |  |  |
| `BillingIssueType` | `VF_TODO` |  |  |  |  | `String(1)` |  | Issue Type |  |  |
| `InvoiceListStatus` | `RELIK` |  |  |  |  | `String(1)` |  | Invoice List Status |  |  |
| `OvrlItmGeneralIncompletionSts` | `UVALL_SU` |  |  |  |  | `String(1)` |  | All Items |  |  |
| `OverallPricingIncompletionSts` | `UVPRS_UK` |  |  |  |  | `String(1)` |  | Pricing – All Items |  |  |
| `InvoiceClearingStatus` | `CLRST` |  |  |  |  | `String(1)` |  | Clearing Status |  |  |
| `InvoiceListType` | `FKART_RL` |  |  |  |  | `String(4)` |  | Invoice List Type |  |  |
| `InvoiceListBillingDate` | `FKDAT_RL` |  |  |  |  | `Date` |  | Inv. List Bill. Date |  |  |
| `ForeignTradeStstclCurrency` | `GRWCU` |  |  |  |  | `String(5)` |  | Currency |  |  |


## Entity: `BillingDocumentItem`

- **ABAP CDS Name:** `I_BillingDocumentItem`
- **Label:** Billing Document Item
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** VBRP

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `BillingDocument` | `VBELN_VF` | `VBRP` | `VBELN` |  |  | `String(10)` | Y | Billing Document |  |  |
| `BillingDocumentItem` | `POSNR_VF` | `VBRP` | `POSNR` |  |  | `String(6)` | Y | Item |  |  |
| `SalesDocumentItemCategory` | `SALES_DOC_ITEM_CATEGORY` |  |  |  |  | `String(4)` |  | Sales Doc. Item Cat. |  |  |
| `SalesDocumentItemType` | `POSAR` |  |  |  |  | `String(1)` |  | Item Type |  |  |
| `ReturnItemProcessingType` | `SHKZG_VF` |  |  |  |  | `String(1)` |  | Returns |  |  |
| `CreatedByUser` | `ERNAM` |  |  |  |  | `String(12)` |  | Created By |  |  |
| `CreationDate` | `ERDAT` | `VBRK` | `ERDAT` |  |  | `Date` |  | Created On |  |  |
| `CreationTime` | `ERZET` |  |  |  |  | `String(6)` |  | Time |  |  |
| `ReferenceLogicalSystem` | `LOGSYS` |  |  |  |  | `String(10)` |  | Logical System |  |  |
| `OrganizationDivision` | `SALES_ORDER_DIVISON` |  |  |  |  | `String(2)` |  | Division of Order |  |  |
| `Division` | `SPART` | `VBRK` | `SPART` |  |  | `String(2)` |  | Division |  |  |
| `SalesOffice` | `VKBUR` |  |  |  |  | `String(4)` |  | Sales Office |  |  |
| `Material` | `MATNR` | `VBRP` | `MATNR` |  |  | `String(40)` |  | Material |  |  |
| `Product` | `PRODUCTNUMBER` |  |  |  |  | `String(40)` |  | Product |  |  |
| `OriginallyRequestedMaterial` | `MATWA` |  |  |  |  | `String(40)` |  | Material Entered |  |  |
| `InternationalArticleNumber` | `EAN11` |  |  |  |  | `String(18)` |  | EAN/UPC |  |  |
| `PricingReferenceMaterial` | `PMATN` |  |  |  |  | `String(40)` |  | Pricing Ref. Matl |  |  |
| `Batch` | `CHARG_D` |  |  |  |  | `String(10)` |  | Batch |  |  |
| `ProductHierarchyNode` | `PRODH_D` |  |  |  |  | `String(18)` |  | Product Hierarchy |  |  |
| `MaterialGroup` | `MATKL` |  |  |  |  | `String(9)` |  | Material Group |  |  |
| `ProductGroup` | `PRODUCTGROUP` |  |  |  |  | `String(9)` |  | Product Group |  |  |
| `AdditionalMaterialGroup1` | `MVGR1` |  |  |  |  | `String(3)` |  | Material Group 1 |  |  |
| `AdditionalMaterialGroup2` | `MVGR2` |  |  |  |  | `String(3)` |  | Material Group 2 |  |  |
| `AdditionalMaterialGroup3` | `MVGR3` |  |  |  |  | `String(3)` |  | Material Group 3 |  |  |
| `AdditionalMaterialGroup4` | `MVGR4` |  |  |  |  | `String(3)` |  | Material Group 4 |  |  |
| `AdditionalMaterialGroup5` | `MVGR5` |  |  |  |  | `String(3)` |  | Material Group 5 |  |  |
| `ProductConfiguration` | `CUOBJ_VA` |  |  |  |  | `String(18)` |  | Configuration |  |  |
| `MaterialCommissionGroup` | `PROVG` |  |  |  |  | `String(2)` |  | Commission Group |  |  |
| `Plant` | `WERKS_D` | `VBRP` | `WERKS` |  |  | `String(4)` |  | Plant |  |  |
| `StorageLocation` | `LGORT_D` |  |  |  |  | `String(4)` |  | Storage Location |  |  |
| `ReplacementPartType` | `ATPKZ` |  |  |  |  | `String(1)` |  | Replacement Part |  |  |
| `MaterialGroupHierarchy1` | `WGRU_HIE1` |  |  |  |  | `String(18)` |  | Material Group 1 |  |  |
| `MaterialGroupHierarchy2` | `WGRU_HIE2` |  |  |  |  | `String(18)` |  | Material Group 2 |  |  |
| `PlantRegion` | `WKREG` |  |  |  |  | `String(3)` |  | Region of Dlv. Plant |  |  |
| `PlantCounty` | `WKCOU` |  |  |  |  | `String(3)` |  | County of Dlv.Plant |  |  |
| `PlantCity` | `WKCTY` |  |  |  |  | `String(4)` |  | City of Deliv. Plant |  |  |
| `TransitPlant` | `TRANSIT_PLANT` |  |  |  |  | `String(4)` |  | Transit Plant |  |  |
| `ValueChainCategory` | `VCM_CHAIN_CATEGORY` |  |  |  |  | `String(4)` |  | Value Chain Category |  |  |
| `BOMExplosion` | `SERNR` |  |  |  |  | `String(8)` |  | BOM Explosion Number |  |  |
| `MaterialDeterminationType` | `PROSA` |  |  |  |  | `String(1)` |  | Mat.Determ.Active |  |  |
| `SoldProduct` | `SDBIL_SOLD_PRODUCT` |  |  |  |  | `String(40)` |  | Product Sold |  |  |
| `BillingDocumentItemText` | `ARKTX` |  |  |  |  | `String(40)` |  | Item Description |  |  |
| `ServicesRenderedDate` | `FBUDA` |  |  |  |  | `Date` |  | Serv. Rendered Date |  |  |
| `BillingQuantity` | `FKIMG` |  |  |  |  | `Decimal(13,3)` |  | Invoiced Quantity | BillingQuantityUnit |  |
| `BillingQuantityUnit` | `VRKME` |  |  |  |  | `String(3)` |  | Sales Unit |  |  |
| `BillingQuantityInBaseUnit` | `FKLMG` |  |  |  |  | `Decimal(13,3)` |  | Billing Qty in SKU | BaseUnit |  |
| `BaseUnit` | `MEINS` |  |  |  |  | `String(3)` |  | Base Unit of Measure |  |  |
| `MRPRequiredQuantityInBaseUnit` | `LMENG` |  |  |  |  | `Decimal(13,3)` |  | Required Quantity | BaseUnit |  |
| `BillingToBaseQuantityDnmntr` | `UMVKN` |  |  |  |  | `Decimal(5,0)` |  | Denominator |  |  |
| `BillingToBaseQuantityNmrtr` | `UMVKZ` |  |  |  |  | `Decimal(5,0)` |  | Numerator |  |  |
| `ItemGrossWeight` | `BRGEW_15` |  |  |  |  | `Decimal(15,3)` |  | Gross Weight | ItemWeightUnit |  |
| `ItemNetWeight` | `NTGEW_15` |  |  |  |  | `Decimal(15,3)` |  | Net Weight | ItemWeightUnit |  |
| `ItemWeightUnit` | `GEWEI` |  |  |  |  | `String(3)` |  | Unit of Weight |  |  |
| `ItemVolume` | `VOLUM_15` |  |  |  |  | `Decimal(15,3)` |  | Volume | ItemVolumeUnit |  |
| `ItemVolumeUnit` | `VOLEH` |  |  |  |  | `String(3)` |  | Volume Unit |  |  |
| `BillToPartyCountry` | `LLAND_AUFT` |  |  |  |  | `String(3)` |  | Dest. Ctry/Reg. Ord. |  |  |
| `BillToPartyRegion` | `REGIO_AUFT` |  |  |  |  | `String(3)` |  | Region Order |  |  |
| `BillingPlanRule` | `FAREG` |  |  |  |  | `String(1)` |  | Billing Rule |  |  |
| `BillingPlan` | `FPLNR` |  |  |  |  | `String(10)` |  | Bill. Plan No. |  |  |
| `BillingPlanItem` | `FPLTR` |  |  |  |  | `String(6)` |  | Item |  |  |
| `DownPaymentProcessingVariant` | `SDBIL_DWN_PAYT_PROCG_VAR` |  |  |  |  | `String(1)` |  | Down Payment Variant |  |  |
| `NetAmount` | `NETWR_FP` |  |  |  |  | `Decimal(34,4)` |  | Net Value | TransactionCurrency |  |
| `TransactionCurrency` | `WAERK` | `VBRK` | `WAERK` |  |  | `String(5)` |  | Document Currency |  |  |
| `GrossAmount` | `BRTWR_FP` |  |  |  |  | `Decimal(34,4)` |  | Gross Value | TransactionCurrency |  |
| `PricingDate` | `PRSDT` |  |  |  |  | `Date` |  | Pricing Date |  |  |
| `PriceDetnExchangeRate` | `KURSK_NOT_CONVERTED` |  |  |  |  | `Decimal(9,5)` |  | Exchange Rate |  |  |
| `PricingScaleQuantityInBaseUnit` | `SMENG` |  |  |  |  | `Decimal(13,3)` |  | Scale Quantity | BaseUnit |  |
| `TaxAmount` | `MWSBP` |  |  |  |  | `Decimal(34,4)` |  | Tax Amount | TransactionCurrency |  |
| `CostAmount` | `WAVWR` |  |  |  |  | `Decimal(34,4)` |  | Cost | TransactionCurrency |  |
| `Subtotal1Amount` | `KZWI1` |  |  |  |  | `Decimal(34,4)` |  | Subtotal 1 | TransactionCurrency |  |
| `Subtotal2Amount` | `KZWI2` |  |  |  |  | `Decimal(34,4)` |  | Subtotal 2 | TransactionCurrency |  |
| `Subtotal3Amount` | `KZWI3` |  |  |  |  | `Decimal(34,4)` |  | Subtotal 3 | TransactionCurrency |  |
| `Subtotal4Amount` | `KZWI4` |  |  |  |  | `Decimal(34,4)` |  | Subtotal 4 | TransactionCurrency |  |
| `Subtotal5Amount` | `KZWI5` |  |  |  |  | `Decimal(34,4)` |  | Subtotal 5 | TransactionCurrency |  |
| `Subtotal6Amount` | `KZWI6` |  |  |  |  | `Decimal(34,4)` |  | Subtotal 6 | TransactionCurrency |  |
| `StatisticalValueControl` | `KOWRR` |  |  |  |  | `String(1)` |  | Statistical Value |  |  |
| `CashDiscountIsDeductible` | `SKTOF` |  |  |  |  | `Boolean` |  | Cash Discount |  |  |
| `CustomerConditionGroup1` | `KDKG1` |  |  |  |  | `String(2)` |  | Condition Group 1 |  |  |
| `CustomerConditionGroup2` | `KDKG2` |  |  |  |  | `String(2)` |  | Condition Group 2 |  |  |
| `CustomerConditionGroup3` | `KDKG3` |  |  |  |  | `String(2)` |  | Condition Group 3 |  |  |
| `CustomerConditionGroup4` | `KDKG4` |  |  |  |  | `String(2)` |  | Condition Group 4 |  |  |
| `CustomerConditionGroup5` | `KDKG5` |  |  |  |  | `String(2)` |  | Condition Group 5 |  |  |
| `ManualPriceChangeType` | `MPROK` |  |  |  |  | `String(1)` |  | Manual Price |  |  |
| `MaterialPricingGroup` | `KONDM` |  |  |  |  | `String(2)` |  | Material Price Grp |  |  |
| `StatisticsExchangeRate` | `STCUR_AP_NOT_CONVERTED` |  |  |  |  | `Decimal(9,5)` |  | Exchange Rate Stats. |  |  |
| `MainItemPricingRefMaterial` | `UPMAT` |  |  |  |  | `String(40)` |  | Pricing Ref.Material |  |  |
| `MainItemMaterialPricingGroup` | `UKONM` |  |  |  |  | `String(2)` |  | MnItem MatPricingGrp |  |  |
| `TimeSheetOvertimeCategory` | `CATS_OVERTIME_CATEGORY` |  |  |  |  | `String(4)` |  | Overtime Category |  |  |
| `PricingRelevance` | `PRSFD` |  |  |  |  | `String(1)` |  | Pricing Relevance |  |  |
| `DepartureCountry` | `ALAND` |  |  |  |  | `String(3)` |  | Departure Ctry/Reg. |  |  |
| `TaxJurisdiction` | `TXJCD` |  |  |  |  | `String(15)` |  | Tax Jurisdiction |  |  |
| `ProductTaxClassification1` | `PRODUCT_TAX_CLASSIFICATION_1` |  |  |  |  | `String(1)` |  | Product Tax Classification 1 |  |  |
| `ProductTaxClassification2` | `PRODUCT_TAX_CLASSIFICATION_2` |  |  |  |  | `String(1)` |  | Product Tax Classification 2 |  |  |
| `ProductTaxClassification3` | `PRODUCT_TAX_CLASSIFICATION_3` |  |  |  |  | `String(1)` |  | Product Tax Classification 3 |  |  |
| `ProductTaxClassification4` | `PRODUCT_TAX_CLASSIFICATION_4` |  |  |  |  | `String(1)` |  | Product Tax Classification 4 |  |  |
| `ProductTaxClassification5` | `PRODUCT_TAX_CLASSIFICATION_5` |  |  |  |  | `String(1)` |  | Product Tax Classification 5 |  |  |
| `ProductTaxClassification6` | `PRODUCT_TAX_CLASSIFICATION_6` |  |  |  |  | `String(1)` |  | Product Tax Classification 6 |  |  |
| `ProductTaxClassification7` | `PRODUCT_TAX_CLASSIFICATION_7` |  |  |  |  | `String(1)` |  | Product Tax Classification 7 |  |  |
| `ProductTaxClassification8` | `PRODUCT_TAX_CLASSIFICATION_8` |  |  |  |  | `String(1)` |  | Product Tax Classification 8 |  |  |
| `ProductTaxClassification9` | `PRODUCT_TAX_CLASSIFICATION_9` |  |  |  |  | `String(1)` |  | Product Tax Classification 9 |  |  |
| `ZeroVATRsn` | `J_1ARFZVAT` |  |  |  |  | `String(1)` |  | Reason 0 VAT |  |  |
| `TaxCode` | `MWSKZ` |  |  |  |  | `String(2)` |  | Tax Code |  |  |
| `TaxRateValidityStartDate` | `FOT_TXDAT_FROM` |  |  |  |  | `Date` |  | Tax Rate Valid-From |  |  |
| `CountryOfOrigin` | `HERKL` |  |  |  |  | `String(3)` |  | Cntry/Reg of Origin |  |  |
| `RegionOfOrigin` | `HERKR` |  |  |  |  | `String(3)` |  | Region of Origin |  |  |
| `CommodityCode` | `/SAPSLL/COMCO` |  |  |  |  | `String(30)` |  | Commodity Code |  |  |
| `EligibleAmountForCashDiscount` | `SKFBP` |  |  |  |  | `Decimal(34,4)` |  | Cash Disc. Bas. | TransactionCurrency |  |
| `BusinessArea` | `GSBER` |  |  |  |  | `String(4)` |  | Business Area |  |  |
| `ProfitCenter` | `PRCTR` |  |  |  |  | `String(10)` |  | Profit Center |  |  |
| `OrderID` | `AUFNR` |  |  |  |  | `String(12)` |  | Order |  |  |
| `WBSElement` | `PS_PSP_PNR` |  |  |  |  | `String(8)` |  | WBS Element |  |  |
| `WBSElementInternalID` | `PS_S4_PSPNR` |  |  |  |  | `String(8)` |  | WBS Internal ID |  |  |
| `ProviderContract` | `VTKEY_KK` |  |  |  |  | `String(20)` |  | Provider Contract |  |  |
| `ProviderContractItem` | `PROVIDER_CONTRACT_ITEM` |  |  |  |  | `String(6)` |  | Provider Contract Item |  |  |
| `BillingPerformancePeriodStrDte` | `FM_PEROP_SD_LOW` |  |  |  |  | `Date` |  | Per. of Perf. Start |  |  |
| `BillingPeriodOfPerfStartDate` | `FM_PEROP_SD_LOW` |  |  |  |  | `Date` |  | Per. of Perf. Start |  |  |
| `BillingPerformancePeriodEndDte` | `FM_PEROP_SD_HIGH` |  |  |  |  | `Date` |  | Per. of Perf. End |  |  |
| `BillingPeriodOfPerfEndDate` | `FM_PEROP_SD_HIGH` |  |  |  |  | `Date` |  | Per. of Perf. End |  |  |
| `ControllingArea` | `KOKRS` |  |  |  |  | `String(4)` |  | Controlling Area |  |  |
| `ProfitabilitySegment` | `RKEOBJNR_NUMC` |  |  |  |  | `String(10)` |  | Profitability Segment (Deprecated) |  |  |
| `ProfitabilitySegment_2` | `RKEOBJNR_CHAR` |  |  |  |  | `String(10)` |  | Profitability Segment |  |  |
| `CostCenter` | `KOSTL` |  |  |  |  | `String(10)` |  | Cost Center |  |  |
| `OriginSDDocument` | `VBELV` |  |  |  |  | `String(10)` |  | Originating Document |  |  |
| `OriginSDDocumentItem` | `POSNV` |  |  |  |  | `String(6)` |  | Originating Item |  |  |
| `PriceDetnExchangeRateDate` | `WWERT_D` |  |  |  |  | `Date` |  | Translation Date |  |  |
| `MatlAccountAssignmentGroup` | `KTGRM` |  |  |  |  | `String(2)` |  | Acct Assmt Grp Mat. |  |  |
| `ReferenceSDDocument` | `VGBEL` |  |  |  |  | `String(10)` |  | Reference Document |  |  |
| `ReferenceSDDocumentItem` | `VGPOS` |  |  |  |  | `String(6)` |  | Reference Item |  |  |
| `ReferenceSDDocumentCategory` | `REFERENCE_DOC_CATEGORY` |  |  |  |  | `String(4)` |  | Ref. Doc. Category |  |  |
| `SalesDocument` | `VBELN_VA` | `VBRP` | `AUBEL` |  |  | `String(10)` |  | Sales Document |  |  |
| `SalesDocumentItem` | `POSNR_VA` | `VBRP` | `AUPOS` |  |  | `String(6)` |  | Sales Document Item |  |  |
| `SalesSDDocumentCategory` | `SALES_DOCUMENT_CATEGORY` |  |  |  |  | `String(4)` |  | Sales Doc. Category |  |  |
| `HigherLevelItem` | `UEPOS` |  |  |  |  | `String(6)` |  | Higher-Level Item |  |  |
| `HigherLvlItmOfBatSpltItm` | `UECHA` |  |  |  |  | `String(6)` |  | HigherLevelItemBatch |  |  |
| `BillingDocumentItemInPartSgmt` | `POSPA` |  |  |  |  | `String(6)` |  | Partner Item |  |  |
| `ExternalReferenceDocument` | `EXT_REFERENCE_DOCUMENT` |  |  |  |  | `String(10)` |  | Ext. Reference Document |  |  |
| `ExternalReferenceDocumentItem` | `EXT_REFERENCE_DOCUMENT_ITEM` |  |  |  |  | `String(6)` |  | Ext. Ref. Document Item |  |  |
| `BillingDocExtReferenceDocItem` | `BILLINGDOCEXTREFERENCEDOCITEM` |  |  |  |  | `String(6)` |  | Ext. Reference Doc. Item |  |  |
| `PrelimBillingDocument` | `PBD_ID` |  |  |  |  | `String(10)` |  | Prelimin. Bill. Doc. |  |  |
| `PrelimBillingDocumentItem` | `PBD_ITEM_ID` |  |  |  |  | `String(6)` |  | Prelimin. Doc. Item |  |  |
| `SalesGroup` | `VKGRP` |  |  |  |  | `String(3)` |  | Sales Group |  |  |
| `AdditionalCustomerGroup1` | `KVGR1` |  |  |  |  | `String(3)` |  | Customer Group 1 |  |  |
| `AdditionalCustomerGroup2` | `KVGR2` |  |  |  |  | `String(3)` |  | Customer Group 2 |  |  |
| `AdditionalCustomerGroup3` | `KVGR3` |  |  |  |  | `String(3)` |  | Customer Group 3 |  |  |
| `AdditionalCustomerGroup4` | `KVGR4` |  |  |  |  | `String(3)` |  | Customer Group 4 |  |  |
| `AdditionalCustomerGroup5` | `KVGR5` |  |  |  |  | `String(3)` |  | Customer Group 5 |  |  |
| `SDDocumentReason` | `AUGRU` |  |  |  |  | `String(3)` |  | Order Reason |  |  |
| `RetailPromotion` | `WAKTION` |  |  |  |  | `String(10)` |  | Retail Promotion |  |  |
| `RebateBasisAmount` | `BONBA` |  |  |  |  | `Decimal(34,4)` |  | Rebate Basis | TransactionCurrency |  |
| `VolumeRebateGroup` | `BONUS` |  |  |  |  | `String(2)` |  | Volume Rebate Group |  |  |
| `ItemIsRelevantForCredit` | `CMPNT` |  |  |  |  | `Boolean` |  | Credit Funct. Active |  |  |
| `CreditRelatedPrice` | `CMPRE` |  |  |  |  | `Decimal(34,4)` |  | Credit Price | TransactionCurrency |  |
| `SalesDeal` | `KNUMA_AG` |  |  |  |  | `String(10)` |  | Sales Deal |  |  |
| `SalesPromotion` | `KNUMA_PI` |  |  |  |  | `String(10)` |  | Promotion |  |  |
| `SalesOrderSalesDistrict` | `BZIRK_AUFT` |  |  |  |  | `String(6)` |  | Sales Distr. Order |  |  |
| `SalesOrderCustomerGroup` | `KDGRP_AUFT` |  |  |  |  | `String(2)` |  | Customer Grp Order |  |  |
| `SalesOrderCustomerPriceGroup` | `KONDA_AUFT` |  |  |  |  | `String(2)` |  | Price Group of Order |  |  |
| `SalesOrderPriceListType` | `PLTYP_AUFT` |  |  |  |  | `String(2)` |  | Price List Order |  |  |
| `SalesOrderSalesOrganization` | `VKORG_AUFT` |  |  |  |  | `String(4)` |  | Sales Org. of Order |  |  |
| `SalesOrderDistributionChannel` | `VTWEG_AUFT` |  |  |  |  | `String(2)` |  | Distr. Channel Order |  |  |
| `SalesDocIsCreatedFromReference` | `AUREF` |  |  |  |  | `Boolean` |  | SalesDocumentRefer |  |  |
| `ShippingPoint` | `VSTEL` |  |  |  |  | `String(4)` |  | Shipping Point |  |  |
| `ServiceDocumentType` | `FCO_SRVDOC_TYPE` |  |  |  |  | `String(4)` |  | Service Doc. Type |  |  |
| `ServiceDocument` | `FCO_SRVDOC_ID` |  |  |  |  | `String(10)` |  | Service Document |  |  |
| `ServiceDocumentItem` | `FCO_SRVDOC_ITEM_ID` |  |  |  |  | `String(6)` |  | Service Doc. Item |  |  |
| `BusinessSolutionOrder` | `CRMS4_SOLO_OBJECT_ID` |  |  |  |  | `String(10)` |  | Solution Order |  |  |
| `BusinessSolutionOrderItem` | `CRMS4_SOLO_NUMBER_INT` |  |  |  |  | `String(6)` |  | Solution Order Item |  |  |
| `HigherLevelItemUsage` | `UEPVW` |  |  |  |  | `String(1)` |  | Usage of HL Item |  |  |
| `BillingDocumentIsTemporary` | `VF_DRAFT_INDICATOR` |  |  |  |  | `Boolean` |  | Draft Indicator |  |  |
| `SDDocumentCategory` | `VBTYPL` |  |  |  |  | `String(4)` |  | SD Document Category |  |  |
| `BillingDocumentType` | `FKART` | `VBRK` | `FKART` |  |  | `String(4)` |  | Billing Type |  |  |
| `SalesOrganization` | `VKORG` | `VBRK` | `VKORG` |  |  | `String(4)` |  | Sales Organization |  |  |
| `DistributionChannel` | `VTWEG` | `VBRK` | `VTWEG` |  |  | `String(2)` |  | Distribution Channel |  |  |
| `CustomerPriceGroup` | `KONDA` |  |  |  |  | `String(2)` |  | Customer Price Group |  |  |
| `CustomerGroup` | `KDGRP` |  |  |  |  | `String(2)` |  | Customer Group |  |  |
| `Country` | `LLAND` |  |  |  |  | `String(3)` |  | Dest. Country/Region |  |  |
| `Region` | `REGIO` |  |  |  |  | `String(3)` |  | Region |  |  |
| `CityCode` | `CITYC` |  |  |  |  | `String(4)` |  | City Code |  |  |
| `SalesDistrict` | `BZIRK` |  |  |  |  | `String(6)` |  | Sales District |  |  |
| `OverallSDProcessStatus` | `GBSTK` |  |  |  |  | `String(1)` |  | Overall Status |  |  |
| `OverallBillingStatus` | `VF_STATUS` |  |  |  |  | `String(1)` |  | Status |  |  |
| `SoldToParty` | `KUNAG` |  |  |  |  | `String(10)` |  | Sold-to Party |  |  |
| `PayerParty` | `KUNRG` | `VBRK` | `KUNRG` |  |  | `String(10)` |  | Payer |  |  |
| `BillingDocumentDate` | `FKDAT` | `VBRK` | `FKDAT` |  |  | `Date` |  | Billing Date |  |  |
| `CompanyCode` | `BUKRS` | `VBRK` | `BUKRS` |  |  | `String(4)` |  | Company Code |  |  |
| `County` | `COUNC` |  |  |  |  | `String(3)` |  | County Code |  |  |
| `CustomerRebateAgreement` | `KNUMA` |  |  |  |  | `String(10)` |  | Agreement |  |  |
| `BillingDocumentCategory` | `FKTYP` |  |  |  |  | `String(1)` |  | Billing Category |  |  |
| `PricingDocument` | `KNUMV` |  |  |  |  | `String(10)` |  | Doc. Condition No. |  |  |
| `CancelledBillingDocument` | `SFAKN` |  |  |  |  | `String(10)` |  | Canceled Bill. Doc. |  |  |
| `ShipToParty` | `KUNWE` |  |  |  |  | `String(10)` |  | Ship-to Party |  |  |
| `BillToParty` | `KUNRE` |  |  |  |  | `String(10)` |  | Bill-to Party |  |  |
| `SalesEmployee` | `SALES_EMPL` |  |  |  |  | `String(8)` |  | Sales Employee |  |  |
| `ResponsibleEmployee` | `RESP_EMPL` |  |  |  |  | `String(8)` |  | Employee Responsible |  |  |
