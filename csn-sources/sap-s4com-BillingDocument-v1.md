# BillingDocument

> Source file: `sap-s4com-BillingDocument-v1.json`

**Technical Name:** `` | **Data Category:** `DIMENSION` | **VDM Type:** `BASIC` | **Size:** `L`


## Entity: `BillingDocument`

- **ABAP Name:** `I_BillingDocument`
- **Label:** Billing Document
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** VBRK

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `BillingDocument` | `VBELN_VF` | `VBELN` | `VBRK` | `String(10)` | Y | Billing Document |  |  |  |
| `SDDocumentCategory` | `VBTYPL` | `VBTYPL` | `VBRK` | `String(4)` |  | SD Document Category |  |  |  |
| `BillingDocumentCategory` | `FKTYP` | `FKTYP` | `VBRK` | `String(1)` |  | Billing Category |  |  |  |
| `BillingDocumentType` | `FKART` | `FKART` | `VBRK` | `String(4)` |  | Billing Type |  |  |  |
| `CreatedByUser` | `ERNAM` | `ERNAM` | `VBRK` | `String(12)` |  | Created By |  |  |  |
| `CreationDate` | `ERDAT` | `ERDAT` | `VBRK` | `Date` |  | Created On |  |  |  |
| `CreationTime` | `ERZET` | `ERZET` | `VBRK` | `String(6)` |  | Time |  |  |  |
| `LastChangeDate` | `AEDAT` | `AEDAT` | `VBRK` | `Date` |  | Changed On |  |  |  |
| `LastChangeDateTime` | `TIMESTAMPL` | `TIMESTAMPL` | `VBRK` | `Timestamp` |  | Time Stamp |  |  |  |
| `LogicalSystem` | `LOGSYS` | `LOGSYS` | `VBRK` | `String(10)` |  | Logical System |  |  |  |
| `SalesOrganization` | `VKORG` | `VKORG` | `VBRK` | `String(4)` |  | Sales Organization |  |  |  |
| `DistributionChannel` | `VTWEG` | `VTWEG` | `VBRK` | `String(2)` |  | Distribution Channel |  |  |  |
| `Division` | `SPART` | `SPART` | `VBRK` | `String(2)` |  | Division |  |  |  |
| `BillingDocumentDate` | `FKDAT` | `FKDAT` | `VBRK` | `Date` |  | Billing Date |  |  |  |
| `BillingDocumentIsCancelled` | `FKSTO` | `FKSTO` | `VBRK` | `Boolean` |  | Canceled |  |  |  |
| `CancelledBillingDocument` | `SFAKN` | `SFAKN` | `VBRK` | `String(10)` |  | Canceled Bill. Doc. |  |  |  |
| `BillingDocCombinationCriteria` | `DZUKRI` | `DZUKRI` | `VBRK` | `String(40)` |  | Combination Criteria |  |  |  |
| `ManualInvoiceMaintIsRelevant` | `MRNKZ` | `MRNKZ` | `VBRK` | `Boolean` |  | Man. Invoice Maint. |  |  |  |
| `NmbrOfPages` | `J_1ANOPG` | `J_1ANOPG` | `VBRK` | `String(3)` |  | Number of Pages |  |  |  |
| `IsIntrastatReportingRelevant` | `INTRA_REL` | `INTRA_REL` | `VBRK` | `Boolean` |  | Intrastat Relevance |  |  |  |
| `IsIntrastatReportingExcluded` | `INTRA_EXCL` | `INTRA_EXCL` | `VBRK` | `Boolean` |  | Intrastat Exclusion |  |  |  |
| `BillingDocumentIsTemporary` | `VF_DRAFT_INDICATOR` | `VF_DRAFT_INDICATOR` | `VBRK` | `Boolean` |  | Draft Indicator |  |  |  |
| `TotalNetAmount` | `NETWR` | `NETWR` | `VBRK` | `Decimal(34,4)` |  | Net Value | TransactionCurrency |  |  |
| `TransactionCurrency` | `WAERK` | `WAERK` | `VBRK` | `String(5)` |  | Document Currency |  |  |  |
| `StatisticsCurrency` | `STWAE` | `STWAE` | `VBRK` | `String(5)` |  | Statistics Currency |  |  |  |
| `TotalTaxAmount` | `MWSBP` | `MWSBP` | `VBRK` | `Decimal(34,4)` |  | Tax Amount | TransactionCurrency |  |  |
| `CustomerPriceGroup` | `KONDA` | `KONDA` | `VBRK` | `String(2)` |  | Customer Price Group |  |  |  |
| `PriceListType` | `PLTYP` | `PLTYP` | `VBRK` | `String(2)` |  | Price List Type |  |  |  |
| `TaxDepartureCountry` | `LANDTX` | `LANDTX` | `VBRK` | `String(3)` |  | Tax Departure C/R |  |  |  |
| `VATRegistration` | `STCEG` | `STCEG` | `VBRK` | `String(20)` |  | VAT Registration No. |  |  |  |
| `VATRegistrationOrigin` | `STCEG_H` | `STCEG_H` | `VBRK` | `String(1)` |  | Origin Sales Tax No. |  |  |  |
| `VATRegistrationCountry` | `STCEG_L` | `STCEG_L` | `VBRK` | `String(3)` |  | Ctry/Rgn Sls Tax No. |  |  |  |
| `HierarchyTypePricing` | `HITYP_PR` | `HITYP_PR` | `VBRK` | `String(1)` |  | HierarchyTypePricing |  |  |  |
| `CustomerTaxClassification1` | `TAXK1` | `TAXK1` | `VBRK` | `String(1)` |  | Tax Class.1 Customer |  |  |  |
| `CustomerTaxClassification2` | `TAXK2` | `TAXK2` | `VBRK` | `String(1)` |  | Tax Class.2 Customer |  |  |  |
| `CustomerTaxClassification3` | `TAXK3` | `TAXK3` | `VBRK` | `String(1)` |  | Tax Class.3 Customer |  |  |  |
| `CustomerTaxClassification4` | `TAXK4` | `TAXK4` | `VBRK` | `String(1)` |  | Tax Class.4 Customer |  |  |  |
| `CustomerTaxClassification5` | `TAXK5` | `TAXK5` | `VBRK` | `String(1)` |  | Tax Class.5 Customer |  |  |  |
| `CustomerTaxClassification6` | `TAXK6` | `TAXK6` | `VBRK` | `String(1)` |  | Tax Class.6 Customer |  |  |  |
| `CustomerTaxClassification7` | `TAXK7` | `TAXK7` | `VBRK` | `String(1)` |  | Tax Class.7 Customer |  |  |  |
| `CustomerTaxClassification8` | `TAXK8` | `TAXK8` | `VBRK` | `String(1)` |  | Tax Class.8 Customer |  |  |  |
| `CustomerTaxClassification9` | `TAXK9` | `TAXK9` | `VBRK` | `String(1)` |  | Tax Class.9 Customer |  |  |  |
| `IsEUTriangularDeal` | `XEGDR` | `XEGDR` | `VBRK` | `Boolean` |  | EU Triangular Deal |  |  |  |
| `SDPricingProcedure` | `KALSMASD` | `KALSMASD` | `VBRK` | `String(6)` |  | Pricing Procedure |  |  |  |
| `ShippingCondition` | `VSBED` | `VSBED` | `VBRK` | `String(2)` |  | Shipping Conditions |  |  |  |
| `PlantSupplier` | `LIFNR_WK` | `LIFNR_WK` | `VBRK` | `String(10)` |  | Sppl. No. Plnt |  |  |  |
| `IncotermsVersion` | `INCOV` | `INCOV` | `VBRK` | `String(4)` |  | Incoterms Version |  |  |  |
| `IncotermsClassification` | `INCO1` | `INCO1` | `VBRK` | `String(3)` |  | Incoterms |  |  |  |
| `IncotermsTransferLocation` | `INCO2` | `INCO2` | `VBRK` | `String(28)` |  | Incoterms (Part 2) |  |  |  |
| `IncotermsLocation1` | `INCO2_L` | `INCO2_L` | `VBRK` | `String(70)` |  | Incoterms Location 1 |  |  |  |
| `IncotermsLocation2` | `INCO3_L` | `INCO3_L` | `VBRK` | `String(70)` |  | Incoterms Location 2 |  |  |  |
| `PayerParty` | `KUNRG` | `KUNRG` | `VBRK` | `String(10)` |  | Payer |  |  |  |
| `ContractAccount` | `CORR_VKONT_KK` | `CORR_VKONT_KK` | `VBRK` | `String(12)` |  | Contract Account |  |  |  |
| `CustomerPaymentTerms` | `DZTERM` | `DZTERM` | `VBRK` | `String(4)` |  | Terms of Payment |  |  |  |
| `PaymentMethod` | `SCHZW_BSEG` | `SCHZW_BSEG` | `VBRK` | `String(1)` |  | Payment Method |  |  |  |
| `PaymentReference` | `KIDNO` | `KIDNO` | `VBRK` | `String(30)` |  | Payment Reference |  |  |  |
| `FixedValueDate` | `VALDT` | `VALDT` | `VBRK` | `Date` |  | Fixed Value Date |  |  |  |
| `AdditionalValueDays` | `VALTG` | `VALTG` | `VBRK` | `String(2)` |  | Addit. Value Days |  |  |  |
| `SEPAMandate` | `SEPA_MNDID` | `SEPA_MNDID` | `VBRK` | `String(35)` |  | Mandate Reference |  |  |  |
| `CompanyCode` | `BUKRS` | `BUKRS` | `VBRK` | `String(4)` |  | Company Code |  |  |  |
| `FiscalYear` | `GJAHR` | `GJAHR` | `VBRK` | `String(4)` |  | Fiscal Year |  |  |  |
| `AccountingDocument` | `BELNR_D` | `BELNR` | `VBRK` | `String(10)` |  | Document Number |  |  |  |
| `FiscalPeriod` | `POPER` | `POPER` | `VBRK` | `String(3)` |  | Posting Period |  |  | ECC: unpadded '3' (MONAT); S/4: zero-padded '003' |
| `CustomerAccountAssignmentGroup` | `KTGRD` | `KTGRD` | `VBRK` | `String(2)` |  | Acct Assmt Grp Cust. |  |  |  |
| `AccountingExchangeRateIsSet` | `CPKUR` | `CPKUR` | `VBRK` | `Boolean` |  | Set Exchange Rate |  |  |  |
| `AccountingExchangeRate` | `KURRF_NOT_CONVERTED` | `KURRF_NOT_CONVERTED` | `VBRK` | `Decimal(9,5)` |  | Accounting Exchange Rate |  |  |  |
| `ExchangeRateDate` | `WWERT_D` | `WWERT` | `VBRK` | `Date` |  | Translation Date |  |  |  |
| `ExchangeRateType` | `KURST` | `KURST` | `VBRK` | `String(4)` |  | Exchange Rate Type |  |  |  |
| `DocumentReferenceID` | `XBLNR_V1` | `XBLNR_V1` | `VBRK` | `String(16)` |  | Reference |  |  |  |
| `AssignmentReference` | `ORDNR_V` | `ORDNR_V` | `VBRK` | `String(18)` |  | Assignment |  |  |  |
| `ReversalReason` | `STGRD` | `STGRD` | `VBRK` | `String(2)` |  | Reversal Reason |  |  |  |
| `DunningArea` | `MABER` | `MABER` | `VBRK` | `String(2)` |  | Dunning Area |  |  |  |
| `DunningBlockingReason` | `MANSP` | `MANSP` | `VBRK` | `String(1)` |  | Dunning Block |  |  |  |
| `DunningKey` | `MSCHL` | `MSCHL` | `VBRK` | `String(1)` |  | Dunning Key |  |  |  |
| `InternalFinancialDocument` | `LCNUM` | `LCNUM` | `VBRK` | `String(10)` |  | Financial Doc. No. |  |  |  |
| `IsRelevantForAccrual` | `ISACCRUALRELEVANT` | `ISACCRUALRELEVANT` | `VBRK` | `Boolean` |  | Relevant for Accrual |  |  |  |
| `SoldToParty` | `KUNAG` | `KUNAG` | `VBRK` | `String(10)` |  | Sold-to Party |  |  |  |
| `PartnerCompany` | `RASSC` | `RASSC` | `VBRK` | `String(6)` |  | Trading Partner No. |  |  |  |
| `PurchaseOrderByCustomer` | `BSTKD` | `BSTKD` | `VBRK` | `String(35)` |  | Customer Reference |  |  |  |
| `CustomerGroup` | `KDGRP` | `KDGRP` | `VBRK` | `String(2)` |  | Customer Group |  |  |  |
| `Country` | `LLAND` | `LLAND` | `VBRK` | `String(3)` |  | Dest. Country/Region |  |  |  |
| `CityCode` | `CITYC` | `CITYC` | `VBRK` | `String(4)` |  | City Code |  |  |  |
| `SalesDistrict` | `BZIRK` | `BZIRK` | `VBRK` | `String(6)` |  | Sales District |  |  |  |
| `Region` | `REGIO` | `REGIO` | `VBRK` | `String(3)` |  | Region |  |  |  |
| `County` | `COUNC` | `COUNC` | `VBRK` | `String(3)` |  | County Code |  |  |  |
| `CreditControlArea` | `KKBER` | `KKBER` | `VBRK` | `String(4)` |  | Credit Control Area |  |  |  |
| `CustomerRebateAgreement` | `KNUMA` | `KNUMA` | `VBRK` | `String(10)` |  | Agreement |  |  |  |
| `PricingDocument` | `KNUMV` | `KNUMV` | `VBRK` | `String(10)` |  | Doc. Condition No. |  |  |  |
| `OverallSDProcessStatus` | `GBSTK` | `GBSTK` | `VBRK` | `String(1)` |  | Overall Status |  |  |  |
| `OverallBillingStatus` | `VF_STATUS` | `VF_STATUS` | `VBRK` | `String(1)` |  | Status |  |  |  |
| `AccountingPostingStatus` | `BUCHK` | `BUCHK` | `VBRK` | `String(1)` |  | Posting Status |  |  |  |
| `AccountingTransferStatus` | `RFBSK` | `RFBSK` | `VBRK` | `String(1)` |  | Posting Status |  |  |  |
| `BillingIssueType` | `VF_TODO` | `VF_TODO` | `VBRK` | `String(1)` |  | Issue Type |  |  |  |
| `InvoiceListStatus` | `RELIK` | `RELIK` | `VBRK` | `String(1)` |  | Invoice List Status |  |  |  |
| `OvrlItmGeneralIncompletionSts` | `UVALL_SU` | `UVALL_SU` | `VBRK` | `String(1)` |  | All Items |  |  |  |
| `OverallPricingIncompletionSts` | `UVPRS_UK` | `UVPRS_UK` | `VBRK` | `String(1)` |  | Pricing – All Items |  |  |  |
| `InvoiceClearingStatus` | `CLRST` | `CLRST` | `VBRK` | `String(1)` |  | Clearing Status |  |  |  |
| `InvoiceListType` | `FKART_RL` | `FKART_RL` | `VBRK` | `String(4)` |  | Invoice List Type |  |  |  |
| `InvoiceListBillingDate` | `FKDAT_RL` | `FKDAT_RL` | `VBRK` | `Date` |  | Inv. List Bill. Date |  |  |  |
| `ForeignTradeStstclCurrency` | `GRWCU` | `GRWCU` | `VBRK` | `String(5)` |  | Currency |  |  |  |


