# Product

> Source file: `sap-s4com-Product-v1.json`


## Entity: `ProdIntlTradeClassification`

- **ABAP Name:** `I_ProdCommodityCodeDEX`
- **Label:** Data Extraction for Product Commodity Code by Country/Region
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `TrdClassfctnNmbrSchm` | `TrdClassfctnNmbrSchm` | `String(10)` | Y | Numbering Scheme |  |  | S/4 only entity (no ECC CDC mapping) |
| `Product` | `Product` | `String(40)` | Y | Product |  | _Product | S/4 only entity (no ECC CDC mapping) |
| `CommodityCode` | `CommodityCode` | `String(30)` | Y | Commodity Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityStartDate` | `ValidityStartDate` | `Date` | Y | Valid From |  |  | S/4 only entity (no ECC CDC mapping) |
| `Country` | `Country` | `String(3)` | Y | Country/Region |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityEndDate` | `ValidityEndDate` | `Date` |  | Valid To |  |  | S/4 only entity (no ECC CDC mapping) |
| `TrdClassfctnNmbrUUID` | `TrdClassfctnNmbrUUID` | `UUID` |  |  |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `ProdWhseManagementStorageType`

- **ABAP Name:** `I_ProdWrhsMgmtStorageType`
- **Label:** Product Data For Each Storage Type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Product` | `Product` | `String(40)` | Y | Product |  |  | S/4 only entity (no ECC CDC mapping) |
| `WarehouseNumber` | `WarehouseNumber` | `String(3)` | Y | Warehouse Number |  |  | S/4 only entity (no ECC CDC mapping) |
| `StorageType` | `StorageType` | `String(3)` | Y | Storage Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProdStorTypeMatlIsMrkdForDeltn` | `ProdStorTypeMatlIsMrkdForDeltn` | `Boolean` |  | Del. flag: stge type |  |  | S/4 only entity (no ECC CDC mapping) |
| `StorageBin` | `StorageBin` | `String(10)` |  | Storage Bin |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProdWrhsMaxStorageBinQuantity` | `ProdWrhsMaxStorageBinQuantity` | `Decimal(13,3)` |  | Maximum bin quantity | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `ProdWrhsMinStorageBinQuantity` | `ProdWrhsMinStorageBinQuantity` | `Decimal(13,3)` |  | Minimum bin quantity | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `ProdWrhsStorTypeCtrlQuantity` | `ProdWrhsStorTypeCtrlQuantity` | `Decimal(13,3)` |  | Control quantity | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `ProdWrhsStorTypeReplnmtQty` | `ProdWrhsStorTypeReplnmtQty` | `Decimal(13,3)` |  | Replenishment qty | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `LeanWrhsManagementPickingArea` | `LeanWrhsManagementPickingArea` | `String(3)` |  | Picking Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProdWrhsStorTypeRoundingQty` | `ProdWrhsStorTypeRoundingQty` | `Decimal(13,3)` |  | Rounding qty | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `BaseUnit` | `BaseUnit` | `String(3)` |  | Base Unit of Measure |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `Product`

- **ABAP Name:** `I_Product`
- **Label:** Product
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Product` | `Product` | `String(40)` | Y | Product |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductExternalID` | `ProductExternalID` | `String(40)` |  | Material |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductOID` | `ProductOID` | `String(128)` |  | Product OID |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductType` | `ProductType` | `String(4)` |  | Product Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `CreationDate` | `CreationDate` | `Date` |  | Created On |  |  | S/4 only entity (no ECC CDC mapping) |
| `CreationTime` | `CreationTime` | `String(6)` |  | Created At Time |  |  | S/4 only entity (no ECC CDC mapping) |
| `CreationDateTime` | `CreationDateTime` | `Timestamp` |  | Created On |  |  | S/4 only entity (no ECC CDC mapping) |
| `CreatedByUser` | `CreatedByUser` | `String(12)` |  | Created By |  |  | S/4 only entity (no ECC CDC mapping) |
| `LastChangeDate` | `LastChangeDate` | `Date` |  | Last Change |  |  | S/4 only entity (no ECC CDC mapping) |
| `LastChangedByUser` | `LastChangedByUser` | `String(12)` |  | Changed By |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsMarkedForDeletion` | `IsMarkedForDeletion` | `Boolean` |  | Marked for Deletion |  |  | S/4 only entity (no ECC CDC mapping) |
| `CrossPlantStatus` | `CrossPlantStatus` | `String(2)` |  | CrossPlantProdStatus |  |  | S/4 only entity (no ECC CDC mapping) |
| `CrossPlantStatusValidityDate` | `CrossPlantStatusValidityDate` | `Date` |  | Valid from |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductOldID` | `ProductOldID` | `String(40)` |  | Old Product Number |  |  | S/4 only entity (no ECC CDC mapping) |
| `GrossWeight` | `GrossWeight` | `Decimal(13,3)` |  | Gross Weight | WeightUnit |  | S/4 only entity (no ECC CDC mapping) |
| `PurchaseOrderQuantityUnit` | `PurchaseOrderQuantityUnit` | `String(3)` |  | Order Unit |  |  | S/4 only entity (no ECC CDC mapping) |
| `SourceOfSupply` | `SourceOfSupply` | `String(1)` |  | Source of supply |  |  | S/4 only entity (no ECC CDC mapping) |
| `WeightUnit` | `WeightUnit` | `String(3)` |  | Unit of Weight |  |  | S/4 only entity (no ECC CDC mapping) |
| `CountryOfOrigin` | `CountryOfOrigin` | `String(3)` |  | Cntry/Reg of Origin |  |  | S/4 only entity (no ECC CDC mapping) |
| `CompetitorID` | `CompetitorID` | `String(10)` |  | Competitor |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductGroup` | `ProductGroup` | `String(9)` |  | Product Group |  | _ProductGroup_2 | S/4 only entity (no ECC CDC mapping) |
| `BaseUnit` | `BaseUnit` | `String(3)` |  | Base Unit of Measure |  |  | S/4 only entity (no ECC CDC mapping) |
| `ItemCategoryGroup` | `ItemCategoryGroup` | `String(4)` |  | Gen. item cat. grp |  |  | S/4 only entity (no ECC CDC mapping) |
| `NetWeight` | `NetWeight` | `Decimal(13,3)` |  | Net Weight | WeightUnit |  | S/4 only entity (no ECC CDC mapping) |
| `ProductHierarchy` | `ProductHierarchy` | `String(18)` |  | Product Hierarchy |  |  | S/4 only entity (no ECC CDC mapping) |
| `Division` | `Division` | `String(2)` |  | Division |  |  | S/4 only entity (no ECC CDC mapping) |
| `VarblPurOrdUnitIsActive` | `VarblPurOrdUnitIsActive` | `String(1)` |  | Var. Order Unit |  |  | S/4 only entity (no ECC CDC mapping) |
| `VolumeUnit` | `VolumeUnit` | `String(3)` |  | Volume Unit |  |  | S/4 only entity (no ECC CDC mapping) |
| `MaterialVolume` | `MaterialVolume` | `Decimal(13,3)` |  | Volume | VolumeUnit |  | S/4 only entity (no ECC CDC mapping) |
| `SalesStatus` | `SalesStatus` | `String(2)` |  | X-DChain Status |  |  | S/4 only entity (no ECC CDC mapping) |
| `TransportationGroup` | `TransportationGroup` | `String(4)` |  | Transportation Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `SalesStatusValidityDate` | `SalesStatusValidityDate` | `Date` |  | Valid from |  |  | S/4 only entity (no ECC CDC mapping) |
| `AuthorizationGroup` | `AuthorizationGroup` | `String(4)` |  | Authorization Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `ANPCode` | `ANPCode` | `String(9)` |  | ANP Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductCategory` | `ProductCategory` | `String(2)` |  | Product Category |  |  | S/4 only entity (no ECC CDC mapping) |
| `Brand` | `Brand` | `String(4)` |  | Brand |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProcurementRule` | `ProcurementRule` | `String(1)` |  | Procurement rule |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityStartDate` | `ValidityStartDate` | `Date` |  | Valid From |  |  | S/4 only entity (no ECC CDC mapping) |
| `LowLevelCode` | `LowLevelCode` | `String(3)` |  | Low-Level Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProdNoInGenProdInPrepackProd` | `ProdNoInGenProdInPrepackProd` | `String(40)` |  | Generic Material |  |  | S/4 only entity (no ECC CDC mapping) |
| `SerialIdentifierAssgmtProfile` | `SerialIdentifierAssgmtProfile` | `String(4)` |  | Serial No. Profile |  |  | S/4 only entity (no ECC CDC mapping) |
| `SizeOrDimensionText` | `SizeOrDimensionText` | `String(32)` |  | Size/dimensions |  |  | S/4 only entity (no ECC CDC mapping) |
| `IndustryStandardName` | `IndustryStandardName` | `String(18)` |  | Industry Std Desc. |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductStandardID` | `ProductStandardID` | `String(18)` |  | GTIN |  |  | S/4 only entity (no ECC CDC mapping) |
| `InternationalArticleNumberCat` | `InternationalArticleNumberCat` | `String(2)` |  | EAN Category |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductIsConfigurable` | `ProductIsConfigurable` | `Boolean` |  | Configurable |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsBatchManagementRequired` | `IsBatchManagementRequired` | `Boolean` |  | Batch Management |  |  | S/4 only entity (no ECC CDC mapping) |
| `HasEmptiesBOM` | `HasEmptiesBOM` | `Boolean` |  | With Empties BOM |  |  | S/4 only entity (no ECC CDC mapping) |
| `ExternalProductGroup` | `ExternalProductGroup` | `String(18)` |  | Ext. Product Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `CrossPlantConfigurableProduct` | `CrossPlantConfigurableProduct` | `String(40)` |  | Cross-plant CP |  |  | S/4 only entity (no ECC CDC mapping) |
| `SerialNoExplicitnessLevel` | `SerialNoExplicitnessLevel` | `String(1)` |  | Serialization Level |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductManufacturerNumber` | `ProductManufacturerNumber` | `String(40)` |  | Mfr Part Number |  |  | S/4 only entity (no ECC CDC mapping) |
| `ManufacturerNumber` | `ManufacturerNumber` | `String(10)` |  | Manufacturer |  |  | S/4 only entity (no ECC CDC mapping) |
| `ManufacturerPartProfile` | `ManufacturerPartProfile` | `String(4)` |  | Mfr Part Profile |  |  | S/4 only entity (no ECC CDC mapping) |
| `QltyMgmtInProcmtIsActive` | `QltyMgmtInProcmtIsActive` | `Boolean` |  | QM in Procur. Active |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsApprovedBatchRecordReqd` | `IsApprovedBatchRecordReqd` | `Boolean` |  | Appr.Batch Recd Req. |  |  | S/4 only entity (no ECC CDC mapping) |
| `HandlingIndicator` | `HandlingIndicator` | `String(4)` |  | Handling Indicator |  |  | S/4 only entity (no ECC CDC mapping) |
| `WarehouseProductGroup` | `WarehouseProductGroup` | `String(4)` |  | WH Material Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `WarehouseStorageCondition` | `WarehouseStorageCondition` | `String(2)` |  | Whse Stor. Condition |  |  | S/4 only entity (no ECC CDC mapping) |
| `StandardHandlingUnitType` | `StandardHandlingUnitType` | `String(4)` |  | Standard HU Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `SerialNumberProfile` | `SerialNumberProfile` | `String(4)` |  | Serial No. Profile |  |  | S/4 only entity (no ECC CDC mapping) |
| `AdjustmentProfile` | `AdjustmentProfile` | `String(3)` |  | Adjust. Profile |  |  | S/4 only entity (no ECC CDC mapping) |
| `PreferredUnitOfMeasure` | `PreferredUnitOfMeasure` | `String(3)` |  | Preferred UoM |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsPilferable` | `IsPilferable` | `Boolean` |  | Pilferable |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsRelevantForHzdsSubstances` | `IsRelevantForHzdsSubstances` | `Boolean` |  | Relevant for HS |  |  | S/4 only entity (no ECC CDC mapping) |
| `QuarantinePeriod` | `QuarantinePeriod` | `Decimal(3,0)` |  | Quarant. Per. | TimeUnitForQuarantinePeriod |  | S/4 only entity (no ECC CDC mapping) |
| `TimeUnitForQuarantinePeriod` | `TimeUnitForQuarantinePeriod` | `String(3)` |  | Time Unit |  |  | S/4 only entity (no ECC CDC mapping) |
| `QualityInspectionGroup` | `QualityInspectionGroup` | `String(4)` |  | Quality Inspec. Grp |  |  | S/4 only entity (no ECC CDC mapping) |
| `HandlingUnitType` | `HandlingUnitType` | `String(4)` |  | Handling Unit Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `HasVariableTareWeight` | `HasVariableTareWeight` | `Boolean` |  | Varb. Tare Weight |  |  | S/4 only entity (no ECC CDC mapping) |
| `MaximumPackagingLength` | `MaximumPackagingLength` | `Decimal(15,3)` |  | Max. Pack. Length | UnitForMaxPackagingDimensions |  | S/4 only entity (no ECC CDC mapping) |
| `MaximumPackagingWidth` | `MaximumPackagingWidth` | `Decimal(15,3)` |  | Max. Pack. Width | UnitForMaxPackagingDimensions |  | S/4 only entity (no ECC CDC mapping) |
| `MaximumPackagingHeight` | `MaximumPackagingHeight` | `Decimal(15,3)` |  | Max. Pack. Height | UnitForMaxPackagingDimensions |  | S/4 only entity (no ECC CDC mapping) |
| `MaximumCapacity` | `MaximumCapacity` | `Decimal(15,3)` |  | Maximum Capacity |  |  | S/4 only entity (no ECC CDC mapping) |
| `OvercapacityTolerance` | `OvercapacityTolerance` | `Decimal(3,1)` |  | Overcapacity Toler. |  |  | S/4 only entity (no ECC CDC mapping) |
| `UnitForMaxPackagingDimensions` | `UnitForMaxPackagingDimensions` | `String(3)` |  | Unit of Measurement |  |  | S/4 only entity (no ECC CDC mapping) |
| `BaseUnitSpecificProductLength` | `BaseUnitSpecificProductLength` | `Decimal(13,3)` |  | Length | ProductMeasurementUnit |  | S/4 only entity (no ECC CDC mapping) |
| `BaseUnitSpecificProductWidth` | `BaseUnitSpecificProductWidth` | `Decimal(13,3)` |  | Width | ProductMeasurementUnit |  | S/4 only entity (no ECC CDC mapping) |
| `BaseUnitSpecificProductHeight` | `BaseUnitSpecificProductHeight` | `Decimal(13,3)` |  | Height | ProductMeasurementUnit |  | S/4 only entity (no ECC CDC mapping) |
| `ProductMeasurementUnit` | `ProductMeasurementUnit` | `String(3)` |  | Unit of Dimension |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductValidStartDate` | `ProductValidStartDate` | `Date` |  | Valid From |  |  | S/4 only entity (no ECC CDC mapping) |
| `ArticleCategory` | `ArticleCategory` | `String(2)` |  | Product Category |  |  | S/4 only entity (no ECC CDC mapping) |
| `ContentUnit` | `ContentUnit` | `String(3)` |  | Content Unit |  |  | S/4 only entity (no ECC CDC mapping) |
| `NetContent` | `NetContent` | `Decimal(13,3)` |  | Net Contents | ContentUnit |  | S/4 only entity (no ECC CDC mapping) |
| `ComparisonPriceQuantity` | `ComparisonPriceQuantity` | `Decimal(5,0)` |  | Comparison Price Unit | ContentUnit |  | S/4 only entity (no ECC CDC mapping) |
| `GrossContent` | `GrossContent` | `Decimal(13,3)` |  | Gross Contents | ContentUnit |  | S/4 only entity (no ECC CDC mapping) |
| `ProductValidEndDate` | `ProductValidEndDate` | `Date` |  | Valid To |  |  | S/4 only entity (no ECC CDC mapping) |
| `AssortmentListType` | `AssortmentListType` | `String(1)` |  | Assortment List Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `HasTextilePartsWthAnimalOrigin` | `HasTextilePartsWthAnimalOrigin` | `Boolean` |  | Animal Origin |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductSeasonUsageCategory` | `ProductSeasonUsageCategory` | `String(1)` |  | Season Usage |  |  | S/4 only entity (no ECC CDC mapping) |
| `IndustrySector` | `IndustrySector` | `String(1)` |  | Industry |  |  | S/4 only entity (no ECC CDC mapping) |
| `ChangeNumber` | `ChangeNumber` | `String(12)` |  | Change Number |  |  | S/4 only entity (no ECC CDC mapping) |
| `MaterialRevisionLevel` | `MaterialRevisionLevel` | `String(2)` |  | Revision Level |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsActiveEntity` | `IsActiveEntity` | `Boolean` |  | Is active |  |  | S/4 only entity (no ECC CDC mapping) |
| `LastChangeDateTime` | `LastChangeDateTime` | `Timestamp` |  | Last Changed |  |  | S/4 only entity (no ECC CDC mapping) |
| `LastChangeTime` | `LastChangeTime` | `String(6)` |  | Last Changed Time |  |  | S/4 only entity (no ECC CDC mapping) |
| `DangerousGoodsIndProfile` | `DangerousGoodsIndProfile` | `String(3)` |  | DG indicator profile |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductUUID` | `ProductUUID` | `UUID` |  | Product |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProdSupChnMgmtUUID22` | `ProdSupChnMgmtUUID22` | `String(22)` |  | Product ID |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductDocumentChangeNumber` | `ProductDocumentChangeNumber` | `String(6)` |  | Document Change No. |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductDocumentPageCount` | `ProductDocumentPageCount` | `String(3)` |  | Number Of Sheets |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductDocumentPageNumber` | `ProductDocumentPageNumber` | `String(3)` |  | Page Number |  |  | S/4 only entity (no ECC CDC mapping) |
| `OwnInventoryManagedProduct` | `OwnInventoryManagedProduct` | `String(40)` |  | Int. material number |  |  | S/4 only entity (no ECC CDC mapping) |
| `DocumentIsCreatedByCAD` | `DocumentIsCreatedByCAD` | `Boolean` |  | CAD Indicator |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductionOrInspectionMemoTxt` | `ProductionOrInspectionMemoTxt` | `String(18)` |  | Prod./insp. memo |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductionMemoPageFormat` | `ProductionMemoPageFormat` | `String(4)` |  | Page format |  |  | S/4 only entity (no ECC CDC mapping) |
| `GlobalTradeItemNumberVariant` | `GlobalTradeItemNumberVariant` | `String(2)` |  | EAN Variant |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductIsHighlyViscous` | `ProductIsHighlyViscous` | `Boolean` |  | Highly viscous |  |  | S/4 only entity (no ECC CDC mapping) |
| `TransportIsInBulk` | `TransportIsInBulk` | `Boolean` |  | In bulk/liquid |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProdAllocDetnProcedure` | `ProdAllocDetnProcedure` | `String(18)` |  | Product allocation |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProdEffctyParamValsAreAssigned` | `ProdEffctyParamValsAreAssigned` | `Boolean` |  | Assign effect. vals |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProdIsEnvironmentallyRelevant` | `ProdIsEnvironmentallyRelevant` | `Boolean` |  | Environmentally rlvt |  |  | S/4 only entity (no ECC CDC mapping) |
| `LaboratoryOrDesignOffice` | `LaboratoryOrDesignOffice` | `String(3)` |  | Lab/Office |  |  | S/4 only entity (no ECC CDC mapping) |
| `PackagingMaterialGroup` | `PackagingMaterialGroup` | `String(4)` |  | Matl Grp Pack.Matls |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductIsLocked` | `ProductIsLocked` | `Boolean` |  | Product locked |  |  | S/4 only entity (no ECC CDC mapping) |
| `DiscountInKindEligibility` | `DiscountInKindEligibility` | `String(1)` |  | Qual.f.FreeGoodsDis. |  |  | S/4 only entity (no ECC CDC mapping) |
| `SmartFormName` | `SmartFormName` | `String(30)` |  | Form Name |  |  | S/4 only entity (no ECC CDC mapping) |
| `PackingReferenceProduct` | `PackingReferenceProduct` | `String(40)` |  | Ref. Mat. for Pckg |  |  | S/4 only entity (no ECC CDC mapping) |
| `BasicMaterial` | `BasicMaterial` | `String(48)` |  | Basic Material |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductDocumentNumber` | `ProductDocumentNumber` | `String(22)` |  | Document |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductDocumentVersion` | `ProductDocumentVersion` | `String(2)` |  | Document Version |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductDocumentType` | `ProductDocumentType` | `String(3)` |  | Document Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductDocumentPageFormat` | `ProductDocumentPageFormat` | `String(4)` |  | Page Format |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductConfiguration` | `ProductConfiguration` | `String(18)` |  | Internal object no. |  |  | S/4 only entity (no ECC CDC mapping) |
| `SegmentationStrategy` | `SegmentationStrategy` | `String(8)` |  | Seg. Strategy |  |  | S/4 only entity (no ECC CDC mapping) |
| `SegmentationIsRelevant` | `SegmentationIsRelevant` | `Boolean` |  | Seg. Relevant |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductCompositionIsRelevant` | `ProductCompositionIsRelevant` | `Boolean` |  | Product Composition |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsChemicalComplianceRelevant` | `IsChemicalComplianceRelevant` | `String(1)` |  | Chemical Compliance Relevance Indicator |  |  | S/4 only entity (no ECC CDC mapping) |
| `ManufacturerBookPartNumber` | `ManufacturerBookPartNumber` | `String(40)` |  | MS Book Part No |  |  | S/4 only entity (no ECC CDC mapping) |
| `LogisticalProductCategory` | `LogisticalProductCategory` | `String(1)` |  | Logl Material Cat. |  |  | S/4 only entity (no ECC CDC mapping) |
| `SalesProduct` | `SalesProduct` | `String(40)` |  | Sales Material No. |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProdCharc1InternalNumber` | `ProdCharc1InternalNumber` | `String(10)` |  | Int. Char. Number |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProdCharc2InternalNumber` | `ProdCharc2InternalNumber` | `String(10)` |  | Int. Char. Number |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProdCharc3InternalNumber` | `ProdCharc3InternalNumber` | `String(10)` |  | Int. Char. Number |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductCharacteristic1` | `ProductCharacteristic1` | `String(18)` |  | Color |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductCharacteristic2` | `ProductCharacteristic2` | `String(18)` |  | Main Size |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductCharacteristic3` | `ProductCharacteristic3` | `String(18)` |  | Second Size |  |  | S/4 only entity (no ECC CDC mapping) |
| `MaintenanceStatus` | `MaintenanceStatus` | `String(15)` |  | Maintenance Status |  |  | S/4 only entity (no ECC CDC mapping) |
| `FashionProdInformationField1` | `FashionProdInformationField1` | `String(10)` |  | Fsh. Attribute1 |  |  | S/4 only entity (no ECC CDC mapping) |
| `FashionProdInformationField2` | `FashionProdInformationField2` | `String(10)` |  | Fsh. Attribute2 |  |  | S/4 only entity (no ECC CDC mapping) |
| `FashionProdInformationField3` | `FashionProdInformationField3` | `String(6)` |  | Fsh. Attribute3 |  |  | S/4 only entity (no ECC CDC mapping) |
| `DfsAmmunitionGroupCode` | `DfsAmmunitionGroupCode` | `String(8)` |  | Ammunition Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `DfsRICIdentifier` | `DfsRICIdentifier` | `Integer64` |  | RIC ID |  |  | S/4 only entity (no ECC CDC mapping) |
| `DfsProductSensitivity` | `DfsProductSensitivity` | `String(4)` |  | Sensitivity for Char |  |  | S/4 only entity (no ECC CDC mapping) |
| `DfsManufacturerPartLongNumber` | `DfsManufacturerPartLongNumber` | `String(60)` |  | Long Mfr Part No. |  |  | S/4 only entity (no ECC CDC mapping) |
| `DfsMatlConditionMgmt` | `DfsMatlConditionMgmt` | `String(1)` |  | Condition Mgmt |  |  | S/4 only entity (no ECC CDC mapping) |
| `DfsReturnDelivery` | `DfsReturnDelivery` | `String(1)` |  | Return Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `DfsLogisticsLevel` | `DfsLogisticsLevel` | `String(1)` |  | Return to Log.Level |  |  | S/4 only entity (no ECC CDC mapping) |
| `DfsNationalItemIdnNumber` | `DfsNationalItemIdnNumber` | `String(9)` |  | NATO Item ID Number |  |  | S/4 only entity (no ECC CDC mapping) |
| `LstMiProductToleranceType` | `LstMiProductToleranceType` | `String(4)` |  | Tolerance Type |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `ProductConsumption`

- **ABAP Name:** `I_ProductConsumption`
- **Label:** Product Consumption
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Product` | `Product` | `String(40)` | Y | Product |  |  | S/4 only entity (no ECC CDC mapping) |
| `Plant` | `Plant` | `String(4)` | Y | Plant |  |  | S/4 only entity (no ECC CDC mapping) |
| `PostingFiscalYear` | `PostingFiscalYear` | `String(4)` | Y | Fiscal Year |  |  | S/4 only entity (no ECC CDC mapping) |
| `PeriodType` | `PeriodType` | `String(1)` | Y | Period Indicator |  |  | S/4 only entity (no ECC CDC mapping) |
| `NumberOfFollowOnRecords` | `NumberOfFollowOnRecords` | `String(2)` | Y | Follow-on records |  |  | S/4 only entity (no ECC CDC mapping) |
| `TotalConsumption1Quantity` | `TotalConsumption1Quantity` | `Decimal(13,3)` |  | Tot.consumption 1 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `TotalConsumption2Quantity` | `TotalConsumption2Quantity` | `Decimal(13,3)` |  | Tot.consumption 2 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `TotalConsumption3Quantity` | `TotalConsumption3Quantity` | `Decimal(13,3)` |  | Tot.consumption 3 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `TotalConsumption4Quantity` | `TotalConsumption4Quantity` | `Decimal(13,3)` |  | Tot.consumption 4 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `TotalConsumption5Quantity` | `TotalConsumption5Quantity` | `Decimal(13,3)` |  | Tot.consumption 5 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `TotalConsumption6Quantity` | `TotalConsumption6Quantity` | `Decimal(13,3)` |  | Tot.consumption 6 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `TotalConsumption7Quantity` | `TotalConsumption7Quantity` | `Decimal(13,3)` |  | Tot.consumption 7 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `TotalConsumption8Quantity` | `TotalConsumption8Quantity` | `Decimal(13,3)` |  | Tot.consumption 8 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `TotalConsumption9Quantity` | `TotalConsumption9Quantity` | `Decimal(13,3)` |  | Tot.consumption 9 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `TotalConsumption10Quantity` | `TotalConsumption10Quantity` | `Decimal(13,3)` |  | Tot.consumption 10 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `TotalConsumption11Quantity` | `TotalConsumption11Quantity` | `Decimal(13,3)` |  | Tot.consumption 11 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `TotalConsumption12Quantity` | `TotalConsumption12Quantity` | `Decimal(13,3)` |  | Tot.consumption 12 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `TotalConsumption13Quantity` | `TotalConsumption13Quantity` | `Decimal(13,3)` |  | Tot.consumption 13 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `UnplannedConsumption1Quantity` | `UnplannedConsumption1Quantity` | `Decimal(13,3)` |  | Unplnd consump. 1 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `UnplannedConsumption2Quantity` | `UnplannedConsumption2Quantity` | `Decimal(13,3)` |  | Unplnd consump. 2 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `UnplannedConsumption3Quantity` | `UnplannedConsumption3Quantity` | `Decimal(13,3)` |  | Unplnd consump. 3 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `UnplannedConsumption4Quantity` | `UnplannedConsumption4Quantity` | `Decimal(13,3)` |  | Unplnd consump. 4 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `UnplannedConsumption5Quantity` | `UnplannedConsumption5Quantity` | `Decimal(13,3)` |  | Unplnd consump. 5 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `UnplannedConsumption6Quantity` | `UnplannedConsumption6Quantity` | `Decimal(13,3)` |  | Unplnd consump. 6 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `UnplannedConsumption7Quantity` | `UnplannedConsumption7Quantity` | `Decimal(13,3)` |  | Unplnd consump. 7 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `UnplannedConsumption8Quantity` | `UnplannedConsumption8Quantity` | `Decimal(13,3)` |  | Unplnd consump. 8 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `UnplannedConsumption9Quantity` | `UnplannedConsumption9Quantity` | `Decimal(13,3)` |  | Unplnd consump. 9 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `UnplannedConsumption10Quantity` | `UnplannedConsumption10Quantity` | `Decimal(13,3)` |  | Unplnd consump. 10 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `UnplannedConsumption11Quantity` | `UnplannedConsumption11Quantity` | `Decimal(13,3)` |  | Unplnd consump. 11 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `UnplannedConsumption12Quantity` | `UnplannedConsumption12Quantity` | `Decimal(13,3)` |  | Unplnd consump. 12 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `UnplannedConsumption13Quantity` | `UnplannedConsumption13Quantity` | `Decimal(13,3)` |  | Unplnd consump. 13 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `MnllyCrrtdTotCnsmpn1Quantity` | `MnllyCrrtdTotCnsmpn1Quantity` | `Decimal(13,3)` |  | Corr.tot.consum 1 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `MnllyCrrtdTotCnsmpn2Quantity` | `MnllyCrrtdTotCnsmpn2Quantity` | `Decimal(13,3)` |  | Corr.tot.consum 2 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `MnllyCrrtdTotCnsmpn3Quantity` | `MnllyCrrtdTotCnsmpn3Quantity` | `Decimal(13,3)` |  | Corr.tot.consum 3 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `MnllyCrrtdTotCnsmpn4Quantity` | `MnllyCrrtdTotCnsmpn4Quantity` | `Decimal(13,3)` |  | Corr.tot.consum 4 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `MnllyCrrtdTotCnsmpn5Quantity` | `MnllyCrrtdTotCnsmpn5Quantity` | `Decimal(13,3)` |  | Corr.tot.consum 5 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `MnllyCrrtdTotCnsmpn6Quantity` | `MnllyCrrtdTotCnsmpn6Quantity` | `Decimal(13,3)` |  | Corr.tot.consum 6 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `MnllyCrrtdTotCnsmpn7Quantity` | `MnllyCrrtdTotCnsmpn7Quantity` | `Decimal(13,3)` |  | Corr.tot.consum 7 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `MnllyCrrtdTotCnsmpn8Quantity` | `MnllyCrrtdTotCnsmpn8Quantity` | `Decimal(13,3)` |  | Corr.tot.consum 8 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `MnllyCrrtdTotCnsmpn9Quantity` | `MnllyCrrtdTotCnsmpn9Quantity` | `Decimal(13,3)` |  | Corr.tot.consum 9 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `MnllyCrrtdTotCnsmpn10Quantity` | `MnllyCrrtdTotCnsmpn10Quantity` | `Decimal(13,3)` |  | Corr.tot.consum 10 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `MnllyCrrtdTotCnsmpn11Quantity` | `MnllyCrrtdTotCnsmpn11Quantity` | `Decimal(13,3)` |  | Corr.tot.consum 11 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `MnllyCrrtdTotCnsmpn12Quantity` | `MnllyCrrtdTotCnsmpn12Quantity` | `Decimal(13,3)` |  | Corr.tot.consum 12 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `MnllyCrrtdTotCnsmpn13Quantity` | `MnllyCrrtdTotCnsmpn13Quantity` | `Decimal(13,3)` |  | Corr.tot.consum 13 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `MnllyCrrtdUnplndCnsmpn1Qty` | `MnllyCrrtdUnplndCnsmpn1Qty` | `Decimal(13,3)` |  | Corr.unpl.cons. 1 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `MnllyCrrtdUnplndCnsmpn2Qty` | `MnllyCrrtdUnplndCnsmpn2Qty` | `Decimal(13,3)` |  | Corr.unpl.cons. 2 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `MnllyCrrtdUnplndCnsmpn3Qty` | `MnllyCrrtdUnplndCnsmpn3Qty` | `Decimal(13,3)` |  | Corr.unpl.cons. 3 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `MnllyCrrtdUnplndCnsmpn4Qty` | `MnllyCrrtdUnplndCnsmpn4Qty` | `Decimal(13,3)` |  | Corr.unpl.cons. 4 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `MnllyCrrtdUnplndCnsmpn5Qty` | `MnllyCrrtdUnplndCnsmpn5Qty` | `Decimal(13,3)` |  | Corr.unpl.cons. 5 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `MnllyCrrtdUnplndCnsmpn6Qty` | `MnllyCrrtdUnplndCnsmpn6Qty` | `Decimal(13,3)` |  | Corr.unpl.cons. 6 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `MnllyCrrtdUnplndCnsmpn7Qty` | `MnllyCrrtdUnplndCnsmpn7Qty` | `Decimal(13,3)` |  | Corr.unpl.cons. 7 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `MnllyCrrtdUnplndCnsmpn8Qty` | `MnllyCrrtdUnplndCnsmpn8Qty` | `Decimal(13,3)` |  | Corr.unpl.cons. 8 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `MnllyCrrtdUnplndCnsmpn9Qty` | `MnllyCrrtdUnplndCnsmpn9Qty` | `Decimal(13,3)` |  | Corr.unpl.cons. 9 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `MnllyCrrtdUnplndCnsmpn10Qty` | `MnllyCrrtdUnplndCnsmpn10Qty` | `Decimal(13,3)` |  | Corr.unpl.cons. 10 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `MnllyCrrtdUnplndCnsmpn11Qty` | `MnllyCrrtdUnplndCnsmpn11Qty` | `Decimal(13,3)` |  | Corr.unpl.cons. 11 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `MnllyCrrtdUnplndCnsmpn12Qty` | `MnllyCrrtdUnplndCnsmpn12Qty` | `Decimal(13,3)` |  | Corr.unpl.cons. 12 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `MnllyCrrtdUnplndCnsmpn13Qty` | `MnllyCrrtdUnplndCnsmpn13Qty` | `Decimal(13,3)` |  | Corr.unpl.cons. 13 | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `BaseUnit` | `BaseUnit` | `String(3)` |  | Base Unit of Measure |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `ProductDescription`

- **ABAP Name:** `I_ProductDescription_2`
- **Label:** Product Descriptions
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Product` | `Product` | `String(40)` | Y | Product |  |  | S/4 only entity (no ECC CDC mapping) |
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductDescription` | `ProductDescription` | `String(40)` |  | Product Description |  |  | S/4 only entity (no ECC CDC mapping) |
| `LanguageISOCode` | `LanguageISOCode` | `String(2)` |  | Language |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `ProductGroup`

- **ABAP Name:** `I_ProductGroup_2`
- **Label:** Product Group
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `ProductGroup` | `ProductGroup` | `String(9)` | Y | Product Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `AuthorizationGroup` | `AuthorizationGroup` | `String(4)` |  | Authorization Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValuationClass` | `ValuationClass` | `String(4)` |  | Valuation Class |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchasingAcknProfile` | `PurchasingAcknProfile` | `String(4)` |  | Purchasing value key |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `ProductGroupText`

- **ABAP Name:** `I_ProductGroupText_2`
- **Label:** Product Group - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `ProductGroup` | `ProductGroup` | `String(9)` | Y | Product Group |  | _ProductGroup | S/4 only entity (no ECC CDC mapping) |
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductGroupName` | `ProductGroupName` | `String(20)` |  | Product Group Description |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductGroupText` | `ProductGroupText` | `String(60)` |  | Mat.Grp Desc. 2 |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `ProductMRPArea`

- **ABAP Name:** `I_ProductMRPArea`
- **Label:** MRP Area Details of a Product
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Product` | `Product` | `String(40)` | Y | Product |  | _Product | S/4 only entity (no ECC CDC mapping) |
| `MRPArea` | `MRPArea` | `String(10)` | Y | MRP Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `MRPPlant` | `MRPPlant` | `String(4)` |  | MRP Area Plant |  |  | S/4 only entity (no ECC CDC mapping) |
| `MRPGroup` | `MRPGroup` | `String(4)` |  | MRP Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `MRPType` | `MRPType` | `String(2)` |  | MRP Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `MRPController` | `MRPController` | `String(3)` |  | MRP Controller |  |  | S/4 only entity (no ECC CDC mapping) |
| `MRPProfile` | `MRPProfile` | `String(4)` |  | MRP Profile |  |  | S/4 only entity (no ECC CDC mapping) |
| `LotSizingProcedure` | `LotSizingProcedure` | `String(2)` |  | Lot Sizing Procedure |  |  | S/4 only entity (no ECC CDC mapping) |
| `MRPPlanningCalendar` | `MRPPlanningCalendar` | `String(3)` |  | Planning Calendar |  |  | S/4 only entity (no ECC CDC mapping) |
| `MRPPlanningCycle` | `MRPPlanningCycle` | `String(3)` |  | Planning Cycle |  |  | S/4 only entity (no ECC CDC mapping) |
| `MRPSafetyStockMethod` | `MRPSafetyStockMethod` | `String(2)` |  | Safety Stock Method |  |  | S/4 only entity (no ECC CDC mapping) |
| `MaterialProcurementProfile` | `MaterialProcurementProfile` | `String(2)` |  | Procurement Profile |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductionStorageLocation` | `ProductionStorageLocation` | `String(4)` |  | Production Storage Location |  |  | S/4 only entity (no ECC CDC mapping) |
| `DfltStorLocForExtProcmt` | `DfltStorLocForExtProcmt` | `String(4)` |  | External Procurement Storage Location |  |  | S/4 only entity (no ECC CDC mapping) |
| `RangeOfCoverageProfile` | `RangeOfCoverageProfile` | `String(3)` |  | Range-of-Coverage Profile |  |  | S/4 only entity (no ECC CDC mapping) |
| `SafetyTimePeriodProfile` | `SafetyTimePeriodProfile` | `String(3)` |  | Period Profile for Safety Time |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductSafetyTimeMRPRelevance` | `ProductSafetyTimeMRPRelevance` | `String(1)` |  | Safety Time MRP Relevance |  |  | S/4 only entity (no ECC CDC mapping) |
| `DependentRqmtMRPRelevance` | `DependentRqmtMRPRelevance` | `String(1)` |  | Dependent Requirements MRP Relevance |  |  | S/4 only entity (no ECC CDC mapping) |
| `StorageCostsPercentageCode` | `StorageCostsPercentageCode` | `String(1)` |  | Storage Costs Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `RoundingProfile` | `RoundingProfile` | `String(4)` |  | Rounding Profile |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsMarkedForDeletion` | `IsMarkedForDeletion` | `Boolean` |  | Deletion Indicator |  |  | S/4 only entity (no ECC CDC mapping) |
| `LastChangedByUser` | `LastChangedByUser` | `String(12)` |  | Changed By |  |  | S/4 only entity (no ECC CDC mapping) |
| `LastChangeDate` | `LastChangeDate` | `Date` |  | Changed On |  |  | S/4 only entity (no ECC CDC mapping) |
| `LastChangeTime` | `LastChangeTime` | `String(6)` |  | Time of Change |  |  | S/4 only entity (no ECC CDC mapping) |
| `PlannedDeliveryDurationInDays` | `PlannedDeliveryDurationInDays` | `Decimal(3,0)` |  | Planned Deliv. Time |  |  | S/4 only entity (no ECC CDC mapping) |
| `PlanningTimeFenceInDays` | `PlanningTimeFenceInDays` | `String(3)` |  | Planning Time Fence |  |  | S/4 only entity (no ECC CDC mapping) |
| `RqmtQtyRcptTaktTmeInWrkgDays` | `RqmtQtyRcptTaktTmeInWrkgDays` | `Decimal(3,0)` |  | Takt time |  |  | S/4 only entity (no ECC CDC mapping) |
| `AssemblyScrapPercent` | `AssemblyScrapPercent` | `Decimal(5,2)` |  | Assembly scrap (%) |  |  | S/4 only entity (no ECC CDC mapping) |
| `BaseUnit` | `BaseUnit` | `String(3)` |  | Base Unit of Measure |  |  | S/4 only entity (no ECC CDC mapping) |
| `MinimumLotSizeQuantity` | `MinimumLotSizeQuantity` | `Decimal(13,3)` |  | Minimum Lot Size | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `MaximumLotSizeQuantity` | `MaximumLotSizeQuantity` | `Decimal(13,3)` |  | Maximum Lot Size | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `MaterialMaxStockLevelQuantity` | `MaterialMaxStockLevelQuantity` | `Decimal(13,3)` |  | Maximum Stock Level | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `SafetyStockQuantity` | `SafetyStockQuantity` | `Decimal(13,3)` |  | Safety Stock | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `LotSizeRoundingQuantity` | `LotSizeRoundingQuantity` | `Decimal(13,3)` |  | Rounding Quantity | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `ReorderThresholdQuantity` | `ReorderThresholdQuantity` | `Decimal(13,3)` |  | Reorder Point | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `ProductPlant`

- **ABAP Name:** `I_ProductPlantBasic`
- **Label:** Product Plant
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Product` | `Product` | `String(40)` | Y | Product |  |  | S/4 only entity (no ECC CDC mapping) |
| `Plant` | `Plant` | `String(4)` | Y | Plant |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchasingGroup` | `PurchasingGroup` | `String(3)` |  | Purchasing Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `CountryOfOrigin` | `CountryOfOrigin` | `String(3)` |  | Country/Region of Origin |  |  | S/4 only entity (no ECC CDC mapping) |
| `RegionOfOrigin` | `RegionOfOrigin` | `String(3)` |  | Region of Origin |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductionInvtryManagedLoc` | `ProductionInvtryManagedLoc` | `String(4)` |  | Storage Location |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProfileCode` | `ProfileCode` | `String(2)` |  | Material Status |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProfileValidityStartDate` | `ProfileValidityStartDate` | `Date` |  | Valid From |  |  | S/4 only entity (no ECC CDC mapping) |
| `AvailabilityCheckType` | `AvailabilityCheckType` | `String(2)` |  | Availability check |  |  | S/4 only entity (no ECC CDC mapping) |
| `FiscalYearVariant` | `FiscalYearVariant` | `String(2)` |  | Fiscal Year Variant |  |  | S/4 only entity (no ECC CDC mapping) |
| `PeriodType` | `PeriodType` | `String(1)` |  | Period Indicator |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProfitCenter` | `ProfitCenter` | `String(10)` |  | Profit Center |  |  | S/4 only entity (no ECC CDC mapping) |
| `GoodsReceiptDuration` | `GoodsReceiptDuration` | `Decimal(3,0)` |  | GR processing time |  |  | S/4 only entity (no ECC CDC mapping) |
| `MaintenanceStatusName` | `MaintenanceStatusName` | `String(15)` |  | Maintenance Status |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsMarkedForDeletion` | `IsMarkedForDeletion` | `Boolean` |  | DF at plant level |  |  | S/4 only entity (no ECC CDC mapping) |
| `MRPType` | `MRPType` | `String(2)` |  | MRP Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `MRPResponsible` | `MRPResponsible` | `String(3)` |  | MRP Controller |  |  | S/4 only entity (no ECC CDC mapping) |
| `ABCIndicator` | `ABCIndicator` | `String(1)` |  | ABC Indicator |  |  | S/4 only entity (no ECC CDC mapping) |
| `MinimumLotSizeQuantity` | `MinimumLotSizeQuantity` | `Decimal(13,3)` |  | Minimum Lot Size | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `MaximumLotSizeQuantity` | `MaximumLotSizeQuantity` | `Decimal(13,3)` |  | Maximum Lot Size | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `FixedLotSizeQuantity` | `FixedLotSizeQuantity` | `Decimal(13,3)` |  | Fixed lot size | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `ConsumptionTaxCtrlCode` | `ConsumptionTaxCtrlCode` | `String(16)` |  | Control Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsCoProduct` | `IsCoProduct` | `Boolean` |  | Co-Product |  |  | S/4 only entity (no ECC CDC mapping) |
| `ConfigurableProduct` | `ConfigurableProduct` | `String(40)` |  | Conf. Material |  | _ConfigurableProduct | S/4 only entity (no ECC CDC mapping) |
| `StockDeterminationGroup` | `StockDeterminationGroup` | `String(4)` |  | Stock Determ. Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `HasPostToInspectionStock` | `HasPostToInspectionStock` | `Boolean` |  | Post to insp. stock |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsBatchManagementRequired` | `IsBatchManagementRequired` | `Boolean` |  | Batch Mgmt Rqt(Plnt) |  |  | S/4 only entity (no ECC CDC mapping) |
| `SerialNumberProfile` | `SerialNumberProfile` | `String(4)` |  | Serial No. Profile |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsNegativeStockAllowed` | `IsNegativeStockAllowed` | `Boolean` |  | Neg. Stocks In Plant |  |  | S/4 only entity (no ECC CDC mapping) |
| `HasConsignmentCtrl` | `HasConsignmentCtrl` | `String(1)` |  | Consign.Control |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsPurgAcrossPurgGroup` | `IsPurgAcrossPurgGroup` | `Boolean` |  | Across Purch.Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsInternalBatchManaged` | `IsInternalBatchManaged` | `Boolean` |  | Batch Management |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductCFOPCategory` | `ProductCFOPCategory` | `String(2)` |  | Matl. CFOP Category |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductIsExciseTaxRelevant` | `ProductIsExciseTaxRelevant` | `Boolean` |  | Is Excise Tax Relevant |  |  | S/4 only entity (no ECC CDC mapping) |
| `UnderDelivToleranceLimit` | `UnderDelivToleranceLimit` | `Decimal(3,1)` |  | Underdelivery Toler. |  |  | S/4 only entity (no ECC CDC mapping) |
| `OverDelivToleranceLimit` | `OverDelivToleranceLimit` | `Decimal(3,1)` |  | Overdelivery Toler. |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProcurementType` | `ProcurementType` | `String(1)` |  | Procurement Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `SpecialProcurementType` | `SpecialProcurementType` | `String(2)` |  | Special Procurement |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductionSchedulingProfile` | `ProductionSchedulingProfile` | `String(6)` |  | Production Scheduling Profile |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductionSupervisor` | `ProductionSupervisor` | `String(3)` |  | Prodn Supervisor |  |  | S/4 only entity (no ECC CDC mapping) |
| `SafetyStockQuantity` | `SafetyStockQuantity` | `Decimal(13,3)` |  | Safety Stock | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `GoodsIssueUnit` | `GoodsIssueUnit` | `String(3)` |  | Unit of Issue |  |  | S/4 only entity (no ECC CDC mapping) |
| `SourceOfSupplyCategory` | `SourceOfSupplyCategory` | `String(1)` |  | Source of supply |  |  | S/4 only entity (no ECC CDC mapping) |
| `ConsumptionReferenceProduct` | `ConsumptionReferenceProduct` | `String(40)` |  | RefMatl: consumption |  |  | S/4 only entity (no ECC CDC mapping) |
| `ConsumptionReferencePlant` | `ConsumptionReferencePlant` | `String(4)` |  | RefPlant:consumption |  |  | S/4 only entity (no ECC CDC mapping) |
| `ConsumptionRefUsageEndDate` | `ConsumptionRefUsageEndDate` | `Date` |  | Date to |  |  | S/4 only entity (no ECC CDC mapping) |
| `ConsumptionQtyMultiplier` | `ConsumptionQtyMultiplier` | `Decimal(4,2)` |  | Multiplier |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductUnitGroup` | `ProductUnitGroup` | `String(4)` |  | Unit of Measure Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `DistrCntrDistributionProfile` | `DistrCntrDistributionProfile` | `String(3)` |  | Distr. profile |  |  | S/4 only entity (no ECC CDC mapping) |
| `ConsignmentControl` | `ConsignmentControl` | `String(1)` |  | Consign.Control |  |  | S/4 only entity (no ECC CDC mapping) |
| `GoodIssueProcessingDays` | `GoodIssueProcessingDays` | `Decimal(3,0)` |  | GI Proc. Time |  |  | S/4 only entity (no ECC CDC mapping) |
| `PlannedDeliveryDurationInDays` | `PlannedDeliveryDurationInDays` | `Decimal(3,0)` |  | Planned Deliv. Time |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductIsCriticalPrt` | `ProductIsCriticalPrt` | `Boolean` |  | Critical Part |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductLogisticsHandlingGroup` | `ProductLogisticsHandlingGroup` | `String(4)` |  | Log. handling group |  |  | S/4 only entity (no ECC CDC mapping) |
| `MaterialFreightGroup` | `MaterialFreightGroup` | `String(8)` |  | Material Freight Grp |  |  | S/4 only entity (no ECC CDC mapping) |
| `OriginalBatchReferenceMaterial` | `OriginalBatchReferenceMaterial` | `String(40)` |  | OB Reference Materl |  |  | S/4 only entity (no ECC CDC mapping) |
| `OriglBatchManagementIsRequired` | `OriglBatchManagementIsRequired` | `String(1)` |  | OB Management |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductConfiguration` | `ProductConfiguration` | `String(18)` |  | Internal object no. |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductMinControlTemperature` | `ProductMinControlTemperature` | `Decimal(7,2)` |  | Min. Temperature | ProductControlTemperatureUnit |  | S/4 only entity (no ECC CDC mapping) |
| `ProductMaxControlTemperature` | `ProductMaxControlTemperature` | `Decimal(7,2)` |  | Max. Temperature | ProductControlTemperatureUnit |  | S/4 only entity (no ECC CDC mapping) |
| `ProductControlTemperatureUnit` | `ProductControlTemperatureUnit` | `String(3)` |  | Temperature UoM |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValuationCategory` | `ValuationCategory` | `String(1)` |  | Valuation Category |  |  | S/4 only entity (no ECC CDC mapping) |
| `BaseUnit` | `BaseUnit` | `String(3)` |  | Base Unit of Measure |  |  | S/4 only entity (no ECC CDC mapping) |
| `ItemUniqueIdentifierIsRelevant` | `ItemUniqueIdentifierIsRelevant` | `Boolean` |  | IUID-Relevant |  |  | S/4 only entity (no ECC CDC mapping) |
| `ItemUniqueIdentifierType` | `ItemUniqueIdentifierType` | `String(10)` |  | IUID Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `ExtAllocOfItmUnqIdtIsRelevant` | `ExtAllocOfItmUnqIdtIsRelevant` | `Boolean` |  | Ext. Allocation |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `ProductPlantCosting`