## Entity: `BillingDocumentItem`

- **ABAP Name:** `I_BillingDocumentItem`
- **Label:** Billing Document Item
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** VBRP

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `BillingDocument` | `VBELN_VF` | `VBELN` | `VBRP` | `String(10)` | Y | Billing Document |  | _BillingDocument |  |
| `BillingDocumentItem` | `POSNR_VF` | `POSNR` | `VBRP` | `String(6)` | Y | Item |  |  |  |
| `SalesDocumentItemCategory` | `SALES_DOC_ITEM_CATEGORY` | `SALES_DOC_ITEM_CATEGORY` | `VBRP` | `String(4)` |  | Sales Doc. Item Cat. |  |  |  |
| `SalesDocumentItemType` | `POSAR` | `POSAR` | `VBRP` | `String(1)` |  | Item Type |  |  |  |
| `ReturnItemProcessingType` | `SHKZG_VF` | `SHKZG_VF` | `VBRP` | `String(1)` |  | Returns |  |  |  |
| `CreatedByUser` | `ERNAM` | `ERNAM` | `VBRP` | `String(12)` |  | Created By |  |  |  |
| `CreationDate` | `ERDAT` | `ERDAT` | `VBRP` | `Date` |  | Created On |  |  |  |
| `CreationTime` | `ERZET` | `ERZET` | `VBRP` | `String(6)` |  | Time |  |  |  |
| `ReferenceLogicalSystem` | `LOGSYS` | `LOGSYS` | `VBRP` | `String(10)` |  | Logical System |  |  |  |
| `OrganizationDivision` | `SALES_ORDER_DIVISON` | `SALES_ORDER_DIVISON` | `VBRP` | `String(2)` |  | Division of Order |  |  |  |
| `Division` | `SPART` | `SPART` | `VBRP` | `String(2)` |  | Division |  |  |  |
| `SalesOffice` | `VKBUR` | `VKBUR` | `VBRP` | `String(4)` |  | Sales Office |  |  |  |
| `Material` | `MATNR` | `MATNR` | `VBRP` | `String(40)` |  | Material |  |  |  |
| `Product` | `PRODUCTNUMBER` | `PRODUCTNUMBER` | `VBRP` | `String(40)` |  | Product |  |  |  |
| `OriginallyRequestedMaterial` | `MATWA` | `MATWA` | `VBRP` | `String(40)` |  | Material Entered |  |  |  |
| `InternationalArticleNumber` | `EAN11` | `EAN11` | `VBRP` | `String(18)` |  | EAN/UPC |  |  |  |
| `PricingReferenceMaterial` | `PMATN` | `PMATN` | `VBRP` | `String(40)` |  | Pricing Ref. Matl |  |  |  |
| `Batch` | `CHARG_D` | `CHARG` | `VBRP` | `String(10)` |  | Batch |  |  |  |
| `ProductHierarchyNode` | `PRODH_D` | `PRODH` | `VBRP` | `String(18)` |  | Product Hierarchy |  |  |  |
| `MaterialGroup` | `MATKL` | `MATKL` | `VBRP` | `String(9)` |  | Material Group |  |  |  |
| `ProductGroup` | `PRODUCTGROUP` | `PRODUCTGROUP` | `VBRP` | `String(9)` |  | Product Group |  |  |  |
| `AdditionalMaterialGroup1` | `MVGR1` | `MVGR1` | `VBRP` | `String(3)` |  | Material Group 1 |  |  |  |
| `AdditionalMaterialGroup2` | `MVGR2` | `MVGR2` | `VBRP` | `String(3)` |  | Material Group 2 |  |  |  |
| `AdditionalMaterialGroup3` | `MVGR3` | `MVGR3` | `VBRP` | `String(3)` |  | Material Group 3 |  |  |  |
| `AdditionalMaterialGroup4` | `MVGR4` | `MVGR4` | `VBRP` | `String(3)` |  | Material Group 4 |  |  |  |
| `AdditionalMaterialGroup5` | `MVGR5` | `MVGR5` | `VBRP` | `String(3)` |  | Material Group 5 |  |  |  |
| `ProductConfiguration` | `CUOBJ_VA` | `CUOBJ_VA` | `VBRP` | `String(18)` |  | Configuration |  |  |  |
| `MaterialCommissionGroup` | `PROVG` | `PROVG` | `VBRP` | `String(2)` |  | Commission Group |  |  |  |
| `Plant` | `WERKS_D` | `WERKS` | `VBRP` | `String(4)` |  | Plant |  |  |  |
| `StorageLocation` | `LGORT_D` | `LGORT` | `VBRP` | `String(4)` |  | Storage Location |  |  |  |
| `ReplacementPartType` | `ATPKZ` | `ATPKZ` | `VBRP` | `String(1)` |  | Replacement Part |  |  |  |
| `MaterialGroupHierarchy1` | `WGRU_HIE1` | `WGRU_HIE1` | `VBRP` | `String(18)` |  | Material Group 1 |  |  |  |
| `MaterialGroupHierarchy2` | `WGRU_HIE2` | `WGRU_HIE2` | `VBRP` | `String(18)` |  | Material Group 2 |  |  |  |
| `PlantRegion` | `WKREG` | `WKREG` | `VBRP` | `String(3)` |  | Region of Dlv. Plant |  |  |  |
| `PlantCounty` | `WKCOU` | `WKCOU` | `VBRP` | `String(3)` |  | County of Dlv.Plant |  |  |  |
| `PlantCity` | `WKCTY` | `WKCTY` | `VBRP` | `String(4)` |  | City of Deliv. Plant |  |  |  |
| `TransitPlant` | `TRANSIT_PLANT` | `TRANSIT_PLANT` | `VBRP` | `String(4)` |  | Transit Plant |  |  |  |
| `ValueChainCategory` | `VCM_CHAIN_CATEGORY` | `VCM_CHAIN_CATEGORY` | `VBRP` | `String(4)` |  | Value Chain Category |  |  |  |
| `BOMExplosion` | `SERNR` | `SERNR` | `VBRP` | `String(8)` |  | BOM Explosion Number |  |  |  |
| `MaterialDeterminationType` | `PROSA` | `PROSA` | `VBRP` | `String(1)` |  | Mat.Determ.Active |  |  |  |
| `SoldProduct` | `SDBIL_SOLD_PRODUCT` | `SDBIL_SOLD_PRODUCT` | `VBRP` | `String(40)` |  | Product Sold |  |  |  |
| `BillingDocumentItemText` | `ARKTX` | `ARKTX` | `VBRP` | `String(40)` |  | Item Description |  |  |  |
| `ServicesRenderedDate` | `FBUDA` | `FBUDA` | `VBRP` | `Date` |  | Serv. Rendered Date |  |  |  |
| `BillingQuantity` | `FKIMG` | `FKIMG` | `VBRP` | `Decimal(13,3)` |  | Invoiced Quantity | BillingQuantityUnit |  |  |
| `BillingQuantityUnit` | `VRKME` | `VRKME` | `VBRP` | `String(3)` |  | Sales Unit |  |  |  |
| `BillingQuantityInBaseUnit` | `FKLMG` | `FKLMG` | `VBRP` | `Decimal(13,3)` |  | Billing Qty in SKU | BaseUnit |  |  |
| `BaseUnit` | `MEINS` | `MEINS` | `VBRP` | `String(3)` |  | Base Unit of Measure |  |  |  |
| `MRPRequiredQuantityInBaseUnit` | `LMENG` | `LMENG` | `VBRP` | `Decimal(13,3)` |  | Required Quantity | BaseUnit |  |  |
| `BillingToBaseQuantityDnmntr` | `UMVKN` | `UMVKN` | `VBRP` | `Decimal(5,0)` |  | Denominator |  |  |  |
| `BillingToBaseQuantityNmrtr` | `UMVKZ` | `UMVKZ` | `VBRP` | `Decimal(5,0)` |  | Numerator |  |  |  |
| `ItemGrossWeight` | `BRGEW_15` | `BRGEW_15` | `VBRP` | `Decimal(15,3)` |  | Gross Weight | ItemWeightUnit |  |  |
| `ItemNetWeight` | `NTGEW_15` | `NTGEW_15` | `VBRP` | `Decimal(15,3)` |  | Net Weight | ItemWeightUnit |  |  |
| `ItemWeightUnit` | `GEWEI` | `GEWEI` | `VBRP` | `String(3)` |  | Unit of Weight |  |  |  |
| `ItemVolume` | `VOLUM_15` | `VOLUM_15` | `VBRP` | `Decimal(15,3)` |  | Volume | ItemVolumeUnit |  |  |
| `ItemVolumeUnit` | `VOLEH` | `VOLEH` | `VBRP` | `String(3)` |  | Volume Unit |  |  |  |
| `BillToPartyCountry` | `LLAND_AUFT` | `LLAND_AUFT` | `VBRP` | `String(3)` |  | Dest. Ctry/Reg. Ord. |  |  |  |
| `BillToPartyRegion` | `REGIO_AUFT` | `REGIO_AUFT` | `VBRP` | `String(3)` |  | Region Order |  |  |  |
| `BillingPlanRule` | `FAREG` | `FAREG` | `VBRP` | `String(1)` |  | Billing Rule |  |  |  |
| `BillingPlan` | `FPLNR` | `FPLNR` | `VBRP` | `String(10)` |  | Bill. Plan No. |  |  |  |
| `BillingPlanItem` | `FPLTR` | `FPLTR` | `VBRP` | `String(6)` |  | Item |  |  |  |
| `DownPaymentProcessingVariant` | `SDBIL_DWN_PAYT_PROCG_VAR` | `SDBIL_DWN_PAYT_PROCG_VAR` | `VBRP` | `String(1)` |  | Down Payment Variant |  |  |  |
| `NetAmount` | `NETWR_FP` | `NETWR_FP` | `VBRP` | `Decimal(34,4)` |  | Net Value | TransactionCurrency |  |  |
| `TransactionCurrency` | `WAERK` | `WAERK` | `VBRP` | `String(5)` |  | Document Currency |  |  |  |
| `GrossAmount` | `BRTWR_FP` | `BRTWR_FP` | `VBRP` | `Decimal(34,4)` |  | Gross Value | TransactionCurrency |  |  |
| `PricingDate` | `PRSDT` | `PRSDT` | `VBRP` | `Date` |  | Pricing Date |  |  |  |
| `PriceDetnExchangeRate` | `KURSK_NOT_CONVERTED` | `KURSK_NOT_CONVERTED` | `VBRP` | `Decimal(9,5)` |  | Exchange Rate |  |  |  |
| `PricingScaleQuantityInBaseUnit` | `SMENG` | `SMENG` | `VBRP` | `Decimal(13,3)` |  | Scale Quantity | BaseUnit |  |  |
| `TaxAmount` | `MWSBP` | `MWSBP` | `VBRP` | `Decimal(34,4)` |  | Tax Amount | TransactionCurrency |  |  |
| `CostAmount` | `WAVWR` | `WAVWR` | `VBRP` | `Decimal(34,4)` |  | Cost | TransactionCurrency |  |  |
| `Subtotal1Amount` | `KZWI1` | `KZWI1` | `VBRP` | `Decimal(34,4)` |  | Subtotal 1 | TransactionCurrency |  |  |
| `Subtotal2Amount` | `KZWI2` | `KZWI2` | `VBRP` | `Decimal(34,4)` |  | Subtotal 2 | TransactionCurrency |  |  |
| `Subtotal3Amount` | `KZWI3` | `KZWI3` | `VBRP` | `Decimal(34,4)` |  | Subtotal 3 | TransactionCurrency |  |  |
| `Subtotal4Amount` | `KZWI4` | `KZWI4` | `VBRP` | `Decimal(34,4)` |  | Subtotal 4 | TransactionCurrency |  |  |
| `Subtotal5Amount` | `KZWI5` | `KZWI5` | `VBRP` | `Decimal(34,4)` |  | Subtotal 5 | TransactionCurrency |  |  |
| `Subtotal6Amount` | `KZWI6` | `KZWI6` | `VBRP` | `Decimal(34,4)` |  | Subtotal 6 | TransactionCurrency |  |  |
| `StatisticalValueControl` | `KOWRR` | `KOWRR` | `VBRP` | `String(1)` |  | Statistical Value |  |  |  |
| `CashDiscountIsDeductible` | `SKTOF` | `SKTOF` | `VBRP` | `Boolean` |  | Cash Discount |  |  |  |
| `CustomerConditionGroup1` | `KDKG1` | `KDKG1` | `VBRP` | `String(2)` |  | Condition Group 1 |  |  |  |
| `CustomerConditionGroup2` | `KDKG2` | `KDKG2` | `VBRP` | `String(2)` |  | Condition Group 2 |  |  |  |
| `CustomerConditionGroup3` | `KDKG3` | `KDKG3` | `VBRP` | `String(2)` |  | Condition Group 3 |  |  |  |
| `CustomerConditionGroup4` | `KDKG4` | `KDKG4` | `VBRP` | `String(2)` |  | Condition Group 4 |  |  |  |
| `CustomerConditionGroup5` | `KDKG5` | `KDKG5` | `VBRP` | `String(2)` |  | Condition Group 5 |  |  |  |
| `ManualPriceChangeType` | `MPROK` | `MPROK` | `VBRP` | `String(1)` |  | Manual Price |  |  |  |
| `MaterialPricingGroup` | `KONDM` | `KONDM` | `VBRP` | `String(2)` |  | Material Price Grp |  |  |  |
| `StatisticsExchangeRate` | `STCUR_AP_NOT_CONVERTED` | `STCUR_AP_NOT_CONVERTED` | `VBRP` | `Decimal(9,5)` |  | Exchange Rate Stats. |  |  |  |
| `MainItemPricingRefMaterial` | `UPMAT` | `UPMAT` | `VBRP` | `String(40)` |  | Pricing Ref.Material |  |  |  |
| `MainItemMaterialPricingGroup` | `UKONM` | `UKONM` | `VBRP` | `String(2)` |  | MnItem MatPricingGrp |  |  |  |
| `TimeSheetOvertimeCategory` | `CATS_OVERTIME_CATEGORY` | `CATS_OVERTIME_CATEGORY` | `VBRP` | `String(4)` |  | Overtime Category |  |  |  |
| `PricingRelevance` | `PRSFD` | `PRSFD` | `VBRP` | `String(1)` |  | Pricing Relevance |  |  |  |
| `DepartureCountry` | `ALAND` | `ALAND` | `VBRP` | `String(3)` |  | Departure Ctry/Reg. |  |  |  |
| `TaxJurisdiction` | `TXJCD` | `TXJCD` | `VBRP` | `String(15)` |  | Tax Jurisdiction |  |  |  |
| `ProductTaxClassification1` | `PRODUCT_TAX_CLASSIFICATION_1` | `PRODUCT_TAX_CLASSIFICATION_1` | `VBRP` | `String(1)` |  | Product Tax Classification 1 |  |  |  |
| `ProductTaxClassification2` | `PRODUCT_TAX_CLASSIFICATION_2` | `PRODUCT_TAX_CLASSIFICATION_2` | `VBRP` | `String(1)` |  | Product Tax Classification 2 |  |  |  |
| `ProductTaxClassification3` | `PRODUCT_TAX_CLASSIFICATION_3` | `PRODUCT_TAX_CLASSIFICATION_3` | `VBRP` | `String(1)` |  | Product Tax Classification 3 |  |  |  |
| `ProductTaxClassification4` | `PRODUCT_TAX_CLASSIFICATION_4` | `PRODUCT_TAX_CLASSIFICATION_4` | `VBRP` | `String(1)` |  | Product Tax Classification 4 |  |  |  |
| `ProductTaxClassification5` | `PRODUCT_TAX_CLASSIFICATION_5` | `PRODUCT_TAX_CLASSIFICATION_5` | `VBRP` | `String(1)` |  | Product Tax Classification 5 |  |  |  |
| `ProductTaxClassification6` | `PRODUCT_TAX_CLASSIFICATION_6` | `PRODUCT_TAX_CLASSIFICATION_6` | `VBRP` | `String(1)` |  | Product Tax Classification 6 |  |  |  |
| `ProductTaxClassification7` | `PRODUCT_TAX_CLASSIFICATION_7` | `PRODUCT_TAX_CLASSIFICATION_7` | `VBRP` | `String(1)` |  | Product Tax Classification 7 |  |  |  |
| `ProductTaxClassification8` | `PRODUCT_TAX_CLASSIFICATION_8` | `PRODUCT_TAX_CLASSIFICATION_8` | `VBRP` | `String(1)` |  | Product Tax Classification 8 |  |  |  |
| `ProductTaxClassification9` | `PRODUCT_TAX_CLASSIFICATION_9` | `PRODUCT_TAX_CLASSIFICATION_9` | `VBRP` | `String(1)` |  | Product Tax Classification 9 |  |  |  |
| `ZeroVATRsn` | `J_1ARFZVAT` | `J_1ARFZVAT` | `VBRP` | `String(1)` |  | Reason 0 VAT |  |  |  |
| `TaxCode` | `MWSKZ` | `MWSKZ` | `VBRP` | `String(2)` |  | Tax Code |  |  |  |
| `TaxRateValidityStartDate` | `FOT_TXDAT_FROM` | `TXDAT_FROM` | `VBRP` | `Date` |  | Tax Rate Valid-From |  |  |  |
| `CountryOfOrigin` | `HERKL` | `HERKL` | `VBRP` | `String(3)` |  | Cntry/Reg of Origin |  |  |  |
| `RegionOfOrigin` | `HERKR` | `HERKR` | `VBRP` | `String(3)` |  | Region of Origin |  |  |  |
| `CommodityCode` | `/SAPSLL/COMCO` | `/SAPSLL/COMCO` | `VBRP` | `String(30)` |  | Commodity Code |  |  |  |
| `EligibleAmountForCashDiscount` | `SKFBP` | `SKFBP` | `VBRP` | `Decimal(34,4)` |  | Cash Disc. Bas. | TransactionCurrency |  |  |
| `BusinessArea` | `GSBER` | `GSBER` | `VBRP` | `String(4)` |  | Business Area |  |  |  |
| `ProfitCenter` | `PRCTR` | `PRCTR` | `VBRP` | `String(10)` |  | Profit Center |  |  |  |
| `OrderID` | `AUFNR` | `AUFNR` | `VBRP` | `String(12)` |  | Order |  |  |  |
| `WBSElement` | `PS_PSP_PNR` | `PS_PSP_PNR` | `VBRP` | `String(8)` |  | WBS Element |  |  |  |
| `WBSElementInternalID` | `PS_S4_PSPNR` | `PS_S4_PSPNR` | `VBRP` | `String(8)` |  | WBS Internal ID |  |  |  |
| `ProviderContract` | `VTKEY_KK` | `VTKEY_KK` | `VBRP` | `String(20)` |  | Provider Contract |  |  |  |
| `ProviderContractItem` | `PROVIDER_CONTRACT_ITEM` | `PROVIDER_CONTRACT_ITEM` | `VBRP` | `String(6)` |  | Provider Contract Item |  |  |  |
| `BillingPerformancePeriodStrDte` | `FM_PEROP_SD_LOW` | `FM_PEROP_SD_LOW` | `VBRP` | `Date` |  | Per. of Perf. Start |  |  |  |
| `BillingPeriodOfPerfStartDate` | `FM_PEROP_SD_LOW` | `FM_PEROP_SD_LOW` | `VBRP` | `Date` |  | Per. of Perf. Start |  |  |  |
| `BillingPerformancePeriodEndDte` | `FM_PEROP_SD_HIGH` | `FM_PEROP_SD_HIGH` | `VBRP` | `Date` |  | Per. of Perf. End |  |  |  |
| `BillingPeriodOfPerfEndDate` | `FM_PEROP_SD_HIGH` | `FM_PEROP_SD_HIGH` | `VBRP` | `Date` |  | Per. of Perf. End |  |  |  |
| `ControllingArea` | `KOKRS` | `KOKRS` | `VBRP` | `String(4)` |  | Controlling Area |  |  |  |
| `ProfitabilitySegment` | `RKEOBJNR_NUMC` | `RKEOBJNR_NUMC` | `VBRP` | `String(10)` |  | Profitability Segment (Deprecated) |  |  |  |
| `ProfitabilitySegment_2` | `RKEOBJNR_CHAR` | `RKEOBJNR_CHAR` | `VBRP` | `String(10)` |  | Profitability Segment |  |  |  |
| `CostCenter` | `KOSTL` | `KOSTL` | `VBRP` | `String(10)` |  | Cost Center |  |  |  |
| `OriginSDDocument` | `VBELV` | `VBELV` | `VBRP` | `String(10)` |  | Originating Document |  |  |  |
| `OriginSDDocumentItem` | `POSNV` | `POSNV` | `VBRP` | `String(6)` |  | Originating Item |  |  |  |
| `PriceDetnExchangeRateDate` | `WWERT_D` | `WWERT` | `VBRP` | `Date` |  | Translation Date |  |  |  |
| `MatlAccountAssignmentGroup` | `KTGRM` | `KTGRM` | `VBRP` | `String(2)` |  | Acct Assmt Grp Mat. |  |  |  |
| `ReferenceSDDocument` | `VGBEL` | `VGBEL` | `VBRP` | `String(10)` |  | Reference Document |  |  |  |
| `ReferenceSDDocumentItem` | `VGPOS` | `VGPOS` | `VBRP` | `String(6)` |  | Reference Item |  |  |  |
| `ReferenceSDDocumentCategory` | `REFERENCE_DOC_CATEGORY` | `REFERENCE_DOC_CATEGORY` | `VBRP` | `String(4)` |  | Ref. Doc. Category |  |  |  |
| `SalesDocument` | `VBELN_VA` | `VBELN_VA` | `VBRP` | `String(10)` |  | Sales Document |  |  |  |
| `SalesDocumentItem` | `POSNR_VA` | `POSNR_VA` | `VBRP` | `String(6)` |  | Sales Document Item |  |  |  |
| `SalesSDDocumentCategory` | `SALES_DOCUMENT_CATEGORY` | `SALES_DOCUMENT_CATEGORY` | `VBRP` | `String(4)` |  | Sales Doc. Category |  |  |  |
| `HigherLevelItem` | `UEPOS` | `UEPOS` | `VBRP` | `String(6)` |  | Higher-Level Item |  |  |  |
| `HigherLvlItmOfBatSpltItm` | `UECHA` | `UECHA` | `VBRP` | `String(6)` |  | HigherLevelItemBatch |  |  |  |
| `BillingDocumentItemInPartSgmt` | `POSPA` | `POSPA` | `VBRP` | `String(6)` |  | Partner Item |  |  |  |
| `ExternalReferenceDocument` | `EXT_REFERENCE_DOCUMENT` | `EXT_REFERENCE_DOCUMENT` | `VBRP` | `String(10)` |  | Ext. Reference Document |  |  |  |
| `ExternalReferenceDocumentItem` | `EXT_REFERENCE_DOCUMENT_ITEM` | `EXT_REFERENCE_DOCUMENT_ITEM` | `VBRP` | `String(6)` |  | Ext. Ref. Document Item |  |  |  |
| `BillingDocExtReferenceDocItem` | `BILLINGDOCEXTREFERENCEDOCITEM` | `BILLINGDOCEXTREFERENCEDOCITEM` | `VBRP` | `String(6)` |  | Ext. Reference Doc. Item |  |  |  |
| `PrelimBillingDocument` | `PBD_ID` | `PBD_ID` | `VBRP` | `String(10)` |  | Prelimin. Bill. Doc. |  |  |  |
| `PrelimBillingDocumentItem` | `PBD_ITEM_ID` | `PBD_ITEM_ID` | `VBRP` | `String(6)` |  | Prelimin. Doc. Item |  |  |  |
| `SalesGroup` | `VKGRP` | `VKGRP` | `VBRP` | `String(3)` |  | Sales Group |  |  |  |
| `AdditionalCustomerGroup1` | `KVGR1` | `KVGR1` | `VBRP` | `String(3)` |  | Customer Group 1 |  |  |  |
| `AdditionalCustomerGroup2` | `KVGR2` | `KVGR2` | `VBRP` | `String(3)` |  | Customer Group 2 |  |  |  |
| `AdditionalCustomerGroup3` | `KVGR3` | `KVGR3` | `VBRP` | `String(3)` |  | Customer Group 3 |  |  |  |
| `AdditionalCustomerGroup4` | `KVGR4` | `KVGR4` | `VBRP` | `String(3)` |  | Customer Group 4 |  |  |  |
| `AdditionalCustomerGroup5` | `KVGR5` | `KVGR5` | `VBRP` | `String(3)` |  | Customer Group 5 |  |  |  |
| `SDDocumentReason` | `AUGRU` | `AUGRU` | `VBRP` | `String(3)` |  | Order Reason |  |  |  |
| `RetailPromotion` | `WAKTION` | `WAKTION` | `VBRP` | `String(10)` |  | Retail Promotion |  |  |  |
| `RebateBasisAmount` | `BONBA` | `BONBA` | `VBRP` | `Decimal(34,4)` |  | Rebate Basis | TransactionCurrency |  |  |
| `VolumeRebateGroup` | `BONUS` | `BONUS` | `VBRP` | `String(2)` |  | Volume Rebate Group |  |  |  |
| `ItemIsRelevantForCredit` | `CMPNT` | `CMPNT` | `VBRP` | `Boolean` |  | Credit Funct. Active |  |  |  |
| `CreditRelatedPrice` | `CMPRE` | `CMPRE` | `VBRP` | `Decimal(34,4)` |  | Credit Price | TransactionCurrency |  |  |
| `SalesDeal` | `KNUMA_AG` | `KNUMA_AG` | `VBRP` | `String(10)` |  | Sales Deal |  |  |  |
| `SalesPromotion` | `KNUMA_PI` | `KNUMA_PI` | `VBRP` | `String(10)` |  | Promotion |  |  |  |
| `SalesOrderSalesDistrict` | `BZIRK_AUFT` | `BZIRK_AUFT` | `VBRP` | `String(6)` |  | Sales Distr. Order |  |  |  |
| `SalesOrderCustomerGroup` | `KDGRP_AUFT` | `KDGRP_AUFT` | `VBRP` | `String(2)` |  | Customer Grp Order |  |  |  |
| `SalesOrderCustomerPriceGroup` | `KONDA_AUFT` | `KONDA_AUFT` | `VBRP` | `String(2)` |  | Price Group of Order |  |  |  |
| `SalesOrderPriceListType` | `PLTYP_AUFT` | `PLTYP_AUFT` | `VBRP` | `String(2)` |  | Price List Order |  |  |  |
| `SalesOrderSalesOrganization` | `VKORG_AUFT` | `VKORG_AUFT` | `VBRP` | `String(4)` |  | Sales Org. of Order |  |  |  |
| `SalesOrderDistributionChannel` | `VTWEG_AUFT` | `VTWEG_AUFT` | `VBRP` | `String(2)` |  | Distr. Channel Order |  |  |  |
| `SalesDocIsCreatedFromReference` | `AUREF` | `AUREF` | `VBRP` | `Boolean` |  | SalesDocumentRefer |  |  |  |
| `ShippingPoint` | `VSTEL` | `VSTEL` | `VBRP` | `String(4)` |  | Shipping Point |  |  |  |
| `ServiceDocumentType` | `FCO_SRVDOC_TYPE` | `FCO_SRVDOC_TYPE` | `VBRP` | `String(4)` |  | Service Doc. Type |  |  |  |
| `ServiceDocument` | `FCO_SRVDOC_ID` | `FCO_SRVDOC_ID` | `VBRP` | `String(10)` |  | Service Document |  |  |  |
| `ServiceDocumentItem` | `FCO_SRVDOC_ITEM_ID` | `FCO_SRVDOC_ITEM_ID` | `VBRP` | `String(6)` |  | Service Doc. Item |  |  |  |
| `BusinessSolutionOrder` | `CRMS4_SOLO_OBJECT_ID` | `CRMS4_SOLO_OBJECT_ID` | `VBRP` | `String(10)` |  | Solution Order |  |  |  |
| `BusinessSolutionOrderItem` | `CRMS4_SOLO_NUMBER_INT` | `CRMS4_SOLO_NUMBER_INT` | `VBRP` | `String(6)` |  | Solution Order Item |  |  |  |
| `HigherLevelItemUsage` | `UEPVW` | `UEPVW` | `VBRP` | `String(1)` |  | Usage of HL Item |  |  |  |
| `BillingDocumentIsTemporary` | `VF_DRAFT_INDICATOR` | `VF_DRAFT_INDICATOR` | `VBRP` | `Boolean` |  | Draft Indicator |  |  |  |
| `SDDocumentCategory` | `VBTYPL` | `VBTYPL` | `VBRP` | `String(4)` |  | SD Document Category |  |  |  |
| `BillingDocumentType` | `FKART` | `FKART` | `VBRP` | `String(4)` |  | Billing Type |  |  |  |
| `SalesOrganization` | `VKORG` | `VKORG` | `VBRP` | `String(4)` |  | Sales Organization |  |  |  |
| `DistributionChannel` | `VTWEG` | `VTWEG` | `VBRP` | `String(2)` |  | Distribution Channel |  |  |  |
| `CustomerPriceGroup` | `KONDA` | `KONDA` | `VBRP` | `String(2)` |  | Customer Price Group |  |  |  |
| `CustomerGroup` | `KDGRP` | `KDGRP` | `VBRP` | `String(2)` |  | Customer Group |  |  |  |
| `Country` | `LLAND` | `LLAND` | `VBRP` | `String(3)` |  | Dest. Country/Region |  |  |  |
| `Region` | `REGIO` | `REGIO` | `VBRP` | `String(3)` |  | Region |  |  |  |
| `CityCode` | `CITYC` | `CITYC` | `VBRP` | `String(4)` |  | City Code |  |  |  |
| `SalesDistrict` | `BZIRK` | `BZIRK` | `VBRP` | `String(6)` |  | Sales District |  |  |  |
| `OverallSDProcessStatus` | `GBSTK` | `GBSTK` | `VBRP` | `String(1)` |  | Overall Status |  |  |  |
| `OverallBillingStatus` | `VF_STATUS` | `VF_STATUS` | `VBRP` | `String(1)` |  | Status |  |  |  |
| `SoldToParty` | `KUNAG` | `KUNAG` | `VBRP` | `String(10)` |  | Sold-to Party |  |  |  |
| `PayerParty` | `KUNRG` | `KUNRG` | `VBRP` | `String(10)` |  | Payer |  |  |  |
| `BillingDocumentDate` | `FKDAT` | `FKDAT` | `VBRP` | `Date` |  | Billing Date |  |  |  |
| `CompanyCode` | `BUKRS` | `BUKRS` | `VBRP` | `String(4)` |  | Company Code |  |  |  |
| `County` | `COUNC` | `COUNC` | `VBRP` | `String(3)` |  | County Code |  |  |  |
| `CustomerRebateAgreement` | `KNUMA` | `KNUMA` | `VBRP` | `String(10)` |  | Agreement |  |  |  |
| `BillingDocumentCategory` | `FKTYP` | `FKTYP` | `VBRP` | `String(1)` |  | Billing Category |  |  |  |
| `PricingDocument` | `KNUMV` | `KNUMV` | `VBRP` | `String(10)` |  | Doc. Condition No. |  |  |  |
| `CancelledBillingDocument` | `SFAKN` | `SFAKN` | `VBRP` | `String(10)` |  | Canceled Bill. Doc. |  | _CancelledBillingDocument |  |
| `ShipToParty` | `KUNWE` | `KUNWE` | `VBRP` | `String(10)` |  | Ship-to Party |  |  |  |
| `BillToParty` | `KUNRE` | `KUNRE` | `VBRP` | `String(10)` |  | Bill-to Party |  |  |  |
| `SalesEmployee` | `SALES_EMPL` | `SALES_EMPL` | `VBRP` | `String(8)` |  | Sales Employee |  |  |  |
| `ResponsibleEmployee` | `RESP_EMPL` | `RESP_EMPL` | `VBRP` | `String(8)` |  | Employee Responsible |  |  |  |