- **ABAP Name:** `I_ProductPlantCosting`
- **Label:** Product Plant Costing
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Product` | `Product` | `String(40)` | Y | Product |  |  | S/4 only entity (no ECC CDC mapping) |
| `Plant` | `Plant` | `String(4)` | Y | Plant |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsCoProduct` | `IsCoProduct` | `Boolean` |  | Co-Product |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostingLotSize` | `CostingLotSize` | `Decimal(13,3)` |  | Costing Lot Size | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `TaskListGroup` | `TaskListGroup` | `String(8)` |  | Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `TaskListType` | `TaskListType` | `String(1)` |  | Task List Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostingSpecialProcurementType` | `CostingSpecialProcurementType` | `String(2)` |  | Special Procurement Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `SourceBOMAlternative` | `SourceBOMAlternative` | `String(2)` |  | Alternative BOM |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductBOMUsage` | `ProductBOMUsage` | `String(1)` |  | BOM Usage |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductIsCostingRelevant` | `ProductIsCostingRelevant` | `Boolean` |  | Do Not Cost |  |  | S/4 only entity (no ECC CDC mapping) |
| `TaskListGroupCounter` | `TaskListGroupCounter` | `String(2)` |  | Group Counter |  |  | S/4 only entity (no ECC CDC mapping) |
| `VarianceKey` | `VarianceKey` | `String(6)` |  | Variance Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostingProductionVersion` | `CostingProductionVersion` | `String(4)` |  | Production Version |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsFixedPriceCoProduct` | `IsFixedPriceCoProduct` | `Boolean` |  | Fixed-Price Co-Prod. |  |  | S/4 only entity (no ECC CDC mapping) |
| `BaseUnit` | `BaseUnit` | `String(3)` |  | Base Unit of Measure |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `ProductPlantForecast`

- **ABAP Name:** `I_ProductPlantForecast`
- **Label:** Product Plant Forecast
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Product` | `Product` | `String(40)` | Y | Product |  |  | S/4 only entity (no ECC CDC mapping) |
| `Plant` | `Plant` | `String(4)` | Y | Plant |  |  | S/4 only entity (no ECC CDC mapping) |
| `ConsumptionRefUsageEndDate` | `ConsumptionRefUsageEndDate` | `Date` |  | Date to |  |  | S/4 only entity (no ECC CDC mapping) |
| `ConsumptionQtyMultiplier` | `ConsumptionQtyMultiplier` | `Decimal(4,2)` |  | Multiplier |  |  | S/4 only entity (no ECC CDC mapping) |
| `ConsumptionReferenceProduct` | `ConsumptionReferenceProduct` | `String(40)` |  | RefMatl: consumption |  | _ConsumptionReferenceProduct | S/4 only entity (no ECC CDC mapping) |
| `ConsumptionReferencePlant` | `ConsumptionReferencePlant` | `String(4)` |  | RefPlant:consumption |  |  | S/4 only entity (no ECC CDC mapping) |
| `CorrectionFactorIsRequired` | `CorrectionFactorIsRequired` | `Boolean` |  | Correction factors |  |  | S/4 only entity (no ECC CDC mapping) |
| `ForecastModelIsReset` | `ForecastModelIsReset` | `Boolean` |  | Reset automatically |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `ProductPlantInternationalTrade`

- **ABAP Name:** `I_ProductPlantIntlTrd`
- **Label:** Product Plant Intrntionl Trade
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Product` | `Product` | `String(40)` | Y | Product |  |  | S/4 only entity (no ECC CDC mapping) |
| `Plant` | `Plant` | `String(4)` | Y | Plant |  |  | S/4 only entity (no ECC CDC mapping) |
| `CountryOfOrigin` | `CountryOfOrigin` | `String(3)` |  | Country/Region of Origin |  |  | S/4 only entity (no ECC CDC mapping) |
| `RegionOfOrigin` | `RegionOfOrigin` | `String(3)` |  | Region of Origin |  |  | S/4 only entity (no ECC CDC mapping) |
| `ConsumptionTaxCtrlCode` | `ConsumptionTaxCtrlCode` | `String(16)` |  | Control Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `ExportAndImportProductGroup` | `ExportAndImportProductGroup` | `String(4)` |  | Intrastat Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductCASNumber` | `ProductCASNumber` | `String(15)` |  | CAS number (pharm.) |  |  | S/4 only entity (no ECC CDC mapping) |
| `CommoditiyCodeNumberUnit` | `CommoditiyCodeNumberUnit` | `String(3)` |  | Commodity code unit |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProdIntlTradeClassification` | `ProdIntlTradeClassification` | `String(9)` |  | PRODCOM no. |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `ProductPlantProcurement`

- **ABAP Name:** `I_Productplantprocurement`
- **Label:** Product Plant Procurement
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Product` | `Product` | `String(40)` | Y | Product |  |  | S/4 only entity (no ECC CDC mapping) |
| `Plant` | `Plant` | `String(4)` | Y | Plant |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsAutoPurOrdCreationAllowed` | `IsAutoPurOrdCreationAllowed` | `Boolean` |  | Automatic PO |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsSourceListRequired` | `IsSourceListRequired` | `Boolean` |  | Source list |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsPurgAcrossPurgGroup` | `IsPurgAcrossPurgGroup` | `Boolean` |  | Across Purch.Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `SourceOfSupplyCategory` | `SourceOfSupplyCategory` | `String(1)` |  | Source of supply |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchasingGroup` | `PurchasingGroup` | `String(3)` |  | Purchasing Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsActiveEntity` | `IsActiveEntity` | `Boolean` |  | Is active |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProposedProductSupplyArea` | `ProposedProductSupplyArea` | `String(10)` |  | Proposed Supply Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `ItmIsRlvtToJITDelivSchedules` | `ItmIsRlvtToJITDelivSchedules` | `String(1)` |  | JIT Delivery |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `ProductPlantPurchaseTax`

- **ABAP Name:** `I_ProductPurchaseTax`
- **Label:** Product Purchase Tax
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Product` | `Product` | `String(40)` | Y | Product |  | _Product | S/4 only entity (no ECC CDC mapping) |
| `SourceLocationCountry` | `SourceLocationCountry` | `String(3)` | Y | Departure Ctry/Reg. |  |  | S/4 only entity (no ECC CDC mapping) |
| `TaxIndicator` | `TaxIndicator` | `String(1)` |  | Tax ind. f. material |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `ProductPlantQualityManagement`

- **ABAP Name:** `I_Productplantqtmanagement`
- **Label:** Product Plant QM
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Product` | `Product` | `String(40)` | Y | Product |  |  | S/4 only entity (no ECC CDC mapping) |
| `Plant` | `Plant` | `String(4)` | Y | Plant |  |  | S/4 only entity (no ECC CDC mapping) |
| `MaximumStoragePeriod` | `MaximumStoragePeriod` | `Decimal(5,0)` |  | Max. Storage Period |  |  | S/4 only entity (no ECC CDC mapping) |
| `QualityMgmtCtrlKey` | `QualityMgmtCtrlKey` | `String(8)` |  | QM Control Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `MatlQualityAuthorizationGroup` | `MatlQualityAuthorizationGroup` | `String(6)` |  | QM Material Auth. |  |  | S/4 only entity (no ECC CDC mapping) |
| `HasPostToInspectionStock` | `HasPostToInspectionStock` | `Boolean` |  | Post to insp. stock |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsActiveEntity` | `IsActiveEntity` | `Boolean` |  | Is active |  |  | S/4 only entity (no ECC CDC mapping) |
| `InspLotDocumentationIsRequired` | `InspLotDocumentationIsRequired` | `Boolean` |  | Documentation reqd |  |  | S/4 only entity (no ECC CDC mapping) |
| `SuplrQualityManagementSystem` | `SuplrQualityManagementSystem` | `String(4)` |  | Target QM System |  |  | S/4 only entity (no ECC CDC mapping) |
| `RecrrgInspIntervalTimeInDays` | `RecrrgInspIntervalTimeInDays` | `Decimal(5,0)` |  | Inspection Interval |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductQualityCertificateType` | `ProductQualityCertificateType` | `String(4)` |  | Certificate Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductPlantHasInspectionSetup` | `ProductPlantHasInspectionSetup` | `Boolean` |  | Inspection Setup |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `ProductPlantStorage`

- **ABAP Name:** `I_Productplantstorage`
- **Label:** Product plant storage
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Product` | `Product` | `String(40)` | Y | Product |  |  | S/4 only entity (no ECC CDC mapping) |
| `Plant` | `Plant` | `String(4)` | Y | Plant |  |  | S/4 only entity (no ECC CDC mapping) |
| `InventoryForCycleCountInd` | `InventoryForCycleCountInd` | `String(1)` |  | CC Phys. Inv. Ind. |  |  | S/4 only entity (no ECC CDC mapping) |
| `MaximumStoragePeriod` | `MaximumStoragePeriod` | `Decimal(5,0)` |  | Max. Storage Period |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProvisioningServiceLevel` | `ProvisioningServiceLevel` | `String(1)` |  | Service Level |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsActiveEntity` | `IsActiveEntity` | `Boolean` |  | Is active |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProdMaximumStoragePeriodUnit` | `ProdMaximumStoragePeriodUnit` | `String(3)` |  | Time unit |  |  | S/4 only entity (no ECC CDC mapping) |
| `WrhsMgmtPtwyAndStkRemovalStrgy` | `WrhsMgmtPtwyAndStkRemovalStrgy` | `String(1)` |  | Putaway/StkRmvl |  |  | S/4 only entity (no ECC CDC mapping) |
| `CycleCountingIndicatorIsFixed` | `CycleCountingIndicatorIsFixed` | `Boolean` |  | CC indicator fixed |  |  | S/4 only entity (no ECC CDC mapping) |
| `SegmentationStrategyForPlant` | `SegmentationStrategyForPlant` | `String(8)` |  | Segment. Strategy |  |  | S/4 only entity (no ECC CDC mapping) |
| `DefaultSegmentValue` | `DefaultSegmentValue` | `String(40)` |  | Stock Segment |  |  | S/4 only entity (no ECC CDC mapping) |
| `SgmtHasPrioInProductStockSort` | `SgmtHasPrioInProductStockSort` | `Boolean` |  | Sort Stock |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `ProductPlantSupplyPlanning`

- **ABAP Name:** `I_ProductPlantSupplyPlanning`
- **Label:** Product Plant Supply Planning
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Product` | `Product` | `String(40)` | Y | Product |  | _Product | S/4 only entity (no ECC CDC mapping) |
| `Plant` | `Plant` | `String(4)` | Y | Plant |  |  | S/4 only entity (no ECC CDC mapping) |
| `FixedLotSizeQuantity` | `FixedLotSizeQuantity` | `Decimal(13,3)` |  | Fixed lot size | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `MaximumLotSizeQuantity` | `MaximumLotSizeQuantity` | `Decimal(13,3)` |  | Maximum Lot Size | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `MinimumLotSizeQuantity` | `MinimumLotSizeQuantity` | `Decimal(13,3)` |  | Minimum Lot Size | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `LotSizeRoundingQuantity` | `LotSizeRoundingQuantity` | `Decimal(13,3)` |  | Rounding value | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `LotSizingProcedure` | `LotSizingProcedure` | `String(2)` |  | Lot Sizing Procedure |  |  | S/4 only entity (no ECC CDC mapping) |
| `MRPType` | `MRPType` | `String(2)` |  | MRP Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `MRPResponsible` | `MRPResponsible` | `String(3)` |  | MRP Controller |  |  | S/4 only entity (no ECC CDC mapping) |
| `SafetyStockQuantity` | `SafetyStockQuantity` | `Decimal(13,3)` |  | Safety Stock | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `MinimumSafetyStockQuantity` | `MinimumSafetyStockQuantity` | `Decimal(13,3)` |  | Min. Saf. Stock | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `PlanningTimeFence` | `PlanningTimeFence` | `String(3)` |  | Planning time fence |  |  | S/4 only entity (no ECC CDC mapping) |
| `ConsumptionValueCategory` | `ConsumptionValueCategory` | `String(1)` |  | ABC Indicator |  |  | S/4 only entity (no ECC CDC mapping) |
| `MaximumStockQuantity` | `MaximumStockQuantity` | `Decimal(13,3)` |  | Maximum Stock Level | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `ReorderThresholdQuantity` | `ReorderThresholdQuantity` | `Decimal(13,3)` |  | Reorder Point | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `PlannedDeliveryDurationInDays` | `PlannedDeliveryDurationInDays` | `Decimal(3,0)` |  | Planned Deliv. Time |  |  | S/4 only entity (no ECC CDC mapping) |
| `SafetySupplyDurationInDays` | `SafetySupplyDurationInDays` | `String(2)` |  | Safety Time |  |  | S/4 only entity (no ECC CDC mapping) |
| `PlanningStrategyGroup` | `PlanningStrategyGroup` | `String(2)` |  | Strategy Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `TotalReplenishmentLeadTime` | `TotalReplenishmentLeadTime` | `Decimal(3,0)` |  | Tot. repl. lead time |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProcurementType` | `ProcurementType` | `String(1)` |  | Procurement Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProcurementSubType` | `ProcurementSubType` | `String(2)` |  | Special Procurement |  |  | S/4 only entity (no ECC CDC mapping) |
| `AssemblyScrapPercent` | `AssemblyScrapPercent` | `Decimal(5,2)` |  | Assembly scrap (%) |  |  | S/4 only entity (no ECC CDC mapping) |
| `AvailabilityCheckType` | `AvailabilityCheckType` | `String(2)` |  | Availability check |  |  | S/4 only entity (no ECC CDC mapping) |
| `GoodsReceiptDuration` | `GoodsReceiptDuration` | `Decimal(3,0)` |  | GR processing time |  |  | S/4 only entity (no ECC CDC mapping) |
| `PlanAndOrderDayDetermination` | `PlanAndOrderDayDetermination` | `String(3)` |  | Planning Cycle |  |  | S/4 only entity (no ECC CDC mapping) |
| `RoundingProfile` | `RoundingProfile` | `String(4)` |  | Rounding Profile |  |  | S/4 only entity (no ECC CDC mapping) |
| `DfltStorageLocationExtProcmt` | `DfltStorageLocationExtProcmt` | `String(4)` |  | Storage Location |  |  | S/4 only entity (no ECC CDC mapping) |
| `GoodIssueProcessingDays` | `GoodIssueProcessingDays` | `Decimal(3,0)` |  | GI Proc. Time |  |  | S/4 only entity (no ECC CDC mapping) |
| `ConsignmentControl` | `ConsignmentControl` | `String(1)` |  | Consign.Control |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsActiveEntity` | `IsActiveEntity` | `Boolean` |  | Is active |  |  | S/4 only entity (no ECC CDC mapping) |
| `MRPGroup` | `MRPGroup` | `String(4)` |  | MRP Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `LotSizeIndependentCosts` | `LotSizeIndependentCosts` | `Decimal(34,4)` |  | LS-Independent Costs | Currency |  | S/4 only entity (no ECC CDC mapping) |
| `StorageCostsPercentageCode` | `StorageCostsPercentageCode` | `String(1)` |  | Storage Costs Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `RqmtQtyRcptTaktTmeInWrkgDays` | `RqmtQtyRcptTaktTmeInWrkgDays` | `Decimal(3,0)` |  | Takt time |  |  | S/4 only entity (no ECC CDC mapping) |
| `MRPPlanningCalendar` | `MRPPlanningCalendar` | `String(3)` |  | Planning Calendar |  |  | S/4 only entity (no ECC CDC mapping) |
| `RangeOfCvrgPrflCode` | `RangeOfCvrgPrflCode` | `String(3)` |  | Coverage Profile |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductSafetyTimeMRPRelevance` | `ProductSafetyTimeMRPRelevance` | `String(1)` |  | Safety Time Ind |  |  | S/4 only entity (no ECC CDC mapping) |
| `SafetyTimePeriodProfile` | `SafetyTimePeriodProfile` | `String(3)` |  | Time Profile |  |  | S/4 only entity (no ECC CDC mapping) |
| `DependentRqmtMRPRelevance` | `DependentRqmtMRPRelevance` | `String(1)` |  | MRP Relevant |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductServiceLevelInPercent` | `ProductServiceLevelInPercent` | `Decimal(3,1)` |  | Service level (%) |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProdInhProdnDurationInWorkDays` | `ProdInhProdnDurationInWorkDays` | `Decimal(3,0)` |  | In-house production |  |  | S/4 only entity (no ECC CDC mapping) |
| `MRPAvailabilityType` | `MRPAvailabilityType` | `String(1)` |  | Mixed MRP |  |  | S/4 only entity (no ECC CDC mapping) |
| `CrossProjectProduct` | `CrossProjectProduct` | `String(1)` |  | Cross-Project |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProdnPlngAndControlCalendar` | `ProdnPlngAndControlCalendar` | `String(3)` |  | Planning Calendar |  |  | S/4 only entity (no ECC CDC mapping) |
| `FollowUpProduct` | `FollowUpProduct` | `String(40)` |  | Follow-Up Material |  |  | S/4 only entity (no ECC CDC mapping) |
| `RepetitiveManufacturingIsAllwd` | `RepetitiveManufacturingIsAllwd` | `Boolean` |  | Repetitive Manufacturing Enabled |  |  | S/4 only entity (no ECC CDC mapping) |
| `DependentRequirementsType` | `DependentRequirementsType` | `String(1)` |  | Indiv./ Coll. |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductIsBulkComponent` | `ProductIsBulkComponent` | `Boolean` |  | Bulk Material |  |  | S/4 only entity (no ECC CDC mapping) |
| `RepetitiveManufacturingProfile` | `RepetitiveManufacturingProfile` | `String(4)` |  | Repetitive Manufacturing Profile |  |  | S/4 only entity (no ECC CDC mapping) |
| `BackwardCnsmpnPeriodInWorkDays` | `BackwardCnsmpnPeriodInWorkDays` | `String(3)` |  | Backward Consumption Period |  |  | S/4 only entity (no ECC CDC mapping) |
| `FwdConsumptionPeriodInWorkDays` | `FwdConsumptionPeriodInWorkDays` | `String(3)` |  | Forward Consumption Period |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProdRqmtsConsumptionMode` | `ProdRqmtsConsumptionMode` | `String(1)` |  | Consumption mode |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProdFcstRequirementsSplitCode` | `ProdFcstRequirementsSplitCode` | `String(1)` |  | Splitting Indicator |  |  | S/4 only entity (no ECC CDC mapping) |
| `EffectiveOutDate` | `EffectiveOutDate` | `Date` |  | Effective-Out Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `MRPProfile` | `MRPProfile` | `String(4)` |  | MRP profile |  |  | S/4 only entity (no ECC CDC mapping) |
| `SchedulingFloatProfile` | `SchedulingFloatProfile` | `String(3)` |  | Scheduling Float Profile |  |  | S/4 only entity (no ECC CDC mapping) |
| `ComponentScrapInPercent` | `ComponentScrapInPercent` | `Decimal(5,2)` |  | Component Scrap (%) |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductDiscontinuationCode` | `ProductDiscontinuationCode` | `String(1)` |  | Discontinuation ind. |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductRequirementsGrouping` | `ProductRequirementsGrouping` | `String(1)` |  | Requirements group |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductionInvtryManagedLoc` | `ProductionInvtryManagedLoc` | `String(4)` |  | Storage Location |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductComponentBackflushCode` | `ProductComponentBackflushCode` | `String(1)` |  | Backflush |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProposedProductSupplyArea` | `ProposedProductSupplyArea` | `String(10)` |  | Proposed Supply Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `PlannedOrderActionControl` | `PlannedOrderActionControl` | `String(2)` |  | Action Control |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductUnitGroup` | `ProductUnitGroup` | `String(4)` |  | Unit of Measure Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `MRPSafetyStockMethod` | `MRPSafetyStockMethod` | `String(2)` |  | Safety Stock Method |  |  | S/4 only entity (no ECC CDC mapping) |
| `JITProdnConfProfile` | `JITProdnConfProfile` | `String(4)` |  | JIT Production Confirmation Profile |  |  | S/4 only entity (no ECC CDC mapping) |
| `Currency` | `Currency` | `String(5)` |  | Currency |  |  | S/4 only entity (no ECC CDC mapping) |
| `CompanyCode` | `CompanyCode` | `String(4)` |  | Company Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValuationArea` | `ValuationArea` | `String(4)` |  | Valuation Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `BaseUnit` | `BaseUnit` | `String(3)` |  | Base Unit of Measure |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `ProductPlantWorkScheduling`

- **ABAP Name:** `I_ProductWorkScheduling`
- **Label:** Product WorkScheduling core entity
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Product` | `Product` | `String(40)` | Y | Product |  |  | S/4 only entity (no ECC CDC mapping) |
| `Plant` | `Plant` | `String(4)` | Y | Plant |  |  | S/4 only entity (no ECC CDC mapping) |
| `MaterialBaseQuantity` | `MaterialBaseQuantity` | `Decimal(13,3)` |  | Base quantity | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `UnlimitedOverDelivIsAllowed` | `UnlimitedOverDelivIsAllowed` | `Boolean` |  | Unltd Overdelivery |  |  | S/4 only entity (no ECC CDC mapping) |
| `OverDelivToleranceLimit` | `OverDelivToleranceLimit` | `Decimal(3,1)` |  | Overdelivery Toler. |  |  | S/4 only entity (no ECC CDC mapping) |
| `UnderDelivToleranceLimit` | `UnderDelivToleranceLimit` | `Decimal(3,1)` |  | Underdelivery Toler. |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductionInvtryManagedLoc` | `ProductionInvtryManagedLoc` | `String(4)` |  | Storage Location |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsActiveEntity` | `IsActiveEntity` | `Boolean` |  | Is active |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProdnOrderIsBatchRequired` | `ProdnOrderIsBatchRequired` | `String(1)` |  | Batch entry |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProdIsWithdrawnFrmProdnBin` | `ProdIsWithdrawnFrmProdnBin` | `Boolean` |  | Withdr.from prod.bin |  |  | S/4 only entity (no ECC CDC mapping) |
| `TransitionMatrixProductsGroup` | `TransitionMatrixProductsGroup` | `String(20)` |  | Material Grouping |  |  | S/4 only entity (no ECC CDC mapping) |
| `OrderChangeManagementProfile` | `OrderChangeManagementProfile` | `String(6)` |  | Change overall prof. |  |  | S/4 only entity (no ECC CDC mapping) |
| `MatlCompIsMarkedForBackflush` | `MatlCompIsMarkedForBackflush` | `String(1)` |  | Backflush |  |  | S/4 only entity (no ECC CDC mapping) |
| `SetupAndTeardownTime` | `SetupAndTeardownTime` | `Decimal(5,2)` |  | Setup time |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductionSchedulingProfile` | `ProductionSchedulingProfile` | `String(6)` |  | Production Scheduling Profile |  |  | S/4 only entity (no ECC CDC mapping) |
| `TransitionTime` | `TransitionTime` | `Decimal(5,2)` |  | Interoperation |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProcessingTimeInDays` | `ProcessingTimeInDays` | `Decimal(5,2)` |  | Processing time |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductionSupervisor` | `ProductionSupervisor` | `String(3)` |  | Prodn Supervisor |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductProductionQuantityUnit` | `ProductProductionQuantityUnit` | `String(3)` |  | Production unit |  |  | S/4 only entity (no ECC CDC mapping) |
| `HasProductionVersion` | `HasProductionVersion` | `Boolean` |  | Version Indicator |  |  | S/4 only entity (no ECC CDC mapping) |
| `BaseUnit` | `BaseUnit` | `String(3)` |  | Base Unit of Measure |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `ProductProcurement`

- **ABAP Name:** `I_Productprocurement`
- **Label:** Product Procurement
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Product` | `Product` | `String(40)` | Y | Material |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchaseOrderQuantityUnit` | `PurchaseOrderQuantityUnit` | `String(3)` |  | Order Unit |  |  | S/4 only entity (no ECC CDC mapping) |
| `VarblPurOrdUnitStatus` | `VarblPurOrdUnitStatus` | `String(1)` |  | Var. Order Unit |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchasingAcknProfile` | `PurchasingAcknProfile` | `String(4)` |  | Purchasing value key |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProcurementRule` | `ProcurementRule` | `String(1)` |  | Procurement rule |  |  | S/4 only entity (no ECC CDC mapping) |
| `SourceOfSupplyCategory` | `SourceOfSupplyCategory` | `String(1)` |  | Source of supply |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchasingGroup` | `PurchasingGroup` | `String(3)` |  | Purchasing Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsActiveEntity` | `IsActiveEntity` | `Boolean` |  | Is active |  |  | S/4 only entity (no ECC CDC mapping) |
| `AuthorizationGroup` | `AuthorizationGroup` | `String(4)` |  | Authorization Group |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `ProductQualityManagement`

- **ABAP Name:** `I_Productqm`
- **Label:** Product QM active core entity
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Product` | `Product` | `String(40)` | Y | Product |  |  | S/4 only entity (no ECC CDC mapping) |
| `QltyMgmtInProcmtIsActive` | `QltyMgmtInProcmtIsActive` | `Boolean` |  | QM in Procur. Active |  |  | S/4 only entity (no ECC CDC mapping) |
| `AuthorizationGroup` | `AuthorizationGroup` | `String(4)` |  | Authorization Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `CatalogProfile` | `CatalogProfile` | `String(9)` |  | Catalog Profile |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `ProductSales`

- **ABAP Name:** `I_ProductSales`
- **Label:** Product Sales
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Product` | `Product` | `String(40)` | Y | Material |  |  | S/4 only entity (no ECC CDC mapping) |
| `SalesStatus` | `SalesStatus` | `String(2)` |  | X-DChain Status |  |  | S/4 only entity (no ECC CDC mapping) |
| `SalesStatusValidityDate` | `SalesStatusValidityDate` | `Date` |  | Cross-Distr. Chain Product Validity |  |  | S/4 only entity (no ECC CDC mapping) |
| `TaxClassification` | `TaxClassification` | `String(1)` |  | Tax classification |  |  | S/4 only entity (no ECC CDC mapping) |
| `TransportationGroup` | `TransportationGroup` | `String(4)` |  | Transportation Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `AllowedPackagingWeightQty` | `AllowedPackagingWeightQty` | `Decimal(13,3)` |  | Allowed Pkg wt | AllowedPackagingWeightQtyUnit |  | S/4 only entity (no ECC CDC mapping) |
| `AllowedPackagingWeightQtyUnit` | `AllowedPackagingWeightQtyUnit` | `String(3)` |  | Allowed Packaging Unit of Weight |  |  | S/4 only entity (no ECC CDC mapping) |
| `AllowedPackagingVolumeQty` | `AllowedPackagingVolumeQty` | `Decimal(13,3)` |  | Allowed Volume | AllowedPackagingVolumeQtyUnit |  | S/4 only entity (no ECC CDC mapping) |
| `AllowedPackagingVolumeQtyUnit` | `AllowedPackagingVolumeQtyUnit` | `String(3)` |  | Allowed Packaging Unit of Volume |  |  | S/4 only entity (no ECC CDC mapping) |
| `PricingReferenceProduct` | `PricingReferenceProduct` | `String(40)` |  | Pricing Ref. Matl |  | _PricingReferenceProduct | S/4 only entity (no ECC CDC mapping) |
| `VariantsPricingProfile` | `VariantsPricingProfile` | `String(1)` |  | Pricing profile |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsVariantPriceAllowed` | `IsVariantPriceAllowed` | `Boolean` |  | Var. Price Allowed |  |  | S/4 only entity (no ECC CDC mapping) |
| `LoadingGroup` | `LoadingGroup` | `String(4)` |  | Loading Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsActiveEntity` | `IsActiveEntity` | `Boolean` |  | Is active |  |  | S/4 only entity (no ECC CDC mapping) |
| `ExcessWeightTolerance` | `ExcessWeightTolerance` | `Decimal(3,1)` |  | Excess Weight Tolerance |  |  | S/4 only entity (no ECC CDC mapping) |
| `ExcessVolumeTolerance` | `ExcessVolumeTolerance` | `Decimal(3,1)` |  | Excess Volume Tolerance |  |  | S/4 only entity (no ECC CDC mapping) |
| `PackagingMaterialType` | `PackagingMaterialType` | `String(4)` |  | Packaging Material Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsClosedPackagingMaterial` | `IsClosedPackagingMaterial` | `Boolean` |  | Closed |  |  | S/4 only entity (no ECC CDC mapping) |
| `VolumeMaximumLevel` | `VolumeMaximumLevel` | `Decimal(3,0)` |  | Maximum level |  |  | S/4 only entity (no ECC CDC mapping) |
| `AuthorizationGroup` | `AuthorizationGroup` | `String(4)` |  | Authorization Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `MaterialFreightGroup` | `MaterialFreightGroup` | `String(8)` |  | Material Freight Grp |  |  | S/4 only entity (no ECC CDC mapping) |
| `StackingFactor` | `StackingFactor` | `Integer` |  | Stackability factor |  |  | S/4 only entity (no ECC CDC mapping) |
| `ServiceDuration` | `ServiceDuration` | `Decimal(13,3)` |  | Duration of Work |  |  | S/4 only entity (no ECC CDC mapping) |
| `ServiceDurationUnit` | `ServiceDurationUnit` | `String(3)` |  | Unit |  |  | S/4 only entity (no ECC CDC mapping) |
| `ServiceProfile` | `ServiceProfile` | `String(10)` |  | Service Profile |  |  | S/4 only entity (no ECC CDC mapping) |
| `ResponseProfile` | `ResponseProfile` | `String(10)` |  | Response Prof. |  |  | S/4 only entity (no ECC CDC mapping) |
| `CABillgCycle` | `CABillgCycle` | `String(4)` |  | Billing Cycle |  |  | S/4 only entity (no ECC CDC mapping) |
| `SubscrpnProdBillgCycDetn` | `SubscrpnProdBillgCycDetn` | `String(4)` |  | Billing Cycle Determ |  |  | S/4 only entity (no ECC CDC mapping) |
| `SubscrpnProdTechRsceSchema` | `SubscrpnProdTechRsceSchema` | `String(2)` |  | Assignment Schema |  |  | S/4 only entity (no ECC CDC mapping) |
| `ContractAutoRenewalType` | `ContractAutoRenewalType` | `String(1)` |  | Ctr. Auto Renew Ind. |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `ProductSalesDelivery`

- **ABAP Name:** `I_ProductSalesDelivery`
- **Label:** Product Sales Delivery
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Product` | `Product` | `String(40)` | Y | Product |  | _Product | S/4 only entity (no ECC CDC mapping) |
| `ProductSalesOrg` | `ProductSalesOrg` | `String(4)` | Y | Sales Organization |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductDistributionChnl` | `ProductDistributionChnl` | `String(2)` | Y | Distribution Channel |  |  | S/4 only entity (no ECC CDC mapping) |
| `MinimumOrderQuantity` | `MinimumOrderQuantity` | `Decimal(13,3)` |  | Minimum order qty | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `SupplyingPlant` | `SupplyingPlant` | `String(4)` |  | Delivering Plant |  |  | S/4 only entity (no ECC CDC mapping) |
| `PriceSpecificationProductGroup` | `PriceSpecificationProductGroup` | `String(2)` |  | Product Price Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `AccountDetnProductGroup` | `AccountDetnProductGroup` | `String(2)` |  | Acct Assmt Grp Mat. |  |  | S/4 only entity (no ECC CDC mapping) |
| `DeliveryNoteProcMinDelivQty` | `DeliveryNoteProcMinDelivQty` | `Decimal(13,3)` |  | Minimum Delivery Qty | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `ItemCategoryGroup` | `ItemCategoryGroup` | `String(4)` |  | Item Category Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `DeliveryQuantityUnit` | `DeliveryQuantityUnit` | `String(3)` |  | Unit Of Measure |  |  | S/4 only entity (no ECC CDC mapping) |
| `DeliveryQuantity` | `DeliveryQuantity` | `Decimal(13,3)` |  | Delivery unit | DeliveryQuantityUnit |  | S/4 only entity (no ECC CDC mapping) |
| `ProductSalesStatus` | `ProductSalesStatus` | `String(2)` |  | DChain-spec. status |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductSalesStatusValidityDate` | `ProductSalesStatusValidityDate` | `Date` |  | Valid from |  |  | S/4 only entity (no ECC CDC mapping) |
| `SalesMeasureUnit` | `SalesMeasureUnit` | `String(3)` |  | Sales Unit |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsMarkedForDeletion` | `IsMarkedForDeletion` | `Boolean` |  | DF distr. chain lvl |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductHierarchy` | `ProductHierarchy` | `String(18)` |  | Product Hierarchy |  |  | S/4 only entity (no ECC CDC mapping) |
| `FirstSalesSpecProductGroup` | `FirstSalesSpecProductGroup` | `String(3)` |  | Product Group 1 |  |  | S/4 only entity (no ECC CDC mapping) |
| `SecondSalesSpecProductGroup` | `SecondSalesSpecProductGroup` | `String(3)` |  | Product Group 2 |  |  | S/4 only entity (no ECC CDC mapping) |
| `ThirdSalesSpecProductGroup` | `ThirdSalesSpecProductGroup` | `String(3)` |  | Product Group 3 |  |  | S/4 only entity (no ECC CDC mapping) |
| `FourthSalesSpecProductGroup` | `FourthSalesSpecProductGroup` | `String(3)` |  | Product Group 4 |  |  | S/4 only entity (no ECC CDC mapping) |
| `FifthSalesSpecProductGroup` | `FifthSalesSpecProductGroup` | `String(3)` |  | Product Group 5 |  |  | S/4 only entity (no ECC CDC mapping) |
| `MinimumMakeToOrderOrderQty` | `MinimumMakeToOrderOrderQty` | `Decimal(13,3)` |  | Min. MtO quantity | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `LogisticsStatisticsGroup` | `LogisticsStatisticsGroup` | `String(1)` |  | Matl statistics grp |  |  | S/4 only entity (no ECC CDC mapping) |
| `VolumeRebateGroup` | `VolumeRebateGroup` | `String(2)` |  | Volume Rebate Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductCommissionGroup` | `ProductCommissionGroup` | `String(2)` |  | Commission Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `CashDiscountIsDeductible` | `CashDiscountIsDeductible` | `Boolean` |  | Cash Discount |  |  | S/4 only entity (no ECC CDC mapping) |
| `PricingReferenceProduct` | `PricingReferenceProduct` | `String(40)` |  | Pricing Ref. Matl |  |  | S/4 only entity (no ECC CDC mapping) |
| `AssortmentGrade` | `AssortmentGrade` | `String(2)` |  | Assortment Grade |  |  | S/4 only entity (no ECC CDC mapping) |
| `StoreListingProcedure` | `StoreListingProcedure` | `String(2)` |  | LP for Stores |  |  | S/4 only entity (no ECC CDC mapping) |
| `DistrCntrListingProcedure` | `DistrCntrListingProcedure` | `String(2)` |  | LP distr. ctrs |  |  | S/4 only entity (no ECC CDC mapping) |
| `StoreListingStartDate` | `StoreListingStartDate` | `Date` |  | Store Listed from |  |  | S/4 only entity (no ECC CDC mapping) |
| `StoreListingEndDate` | `StoreListingEndDate` | `Date` |  | Store Listed to |  |  | S/4 only entity (no ECC CDC mapping) |
| `DistrCntrListingStartDate` | `DistrCntrListingStartDate` | `Date` |  | DC Listed from |  |  | S/4 only entity (no ECC CDC mapping) |
| `DistrCntrListingEndDate` | `DistrCntrListingEndDate` | `Date` |  | DC Listed to |  |  | S/4 only entity (no ECC CDC mapping) |
| `StoreSaleStartDate` | `StoreSaleStartDate` | `Date` |  | For sale from (str) |  |  | S/4 only entity (no ECC CDC mapping) |
| `StoreSaleEndDate` | `StoreSaleEndDate` | `Date` |  | For sale till (str) |  |  | S/4 only entity (no ECC CDC mapping) |
| `DistrCntrSaleStartDate` | `DistrCntrSaleStartDate` | `Date` |  | For sale from (DC) |  |  | S/4 only entity (no ECC CDC mapping) |
| `DistrCntrSaleEndDate` | `DistrCntrSaleEndDate` | `Date` |  | For sale till (DC) |  |  | S/4 only entity (no ECC CDC mapping) |
| `RoundingProfile` | `RoundingProfile` | `String(4)` |  | Rounding Profile |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductUnitGroup` | `ProductUnitGroup` | `String(4)` |  | Unit of Measure Grp |  |  | S/4 only entity (no ECC CDC mapping) |
| `MaxDeliveryQtyStoreOrder` | `MaxDeliveryQtyStoreOrder` | `Decimal(13,3)` |  | Max. delivery qty | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `PriceFixingCategory` | `PriceFixingCategory` | `String(1)` |  | Price fixing |  |  | S/4 only entity (no ECC CDC mapping) |
| `VariableSalesUnitIsNotAllowed` | `VariableSalesUnitIsNotAllowed` | `Boolean` |  | Sales unit not var. |  |  | S/4 only entity (no ECC CDC mapping) |
| `CompetitionPressureCategory` | `CompetitionPressureCategory` | `String(1)` |  | Competition charactn |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductHasAttributeID01` | `ProductHasAttributeID01` | `Boolean` |  | Product Attribute 1 |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductHasAttributeID02` | `ProductHasAttributeID02` | `Boolean` |  | Product Attribute 2 |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductHasAttributeID03` | `ProductHasAttributeID03` | `Boolean` |  | Product Attribute 3 |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductHasAttributeID04` | `ProductHasAttributeID04` | `Boolean` |  | Product Attribute 4 |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductHasAttributeID05` | `ProductHasAttributeID05` | `Boolean` |  | Product Attribute 5 |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductHasAttributeID06` | `ProductHasAttributeID06` | `Boolean` |  | Product Attribute 6 |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductHasAttributeID07` | `ProductHasAttributeID07` | `Boolean` |  | Product Attribute 7 |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductHasAttributeID08` | `ProductHasAttributeID08` | `Boolean` |  | Product Attribute 8 |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductHasAttributeID09` | `ProductHasAttributeID09` | `Boolean` |  | Product Attribute 9 |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductHasAttributeID10` | `ProductHasAttributeID10` | `Boolean` |  | Product Attribute 10 |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsActiveEntity` | `IsActiveEntity` | `Boolean` |  | Is active |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProdExtAssortmentPriority` | `ProdExtAssortmentPriority` | `String(1)` |  | Ext. asst priority |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProdIsEntlmntRlvt` | `ProdIsEntlmntRlvt` | `Boolean` |  | Rel. Entitlement Gen |  |  | S/4 only entity (no ECC CDC mapping) |
| `BaseUnit` | `BaseUnit` | `String(3)` |  | Base Unit of Measure |  |  | S/4 only entity (no ECC CDC mapping) |
| `SubscrpnContrDfltDuration` | `SubscrpnContrDfltDuration` | `String(3)` |  | Def Contract Term |  |  | S/4 only entity (no ECC CDC mapping) |
| `SubscrpnContrAltvDuration1` | `SubscrpnContrAltvDuration1` | `String(3)` |  | Contract Term 1 |  |  | S/4 only entity (no ECC CDC mapping) |
| `SubscrpnContrAltvDuration2` | `SubscrpnContrAltvDuration2` | `String(3)` |  | Contract Term 2 |  |  | S/4 only entity (no ECC CDC mapping) |
| `SubscrpnContrDurationUnit` | `SubscrpnContrDurationUnit` | `String(1)` |  | Unit Contract Term |  |  | S/4 only entity (no ECC CDC mapping) |
| `SubscrpnContrDfltExtnDurn` | `SubscrpnContrDfltExtnDurn` | `String(3)` |  | Def Extension Period |  |  | S/4 only entity (no ECC CDC mapping) |
| `SubscrpnContrAltvExtnDurn1` | `SubscrpnContrAltvExtnDurn1` | `String(3)` |  | Extension Period 1 |  |  | S/4 only entity (no ECC CDC mapping) |
| `SubscrpnContrAltvExtnDurn2` | `SubscrpnContrAltvExtnDurn2` | `String(3)` |  | Extension Period 2 |  |  | S/4 only entity (no ECC CDC mapping) |
| `SubscrpnContrExtnDurnUnit` | `SubscrpnContrExtnDurnUnit` | `String(1)` |  | Unit for Extension |  |  | S/4 only entity (no ECC CDC mapping) |
| `LstMiProductPackageSizeCode` | `LstMiProductPackageSizeCode` | `String(3)` |  | Package Size |  |  | S/4 only entity (no ECC CDC mapping) |
| `LstMiProductPackageType` | `LstMiProductPackageType` | `String(3)` |  | Package Type |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `ProductStorage`

- **ABAP Name:** `I_ProductStorage_2`
- **Label:** Product Storage
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Product` | `Product` | `String(40)` | Y | Material |  |  | S/4 only entity (no ECC CDC mapping) |
| `StorageConditions` | `StorageConditions` | `String(2)` |  | Storage conditions |  | _Storagecondition | S/4 only entity (no ECC CDC mapping) |
| `TemperatureConditionInd` | `TemperatureConditionInd` | `String(2)` |  | Temp. conditions |  |  | S/4 only entity (no ECC CDC mapping) |
| `HazardousMaterialNumber` | `HazardousMaterialNumber` | `String(40)` |  | Haz. material number |  |  | S/4 only entity (no ECC CDC mapping) |
| `NmbrOfGROrGISlipsToPrintQty` | `NmbrOfGROrGISlipsToPrintQty` | `Decimal(13,3)` |  | GR slips quantity | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `LabelType` | `LabelType` | `String(2)` |  | Label type |  |  | S/4 only entity (no ECC CDC mapping) |
| `LabelForm` | `LabelForm` | `String(2)` |  | Label form |  |  | S/4 only entity (no ECC CDC mapping) |
| `MinRemainingShelfLife` | `MinRemainingShelfLife` | `Decimal(4,0)` |  | Min. Rem. Shelf Life |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductExpirationDateCode` | `ProductExpirationDateCode` | `String(1)` |  | Expiration Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `StorageBinInstruction` | `StorageBinInstruction` | `String(2)` |  | Container reqmts |  |  | S/4 only entity (no ECC CDC mapping) |
| `TotalShelfLifeStoragePercent` | `TotalShelfLifeStoragePercent` | `Decimal(3,0)` |  | Storage percentage |  |  | S/4 only entity (no ECC CDC mapping) |
| `ShelfLifeExpirationDatePeriod` | `ShelfLifeExpirationDatePeriod` | `String(1)` |  | Period Ind. for SLED |  |  | S/4 only entity (no ECC CDC mapping) |
| `ShelfLifeExprtnDateRndngRule` | `ShelfLifeExprtnDateRndngRule` | `String(1)` |  | Rounding rule SLED |  |  | S/4 only entity (no ECC CDC mapping) |
| `AuthorizationGroup` | `AuthorizationGroup` | `String(4)` |  | Authorization Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsActiveEntity` | `IsActiveEntity` | `Boolean` |  | Is active |  |  | S/4 only entity (no ECC CDC mapping) |
| `TotalShelfLife` | `TotalShelfLife` | `Decimal(4,0)` |  | Total Shelf Life |  |  | S/4 only entity (no ECC CDC mapping) |
| `BaseUnit` | `BaseUnit` | `String(3)` |  | Base Unit of Measure |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `ProductUnitOfMeasure`

- **ABAP Name:** `I_ProductUnitsOfMeasure`
- **Label:** Units of Measure of Product
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Product` | `Product` | `String(40)` | Y | Product |  |  | S/4 only entity (no ECC CDC mapping) |
| `AlternativeUnit` | `AlternativeUnit` | `String(3)` | Y | AlternativeUnit |  |  | S/4 only entity (no ECC CDC mapping) |
| `QuantityNumerator` | `QuantityNumerator` | `Decimal(5,0)` |  | Units / Quantity - Base Unit of Measure | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `QuantityDenominator` | `QuantityDenominator` | `Decimal(5,0)` |  | Units / Quantity - Alt Unit of Measure | AlternativeUnit |  | S/4 only entity (no ECC CDC mapping) |
| `MaterialVolume` | `MaterialVolume` | `Decimal(13,3)` |  | Volume | VolumeUnit |  | S/4 only entity (no ECC CDC mapping) |
| `VolumeUnit` | `VolumeUnit` | `String(3)` |  | Volume Unit |  |  | S/4 only entity (no ECC CDC mapping) |
| `GrossWeight` | `GrossWeight` | `Decimal(13,3)` |  | Gross Weight | WeightUnit |  | S/4 only entity (no ECC CDC mapping) |
| `WeightUnit` | `WeightUnit` | `String(3)` |  | Unit of Weight |  |  | S/4 only entity (no ECC CDC mapping) |
| `GlobalTradeItemNumber` | `GlobalTradeItemNumber` | `String(18)` |  | EAN/UPC |  |  | S/4 only entity (no ECC CDC mapping) |
| `GlobalTradeItemNumberCategory` | `GlobalTradeItemNumberCategory` | `String(2)` |  | GTIN Category |  |  | S/4 only entity (no ECC CDC mapping) |
| `UnitSpecificProductLength` | `UnitSpecificProductLength` | `Decimal(13,3)` |  | Length | ProductMeasurementUnit |  | S/4 only entity (no ECC CDC mapping) |
| `UnitSpecificProductWidth` | `UnitSpecificProductWidth` | `Decimal(13,3)` |  | Width | ProductMeasurementUnit |  | S/4 only entity (no ECC CDC mapping) |
| `UnitSpecificProductHeight` | `UnitSpecificProductHeight` | `Decimal(13,3)` |  | Height | ProductMeasurementUnit |  | S/4 only entity (no ECC CDC mapping) |
| `ProductMeasurementUnit` | `ProductMeasurementUnit` | `String(3)` |  | Unit of Dimension |  |  | S/4 only entity (no ECC CDC mapping) |
| `LowerLevelPackagingUnit` | `LowerLevelPackagingUnit` | `String(3)` |  | Lower-level unit |  |  | S/4 only entity (no ECC CDC mapping) |
| `RemainingVolumeAfterNesting` | `RemainingVolumeAfterNesting` | `Decimal(3,0)` |  | Rem.Vol.After Nestng |  |  | S/4 only entity (no ECC CDC mapping) |
| `MaximumStackingFactor` | `MaximumStackingFactor` | `Integer` |  | Max. Stacking Factor |  |  | S/4 only entity (no ECC CDC mapping) |
| `CapacityUsage` | `CapacityUsage` | `Decimal(15,3)` |  | Capacity Usage |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsActiveEntity` | `IsActiveEntity` | `Boolean` |  | Is active |  |  | S/4 only entity (no ECC CDC mapping) |
| `UnitOfMeasureCategory` | `UnitOfMeasureCategory` | `String(1)` |  | UoM Category |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductGTINVariant` | `ProductGTINVariant` | `String(2)` |  | EAN Variant |  |  | S/4 only entity (no ECC CDC mapping) |
| `BaseUnit` | `BaseUnit` | `String(3)` |  | Base Unit of Measure |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `ProductUnitOfMeasureEAN`

- **ABAP Name:** `I_ProductUnitOfMeasureEAN`
- **Label:** International Article Number of Product
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Product` | `Product` | `String(40)` | Y | Material |  |  | S/4 only entity (no ECC CDC mapping) |
| `AlternativeUnit` | `AlternativeUnit` | `String(3)` | Y | Display Unit/Measure |  |  | S/4 only entity (no ECC CDC mapping) |
| `ConsecutiveNumber` | `ConsecutiveNumber` | `String(5)` | Y | Consecutive number |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductStandardID` | `ProductStandardID` | `String(18)` |  | EAN/UPC |  |  | S/4 only entity (no ECC CDC mapping) |
| `InternationalArticleNumberCat` | `InternationalArticleNumberCat` | `String(2)` |  | GTIN Category |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsMainGlobalTradeItemNumber` | `IsMainGlobalTradeItemNumber` | `Boolean` |  | Main EAN |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `ProductValuation`

- **ABAP Name:** `I_ProductValuationBasic`
- **Label:** Product Valuation
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Product` | `Product` | `String(40)` | Y | Product |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValuationArea` | `ValuationArea` | `String(4)` | Y | Valuation Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValuationType` | `ValuationType` | `String(10)` | Y | Valuation Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValuationClass` | `ValuationClass` | `String(4)` |  | Valuation Class |  |  | S/4 only entity (no ECC CDC mapping) |
| `PriceDeterminationControl` | `PriceDeterminationControl` | `String(1)` |  | Price Determ. |  |  | S/4 only entity (no ECC CDC mapping) |
| `FiscalMonthCurrentPeriod` | `FiscalMonthCurrentPeriod` | `String(2)` |  | Current Period |  |  | S/4 only entity (no ECC CDC mapping) |
| `FiscalYearCurrentPeriod` | `FiscalYearCurrentPeriod` | `String(4)` |  | Year Current Period |  |  | S/4 only entity (no ECC CDC mapping) |
| `StandardPrice` | `StandardPrice` | `Decimal(34,4)` |  | Standard price | Currency |  | S/4 only entity (no ECC CDC mapping) |
| `PriceUnitQty` | `PriceUnitQty` | `Decimal(5,0)` |  | Price unit |  |  | S/4 only entity (no ECC CDC mapping) |
| `InventoryValuationProcedure` | `InventoryValuationProcedure` | `String(1)` |  | Price Control |  |  | S/4 only entity (no ECC CDC mapping) |
| `FuturePriceValidityStartDate` | `FuturePriceValidityStartDate` | `Date` |  | Valid from |  |  | S/4 only entity (no ECC CDC mapping) |
| `PrevInvtryPriceInCoCodeCrcy` | `PrevInvtryPriceInCoCodeCrcy` | `Decimal(34,4)` |  | Previous Price | Currency |  | S/4 only entity (no ECC CDC mapping) |
| `MovingAveragePrice` | `MovingAveragePrice` | `Decimal(34,4)` |  | Moving price | Currency |  | S/4 only entity (no ECC CDC mapping) |
| `ValuationCategory` | `ValuationCategory` | `String(1)` |  | Valuation Category |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductUsageType` | `ProductUsageType` | `String(1)` |  | Product Usage |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductOriginType` | `ProductOriginType` | `String(1)` |  | Product Origin |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsProducedInhouse` | `IsProducedInhouse` | `Boolean` |  | In-House Production |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProdCostEstNumber` | `ProdCostEstNumber` | `String(12)` |  | ProdCostEst.No. |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsMarkedForDeletion` | `IsMarkedForDeletion` | `Boolean` |  | Del. flag val. type |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValuationMargin` | `ValuationMargin` | `Decimal(6,2)` |  | Valuation Margin |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsActiveEntity` | `IsActiveEntity` | `Boolean` |  | Is active |  |  | S/4 only entity (no ECC CDC mapping) |
| `CompanyCode` | `CompanyCode` | `String(4)` |  | Company Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValuationClassSalesOrderStock` | `ValuationClassSalesOrderStock` | `String(4)` |  | VC: Sales Order Stk |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProjectStockValuationClass` | `ProjectStockValuationClass` | `String(4)` |  | Proj. stk val. class |  |  | S/4 only entity (no ECC CDC mapping) |
| `TaxBasedPricesPriceUnitQty` | `TaxBasedPricesPriceUnitQty` | `Decimal(5,0)` |  | Price Unit | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `PriceLastChangeDate` | `PriceLastChangeDate` | `Date` |  | Last Price Change |  |  | S/4 only entity (no ECC CDC mapping) |
| `FuturePrice` | `FuturePrice` | `Decimal(34,4)` |  | Future Price | Currency |  | S/4 only entity (no ECC CDC mapping) |
| `MaintenanceStatus` | `MaintenanceStatus` | `String(15)` |  | Maintenance Status |  |  | S/4 only entity (no ECC CDC mapping) |
| `Currency` | `Currency` | `String(5)` |  | Currency |  |  | S/4 only entity (no ECC CDC mapping) |
| `BaseUnit` | `BaseUnit` | `String(3)` |  | Base Unit of Measure |  |  | S/4 only entity (no ECC CDC mapping) |
| `MLIsActiveAtProductLevel` | `MLIsActiveAtProductLevel` | `Boolean` |  | ML Act. |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `ProductValuationAccounting`

- **ABAP Name:** `I_ProductValuationAccounting_2`
- **Label:** Product Valuation Account
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Product` | `Product` | `String(40)` | Y | Product |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValuationArea` | `ValuationArea` | `String(4)` | Y | Valuation Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValuationType` | `ValuationType` | `String(10)` | Y | Valuation Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `CommercialPrice1InCoCodeCrcy` | `CommercialPrice1InCoCodeCrcy` | `Decimal(34,4)` |  | Commercial price 1 | Currency |  | S/4 only entity (no ECC CDC mapping) |
| `CommercialPrice2InCoCodeCrcy` | `CommercialPrice2InCoCodeCrcy` | `Decimal(34,4)` |  | Commercial price 2 | Currency |  | S/4 only entity (no ECC CDC mapping) |
| `CommercialPrice3InCoCodeCrcy` | `CommercialPrice3InCoCodeCrcy` | `Decimal(34,4)` |  | Commercial price 3 | Currency |  | S/4 only entity (no ECC CDC mapping) |
| `DevaluationYearCount` | `DevaluationYearCount` | `String(2)` |  | Devaluation Ind. |  |  | S/4 only entity (no ECC CDC mapping) |
| `FuturePrice` | `FuturePrice` | `Decimal(34,4)` |  | Future Price | Currency |  | S/4 only entity (no ECC CDC mapping) |
| `FuturePriceValidityStartDate` | `FuturePriceValidityStartDate` | `Date` |  | Valid from |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsLIFOAndFIFORelevant` | `IsLIFOAndFIFORelevant` | `Boolean` |  | TRUE |  |  | S/4 only entity (no ECC CDC mapping) |
| `LIFOValuationPoolNumber` | `LIFOValuationPoolNumber` | `String(4)` |  | LIFO Pool |  |  | S/4 only entity (no ECC CDC mapping) |
| `StandardPricePrevYear` | `StandardPricePrevYear` | `Decimal(34,4)` |  | Standard price | Currency |  | S/4 only entity (no ECC CDC mapping) |
| `TaxPricel1InCoCodeCrcy` | `TaxPricel1InCoCodeCrcy` | `Decimal(34,4)` |  | Tax price 1 | Currency |  | S/4 only entity (no ECC CDC mapping) |
| `TaxPrice2InCoCodeCrcy` | `TaxPrice2InCoCodeCrcy` | `Decimal(34,4)` |  | Tax price 2 | Currency |  | S/4 only entity (no ECC CDC mapping) |
| `TaxPrice3InCoCodeCrcy` | `TaxPrice3InCoCodeCrcy` | `Decimal(34,4)` |  | Tax price 3 | Currency |  | S/4 only entity (no ECC CDC mapping) |
| `TaxBasedPricesPriceUnitQty` | `TaxBasedPricesPriceUnitQty` | `Decimal(5,0)` |  | Price Unit | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `CompanyCode` | `CompanyCode` | `String(4)` |  | Company Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `Currency` | `Currency` | `String(5)` |  | Currency |  |  | S/4 only entity (no ECC CDC mapping) |
| `BaseUnit` | `BaseUnit` | `String(3)` |  | Base Unit of Measure |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `ProductValuationCosting`

- **ABAP Name:** `I_ProductValuationCosting`
- **Label:** Product Valuation Costing Core Entity
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Product` | `Product` | `String(40)` | Y | Product |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValuationArea` | `ValuationArea` | `String(4)` | Y | Valuation Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValuationType` | `ValuationType` | `String(10)` | Y | Valuation Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsMaterialCostedWithQtyStruc` | `IsMaterialCostedWithQtyStruc` | `Boolean` |  | With Qty Structure |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsMaterialRelatedOrigin` | `IsMaterialRelatedOrigin` | `Boolean` |  | Material origin |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostOriginGroup` | `CostOriginGroup` | `String(4)` |  | Origin Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostingOverheadGroup` | `CostingOverheadGroup` | `String(10)` |  | Overhead Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `PlannedPrice1InCoCodeCrcy` | `PlannedPrice1InCoCodeCrcy` | `Decimal(34,4)` |  | Planned price 1 | Currency |  | S/4 only entity (no ECC CDC mapping) |
| `PlannedPrice2InCoCodeCrcy` | `PlannedPrice2InCoCodeCrcy` | `Decimal(34,4)` |  | Planned price 2 | Currency |  | S/4 only entity (no ECC CDC mapping) |
| `PlannedPrice3InCoCodeCrcy` | `PlannedPrice3InCoCodeCrcy` | `Decimal(34,4)` |  | Planned price 3 | Currency |  | S/4 only entity (no ECC CDC mapping) |
| `FuturePlndPrice1ValdtyDate` | `FuturePlndPrice1ValdtyDate` | `Date` |  | Planned price date 1 |  |  | S/4 only entity (no ECC CDC mapping) |
| `FuturePlndPrice2ValdtyDate` | `FuturePlndPrice2ValdtyDate` | `Date` |  | Planned price date 2 |  |  | S/4 only entity (no ECC CDC mapping) |
| `FuturePlndPrice3ValdtyDate` | `FuturePlndPrice3ValdtyDate` | `Date` |  | Planned price date 3 |  |  | S/4 only entity (no ECC CDC mapping) |
| `PlannedPrice` | `PlannedPrice` | `Decimal(34,4)` |  | Future Planned Price | Currency |  | S/4 only entity (no ECC CDC mapping) |
| `Currency` | `Currency` | `String(5)` |  | Currency |  |  | S/4 only entity (no ECC CDC mapping) |
| `CompanyCode` | `CompanyCode` | `String(4)` |  | Company Code |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `ProductWarehouseManagement`

- **ABAP Name:** `I_ProductWrhsMgmt`
- **Label:** Product Warehouse Management
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Product` | `Product` | `String(40)` | Y | Product |  |  | S/4 only entity (no ECC CDC mapping) |
| `WarehouseNumber` | `WarehouseNumber` | `String(3)` | Y | Warehouse Number |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProdWrhsMatlDataIsMrkdForDeltn` | `ProdWrhsMatlDataIsMrkdForDeltn` | `Boolean` |  | Del.flag:warehse no. |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProdStorageSectionMethod` | `ProdStorageSectionMethod` | `String(3)` |  | Storage Section Ind. |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProdWrhsStkPlacementStorType` | `ProdWrhsStkPlacementStorType` | `String(3)` |  | Stock placement |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProdWrhsStkRemovalStorageType` | `ProdWrhsStkRemovalStorageType` | `String(3)` |  | Stock removal |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProdWrhs1stLoadgEquipQuantity` | `ProdWrhs1stLoadgEquipQuantity` | `Decimal(13,3)` |  | Loading equip. qty 1 | ProdWrhs1stLoadgEquipQtyUnit |  | S/4 only entity (no ECC CDC mapping) |
| `ProdWrhs2ndLoadgEquipQuantity` | `ProdWrhs2ndLoadgEquipQuantity` | `Decimal(13,3)` |  | Loading equip. qty 2 | ProdWrhs2ndLoadgEquipQtyUnit |  | S/4 only entity (no ECC CDC mapping) |
| `ProdWrhs3rdLoadgEquipQuantity` | `ProdWrhs3rdLoadgEquipQuantity` | `Decimal(13,3)` |  | Loading equip. qty 3 | ProdWrhs3rdLoadgEquipQtyUnit |  | S/4 only entity (no ECC CDC mapping) |
| `ProdWrhs1stLoadgEquipQtyUnit` | `ProdWrhs1stLoadgEquipQtyUnit` | `String(3)` |  | Unit of measure 1 |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProdWrhs2ndLoadgEquipQtyUnit` | `ProdWrhs2ndLoadgEquipQtyUnit` | `String(3)` |  | Unit of measure 2 |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProdWrhs3rdLoadgEquipQtyUnit` | `ProdWrhs3rdLoadgEquipQtyUnit` | `String(3)` |  | Unit of measure 3 |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductStorageUnitType1` | `ProductStorageUnitType1` | `String(3)` |  | Storage Unit Type 1 |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductStorageUnitType2` | `ProductStorageUnitType2` | `String(3)` |  | Storage Unit Type 2 |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductStorageUnitType3` | `ProductStorageUnitType3` | `String(3)` |  | Storage Unit Type 3 |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProdWarehouseManagementUnit` | `ProdWarehouseManagementUnit` | `String(3)` |  | WM unit |  |  | S/4 only entity (no ECC CDC mapping) |
| `AdditionToExistingStkIsAllowed` | `AdditionToExistingStkIsAllowed` | `Boolean` |  | Allow addn to stock |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductBulkStorageMethod` | `ProductBulkStorageMethod` | `String(2)` |  | Bulk storage |  |  | S/4 only entity (no ECC CDC mapping) |
| `WrhsMgmtMsgToInvtryMgmtIsRqd` | `WrhsMgmtMsgToInvtryMgmtIsRqd` | `Boolean` |  | Message to inv. mgmt |  |  | S/4 only entity (no ECC CDC mapping) |
| `WrhsMgmtHasSpecialMovement` | `WrhsMgmtHasSpecialMovement` | `String(1)` |  | Special movement |  |  | S/4 only entity (no ECC CDC mapping) |
| `CapacityUsage` | `CapacityUsage` | `Decimal(11,3)` |  | Capacity usage |  |  | S/4 only entity (no ECC CDC mapping) |
| `CapacityConsumptionUnit` | `CapacityConsumptionUnit` | `String(3)` |  | Cap.consumption unit |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProdWrhsPickingStorageType` | `ProdWrhsPickingStorageType` | `String(3)` |  | Picking storage type |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProdWrhsMatlMasterDefaultUnit` | `ProdWrhsMatlMasterDefaultUnit` | `String(1)` |  | Proposed UoM frm mat |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProdIsRlvtForTwoStepPicking` | `ProdIsRlvtForTwoStepPicking` | `String(1)` |  | 2-step picking |  |  | S/4 only entity (no ECC CDC mapping) |
