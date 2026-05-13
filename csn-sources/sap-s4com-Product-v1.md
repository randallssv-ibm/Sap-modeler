# Product

> Source file: `sap-s4com-Product-v1.json`


## Entity: `ProdIntlTradeClassification`

- **ABAP Name:** `I_ProdCommodityCodeDEX`
- **Label:** Data Extraction for Product Commodity Code by Country/Region
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `TrdClassfctnNmbrSchm` |  |  |  | `String(10)` | Y | Numbering Scheme |  |  | S/4 only entity — no ECC CDC mapping |
| `Product` |  |  |  | `String(40)` | Y | Product |  | _Product | S/4 only entity — no ECC CDC mapping |
| `CommodityCode` |  |  |  | `String(30)` | Y | Commodity Code |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityStartDate` |  |  |  | `Date` | Y | Valid From |  |  | S/4 only entity — no ECC CDC mapping |
| `Country` |  |  |  | `String(3)` | Y | Country/Region |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityEndDate` |  |  |  | `Date` |  | Valid To |  |  | S/4 only entity — no ECC CDC mapping |
| `TrdClassfctnNmbrUUID` |  |  |  | `UUID` |  |  |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `ProdWhseManagementStorageType`

- **ABAP Name:** `I_ProdWrhsMgmtStorageType`
- **Label:** Product Data For Each Storage Type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  | `String(40)` | Y | Product |  |  | S/4 only entity — no ECC CDC mapping |
| `WarehouseNumber` |  |  |  | `String(3)` | Y | Warehouse Number |  |  | S/4 only entity — no ECC CDC mapping |
| `StorageType` |  |  |  | `String(3)` | Y | Storage Type |  |  | S/4 only entity — no ECC CDC mapping |
| `ProdStorTypeMatlIsMrkdForDeltn` |  |  |  | `Boolean` |  | Del. flag: stge type |  |  | S/4 only entity — no ECC CDC mapping |
| `StorageBin` |  |  |  | `String(10)` |  | Storage Bin |  |  | S/4 only entity — no ECC CDC mapping |
| `ProdWrhsMaxStorageBinQuantity` |  |  |  | `Decimal(13,3)` |  | Maximum bin quantity | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `ProdWrhsMinStorageBinQuantity` |  |  |  | `Decimal(13,3)` |  | Minimum bin quantity | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `ProdWrhsStorTypeCtrlQuantity` |  |  |  | `Decimal(13,3)` |  | Control quantity | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `ProdWrhsStorTypeReplnmtQty` |  |  |  | `Decimal(13,3)` |  | Replenishment qty | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `LeanWrhsManagementPickingArea` |  |  |  | `String(3)` |  | Picking Area |  |  | S/4 only entity — no ECC CDC mapping |
| `ProdWrhsStorTypeRoundingQty` |  |  |  | `Decimal(13,3)` |  | Rounding qty | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `BaseUnit` |  |  |  | `String(3)` |  | Base Unit of Measure |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `Product`

- **ABAP Name:** `I_Product`
- **Label:** Product
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  | `String(40)` | Y | Product |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductExternalID` |  |  |  | `String(40)` |  | Material |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductOID` |  |  |  | `String(128)` |  | Product OID |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductType` |  |  |  | `String(4)` |  | Product Type |  |  | S/4 only entity — no ECC CDC mapping |
| `CreationDate` |  |  |  | `Date` |  | Created On |  |  | S/4 only entity — no ECC CDC mapping |
| `CreationTime` |  |  |  | `String(6)` |  | Created At Time |  |  | S/4 only entity — no ECC CDC mapping |
| `CreationDateTime` |  |  |  | `Timestamp` |  | Created On |  |  | S/4 only entity — no ECC CDC mapping |
| `CreatedByUser` |  |  |  | `String(12)` |  | Created By |  |  | S/4 only entity — no ECC CDC mapping |
| `LastChangeDate` |  |  |  | `Date` |  | Last Change |  |  | S/4 only entity — no ECC CDC mapping |
| `LastChangedByUser` |  |  |  | `String(12)` |  | Changed By |  |  | S/4 only entity — no ECC CDC mapping |
| `IsMarkedForDeletion` |  |  |  | `Boolean` |  | Marked for Deletion |  |  | S/4 only entity — no ECC CDC mapping |
| `CrossPlantStatus` |  |  |  | `String(2)` |  | CrossPlantProdStatus |  |  | S/4 only entity — no ECC CDC mapping |
| `CrossPlantStatusValidityDate` |  |  |  | `Date` |  | Valid from |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductOldID` |  |  |  | `String(40)` |  | Old Product Number |  |  | S/4 only entity — no ECC CDC mapping |
| `GrossWeight` |  |  |  | `Decimal(13,3)` |  | Gross Weight | WeightUnit |  | S/4 only entity — no ECC CDC mapping |
| `PurchaseOrderQuantityUnit` |  |  |  | `String(3)` |  | Order Unit |  |  | S/4 only entity — no ECC CDC mapping |
| `SourceOfSupply` |  |  |  | `String(1)` |  | Source of supply |  |  | S/4 only entity — no ECC CDC mapping |
| `WeightUnit` |  |  |  | `String(3)` |  | Unit of Weight |  |  | S/4 only entity — no ECC CDC mapping |
| `CountryOfOrigin` |  |  |  | `String(3)` |  | Cntry/Reg of Origin |  |  | S/4 only entity — no ECC CDC mapping |
| `CompetitorID` |  |  |  | `String(10)` |  | Competitor |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductGroup` |  |  |  | `String(9)` |  | Product Group |  | _ProductGroup_2 | S/4 only entity — no ECC CDC mapping |
| `BaseUnit` |  |  |  | `String(3)` |  | Base Unit of Measure |  |  | S/4 only entity — no ECC CDC mapping |
| `ItemCategoryGroup` |  |  |  | `String(4)` |  | Gen. item cat. grp |  |  | S/4 only entity — no ECC CDC mapping |
| `NetWeight` |  |  |  | `Decimal(13,3)` |  | Net Weight | WeightUnit |  | S/4 only entity — no ECC CDC mapping |
| `ProductHierarchy` |  |  |  | `String(18)` |  | Product Hierarchy |  |  | S/4 only entity — no ECC CDC mapping |
| `Division` |  |  |  | `String(2)` |  | Division |  |  | S/4 only entity — no ECC CDC mapping |
| `VarblPurOrdUnitIsActive` |  |  |  | `String(1)` |  | Var. Order Unit |  |  | S/4 only entity — no ECC CDC mapping |
| `VolumeUnit` |  |  |  | `String(3)` |  | Volume Unit |  |  | S/4 only entity — no ECC CDC mapping |
| `MaterialVolume` |  |  |  | `Decimal(13,3)` |  | Volume | VolumeUnit |  | S/4 only entity — no ECC CDC mapping |
| `SalesStatus` |  |  |  | `String(2)` |  | X-DChain Status |  |  | S/4 only entity — no ECC CDC mapping |
| `TransportationGroup` |  |  |  | `String(4)` |  | Transportation Group |  |  | S/4 only entity — no ECC CDC mapping |
| `SalesStatusValidityDate` |  |  |  | `Date` |  | Valid from |  |  | S/4 only entity — no ECC CDC mapping |
| `AuthorizationGroup` |  |  |  | `String(4)` |  | Authorization Group |  |  | S/4 only entity — no ECC CDC mapping |
| `ANPCode` |  |  |  | `String(9)` |  | ANP Code |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductCategory` |  |  |  | `String(2)` |  | Product Category |  |  | S/4 only entity — no ECC CDC mapping |
| `Brand` |  |  |  | `String(4)` |  | Brand |  |  | S/4 only entity — no ECC CDC mapping |
| `ProcurementRule` |  |  |  | `String(1)` |  | Procurement rule |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityStartDate` |  |  |  | `Date` |  | Valid From |  |  | S/4 only entity — no ECC CDC mapping |
| `LowLevelCode` |  |  |  | `String(3)` |  | Low-Level Code |  |  | S/4 only entity — no ECC CDC mapping |
| `ProdNoInGenProdInPrepackProd` |  |  |  | `String(40)` |  | Generic Material |  |  | S/4 only entity — no ECC CDC mapping |
| `SerialIdentifierAssgmtProfile` |  |  |  | `String(4)` |  | Serial No. Profile |  |  | S/4 only entity — no ECC CDC mapping |
| `SizeOrDimensionText` |  |  |  | `String(32)` |  | Size/dimensions |  |  | S/4 only entity — no ECC CDC mapping |
| `IndustryStandardName` |  |  |  | `String(18)` |  | Industry Std Desc. |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductStandardID` |  |  |  | `String(18)` |  | GTIN |  |  | S/4 only entity — no ECC CDC mapping |
| `InternationalArticleNumberCat` |  |  |  | `String(2)` |  | EAN Category |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductIsConfigurable` |  |  |  | `Boolean` |  | Configurable |  |  | S/4 only entity — no ECC CDC mapping |
| `IsBatchManagementRequired` |  |  |  | `Boolean` |  | Batch Management |  |  | S/4 only entity — no ECC CDC mapping |
| `HasEmptiesBOM` |  |  |  | `Boolean` |  | With Empties BOM |  |  | S/4 only entity — no ECC CDC mapping |
| `ExternalProductGroup` |  |  |  | `String(18)` |  | Ext. Product Group |  |  | S/4 only entity — no ECC CDC mapping |
| `CrossPlantConfigurableProduct` |  |  |  | `String(40)` |  | Cross-plant CP |  |  | S/4 only entity — no ECC CDC mapping |
| `SerialNoExplicitnessLevel` |  |  |  | `String(1)` |  | Serialization Level |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductManufacturerNumber` |  |  |  | `String(40)` |  | Mfr Part Number |  |  | S/4 only entity — no ECC CDC mapping |
| `ManufacturerNumber` |  |  |  | `String(10)` |  | Manufacturer |  |  | S/4 only entity — no ECC CDC mapping |
| `ManufacturerPartProfile` |  |  |  | `String(4)` |  | Mfr Part Profile |  |  | S/4 only entity — no ECC CDC mapping |
| `QltyMgmtInProcmtIsActive` |  |  |  | `Boolean` |  | QM in Procur. Active |  |  | S/4 only entity — no ECC CDC mapping |
| `IsApprovedBatchRecordReqd` |  |  |  | `Boolean` |  | Appr.Batch Recd Req. |  |  | S/4 only entity — no ECC CDC mapping |
| `HandlingIndicator` |  |  |  | `String(4)` |  | Handling Indicator |  |  | S/4 only entity — no ECC CDC mapping |
| `WarehouseProductGroup` |  |  |  | `String(4)` |  | WH Material Group |  |  | S/4 only entity — no ECC CDC mapping |
| `WarehouseStorageCondition` |  |  |  | `String(2)` |  | Whse Stor. Condition |  |  | S/4 only entity — no ECC CDC mapping |
| `StandardHandlingUnitType` |  |  |  | `String(4)` |  | Standard HU Type |  |  | S/4 only entity — no ECC CDC mapping |
| `SerialNumberProfile` |  |  |  | `String(4)` |  | Serial No. Profile |  |  | S/4 only entity — no ECC CDC mapping |
| `AdjustmentProfile` |  |  |  | `String(3)` |  | Adjust. Profile |  |  | S/4 only entity — no ECC CDC mapping |
| `PreferredUnitOfMeasure` |  |  |  | `String(3)` |  | Preferred UoM |  |  | S/4 only entity — no ECC CDC mapping |
| `IsPilferable` |  |  |  | `Boolean` |  | Pilferable |  |  | S/4 only entity — no ECC CDC mapping |
| `IsRelevantForHzdsSubstances` |  |  |  | `Boolean` |  | Relevant for HS |  |  | S/4 only entity — no ECC CDC mapping |
| `QuarantinePeriod` |  |  |  | `Decimal(3,0)` |  | Quarant. Per. | TimeUnitForQuarantinePeriod |  | S/4 only entity — no ECC CDC mapping |
| `TimeUnitForQuarantinePeriod` |  |  |  | `String(3)` |  | Time Unit |  |  | S/4 only entity — no ECC CDC mapping |
| `QualityInspectionGroup` |  |  |  | `String(4)` |  | Quality Inspec. Grp |  |  | S/4 only entity — no ECC CDC mapping |
| `HandlingUnitType` |  |  |  | `String(4)` |  | Handling Unit Type |  |  | S/4 only entity — no ECC CDC mapping |
| `HasVariableTareWeight` |  |  |  | `Boolean` |  | Varb. Tare Weight |  |  | S/4 only entity — no ECC CDC mapping |
| `MaximumPackagingLength` |  |  |  | `Decimal(15,3)` |  | Max. Pack. Length | UnitForMaxPackagingDimensions |  | S/4 only entity — no ECC CDC mapping |
| `MaximumPackagingWidth` |  |  |  | `Decimal(15,3)` |  | Max. Pack. Width | UnitForMaxPackagingDimensions |  | S/4 only entity — no ECC CDC mapping |
| `MaximumPackagingHeight` |  |  |  | `Decimal(15,3)` |  | Max. Pack. Height | UnitForMaxPackagingDimensions |  | S/4 only entity — no ECC CDC mapping |
| `MaximumCapacity` |  |  |  | `Decimal(15,3)` |  | Maximum Capacity |  |  | S/4 only entity — no ECC CDC mapping |
| `OvercapacityTolerance` |  |  |  | `Decimal(3,1)` |  | Overcapacity Toler. |  |  | S/4 only entity — no ECC CDC mapping |
| `UnitForMaxPackagingDimensions` |  |  |  | `String(3)` |  | Unit of Measurement |  |  | S/4 only entity — no ECC CDC mapping |
| `BaseUnitSpecificProductLength` |  |  |  | `Decimal(13,3)` |  | Length | ProductMeasurementUnit |  | S/4 only entity — no ECC CDC mapping |
| `BaseUnitSpecificProductWidth` |  |  |  | `Decimal(13,3)` |  | Width | ProductMeasurementUnit |  | S/4 only entity — no ECC CDC mapping |
| `BaseUnitSpecificProductHeight` |  |  |  | `Decimal(13,3)` |  | Height | ProductMeasurementUnit |  | S/4 only entity — no ECC CDC mapping |
| `ProductMeasurementUnit` |  |  |  | `String(3)` |  | Unit of Dimension |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductValidStartDate` |  |  |  | `Date` |  | Valid From |  |  | S/4 only entity — no ECC CDC mapping |
| `ArticleCategory` |  |  |  | `String(2)` |  | Product Category |  |  | S/4 only entity — no ECC CDC mapping |
| `ContentUnit` |  |  |  | `String(3)` |  | Content Unit |  |  | S/4 only entity — no ECC CDC mapping |
| `NetContent` |  |  |  | `Decimal(13,3)` |  | Net Contents | ContentUnit |  | S/4 only entity — no ECC CDC mapping |
| `ComparisonPriceQuantity` |  |  |  | `Decimal(5,0)` |  | Comparison Price Unit | ContentUnit |  | S/4 only entity — no ECC CDC mapping |
| `GrossContent` |  |  |  | `Decimal(13,3)` |  | Gross Contents | ContentUnit |  | S/4 only entity — no ECC CDC mapping |
| `ProductValidEndDate` |  |  |  | `Date` |  | Valid To |  |  | S/4 only entity — no ECC CDC mapping |
| `AssortmentListType` |  |  |  | `String(1)` |  | Assortment List Type |  |  | S/4 only entity — no ECC CDC mapping |
| `HasTextilePartsWthAnimalOrigin` |  |  |  | `Boolean` |  | Animal Origin |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductSeasonUsageCategory` |  |  |  | `String(1)` |  | Season Usage |  |  | S/4 only entity — no ECC CDC mapping |
| `IndustrySector` |  |  |  | `String(1)` |  | Industry |  |  | S/4 only entity — no ECC CDC mapping |
| `ChangeNumber` |  |  |  | `String(12)` |  | Change Number |  |  | S/4 only entity — no ECC CDC mapping |
| `MaterialRevisionLevel` |  |  |  | `String(2)` |  | Revision Level |  |  | S/4 only entity — no ECC CDC mapping |
| `IsActiveEntity` |  |  |  | `Boolean` |  | Is active |  |  | S/4 only entity — no ECC CDC mapping |
| `LastChangeDateTime` |  |  |  | `Timestamp` |  | Last Changed |  |  | S/4 only entity — no ECC CDC mapping |
| `LastChangeTime` |  |  |  | `String(6)` |  | Last Changed Time |  |  | S/4 only entity — no ECC CDC mapping |
| `DangerousGoodsIndProfile` |  |  |  | `String(3)` |  | DG indicator profile |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductUUID` |  |  |  | `UUID` |  | Product |  |  | S/4 only entity — no ECC CDC mapping |
| `ProdSupChnMgmtUUID22` |  |  |  | `String(22)` |  | Product ID |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductDocumentChangeNumber` |  |  |  | `String(6)` |  | Document Change No. |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductDocumentPageCount` |  |  |  | `String(3)` |  | Number Of Sheets |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductDocumentPageNumber` |  |  |  | `String(3)` |  | Page Number |  |  | S/4 only entity — no ECC CDC mapping |
| `OwnInventoryManagedProduct` |  |  |  | `String(40)` |  | Int. material number |  |  | S/4 only entity — no ECC CDC mapping |
| `DocumentIsCreatedByCAD` |  |  |  | `Boolean` |  | CAD Indicator |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductionOrInspectionMemoTxt` |  |  |  | `String(18)` |  | Prod./insp. memo |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductionMemoPageFormat` |  |  |  | `String(4)` |  | Page format |  |  | S/4 only entity — no ECC CDC mapping |
| `GlobalTradeItemNumberVariant` |  |  |  | `String(2)` |  | EAN Variant |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductIsHighlyViscous` |  |  |  | `Boolean` |  | Highly viscous |  |  | S/4 only entity — no ECC CDC mapping |
| `TransportIsInBulk` |  |  |  | `Boolean` |  | In bulk/liquid |  |  | S/4 only entity — no ECC CDC mapping |
| `ProdAllocDetnProcedure` |  |  |  | `String(18)` |  | Product allocation |  |  | S/4 only entity — no ECC CDC mapping |
| `ProdEffctyParamValsAreAssigned` |  |  |  | `Boolean` |  | Assign effect. vals |  |  | S/4 only entity — no ECC CDC mapping |
| `ProdIsEnvironmentallyRelevant` |  |  |  | `Boolean` |  | Environmentally rlvt |  |  | S/4 only entity — no ECC CDC mapping |
| `LaboratoryOrDesignOffice` |  |  |  | `String(3)` |  | Lab/Office |  |  | S/4 only entity — no ECC CDC mapping |
| `PackagingMaterialGroup` |  |  |  | `String(4)` |  | Matl Grp Pack.Matls |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductIsLocked` |  |  |  | `Boolean` |  | Product locked |  |  | S/4 only entity — no ECC CDC mapping |
| `DiscountInKindEligibility` |  |  |  | `String(1)` |  | Qual.f.FreeGoodsDis. |  |  | S/4 only entity — no ECC CDC mapping |
| `SmartFormName` |  |  |  | `String(30)` |  | Form Name |  |  | S/4 only entity — no ECC CDC mapping |
| `PackingReferenceProduct` |  |  |  | `String(40)` |  | Ref. Mat. for Pckg |  |  | S/4 only entity — no ECC CDC mapping |
| `BasicMaterial` |  |  |  | `String(48)` |  | Basic Material |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductDocumentNumber` |  |  |  | `String(22)` |  | Document |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductDocumentVersion` |  |  |  | `String(2)` |  | Document Version |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductDocumentType` |  |  |  | `String(3)` |  | Document Type |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductDocumentPageFormat` |  |  |  | `String(4)` |  | Page Format |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductConfiguration` |  |  |  | `String(18)` |  | Internal object no. |  |  | S/4 only entity — no ECC CDC mapping |
| `SegmentationStrategy` |  |  |  | `String(8)` |  | Seg. Strategy |  |  | S/4 only entity — no ECC CDC mapping |
| `SegmentationIsRelevant` |  |  |  | `Boolean` |  | Seg. Relevant |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductCompositionIsRelevant` |  |  |  | `Boolean` |  | Product Composition |  |  | S/4 only entity — no ECC CDC mapping |
| `IsChemicalComplianceRelevant` |  |  |  | `String(1)` |  | Chemical Compliance Relevance Indicator |  |  | S/4 only entity — no ECC CDC mapping |
| `ManufacturerBookPartNumber` |  |  |  | `String(40)` |  | MS Book Part No |  |  | S/4 only entity — no ECC CDC mapping |
| `LogisticalProductCategory` |  |  |  | `String(1)` |  | Logl Material Cat. |  |  | S/4 only entity — no ECC CDC mapping |
| `SalesProduct` |  |  |  | `String(40)` |  | Sales Material No. |  |  | S/4 only entity — no ECC CDC mapping |
| `ProdCharc1InternalNumber` |  |  |  | `String(10)` |  | Int. Char. Number |  |  | S/4 only entity — no ECC CDC mapping |
| `ProdCharc2InternalNumber` |  |  |  | `String(10)` |  | Int. Char. Number |  |  | S/4 only entity — no ECC CDC mapping |
| `ProdCharc3InternalNumber` |  |  |  | `String(10)` |  | Int. Char. Number |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductCharacteristic1` |  |  |  | `String(18)` |  | Color |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductCharacteristic2` |  |  |  | `String(18)` |  | Main Size |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductCharacteristic3` |  |  |  | `String(18)` |  | Second Size |  |  | S/4 only entity — no ECC CDC mapping |
| `MaintenanceStatus` |  |  |  | `String(15)` |  | Maintenance Status |  |  | S/4 only entity — no ECC CDC mapping |
| `FashionProdInformationField1` |  |  |  | `String(10)` |  | Fsh. Attribute1 |  |  | S/4 only entity — no ECC CDC mapping |
| `FashionProdInformationField2` |  |  |  | `String(10)` |  | Fsh. Attribute2 |  |  | S/4 only entity — no ECC CDC mapping |
| `FashionProdInformationField3` |  |  |  | `String(6)` |  | Fsh. Attribute3 |  |  | S/4 only entity — no ECC CDC mapping |
| `DfsAmmunitionGroupCode` |  |  |  | `String(8)` |  | Ammunition Code |  |  | S/4 only entity — no ECC CDC mapping |
| `DfsRICIdentifier` |  |  |  | `Integer64` |  | RIC ID |  |  | S/4 only entity — no ECC CDC mapping |
| `DfsProductSensitivity` |  |  |  | `String(4)` |  | Sensitivity for Char |  |  | S/4 only entity — no ECC CDC mapping |
| `DfsManufacturerPartLongNumber` |  |  |  | `String(60)` |  | Long Mfr Part No. |  |  | S/4 only entity — no ECC CDC mapping |
| `DfsMatlConditionMgmt` |  |  |  | `String(1)` |  | Condition Mgmt |  |  | S/4 only entity — no ECC CDC mapping |
| `DfsReturnDelivery` |  |  |  | `String(1)` |  | Return Code |  |  | S/4 only entity — no ECC CDC mapping |
| `DfsLogisticsLevel` |  |  |  | `String(1)` |  | Return to Log.Level |  |  | S/4 only entity — no ECC CDC mapping |
| `DfsNationalItemIdnNumber` |  |  |  | `String(9)` |  | NATO Item ID Number |  |  | S/4 only entity — no ECC CDC mapping |
| `LstMiProductToleranceType` |  |  |  | `String(4)` |  | Tolerance Type |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `ProductConsumption`

- **ABAP Name:** `I_ProductConsumption`
- **Label:** Product Consumption
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  | `String(40)` | Y | Product |  |  | S/4 only entity — no ECC CDC mapping |
| `Plant` |  |  |  | `String(4)` | Y | Plant |  |  | S/4 only entity — no ECC CDC mapping |
| `PostingFiscalYear` |  |  |  | `String(4)` | Y | Fiscal Year |  |  | S/4 only entity — no ECC CDC mapping |
| `PeriodType` |  |  |  | `String(1)` | Y | Period Indicator |  |  | S/4 only entity — no ECC CDC mapping |
| `NumberOfFollowOnRecords` |  |  |  | `String(2)` | Y | Follow-on records |  |  | S/4 only entity — no ECC CDC mapping |
| `TotalConsumption1Quantity` |  |  |  | `Decimal(13,3)` |  | Tot.consumption 1 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `TotalConsumption2Quantity` |  |  |  | `Decimal(13,3)` |  | Tot.consumption 2 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `TotalConsumption3Quantity` |  |  |  | `Decimal(13,3)` |  | Tot.consumption 3 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `TotalConsumption4Quantity` |  |  |  | `Decimal(13,3)` |  | Tot.consumption 4 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `TotalConsumption5Quantity` |  |  |  | `Decimal(13,3)` |  | Tot.consumption 5 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `TotalConsumption6Quantity` |  |  |  | `Decimal(13,3)` |  | Tot.consumption 6 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `TotalConsumption7Quantity` |  |  |  | `Decimal(13,3)` |  | Tot.consumption 7 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `TotalConsumption8Quantity` |  |  |  | `Decimal(13,3)` |  | Tot.consumption 8 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `TotalConsumption9Quantity` |  |  |  | `Decimal(13,3)` |  | Tot.consumption 9 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `TotalConsumption10Quantity` |  |  |  | `Decimal(13,3)` |  | Tot.consumption 10 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `TotalConsumption11Quantity` |  |  |  | `Decimal(13,3)` |  | Tot.consumption 11 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `TotalConsumption12Quantity` |  |  |  | `Decimal(13,3)` |  | Tot.consumption 12 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `TotalConsumption13Quantity` |  |  |  | `Decimal(13,3)` |  | Tot.consumption 13 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `UnplannedConsumption1Quantity` |  |  |  | `Decimal(13,3)` |  | Unplnd consump. 1 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `UnplannedConsumption2Quantity` |  |  |  | `Decimal(13,3)` |  | Unplnd consump. 2 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `UnplannedConsumption3Quantity` |  |  |  | `Decimal(13,3)` |  | Unplnd consump. 3 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `UnplannedConsumption4Quantity` |  |  |  | `Decimal(13,3)` |  | Unplnd consump. 4 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `UnplannedConsumption5Quantity` |  |  |  | `Decimal(13,3)` |  | Unplnd consump. 5 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `UnplannedConsumption6Quantity` |  |  |  | `Decimal(13,3)` |  | Unplnd consump. 6 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `UnplannedConsumption7Quantity` |  |  |  | `Decimal(13,3)` |  | Unplnd consump. 7 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `UnplannedConsumption8Quantity` |  |  |  | `Decimal(13,3)` |  | Unplnd consump. 8 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `UnplannedConsumption9Quantity` |  |  |  | `Decimal(13,3)` |  | Unplnd consump. 9 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `UnplannedConsumption10Quantity` |  |  |  | `Decimal(13,3)` |  | Unplnd consump. 10 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `UnplannedConsumption11Quantity` |  |  |  | `Decimal(13,3)` |  | Unplnd consump. 11 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `UnplannedConsumption12Quantity` |  |  |  | `Decimal(13,3)` |  | Unplnd consump. 12 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `UnplannedConsumption13Quantity` |  |  |  | `Decimal(13,3)` |  | Unplnd consump. 13 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `MnllyCrrtdTotCnsmpn1Quantity` |  |  |  | `Decimal(13,3)` |  | Corr.tot.consum 1 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `MnllyCrrtdTotCnsmpn2Quantity` |  |  |  | `Decimal(13,3)` |  | Corr.tot.consum 2 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `MnllyCrrtdTotCnsmpn3Quantity` |  |  |  | `Decimal(13,3)` |  | Corr.tot.consum 3 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `MnllyCrrtdTotCnsmpn4Quantity` |  |  |  | `Decimal(13,3)` |  | Corr.tot.consum 4 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `MnllyCrrtdTotCnsmpn5Quantity` |  |  |  | `Decimal(13,3)` |  | Corr.tot.consum 5 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `MnllyCrrtdTotCnsmpn6Quantity` |  |  |  | `Decimal(13,3)` |  | Corr.tot.consum 6 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `MnllyCrrtdTotCnsmpn7Quantity` |  |  |  | `Decimal(13,3)` |  | Corr.tot.consum 7 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `MnllyCrrtdTotCnsmpn8Quantity` |  |  |  | `Decimal(13,3)` |  | Corr.tot.consum 8 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `MnllyCrrtdTotCnsmpn9Quantity` |  |  |  | `Decimal(13,3)` |  | Corr.tot.consum 9 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `MnllyCrrtdTotCnsmpn10Quantity` |  |  |  | `Decimal(13,3)` |  | Corr.tot.consum 10 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `MnllyCrrtdTotCnsmpn11Quantity` |  |  |  | `Decimal(13,3)` |  | Corr.tot.consum 11 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `MnllyCrrtdTotCnsmpn12Quantity` |  |  |  | `Decimal(13,3)` |  | Corr.tot.consum 12 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `MnllyCrrtdTotCnsmpn13Quantity` |  |  |  | `Decimal(13,3)` |  | Corr.tot.consum 13 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `MnllyCrrtdUnplndCnsmpn1Qty` |  |  |  | `Decimal(13,3)` |  | Corr.unpl.cons. 1 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `MnllyCrrtdUnplndCnsmpn2Qty` |  |  |  | `Decimal(13,3)` |  | Corr.unpl.cons. 2 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `MnllyCrrtdUnplndCnsmpn3Qty` |  |  |  | `Decimal(13,3)` |  | Corr.unpl.cons. 3 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `MnllyCrrtdUnplndCnsmpn4Qty` |  |  |  | `Decimal(13,3)` |  | Corr.unpl.cons. 4 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `MnllyCrrtdUnplndCnsmpn5Qty` |  |  |  | `Decimal(13,3)` |  | Corr.unpl.cons. 5 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `MnllyCrrtdUnplndCnsmpn6Qty` |  |  |  | `Decimal(13,3)` |  | Corr.unpl.cons. 6 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `MnllyCrrtdUnplndCnsmpn7Qty` |  |  |  | `Decimal(13,3)` |  | Corr.unpl.cons. 7 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `MnllyCrrtdUnplndCnsmpn8Qty` |  |  |  | `Decimal(13,3)` |  | Corr.unpl.cons. 8 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `MnllyCrrtdUnplndCnsmpn9Qty` |  |  |  | `Decimal(13,3)` |  | Corr.unpl.cons. 9 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `MnllyCrrtdUnplndCnsmpn10Qty` |  |  |  | `Decimal(13,3)` |  | Corr.unpl.cons. 10 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `MnllyCrrtdUnplndCnsmpn11Qty` |  |  |  | `Decimal(13,3)` |  | Corr.unpl.cons. 11 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `MnllyCrrtdUnplndCnsmpn12Qty` |  |  |  | `Decimal(13,3)` |  | Corr.unpl.cons. 12 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `MnllyCrrtdUnplndCnsmpn13Qty` |  |  |  | `Decimal(13,3)` |  | Corr.unpl.cons. 13 | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `BaseUnit` |  |  |  | `String(3)` |  | Base Unit of Measure |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `ProductDescription`

- **ABAP Name:** `I_ProductDescription_2`
- **Label:** Product Descriptions
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  | `String(40)` | Y | Product |  |  | S/4 only entity — no ECC CDC mapping |
| `Language` |  |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductDescription` |  |  |  | `String(40)` |  | Product Description |  |  | S/4 only entity — no ECC CDC mapping |
| `LanguageISOCode` |  |  |  | `String(2)` |  | Language |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `ProductGroup`

- **ABAP Name:** `I_ProductGroup_2`
- **Label:** Product Group
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `ProductGroup` |  |  |  | `String(9)` | Y | Product Group |  |  | S/4 only entity — no ECC CDC mapping |
| `AuthorizationGroup` |  |  |  | `String(4)` |  | Authorization Group |  |  | S/4 only entity — no ECC CDC mapping |
| `ValuationClass` |  |  |  | `String(4)` |  | Valuation Class |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchasingAcknProfile` |  |  |  | `String(4)` |  | Purchasing value key |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `ProductGroupText`

- **ABAP Name:** `I_ProductGroupText_2`
- **Label:** Product Group - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `ProductGroup` |  |  |  | `String(9)` | Y | Product Group |  | _ProductGroup | S/4 only entity — no ECC CDC mapping |
| `Language` |  |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductGroupName` |  |  |  | `String(20)` |  | Product Group Description |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductGroupText` |  |  |  | `String(60)` |  | Mat.Grp Desc. 2 |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `ProductMRPArea`

- **ABAP Name:** `I_ProductMRPArea`
- **Label:** MRP Area Details of a Product
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  | `String(40)` | Y | Product |  | _Product | S/4 only entity — no ECC CDC mapping |
| `MRPArea` |  |  |  | `String(10)` | Y | MRP Area |  |  | S/4 only entity — no ECC CDC mapping |
| `MRPPlant` |  |  |  | `String(4)` |  | MRP Area Plant |  |  | S/4 only entity — no ECC CDC mapping |
| `MRPGroup` |  |  |  | `String(4)` |  | MRP Group |  |  | S/4 only entity — no ECC CDC mapping |
| `MRPType` |  |  |  | `String(2)` |  | MRP Type |  |  | S/4 only entity — no ECC CDC mapping |
| `MRPController` |  |  |  | `String(3)` |  | MRP Controller |  |  | S/4 only entity — no ECC CDC mapping |
| `MRPProfile` |  |  |  | `String(4)` |  | MRP Profile |  |  | S/4 only entity — no ECC CDC mapping |
| `LotSizingProcedure` |  |  |  | `String(2)` |  | Lot Sizing Procedure |  |  | S/4 only entity — no ECC CDC mapping |
| `MRPPlanningCalendar` |  |  |  | `String(3)` |  | Planning Calendar |  |  | S/4 only entity — no ECC CDC mapping |
| `MRPPlanningCycle` |  |  |  | `String(3)` |  | Planning Cycle |  |  | S/4 only entity — no ECC CDC mapping |
| `MRPSafetyStockMethod` |  |  |  | `String(2)` |  | Safety Stock Method |  |  | S/4 only entity — no ECC CDC mapping |
| `MaterialProcurementProfile` |  |  |  | `String(2)` |  | Procurement Profile |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductionStorageLocation` |  |  |  | `String(4)` |  | Production Storage Location |  |  | S/4 only entity — no ECC CDC mapping |
| `DfltStorLocForExtProcmt` |  |  |  | `String(4)` |  | External Procurement Storage Location |  |  | S/4 only entity — no ECC CDC mapping |
| `RangeOfCoverageProfile` |  |  |  | `String(3)` |  | Range-of-Coverage Profile |  |  | S/4 only entity — no ECC CDC mapping |
| `SafetyTimePeriodProfile` |  |  |  | `String(3)` |  | Period Profile for Safety Time |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductSafetyTimeMRPRelevance` |  |  |  | `String(1)` |  | Safety Time MRP Relevance |  |  | S/4 only entity — no ECC CDC mapping |
| `DependentRqmtMRPRelevance` |  |  |  | `String(1)` |  | Dependent Requirements MRP Relevance |  |  | S/4 only entity — no ECC CDC mapping |
| `StorageCostsPercentageCode` |  |  |  | `String(1)` |  | Storage Costs Code |  |  | S/4 only entity — no ECC CDC mapping |
| `RoundingProfile` |  |  |  | `String(4)` |  | Rounding Profile |  |  | S/4 only entity — no ECC CDC mapping |
| `IsMarkedForDeletion` |  |  |  | `Boolean` |  | Deletion Indicator |  |  | S/4 only entity — no ECC CDC mapping |
| `LastChangedByUser` |  |  |  | `String(12)` |  | Changed By |  |  | S/4 only entity — no ECC CDC mapping |
| `LastChangeDate` |  |  |  | `Date` |  | Changed On |  |  | S/4 only entity — no ECC CDC mapping |
| `LastChangeTime` |  |  |  | `String(6)` |  | Time of Change |  |  | S/4 only entity — no ECC CDC mapping |
| `PlannedDeliveryDurationInDays` |  |  |  | `Decimal(3,0)` |  | Planned Deliv. Time |  |  | S/4 only entity — no ECC CDC mapping |
| `PlanningTimeFenceInDays` |  |  |  | `String(3)` |  | Planning Time Fence |  |  | S/4 only entity — no ECC CDC mapping |
| `RqmtQtyRcptTaktTmeInWrkgDays` |  |  |  | `Decimal(3,0)` |  | Takt time |  |  | S/4 only entity — no ECC CDC mapping |
| `AssemblyScrapPercent` |  |  |  | `Decimal(5,2)` |  | Assembly scrap (%) |  |  | S/4 only entity — no ECC CDC mapping |
| `BaseUnit` |  |  |  | `String(3)` |  | Base Unit of Measure |  |  | S/4 only entity — no ECC CDC mapping |
| `MinimumLotSizeQuantity` |  |  |  | `Decimal(13,3)` |  | Minimum Lot Size | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `MaximumLotSizeQuantity` |  |  |  | `Decimal(13,3)` |  | Maximum Lot Size | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `MaterialMaxStockLevelQuantity` |  |  |  | `Decimal(13,3)` |  | Maximum Stock Level | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `SafetyStockQuantity` |  |  |  | `Decimal(13,3)` |  | Safety Stock | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `LotSizeRoundingQuantity` |  |  |  | `Decimal(13,3)` |  | Rounding Quantity | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `ReorderThresholdQuantity` |  |  |  | `Decimal(13,3)` |  | Reorder Point | BaseUnit |  | S/4 only entity — no ECC CDC mapping |


## Entity: `ProductPlant`

- **ABAP Name:** `I_ProductPlantBasic`
- **Label:** Product Plant
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  | `String(40)` | Y | Product |  |  | S/4 only entity — no ECC CDC mapping |
| `Plant` |  |  |  | `String(4)` | Y | Plant |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchasingGroup` |  |  |  | `String(3)` |  | Purchasing Group |  |  | S/4 only entity — no ECC CDC mapping |
| `CountryOfOrigin` |  |  |  | `String(3)` |  | Country/Region of Origin |  |  | S/4 only entity — no ECC CDC mapping |
| `RegionOfOrigin` |  |  |  | `String(3)` |  | Region of Origin |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductionInvtryManagedLoc` |  |  |  | `String(4)` |  | Storage Location |  |  | S/4 only entity — no ECC CDC mapping |
| `ProfileCode` |  |  |  | `String(2)` |  | Material Status |  |  | S/4 only entity — no ECC CDC mapping |
| `ProfileValidityStartDate` |  |  |  | `Date` |  | Valid From |  |  | S/4 only entity — no ECC CDC mapping |
| `AvailabilityCheckType` |  |  |  | `String(2)` |  | Availability check |  |  | S/4 only entity — no ECC CDC mapping |
| `FiscalYearVariant` |  |  |  | `String(2)` |  | Fiscal Year Variant |  |  | S/4 only entity — no ECC CDC mapping |
| `PeriodType` |  |  |  | `String(1)` |  | Period Indicator |  |  | S/4 only entity — no ECC CDC mapping |
| `ProfitCenter` |  |  |  | `String(10)` |  | Profit Center |  |  | S/4 only entity — no ECC CDC mapping |
| `GoodsReceiptDuration` |  |  |  | `Decimal(3,0)` |  | GR processing time |  |  | S/4 only entity — no ECC CDC mapping |
| `MaintenanceStatusName` |  |  |  | `String(15)` |  | Maintenance Status |  |  | S/4 only entity — no ECC CDC mapping |
| `IsMarkedForDeletion` |  |  |  | `Boolean` |  | DF at plant level |  |  | S/4 only entity — no ECC CDC mapping |
| `MRPType` |  |  |  | `String(2)` |  | MRP Type |  |  | S/4 only entity — no ECC CDC mapping |
| `MRPResponsible` |  |  |  | `String(3)` |  | MRP Controller |  |  | S/4 only entity — no ECC CDC mapping |
| `ABCIndicator` |  |  |  | `String(1)` |  | ABC Indicator |  |  | S/4 only entity — no ECC CDC mapping |
| `MinimumLotSizeQuantity` |  |  |  | `Decimal(13,3)` |  | Minimum Lot Size | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `MaximumLotSizeQuantity` |  |  |  | `Decimal(13,3)` |  | Maximum Lot Size | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `FixedLotSizeQuantity` |  |  |  | `Decimal(13,3)` |  | Fixed lot size | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `ConsumptionTaxCtrlCode` |  |  |  | `String(16)` |  | Control Code |  |  | S/4 only entity — no ECC CDC mapping |
| `IsCoProduct` |  |  |  | `Boolean` |  | Co-Product |  |  | S/4 only entity — no ECC CDC mapping |
| `ConfigurableProduct` |  |  |  | `String(40)` |  | Conf. Material |  | _ConfigurableProduct | S/4 only entity — no ECC CDC mapping |
| `StockDeterminationGroup` |  |  |  | `String(4)` |  | Stock Determ. Group |  |  | S/4 only entity — no ECC CDC mapping |
| `HasPostToInspectionStock` |  |  |  | `Boolean` |  | Post to insp. stock |  |  | S/4 only entity — no ECC CDC mapping |
| `IsBatchManagementRequired` |  |  |  | `Boolean` |  | Batch Mgmt Rqt(Plnt) |  |  | S/4 only entity — no ECC CDC mapping |
| `SerialNumberProfile` |  |  |  | `String(4)` |  | Serial No. Profile |  |  | S/4 only entity — no ECC CDC mapping |
| `IsNegativeStockAllowed` |  |  |  | `Boolean` |  | Neg. Stocks In Plant |  |  | S/4 only entity — no ECC CDC mapping |
| `HasConsignmentCtrl` |  |  |  | `String(1)` |  | Consign.Control |  |  | S/4 only entity — no ECC CDC mapping |
| `IsPurgAcrossPurgGroup` |  |  |  | `Boolean` |  | Across Purch.Group |  |  | S/4 only entity — no ECC CDC mapping |
| `IsInternalBatchManaged` |  |  |  | `Boolean` |  | Batch Management |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductCFOPCategory` |  |  |  | `String(2)` |  | Matl. CFOP Category |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductIsExciseTaxRelevant` |  |  |  | `Boolean` |  | Is Excise Tax Relevant |  |  | S/4 only entity — no ECC CDC mapping |
| `UnderDelivToleranceLimit` |  |  |  | `Decimal(3,1)` |  | Underdelivery Toler. |  |  | S/4 only entity — no ECC CDC mapping |
| `OverDelivToleranceLimit` |  |  |  | `Decimal(3,1)` |  | Overdelivery Toler. |  |  | S/4 only entity — no ECC CDC mapping |
| `ProcurementType` |  |  |  | `String(1)` |  | Procurement Type |  |  | S/4 only entity — no ECC CDC mapping |
| `SpecialProcurementType` |  |  |  | `String(2)` |  | Special Procurement |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductionSchedulingProfile` |  |  |  | `String(6)` |  | Production Scheduling Profile |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductionSupervisor` |  |  |  | `String(3)` |  | Prodn Supervisor |  |  | S/4 only entity — no ECC CDC mapping |
| `SafetyStockQuantity` |  |  |  | `Decimal(13,3)` |  | Safety Stock | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `GoodsIssueUnit` |  |  |  | `String(3)` |  | Unit of Issue |  |  | S/4 only entity — no ECC CDC mapping |
| `SourceOfSupplyCategory` |  |  |  | `String(1)` |  | Source of supply |  |  | S/4 only entity — no ECC CDC mapping |
| `ConsumptionReferenceProduct` |  |  |  | `String(40)` |  | RefMatl: consumption |  |  | S/4 only entity — no ECC CDC mapping |
| `ConsumptionReferencePlant` |  |  |  | `String(4)` |  | RefPlant:consumption |  |  | S/4 only entity — no ECC CDC mapping |
| `ConsumptionRefUsageEndDate` |  |  |  | `Date` |  | Date to |  |  | S/4 only entity — no ECC CDC mapping |
| `ConsumptionQtyMultiplier` |  |  |  | `Decimal(4,2)` |  | Multiplier |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductUnitGroup` |  |  |  | `String(4)` |  | Unit of Measure Group |  |  | S/4 only entity — no ECC CDC mapping |
| `DistrCntrDistributionProfile` |  |  |  | `String(3)` |  | Distr. profile |  |  | S/4 only entity — no ECC CDC mapping |
| `ConsignmentControl` |  |  |  | `String(1)` |  | Consign.Control |  |  | S/4 only entity — no ECC CDC mapping |
| `GoodIssueProcessingDays` |  |  |  | `Decimal(3,0)` |  | GI Proc. Time |  |  | S/4 only entity — no ECC CDC mapping |
| `PlannedDeliveryDurationInDays` |  |  |  | `Decimal(3,0)` |  | Planned Deliv. Time |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductIsCriticalPrt` |  |  |  | `Boolean` |  | Critical Part |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductLogisticsHandlingGroup` |  |  |  | `String(4)` |  | Log. handling group |  |  | S/4 only entity — no ECC CDC mapping |
| `MaterialFreightGroup` |  |  |  | `String(8)` |  | Material Freight Grp |  |  | S/4 only entity — no ECC CDC mapping |
| `OriginalBatchReferenceMaterial` |  |  |  | `String(40)` |  | OB Reference Materl |  |  | S/4 only entity — no ECC CDC mapping |
| `OriglBatchManagementIsRequired` |  |  |  | `String(1)` |  | OB Management |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductConfiguration` |  |  |  | `String(18)` |  | Internal object no. |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductMinControlTemperature` |  |  |  | `Decimal(7,2)` |  | Min. Temperature | ProductControlTemperatureUnit |  | S/4 only entity — no ECC CDC mapping |
| `ProductMaxControlTemperature` |  |  |  | `Decimal(7,2)` |  | Max. Temperature | ProductControlTemperatureUnit |  | S/4 only entity — no ECC CDC mapping |
| `ProductControlTemperatureUnit` |  |  |  | `String(3)` |  | Temperature UoM |  |  | S/4 only entity — no ECC CDC mapping |
| `ValuationCategory` |  |  |  | `String(1)` |  | Valuation Category |  |  | S/4 only entity — no ECC CDC mapping |
| `BaseUnit` |  |  |  | `String(3)` |  | Base Unit of Measure |  |  | S/4 only entity — no ECC CDC mapping |
| `ItemUniqueIdentifierIsRelevant` |  |  |  | `Boolean` |  | IUID-Relevant |  |  | S/4 only entity — no ECC CDC mapping |
| `ItemUniqueIdentifierType` |  |  |  | `String(10)` |  | IUID Type |  |  | S/4 only entity — no ECC CDC mapping |
| `ExtAllocOfItmUnqIdtIsRelevant` |  |  |  | `Boolean` |  | Ext. Allocation |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `ProductPlantCosting`

- **ABAP Name:** `I_ProductPlantCosting`
- **Label:** Product Plant Costing
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  | `String(40)` | Y | Product |  |  | S/4 only entity — no ECC CDC mapping |
| `Plant` |  |  |  | `String(4)` | Y | Plant |  |  | S/4 only entity — no ECC CDC mapping |
| `IsCoProduct` |  |  |  | `Boolean` |  | Co-Product |  |  | S/4 only entity — no ECC CDC mapping |
| `CostingLotSize` |  |  |  | `Decimal(13,3)` |  | Costing Lot Size | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `TaskListGroup` |  |  |  | `String(8)` |  | Group |  |  | S/4 only entity — no ECC CDC mapping |
| `TaskListType` |  |  |  | `String(1)` |  | Task List Type |  |  | S/4 only entity — no ECC CDC mapping |
| `CostingSpecialProcurementType` |  |  |  | `String(2)` |  | Special Procurement Type |  |  | S/4 only entity — no ECC CDC mapping |
| `SourceBOMAlternative` |  |  |  | `String(2)` |  | Alternative BOM |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductBOMUsage` |  |  |  | `String(1)` |  | BOM Usage |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductIsCostingRelevant` |  |  |  | `Boolean` |  | Do Not Cost |  |  | S/4 only entity — no ECC CDC mapping |
| `TaskListGroupCounter` |  |  |  | `String(2)` |  | Group Counter |  |  | S/4 only entity — no ECC CDC mapping |
| `VarianceKey` |  |  |  | `String(6)` |  | Variance Key |  |  | S/4 only entity — no ECC CDC mapping |
| `CostingProductionVersion` |  |  |  | `String(4)` |  | Production Version |  |  | S/4 only entity — no ECC CDC mapping |
| `IsFixedPriceCoProduct` |  |  |  | `Boolean` |  | Fixed-Price Co-Prod. |  |  | S/4 only entity — no ECC CDC mapping |
| `BaseUnit` |  |  |  | `String(3)` |  | Base Unit of Measure |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `ProductPlantForecast`

- **ABAP Name:** `I_ProductPlantForecast`
- **Label:** Product Plant Forecast
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  | `String(40)` | Y | Product |  |  | S/4 only entity — no ECC CDC mapping |
| `Plant` |  |  |  | `String(4)` | Y | Plant |  |  | S/4 only entity — no ECC CDC mapping |
| `ConsumptionRefUsageEndDate` |  |  |  | `Date` |  | Date to |  |  | S/4 only entity — no ECC CDC mapping |
| `ConsumptionQtyMultiplier` |  |  |  | `Decimal(4,2)` |  | Multiplier |  |  | S/4 only entity — no ECC CDC mapping |
| `ConsumptionReferenceProduct` |  |  |  | `String(40)` |  | RefMatl: consumption |  | _ConsumptionReferenceProduct | S/4 only entity — no ECC CDC mapping |
| `ConsumptionReferencePlant` |  |  |  | `String(4)` |  | RefPlant:consumption |  |  | S/4 only entity — no ECC CDC mapping |
| `CorrectionFactorIsRequired` |  |  |  | `Boolean` |  | Correction factors |  |  | S/4 only entity — no ECC CDC mapping |
| `ForecastModelIsReset` |  |  |  | `Boolean` |  | Reset automatically |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `ProductPlantInternationalTrade`

- **ABAP Name:** `I_ProductPlantIntlTrd`
- **Label:** Product Plant Intrntionl Trade
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  | `String(40)` | Y | Product |  |  | S/4 only entity — no ECC CDC mapping |
| `Plant` |  |  |  | `String(4)` | Y | Plant |  |  | S/4 only entity — no ECC CDC mapping |
| `CountryOfOrigin` |  |  |  | `String(3)` |  | Country/Region of Origin |  |  | S/4 only entity — no ECC CDC mapping |
| `RegionOfOrigin` |  |  |  | `String(3)` |  | Region of Origin |  |  | S/4 only entity — no ECC CDC mapping |
| `ConsumptionTaxCtrlCode` |  |  |  | `String(16)` |  | Control Code |  |  | S/4 only entity — no ECC CDC mapping |
| `ExportAndImportProductGroup` |  |  |  | `String(4)` |  | Intrastat Group |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductCASNumber` |  |  |  | `String(15)` |  | CAS number (pharm.) |  |  | S/4 only entity — no ECC CDC mapping |
| `CommoditiyCodeNumberUnit` |  |  |  | `String(3)` |  | Commodity code unit |  |  | S/4 only entity — no ECC CDC mapping |
| `ProdIntlTradeClassification` |  |  |  | `String(9)` |  | PRODCOM no. |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `ProductPlantProcurement`

- **ABAP Name:** `I_Productplantprocurement`
- **Label:** Product Plant Procurement
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  | `String(40)` | Y | Product |  |  | S/4 only entity — no ECC CDC mapping |
| `Plant` |  |  |  | `String(4)` | Y | Plant |  |  | S/4 only entity — no ECC CDC mapping |
| `IsAutoPurOrdCreationAllowed` |  |  |  | `Boolean` |  | Automatic PO |  |  | S/4 only entity — no ECC CDC mapping |
| `IsSourceListRequired` |  |  |  | `Boolean` |  | Source list |  |  | S/4 only entity — no ECC CDC mapping |
| `IsPurgAcrossPurgGroup` |  |  |  | `Boolean` |  | Across Purch.Group |  |  | S/4 only entity — no ECC CDC mapping |
| `SourceOfSupplyCategory` |  |  |  | `String(1)` |  | Source of supply |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchasingGroup` |  |  |  | `String(3)` |  | Purchasing Group |  |  | S/4 only entity — no ECC CDC mapping |
| `IsActiveEntity` |  |  |  | `Boolean` |  | Is active |  |  | S/4 only entity — no ECC CDC mapping |
| `ProposedProductSupplyArea` |  |  |  | `String(10)` |  | Proposed Supply Area |  |  | S/4 only entity — no ECC CDC mapping |
| `ItmIsRlvtToJITDelivSchedules` |  |  |  | `String(1)` |  | JIT Delivery |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `ProductPlantPurchaseTax`

- **ABAP Name:** `I_ProductPurchaseTax`
- **Label:** Product Purchase Tax
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  | `String(40)` | Y | Product |  | _Product | S/4 only entity — no ECC CDC mapping |
| `SourceLocationCountry` |  |  |  | `String(3)` | Y | Departure Ctry/Reg. |  |  | S/4 only entity — no ECC CDC mapping |
| `TaxIndicator` |  |  |  | `String(1)` |  | Tax ind. f. material |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `ProductPlantQualityManagement`

- **ABAP Name:** `I_Productplantqtmanagement`
- **Label:** Product Plant QM
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  | `String(40)` | Y | Product |  |  | S/4 only entity — no ECC CDC mapping |
| `Plant` |  |  |  | `String(4)` | Y | Plant |  |  | S/4 only entity — no ECC CDC mapping |
| `MaximumStoragePeriod` |  |  |  | `Decimal(5,0)` |  | Max. Storage Period |  |  | S/4 only entity — no ECC CDC mapping |
| `QualityMgmtCtrlKey` |  |  |  | `String(8)` |  | QM Control Key |  |  | S/4 only entity — no ECC CDC mapping |
| `MatlQualityAuthorizationGroup` |  |  |  | `String(6)` |  | QM Material Auth. |  |  | S/4 only entity — no ECC CDC mapping |
| `HasPostToInspectionStock` |  |  |  | `Boolean` |  | Post to insp. stock |  |  | S/4 only entity — no ECC CDC mapping |
| `IsActiveEntity` |  |  |  | `Boolean` |  | Is active |  |  | S/4 only entity — no ECC CDC mapping |
| `InspLotDocumentationIsRequired` |  |  |  | `Boolean` |  | Documentation reqd |  |  | S/4 only entity — no ECC CDC mapping |
| `SuplrQualityManagementSystem` |  |  |  | `String(4)` |  | Target QM System |  |  | S/4 only entity — no ECC CDC mapping |
| `RecrrgInspIntervalTimeInDays` |  |  |  | `Decimal(5,0)` |  | Inspection Interval |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductQualityCertificateType` |  |  |  | `String(4)` |  | Certificate Type |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductPlantHasInspectionSetup` |  |  |  | `Boolean` |  | Inspection Setup |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `ProductPlantStorage`

- **ABAP Name:** `I_Productplantstorage`
- **Label:** Product plant storage
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  | `String(40)` | Y | Product |  |  | S/4 only entity — no ECC CDC mapping |
| `Plant` |  |  |  | `String(4)` | Y | Plant |  |  | S/4 only entity — no ECC CDC mapping |
| `InventoryForCycleCountInd` |  |  |  | `String(1)` |  | CC Phys. Inv. Ind. |  |  | S/4 only entity — no ECC CDC mapping |
| `MaximumStoragePeriod` |  |  |  | `Decimal(5,0)` |  | Max. Storage Period |  |  | S/4 only entity — no ECC CDC mapping |
| `ProvisioningServiceLevel` |  |  |  | `String(1)` |  | Service Level |  |  | S/4 only entity — no ECC CDC mapping |
| `IsActiveEntity` |  |  |  | `Boolean` |  | Is active |  |  | S/4 only entity — no ECC CDC mapping |
| `ProdMaximumStoragePeriodUnit` |  |  |  | `String(3)` |  | Time unit |  |  | S/4 only entity — no ECC CDC mapping |
| `WrhsMgmtPtwyAndStkRemovalStrgy` |  |  |  | `String(1)` |  | Putaway/StkRmvl |  |  | S/4 only entity — no ECC CDC mapping |
| `CycleCountingIndicatorIsFixed` |  |  |  | `Boolean` |  | CC indicator fixed |  |  | S/4 only entity — no ECC CDC mapping |
| `SegmentationStrategyForPlant` |  |  |  | `String(8)` |  | Segment. Strategy |  |  | S/4 only entity — no ECC CDC mapping |
| `DefaultSegmentValue` |  |  |  | `String(40)` |  | Stock Segment |  |  | S/4 only entity — no ECC CDC mapping |
| `SgmtHasPrioInProductStockSort` |  |  |  | `Boolean` |  | Sort Stock |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `ProductPlantSupplyPlanning`

- **ABAP Name:** `I_ProductPlantSupplyPlanning`
- **Label:** Product Plant Supply Planning
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  | `String(40)` | Y | Product |  | _Product | S/4 only entity — no ECC CDC mapping |
| `Plant` |  |  |  | `String(4)` | Y | Plant |  |  | S/4 only entity — no ECC CDC mapping |
| `FixedLotSizeQuantity` |  |  |  | `Decimal(13,3)` |  | Fixed lot size | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `MaximumLotSizeQuantity` |  |  |  | `Decimal(13,3)` |  | Maximum Lot Size | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `MinimumLotSizeQuantity` |  |  |  | `Decimal(13,3)` |  | Minimum Lot Size | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `LotSizeRoundingQuantity` |  |  |  | `Decimal(13,3)` |  | Rounding value | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `LotSizingProcedure` |  |  |  | `String(2)` |  | Lot Sizing Procedure |  |  | S/4 only entity — no ECC CDC mapping |
| `MRPType` |  |  |  | `String(2)` |  | MRP Type |  |  | S/4 only entity — no ECC CDC mapping |
| `MRPResponsible` |  |  |  | `String(3)` |  | MRP Controller |  |  | S/4 only entity — no ECC CDC mapping |
| `SafetyStockQuantity` |  |  |  | `Decimal(13,3)` |  | Safety Stock | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `MinimumSafetyStockQuantity` |  |  |  | `Decimal(13,3)` |  | Min. Saf. Stock | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `PlanningTimeFence` |  |  |  | `String(3)` |  | Planning time fence |  |  | S/4 only entity — no ECC CDC mapping |
| `ConsumptionValueCategory` |  |  |  | `String(1)` |  | ABC Indicator |  |  | S/4 only entity — no ECC CDC mapping |
| `MaximumStockQuantity` |  |  |  | `Decimal(13,3)` |  | Maximum Stock Level | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `ReorderThresholdQuantity` |  |  |  | `Decimal(13,3)` |  | Reorder Point | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `PlannedDeliveryDurationInDays` |  |  |  | `Decimal(3,0)` |  | Planned Deliv. Time |  |  | S/4 only entity — no ECC CDC mapping |
| `SafetySupplyDurationInDays` |  |  |  | `String(2)` |  | Safety Time |  |  | S/4 only entity — no ECC CDC mapping |
| `PlanningStrategyGroup` |  |  |  | `String(2)` |  | Strategy Group |  |  | S/4 only entity — no ECC CDC mapping |
| `TotalReplenishmentLeadTime` |  |  |  | `Decimal(3,0)` |  | Tot. repl. lead time |  |  | S/4 only entity — no ECC CDC mapping |
| `ProcurementType` |  |  |  | `String(1)` |  | Procurement Type |  |  | S/4 only entity — no ECC CDC mapping |
| `ProcurementSubType` |  |  |  | `String(2)` |  | Special Procurement |  |  | S/4 only entity — no ECC CDC mapping |
| `AssemblyScrapPercent` |  |  |  | `Decimal(5,2)` |  | Assembly scrap (%) |  |  | S/4 only entity — no ECC CDC mapping |
| `AvailabilityCheckType` |  |  |  | `String(2)` |  | Availability check |  |  | S/4 only entity — no ECC CDC mapping |
| `GoodsReceiptDuration` |  |  |  | `Decimal(3,0)` |  | GR processing time |  |  | S/4 only entity — no ECC CDC mapping |
| `PlanAndOrderDayDetermination` |  |  |  | `String(3)` |  | Planning Cycle |  |  | S/4 only entity — no ECC CDC mapping |
| `RoundingProfile` |  |  |  | `String(4)` |  | Rounding Profile |  |  | S/4 only entity — no ECC CDC mapping |
| `DfltStorageLocationExtProcmt` |  |  |  | `String(4)` |  | Storage Location |  |  | S/4 only entity — no ECC CDC mapping |
| `GoodIssueProcessingDays` |  |  |  | `Decimal(3,0)` |  | GI Proc. Time |  |  | S/4 only entity — no ECC CDC mapping |
| `ConsignmentControl` |  |  |  | `String(1)` |  | Consign.Control |  |  | S/4 only entity — no ECC CDC mapping |
| `IsActiveEntity` |  |  |  | `Boolean` |  | Is active |  |  | S/4 only entity — no ECC CDC mapping |
| `MRPGroup` |  |  |  | `String(4)` |  | MRP Group |  |  | S/4 only entity — no ECC CDC mapping |
| `LotSizeIndependentCosts` |  |  |  | `Decimal(34,4)` |  | LS-Independent Costs | Currency |  | S/4 only entity — no ECC CDC mapping |
| `StorageCostsPercentageCode` |  |  |  | `String(1)` |  | Storage Costs Code |  |  | S/4 only entity — no ECC CDC mapping |
| `RqmtQtyRcptTaktTmeInWrkgDays` |  |  |  | `Decimal(3,0)` |  | Takt time |  |  | S/4 only entity — no ECC CDC mapping |
| `MRPPlanningCalendar` |  |  |  | `String(3)` |  | Planning Calendar |  |  | S/4 only entity — no ECC CDC mapping |
| `RangeOfCvrgPrflCode` |  |  |  | `String(3)` |  | Coverage Profile |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductSafetyTimeMRPRelevance` |  |  |  | `String(1)` |  | Safety Time Ind |  |  | S/4 only entity — no ECC CDC mapping |
| `SafetyTimePeriodProfile` |  |  |  | `String(3)` |  | Time Profile |  |  | S/4 only entity — no ECC CDC mapping |
| `DependentRqmtMRPRelevance` |  |  |  | `String(1)` |  | MRP Relevant |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductServiceLevelInPercent` |  |  |  | `Decimal(3,1)` |  | Service level (%) |  |  | S/4 only entity — no ECC CDC mapping |
| `ProdInhProdnDurationInWorkDays` |  |  |  | `Decimal(3,0)` |  | In-house production |  |  | S/4 only entity — no ECC CDC mapping |
| `MRPAvailabilityType` |  |  |  | `String(1)` |  | Mixed MRP |  |  | S/4 only entity — no ECC CDC mapping |
| `CrossProjectProduct` |  |  |  | `String(1)` |  | Cross-Project |  |  | S/4 only entity — no ECC CDC mapping |
| `ProdnPlngAndControlCalendar` |  |  |  | `String(3)` |  | Planning Calendar |  |  | S/4 only entity — no ECC CDC mapping |
| `FollowUpProduct` |  |  |  | `String(40)` |  | Follow-Up Material |  |  | S/4 only entity — no ECC CDC mapping |
| `RepetitiveManufacturingIsAllwd` |  |  |  | `Boolean` |  | Repetitive Manufacturing Enabled |  |  | S/4 only entity — no ECC CDC mapping |
| `DependentRequirementsType` |  |  |  | `String(1)` |  | Indiv./ Coll. |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductIsBulkComponent` |  |  |  | `Boolean` |  | Bulk Material |  |  | S/4 only entity — no ECC CDC mapping |
| `RepetitiveManufacturingProfile` |  |  |  | `String(4)` |  | Repetitive Manufacturing Profile |  |  | S/4 only entity — no ECC CDC mapping |
| `BackwardCnsmpnPeriodInWorkDays` |  |  |  | `String(3)` |  | Backward Consumption Period |  |  | S/4 only entity — no ECC CDC mapping |
| `FwdConsumptionPeriodInWorkDays` |  |  |  | `String(3)` |  | Forward Consumption Period |  |  | S/4 only entity — no ECC CDC mapping |
| `ProdRqmtsConsumptionMode` |  |  |  | `String(1)` |  | Consumption mode |  |  | S/4 only entity — no ECC CDC mapping |
| `ProdFcstRequirementsSplitCode` |  |  |  | `String(1)` |  | Splitting Indicator |  |  | S/4 only entity — no ECC CDC mapping |
| `EffectiveOutDate` |  |  |  | `Date` |  | Effective-Out Date |  |  | S/4 only entity — no ECC CDC mapping |
| `MRPProfile` |  |  |  | `String(4)` |  | MRP profile |  |  | S/4 only entity — no ECC CDC mapping |
| `SchedulingFloatProfile` |  |  |  | `String(3)` |  | Scheduling Float Profile |  |  | S/4 only entity — no ECC CDC mapping |
| `ComponentScrapInPercent` |  |  |  | `Decimal(5,2)` |  | Component Scrap (%) |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductDiscontinuationCode` |  |  |  | `String(1)` |  | Discontinuation ind. |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductRequirementsGrouping` |  |  |  | `String(1)` |  | Requirements group |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductionInvtryManagedLoc` |  |  |  | `String(4)` |  | Storage Location |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductComponentBackflushCode` |  |  |  | `String(1)` |  | Backflush |  |  | S/4 only entity — no ECC CDC mapping |
| `ProposedProductSupplyArea` |  |  |  | `String(10)` |  | Proposed Supply Area |  |  | S/4 only entity — no ECC CDC mapping |
| `PlannedOrderActionControl` |  |  |  | `String(2)` |  | Action Control |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductUnitGroup` |  |  |  | `String(4)` |  | Unit of Measure Group |  |  | S/4 only entity — no ECC CDC mapping |
| `MRPSafetyStockMethod` |  |  |  | `String(2)` |  | Safety Stock Method |  |  | S/4 only entity — no ECC CDC mapping |
| `JITProdnConfProfile` |  |  |  | `String(4)` |  | JIT Production Confirmation Profile |  |  | S/4 only entity — no ECC CDC mapping |
| `Currency` |  |  |  | `String(5)` |  | Currency |  |  | S/4 only entity — no ECC CDC mapping |
| `CompanyCode` |  |  |  | `String(4)` |  | Company Code |  |  | S/4 only entity — no ECC CDC mapping |
| `ValuationArea` |  |  |  | `String(4)` |  | Valuation Area |  |  | S/4 only entity — no ECC CDC mapping |
| `BaseUnit` |  |  |  | `String(3)` |  | Base Unit of Measure |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `ProductPlantWorkScheduling`

- **ABAP Name:** `I_ProductWorkScheduling`
- **Label:** Product WorkScheduling core entity
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  | `String(40)` | Y | Product |  |  | S/4 only entity — no ECC CDC mapping |
| `Plant` |  |  |  | `String(4)` | Y | Plant |  |  | S/4 only entity — no ECC CDC mapping |
| `MaterialBaseQuantity` |  |  |  | `Decimal(13,3)` |  | Base quantity | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `UnlimitedOverDelivIsAllowed` |  |  |  | `Boolean` |  | Unltd Overdelivery |  |  | S/4 only entity — no ECC CDC mapping |
| `OverDelivToleranceLimit` |  |  |  | `Decimal(3,1)` |  | Overdelivery Toler. |  |  | S/4 only entity — no ECC CDC mapping |
| `UnderDelivToleranceLimit` |  |  |  | `Decimal(3,1)` |  | Underdelivery Toler. |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductionInvtryManagedLoc` |  |  |  | `String(4)` |  | Storage Location |  |  | S/4 only entity — no ECC CDC mapping |
| `IsActiveEntity` |  |  |  | `Boolean` |  | Is active |  |  | S/4 only entity — no ECC CDC mapping |
| `ProdnOrderIsBatchRequired` |  |  |  | `String(1)` |  | Batch entry |  |  | S/4 only entity — no ECC CDC mapping |
| `ProdIsWithdrawnFrmProdnBin` |  |  |  | `Boolean` |  | Withdr.from prod.bin |  |  | S/4 only entity — no ECC CDC mapping |
| `TransitionMatrixProductsGroup` |  |  |  | `String(20)` |  | Material Grouping |  |  | S/4 only entity — no ECC CDC mapping |
| `OrderChangeManagementProfile` |  |  |  | `String(6)` |  | Change overall prof. |  |  | S/4 only entity — no ECC CDC mapping |
| `MatlCompIsMarkedForBackflush` |  |  |  | `String(1)` |  | Backflush |  |  | S/4 only entity — no ECC CDC mapping |
| `SetupAndTeardownTime` |  |  |  | `Decimal(5,2)` |  | Setup time |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductionSchedulingProfile` |  |  |  | `String(6)` |  | Production Scheduling Profile |  |  | S/4 only entity — no ECC CDC mapping |
| `TransitionTime` |  |  |  | `Decimal(5,2)` |  | Interoperation |  |  | S/4 only entity — no ECC CDC mapping |
| `ProcessingTimeInDays` |  |  |  | `Decimal(5,2)` |  | Processing time |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductionSupervisor` |  |  |  | `String(3)` |  | Prodn Supervisor |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductProductionQuantityUnit` |  |  |  | `String(3)` |  | Production unit |  |  | S/4 only entity — no ECC CDC mapping |
| `HasProductionVersion` |  |  |  | `Boolean` |  | Version Indicator |  |  | S/4 only entity — no ECC CDC mapping |
| `BaseUnit` |  |  |  | `String(3)` |  | Base Unit of Measure |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `ProductProcurement`

- **ABAP Name:** `I_Productprocurement`
- **Label:** Product Procurement
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  | `String(40)` | Y | Material |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchaseOrderQuantityUnit` |  |  |  | `String(3)` |  | Order Unit |  |  | S/4 only entity — no ECC CDC mapping |
| `VarblPurOrdUnitStatus` |  |  |  | `String(1)` |  | Var. Order Unit |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchasingAcknProfile` |  |  |  | `String(4)` |  | Purchasing value key |  |  | S/4 only entity — no ECC CDC mapping |
| `ProcurementRule` |  |  |  | `String(1)` |  | Procurement rule |  |  | S/4 only entity — no ECC CDC mapping |
| `SourceOfSupplyCategory` |  |  |  | `String(1)` |  | Source of supply |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchasingGroup` |  |  |  | `String(3)` |  | Purchasing Group |  |  | S/4 only entity — no ECC CDC mapping |
| `IsActiveEntity` |  |  |  | `Boolean` |  | Is active |  |  | S/4 only entity — no ECC CDC mapping |
| `AuthorizationGroup` |  |  |  | `String(4)` |  | Authorization Group |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `ProductQualityManagement`

- **ABAP Name:** `I_Productqm`
- **Label:** Product QM active core entity
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  | `String(40)` | Y | Product |  |  | S/4 only entity — no ECC CDC mapping |
| `QltyMgmtInProcmtIsActive` |  |  |  | `Boolean` |  | QM in Procur. Active |  |  | S/4 only entity — no ECC CDC mapping |
| `AuthorizationGroup` |  |  |  | `String(4)` |  | Authorization Group |  |  | S/4 only entity — no ECC CDC mapping |
| `CatalogProfile` |  |  |  | `String(9)` |  | Catalog Profile |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `ProductSales`

- **ABAP Name:** `I_ProductSales`
- **Label:** Product Sales
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  | `String(40)` | Y | Material |  |  | S/4 only entity — no ECC CDC mapping |
| `SalesStatus` |  |  |  | `String(2)` |  | X-DChain Status |  |  | S/4 only entity — no ECC CDC mapping |
| `SalesStatusValidityDate` |  |  |  | `Date` |  | Cross-Distr. Chain Product Validity |  |  | S/4 only entity — no ECC CDC mapping |
| `TaxClassification` |  |  |  | `String(1)` |  | Tax classification |  |  | S/4 only entity — no ECC CDC mapping |
| `TransportationGroup` |  |  |  | `String(4)` |  | Transportation Group |  |  | S/4 only entity — no ECC CDC mapping |
| `AllowedPackagingWeightQty` |  |  |  | `Decimal(13,3)` |  | Allowed Pkg wt | AllowedPackagingWeightQtyUnit |  | S/4 only entity — no ECC CDC mapping |
| `AllowedPackagingWeightQtyUnit` |  |  |  | `String(3)` |  | Allowed Packaging Unit of Weight |  |  | S/4 only entity — no ECC CDC mapping |
| `AllowedPackagingVolumeQty` |  |  |  | `Decimal(13,3)` |  | Allowed Volume | AllowedPackagingVolumeQtyUnit |  | S/4 only entity — no ECC CDC mapping |
| `AllowedPackagingVolumeQtyUnit` |  |  |  | `String(3)` |  | Allowed Packaging Unit of Volume |  |  | S/4 only entity — no ECC CDC mapping |
| `PricingReferenceProduct` |  |  |  | `String(40)` |  | Pricing Ref. Matl |  | _PricingReferenceProduct | S/4 only entity — no ECC CDC mapping |
| `VariantsPricingProfile` |  |  |  | `String(1)` |  | Pricing profile |  |  | S/4 only entity — no ECC CDC mapping |
| `IsVariantPriceAllowed` |  |  |  | `Boolean` |  | Var. Price Allowed |  |  | S/4 only entity — no ECC CDC mapping |
| `LoadingGroup` |  |  |  | `String(4)` |  | Loading Group |  |  | S/4 only entity — no ECC CDC mapping |
| `IsActiveEntity` |  |  |  | `Boolean` |  | Is active |  |  | S/4 only entity — no ECC CDC mapping |
| `ExcessWeightTolerance` |  |  |  | `Decimal(3,1)` |  | Excess Weight Tolerance |  |  | S/4 only entity — no ECC CDC mapping |
| `ExcessVolumeTolerance` |  |  |  | `Decimal(3,1)` |  | Excess Volume Tolerance |  |  | S/4 only entity — no ECC CDC mapping |
| `PackagingMaterialType` |  |  |  | `String(4)` |  | Packaging Material Type |  |  | S/4 only entity — no ECC CDC mapping |
| `IsClosedPackagingMaterial` |  |  |  | `Boolean` |  | Closed |  |  | S/4 only entity — no ECC CDC mapping |
| `VolumeMaximumLevel` |  |  |  | `Decimal(3,0)` |  | Maximum level |  |  | S/4 only entity — no ECC CDC mapping |
| `AuthorizationGroup` |  |  |  | `String(4)` |  | Authorization Group |  |  | S/4 only entity — no ECC CDC mapping |
| `MaterialFreightGroup` |  |  |  | `String(8)` |  | Material Freight Grp |  |  | S/4 only entity — no ECC CDC mapping |
| `StackingFactor` |  |  |  | `Integer` |  | Stackability factor |  |  | S/4 only entity — no ECC CDC mapping |
| `ServiceDuration` |  |  |  | `Decimal(13,3)` |  | Duration of Work |  |  | S/4 only entity — no ECC CDC mapping |
| `ServiceDurationUnit` |  |  |  | `String(3)` |  | Unit |  |  | S/4 only entity — no ECC CDC mapping |
| `ServiceProfile` |  |  |  | `String(10)` |  | Service Profile |  |  | S/4 only entity — no ECC CDC mapping |
| `ResponseProfile` |  |  |  | `String(10)` |  | Response Prof. |  |  | S/4 only entity — no ECC CDC mapping |
| `CABillgCycle` |  |  |  | `String(4)` |  | Billing Cycle |  |  | S/4 only entity — no ECC CDC mapping |
| `SubscrpnProdBillgCycDetn` |  |  |  | `String(4)` |  | Billing Cycle Determ |  |  | S/4 only entity — no ECC CDC mapping |
| `SubscrpnProdTechRsceSchema` |  |  |  | `String(2)` |  | Assignment Schema |  |  | S/4 only entity — no ECC CDC mapping |
| `ContractAutoRenewalType` |  |  |  | `String(1)` |  | Ctr. Auto Renew Ind. |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `ProductSalesDelivery`

- **ABAP Name:** `I_ProductSalesDelivery`
- **Label:** Product Sales Delivery
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  | `String(40)` | Y | Product |  | _Product | S/4 only entity — no ECC CDC mapping |
| `ProductSalesOrg` |  |  |  | `String(4)` | Y | Sales Organization |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductDistributionChnl` |  |  |  | `String(2)` | Y | Distribution Channel |  |  | S/4 only entity — no ECC CDC mapping |
| `MinimumOrderQuantity` |  |  |  | `Decimal(13,3)` |  | Minimum order qty | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `SupplyingPlant` |  |  |  | `String(4)` |  | Delivering Plant |  |  | S/4 only entity — no ECC CDC mapping |
| `PriceSpecificationProductGroup` |  |  |  | `String(2)` |  | Product Price Group |  |  | S/4 only entity — no ECC CDC mapping |
| `AccountDetnProductGroup` |  |  |  | `String(2)` |  | Acct Assmt Grp Mat. |  |  | S/4 only entity — no ECC CDC mapping |
| `DeliveryNoteProcMinDelivQty` |  |  |  | `Decimal(13,3)` |  | Minimum Delivery Qty | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `ItemCategoryGroup` |  |  |  | `String(4)` |  | Item Category Group |  |  | S/4 only entity — no ECC CDC mapping |
| `DeliveryQuantityUnit` |  |  |  | `String(3)` |  | Unit Of Measure |  |  | S/4 only entity — no ECC CDC mapping |
| `DeliveryQuantity` |  |  |  | `Decimal(13,3)` |  | Delivery unit | DeliveryQuantityUnit |  | S/4 only entity — no ECC CDC mapping |
| `ProductSalesStatus` |  |  |  | `String(2)` |  | DChain-spec. status |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductSalesStatusValidityDate` |  |  |  | `Date` |  | Valid from |  |  | S/4 only entity — no ECC CDC mapping |
| `SalesMeasureUnit` |  |  |  | `String(3)` |  | Sales Unit |  |  | S/4 only entity — no ECC CDC mapping |
| `IsMarkedForDeletion` |  |  |  | `Boolean` |  | DF distr. chain lvl |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductHierarchy` |  |  |  | `String(18)` |  | Product Hierarchy |  |  | S/4 only entity — no ECC CDC mapping |
| `FirstSalesSpecProductGroup` |  |  |  | `String(3)` |  | Product Group 1 |  |  | S/4 only entity — no ECC CDC mapping |
| `SecondSalesSpecProductGroup` |  |  |  | `String(3)` |  | Product Group 2 |  |  | S/4 only entity — no ECC CDC mapping |
| `ThirdSalesSpecProductGroup` |  |  |  | `String(3)` |  | Product Group 3 |  |  | S/4 only entity — no ECC CDC mapping |
| `FourthSalesSpecProductGroup` |  |  |  | `String(3)` |  | Product Group 4 |  |  | S/4 only entity — no ECC CDC mapping |
| `FifthSalesSpecProductGroup` |  |  |  | `String(3)` |  | Product Group 5 |  |  | S/4 only entity — no ECC CDC mapping |
| `MinimumMakeToOrderOrderQty` |  |  |  | `Decimal(13,3)` |  | Min. MtO quantity | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `LogisticsStatisticsGroup` |  |  |  | `String(1)` |  | Matl statistics grp |  |  | S/4 only entity — no ECC CDC mapping |
| `VolumeRebateGroup` |  |  |  | `String(2)` |  | Volume Rebate Group |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductCommissionGroup` |  |  |  | `String(2)` |  | Commission Group |  |  | S/4 only entity — no ECC CDC mapping |
| `CashDiscountIsDeductible` |  |  |  | `Boolean` |  | Cash Discount |  |  | S/4 only entity — no ECC CDC mapping |
| `PricingReferenceProduct` |  |  |  | `String(40)` |  | Pricing Ref. Matl |  |  | S/4 only entity — no ECC CDC mapping |
| `AssortmentGrade` |  |  |  | `String(2)` |  | Assortment Grade |  |  | S/4 only entity — no ECC CDC mapping |
| `StoreListingProcedure` |  |  |  | `String(2)` |  | LP for Stores |  |  | S/4 only entity — no ECC CDC mapping |
| `DistrCntrListingProcedure` |  |  |  | `String(2)` |  | LP distr. ctrs |  |  | S/4 only entity — no ECC CDC mapping |
| `StoreListingStartDate` |  |  |  | `Date` |  | Store Listed from |  |  | S/4 only entity — no ECC CDC mapping |
| `StoreListingEndDate` |  |  |  | `Date` |  | Store Listed to |  |  | S/4 only entity — no ECC CDC mapping |
| `DistrCntrListingStartDate` |  |  |  | `Date` |  | DC Listed from |  |  | S/4 only entity — no ECC CDC mapping |
| `DistrCntrListingEndDate` |  |  |  | `Date` |  | DC Listed to |  |  | S/4 only entity — no ECC CDC mapping |
| `StoreSaleStartDate` |  |  |  | `Date` |  | For sale from (str) |  |  | S/4 only entity — no ECC CDC mapping |
| `StoreSaleEndDate` |  |  |  | `Date` |  | For sale till (str) |  |  | S/4 only entity — no ECC CDC mapping |
| `DistrCntrSaleStartDate` |  |  |  | `Date` |  | For sale from (DC) |  |  | S/4 only entity — no ECC CDC mapping |
| `DistrCntrSaleEndDate` |  |  |  | `Date` |  | For sale till (DC) |  |  | S/4 only entity — no ECC CDC mapping |
| `RoundingProfile` |  |  |  | `String(4)` |  | Rounding Profile |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductUnitGroup` |  |  |  | `String(4)` |  | Unit of Measure Grp |  |  | S/4 only entity — no ECC CDC mapping |
| `MaxDeliveryQtyStoreOrder` |  |  |  | `Decimal(13,3)` |  | Max. delivery qty | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `PriceFixingCategory` |  |  |  | `String(1)` |  | Price fixing |  |  | S/4 only entity — no ECC CDC mapping |
| `VariableSalesUnitIsNotAllowed` |  |  |  | `Boolean` |  | Sales unit not var. |  |  | S/4 only entity — no ECC CDC mapping |
| `CompetitionPressureCategory` |  |  |  | `String(1)` |  | Competition charactn |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductHasAttributeID01` |  |  |  | `Boolean` |  | Product Attribute 1 |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductHasAttributeID02` |  |  |  | `Boolean` |  | Product Attribute 2 |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductHasAttributeID03` |  |  |  | `Boolean` |  | Product Attribute 3 |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductHasAttributeID04` |  |  |  | `Boolean` |  | Product Attribute 4 |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductHasAttributeID05` |  |  |  | `Boolean` |  | Product Attribute 5 |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductHasAttributeID06` |  |  |  | `Boolean` |  | Product Attribute 6 |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductHasAttributeID07` |  |  |  | `Boolean` |  | Product Attribute 7 |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductHasAttributeID08` |  |  |  | `Boolean` |  | Product Attribute 8 |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductHasAttributeID09` |  |  |  | `Boolean` |  | Product Attribute 9 |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductHasAttributeID10` |  |  |  | `Boolean` |  | Product Attribute 10 |  |  | S/4 only entity — no ECC CDC mapping |
| `IsActiveEntity` |  |  |  | `Boolean` |  | Is active |  |  | S/4 only entity — no ECC CDC mapping |
| `ProdExtAssortmentPriority` |  |  |  | `String(1)` |  | Ext. asst priority |  |  | S/4 only entity — no ECC CDC mapping |
| `ProdIsEntlmntRlvt` |  |  |  | `Boolean` |  | Rel. Entitlement Gen |  |  | S/4 only entity — no ECC CDC mapping |
| `BaseUnit` |  |  |  | `String(3)` |  | Base Unit of Measure |  |  | S/4 only entity — no ECC CDC mapping |
| `SubscrpnContrDfltDuration` |  |  |  | `String(3)` |  | Def Contract Term |  |  | S/4 only entity — no ECC CDC mapping |
| `SubscrpnContrAltvDuration1` |  |  |  | `String(3)` |  | Contract Term 1 |  |  | S/4 only entity — no ECC CDC mapping |
| `SubscrpnContrAltvDuration2` |  |  |  | `String(3)` |  | Contract Term 2 |  |  | S/4 only entity — no ECC CDC mapping |
| `SubscrpnContrDurationUnit` |  |  |  | `String(1)` |  | Unit Contract Term |  |  | S/4 only entity — no ECC CDC mapping |
| `SubscrpnContrDfltExtnDurn` |  |  |  | `String(3)` |  | Def Extension Period |  |  | S/4 only entity — no ECC CDC mapping |
| `SubscrpnContrAltvExtnDurn1` |  |  |  | `String(3)` |  | Extension Period 1 |  |  | S/4 only entity — no ECC CDC mapping |
| `SubscrpnContrAltvExtnDurn2` |  |  |  | `String(3)` |  | Extension Period 2 |  |  | S/4 only entity — no ECC CDC mapping |
| `SubscrpnContrExtnDurnUnit` |  |  |  | `String(1)` |  | Unit for Extension |  |  | S/4 only entity — no ECC CDC mapping |
| `LstMiProductPackageSizeCode` |  |  |  | `String(3)` |  | Package Size |  |  | S/4 only entity — no ECC CDC mapping |
| `LstMiProductPackageType` |  |  |  | `String(3)` |  | Package Type |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `ProductStorage`

- **ABAP Name:** `I_ProductStorage_2`
- **Label:** Product Storage
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  | `String(40)` | Y | Material |  |  | S/4 only entity — no ECC CDC mapping |
| `StorageConditions` |  |  |  | `String(2)` |  | Storage conditions |  | _Storagecondition | S/4 only entity — no ECC CDC mapping |
| `TemperatureConditionInd` |  |  |  | `String(2)` |  | Temp. conditions |  |  | S/4 only entity — no ECC CDC mapping |
| `HazardousMaterialNumber` |  |  |  | `String(40)` |  | Haz. material number |  |  | S/4 only entity — no ECC CDC mapping |
| `NmbrOfGROrGISlipsToPrintQty` |  |  |  | `Decimal(13,3)` |  | GR slips quantity | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `LabelType` |  |  |  | `String(2)` |  | Label type |  |  | S/4 only entity — no ECC CDC mapping |
| `LabelForm` |  |  |  | `String(2)` |  | Label form |  |  | S/4 only entity — no ECC CDC mapping |
| `MinRemainingShelfLife` |  |  |  | `Decimal(4,0)` |  | Min. Rem. Shelf Life |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductExpirationDateCode` |  |  |  | `String(1)` |  | Expiration Date |  |  | S/4 only entity — no ECC CDC mapping |
| `StorageBinInstruction` |  |  |  | `String(2)` |  | Container reqmts |  |  | S/4 only entity — no ECC CDC mapping |
| `TotalShelfLifeStoragePercent` |  |  |  | `Decimal(3,0)` |  | Storage percentage |  |  | S/4 only entity — no ECC CDC mapping |
| `ShelfLifeExpirationDatePeriod` |  |  |  | `String(1)` |  | Period Ind. for SLED |  |  | S/4 only entity — no ECC CDC mapping |
| `ShelfLifeExprtnDateRndngRule` |  |  |  | `String(1)` |  | Rounding rule SLED |  |  | S/4 only entity — no ECC CDC mapping |
| `AuthorizationGroup` |  |  |  | `String(4)` |  | Authorization Group |  |  | S/4 only entity — no ECC CDC mapping |
| `IsActiveEntity` |  |  |  | `Boolean` |  | Is active |  |  | S/4 only entity — no ECC CDC mapping |
| `TotalShelfLife` |  |  |  | `Decimal(4,0)` |  | Total Shelf Life |  |  | S/4 only entity — no ECC CDC mapping |
| `BaseUnit` |  |  |  | `String(3)` |  | Base Unit of Measure |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `ProductUnitOfMeasure`

- **ABAP Name:** `I_ProductUnitsOfMeasure`
- **Label:** Units of Measure of Product
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  | `String(40)` | Y | Product |  |  | S/4 only entity — no ECC CDC mapping |
| `AlternativeUnit` |  |  |  | `String(3)` | Y | AlternativeUnit |  |  | S/4 only entity — no ECC CDC mapping |
| `QuantityNumerator` |  |  |  | `Decimal(5,0)` |  | Units / Quantity - Base Unit of Measure | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `QuantityDenominator` |  |  |  | `Decimal(5,0)` |  | Units / Quantity - Alt Unit of Measure | AlternativeUnit |  | S/4 only entity — no ECC CDC mapping |
| `MaterialVolume` |  |  |  | `Decimal(13,3)` |  | Volume | VolumeUnit |  | S/4 only entity — no ECC CDC mapping |
| `VolumeUnit` |  |  |  | `String(3)` |  | Volume Unit |  |  | S/4 only entity — no ECC CDC mapping |
| `GrossWeight` |  |  |  | `Decimal(13,3)` |  | Gross Weight | WeightUnit |  | S/4 only entity — no ECC CDC mapping |
| `WeightUnit` |  |  |  | `String(3)` |  | Unit of Weight |  |  | S/4 only entity — no ECC CDC mapping |
| `GlobalTradeItemNumber` |  |  |  | `String(18)` |  | EAN/UPC |  |  | S/4 only entity — no ECC CDC mapping |
| `GlobalTradeItemNumberCategory` |  |  |  | `String(2)` |  | GTIN Category |  |  | S/4 only entity — no ECC CDC mapping |
| `UnitSpecificProductLength` |  |  |  | `Decimal(13,3)` |  | Length | ProductMeasurementUnit |  | S/4 only entity — no ECC CDC mapping |
| `UnitSpecificProductWidth` |  |  |  | `Decimal(13,3)` |  | Width | ProductMeasurementUnit |  | S/4 only entity — no ECC CDC mapping |
| `UnitSpecificProductHeight` |  |  |  | `Decimal(13,3)` |  | Height | ProductMeasurementUnit |  | S/4 only entity — no ECC CDC mapping |
| `ProductMeasurementUnit` |  |  |  | `String(3)` |  | Unit of Dimension |  |  | S/4 only entity — no ECC CDC mapping |
| `LowerLevelPackagingUnit` |  |  |  | `String(3)` |  | Lower-level unit |  |  | S/4 only entity — no ECC CDC mapping |
| `RemainingVolumeAfterNesting` |  |  |  | `Decimal(3,0)` |  | Rem.Vol.After Nestng |  |  | S/4 only entity — no ECC CDC mapping |
| `MaximumStackingFactor` |  |  |  | `Integer` |  | Max. Stacking Factor |  |  | S/4 only entity — no ECC CDC mapping |
| `CapacityUsage` |  |  |  | `Decimal(15,3)` |  | Capacity Usage |  |  | S/4 only entity — no ECC CDC mapping |
| `IsActiveEntity` |  |  |  | `Boolean` |  | Is active |  |  | S/4 only entity — no ECC CDC mapping |
| `UnitOfMeasureCategory` |  |  |  | `String(1)` |  | UoM Category |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductGTINVariant` |  |  |  | `String(2)` |  | EAN Variant |  |  | S/4 only entity — no ECC CDC mapping |
| `BaseUnit` |  |  |  | `String(3)` |  | Base Unit of Measure |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `ProductUnitOfMeasureEAN`

- **ABAP Name:** `I_ProductUnitOfMeasureEAN`
- **Label:** International Article Number of Product
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  | `String(40)` | Y | Material |  |  | S/4 only entity — no ECC CDC mapping |
| `AlternativeUnit` |  |  |  | `String(3)` | Y | Display Unit/Measure |  |  | S/4 only entity — no ECC CDC mapping |
| `ConsecutiveNumber` |  |  |  | `String(5)` | Y | Consecutive number |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductStandardID` |  |  |  | `String(18)` |  | EAN/UPC |  |  | S/4 only entity — no ECC CDC mapping |
| `InternationalArticleNumberCat` |  |  |  | `String(2)` |  | GTIN Category |  |  | S/4 only entity — no ECC CDC mapping |
| `IsMainGlobalTradeItemNumber` |  |  |  | `Boolean` |  | Main EAN |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `ProductValuation`

- **ABAP Name:** `I_ProductValuationBasic`
- **Label:** Product Valuation
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  | `String(40)` | Y | Product |  |  | S/4 only entity — no ECC CDC mapping |
| `ValuationArea` |  |  |  | `String(4)` | Y | Valuation Area |  |  | S/4 only entity — no ECC CDC mapping |
| `ValuationType` |  |  |  | `String(10)` | Y | Valuation Type |  |  | S/4 only entity — no ECC CDC mapping |
| `ValuationClass` |  |  |  | `String(4)` |  | Valuation Class |  |  | S/4 only entity — no ECC CDC mapping |
| `PriceDeterminationControl` |  |  |  | `String(1)` |  | Price Determ. |  |  | S/4 only entity — no ECC CDC mapping |
| `FiscalMonthCurrentPeriod` |  |  |  | `String(2)` |  | Current Period |  |  | S/4 only entity — no ECC CDC mapping |
| `FiscalYearCurrentPeriod` |  |  |  | `String(4)` |  | Year Current Period |  |  | S/4 only entity — no ECC CDC mapping |
| `StandardPrice` |  |  |  | `Decimal(34,4)` |  | Standard price | Currency |  | S/4 only entity — no ECC CDC mapping |
| `PriceUnitQty` |  |  |  | `Decimal(5,0)` |  | Price unit |  |  | S/4 only entity — no ECC CDC mapping |
| `InventoryValuationProcedure` |  |  |  | `String(1)` |  | Price Control |  |  | S/4 only entity — no ECC CDC mapping |
| `FuturePriceValidityStartDate` |  |  |  | `Date` |  | Valid from |  |  | S/4 only entity — no ECC CDC mapping |
| `PrevInvtryPriceInCoCodeCrcy` |  |  |  | `Decimal(34,4)` |  | Previous Price | Currency |  | S/4 only entity — no ECC CDC mapping |
| `MovingAveragePrice` |  |  |  | `Decimal(34,4)` |  | Moving price | Currency |  | S/4 only entity — no ECC CDC mapping |
| `ValuationCategory` |  |  |  | `String(1)` |  | Valuation Category |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductUsageType` |  |  |  | `String(1)` |  | Product Usage |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductOriginType` |  |  |  | `String(1)` |  | Product Origin |  |  | S/4 only entity — no ECC CDC mapping |
| `IsProducedInhouse` |  |  |  | `Boolean` |  | In-House Production |  |  | S/4 only entity — no ECC CDC mapping |
| `ProdCostEstNumber` |  |  |  | `String(12)` |  | ProdCostEst.No. |  |  | S/4 only entity — no ECC CDC mapping |
| `IsMarkedForDeletion` |  |  |  | `Boolean` |  | Del. flag val. type |  |  | S/4 only entity — no ECC CDC mapping |
| `ValuationMargin` |  |  |  | `Decimal(6,2)` |  | Valuation Margin |  |  | S/4 only entity — no ECC CDC mapping |
| `IsActiveEntity` |  |  |  | `Boolean` |  | Is active |  |  | S/4 only entity — no ECC CDC mapping |
| `CompanyCode` |  |  |  | `String(4)` |  | Company Code |  |  | S/4 only entity — no ECC CDC mapping |
| `ValuationClassSalesOrderStock` |  |  |  | `String(4)` |  | VC: Sales Order Stk |  |  | S/4 only entity — no ECC CDC mapping |
| `ProjectStockValuationClass` |  |  |  | `String(4)` |  | Proj. stk val. class |  |  | S/4 only entity — no ECC CDC mapping |
| `TaxBasedPricesPriceUnitQty` |  |  |  | `Decimal(5,0)` |  | Price Unit | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `PriceLastChangeDate` |  |  |  | `Date` |  | Last Price Change |  |  | S/4 only entity — no ECC CDC mapping |
| `FuturePrice` |  |  |  | `Decimal(34,4)` |  | Future Price | Currency |  | S/4 only entity — no ECC CDC mapping |
| `MaintenanceStatus` |  |  |  | `String(15)` |  | Maintenance Status |  |  | S/4 only entity — no ECC CDC mapping |
| `Currency` |  |  |  | `String(5)` |  | Currency |  |  | S/4 only entity — no ECC CDC mapping |
| `BaseUnit` |  |  |  | `String(3)` |  | Base Unit of Measure |  |  | S/4 only entity — no ECC CDC mapping |
| `MLIsActiveAtProductLevel` |  |  |  | `Boolean` |  | ML Act. |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `ProductValuationAccounting`

- **ABAP Name:** `I_ProductValuationAccounting_2`
- **Label:** Product Valuation Account
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  | `String(40)` | Y | Product |  |  | S/4 only entity — no ECC CDC mapping |
| `ValuationArea` |  |  |  | `String(4)` | Y | Valuation Area |  |  | S/4 only entity — no ECC CDC mapping |
| `ValuationType` |  |  |  | `String(10)` | Y | Valuation Type |  |  | S/4 only entity — no ECC CDC mapping |
| `CommercialPrice1InCoCodeCrcy` |  |  |  | `Decimal(34,4)` |  | Commercial price 1 | Currency |  | S/4 only entity — no ECC CDC mapping |
| `CommercialPrice2InCoCodeCrcy` |  |  |  | `Decimal(34,4)` |  | Commercial price 2 | Currency |  | S/4 only entity — no ECC CDC mapping |
| `CommercialPrice3InCoCodeCrcy` |  |  |  | `Decimal(34,4)` |  | Commercial price 3 | Currency |  | S/4 only entity — no ECC CDC mapping |
| `DevaluationYearCount` |  |  |  | `String(2)` |  | Devaluation Ind. |  |  | S/4 only entity — no ECC CDC mapping |
| `FuturePrice` |  |  |  | `Decimal(34,4)` |  | Future Price | Currency |  | S/4 only entity — no ECC CDC mapping |
| `FuturePriceValidityStartDate` |  |  |  | `Date` |  | Valid from |  |  | S/4 only entity — no ECC CDC mapping |
| `IsLIFOAndFIFORelevant` |  |  |  | `Boolean` |  | TRUE |  |  | S/4 only entity — no ECC CDC mapping |
| `LIFOValuationPoolNumber` |  |  |  | `String(4)` |  | LIFO Pool |  |  | S/4 only entity — no ECC CDC mapping |
| `StandardPricePrevYear` |  |  |  | `Decimal(34,4)` |  | Standard price | Currency |  | S/4 only entity — no ECC CDC mapping |
| `TaxPricel1InCoCodeCrcy` |  |  |  | `Decimal(34,4)` |  | Tax price 1 | Currency |  | S/4 only entity — no ECC CDC mapping |
| `TaxPrice2InCoCodeCrcy` |  |  |  | `Decimal(34,4)` |  | Tax price 2 | Currency |  | S/4 only entity — no ECC CDC mapping |
| `TaxPrice3InCoCodeCrcy` |  |  |  | `Decimal(34,4)` |  | Tax price 3 | Currency |  | S/4 only entity — no ECC CDC mapping |
| `TaxBasedPricesPriceUnitQty` |  |  |  | `Decimal(5,0)` |  | Price Unit | BaseUnit |  | S/4 only entity — no ECC CDC mapping |
| `CompanyCode` |  |  |  | `String(4)` |  | Company Code |  |  | S/4 only entity — no ECC CDC mapping |
| `Currency` |  |  |  | `String(5)` |  | Currency |  |  | S/4 only entity — no ECC CDC mapping |
| `BaseUnit` |  |  |  | `String(3)` |  | Base Unit of Measure |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `ProductValuationCosting`

- **ABAP Name:** `I_ProductValuationCosting`
- **Label:** Product Valuation Costing Core Entity
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  | `String(40)` | Y | Product |  |  | S/4 only entity — no ECC CDC mapping |
| `ValuationArea` |  |  |  | `String(4)` | Y | Valuation Area |  |  | S/4 only entity — no ECC CDC mapping |
| `ValuationType` |  |  |  | `String(10)` | Y | Valuation Type |  |  | S/4 only entity — no ECC CDC mapping |
| `IsMaterialCostedWithQtyStruc` |  |  |  | `Boolean` |  | With Qty Structure |  |  | S/4 only entity — no ECC CDC mapping |
| `IsMaterialRelatedOrigin` |  |  |  | `Boolean` |  | Material origin |  |  | S/4 only entity — no ECC CDC mapping |
| `CostOriginGroup` |  |  |  | `String(4)` |  | Origin Group |  |  | S/4 only entity — no ECC CDC mapping |
| `CostingOverheadGroup` |  |  |  | `String(10)` |  | Overhead Group |  |  | S/4 only entity — no ECC CDC mapping |
| `PlannedPrice1InCoCodeCrcy` |  |  |  | `Decimal(34,4)` |  | Planned price 1 | Currency |  | S/4 only entity — no ECC CDC mapping |
| `PlannedPrice2InCoCodeCrcy` |  |  |  | `Decimal(34,4)` |  | Planned price 2 | Currency |  | S/4 only entity — no ECC CDC mapping |
| `PlannedPrice3InCoCodeCrcy` |  |  |  | `Decimal(34,4)` |  | Planned price 3 | Currency |  | S/4 only entity — no ECC CDC mapping |
| `FuturePlndPrice1ValdtyDate` |  |  |  | `Date` |  | Planned price date 1 |  |  | S/4 only entity — no ECC CDC mapping |
| `FuturePlndPrice2ValdtyDate` |  |  |  | `Date` |  | Planned price date 2 |  |  | S/4 only entity — no ECC CDC mapping |
| `FuturePlndPrice3ValdtyDate` |  |  |  | `Date` |  | Planned price date 3 |  |  | S/4 only entity — no ECC CDC mapping |
| `PlannedPrice` |  |  |  | `Decimal(34,4)` |  | Future Planned Price | Currency |  | S/4 only entity — no ECC CDC mapping |
| `Currency` |  |  |  | `String(5)` |  | Currency |  |  | S/4 only entity — no ECC CDC mapping |
| `CompanyCode` |  |  |  | `String(4)` |  | Company Code |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `ProductWarehouseManagement`

- **ABAP Name:** `I_ProductWrhsMgmt`
- **Label:** Product Warehouse Management
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  | `String(40)` | Y | Product |  |  | S/4 only entity — no ECC CDC mapping |
| `WarehouseNumber` |  |  |  | `String(3)` | Y | Warehouse Number |  |  | S/4 only entity — no ECC CDC mapping |
| `ProdWrhsMatlDataIsMrkdForDeltn` |  |  |  | `Boolean` |  | Del.flag:warehse no. |  |  | S/4 only entity — no ECC CDC mapping |
| `ProdStorageSectionMethod` |  |  |  | `String(3)` |  | Storage Section Ind. |  |  | S/4 only entity — no ECC CDC mapping |
| `ProdWrhsStkPlacementStorType` |  |  |  | `String(3)` |  | Stock placement |  |  | S/4 only entity — no ECC CDC mapping |
| `ProdWrhsStkRemovalStorageType` |  |  |  | `String(3)` |  | Stock removal |  |  | S/4 only entity — no ECC CDC mapping |
| `ProdWrhs1stLoadgEquipQuantity` |  |  |  | `Decimal(13,3)` |  | Loading equip. qty 1 | ProdWrhs1stLoadgEquipQtyUnit |  | S/4 only entity — no ECC CDC mapping |
| `ProdWrhs2ndLoadgEquipQuantity` |  |  |  | `Decimal(13,3)` |  | Loading equip. qty 2 | ProdWrhs2ndLoadgEquipQtyUnit |  | S/4 only entity — no ECC CDC mapping |
| `ProdWrhs3rdLoadgEquipQuantity` |  |  |  | `Decimal(13,3)` |  | Loading equip. qty 3 | ProdWrhs3rdLoadgEquipQtyUnit |  | S/4 only entity — no ECC CDC mapping |
| `ProdWrhs1stLoadgEquipQtyUnit` |  |  |  | `String(3)` |  | Unit of measure 1 |  |  | S/4 only entity — no ECC CDC mapping |
| `ProdWrhs2ndLoadgEquipQtyUnit` |  |  |  | `String(3)` |  | Unit of measure 2 |  |  | S/4 only entity — no ECC CDC mapping |
| `ProdWrhs3rdLoadgEquipQtyUnit` |  |  |  | `String(3)` |  | Unit of measure 3 |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductStorageUnitType1` |  |  |  | `String(3)` |  | Storage Unit Type 1 |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductStorageUnitType2` |  |  |  | `String(3)` |  | Storage Unit Type 2 |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductStorageUnitType3` |  |  |  | `String(3)` |  | Storage Unit Type 3 |  |  | S/4 only entity — no ECC CDC mapping |
| `ProdWarehouseManagementUnit` |  |  |  | `String(3)` |  | WM unit |  |  | S/4 only entity — no ECC CDC mapping |
| `AdditionToExistingStkIsAllowed` |  |  |  | `Boolean` |  | Allow addn to stock |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductBulkStorageMethod` |  |  |  | `String(2)` |  | Bulk storage |  |  | S/4 only entity — no ECC CDC mapping |
| `WrhsMgmtMsgToInvtryMgmtIsRqd` |  |  |  | `Boolean` |  | Message to inv. mgmt |  |  | S/4 only entity — no ECC CDC mapping |
| `WrhsMgmtHasSpecialMovement` |  |  |  | `String(1)` |  | Special movement |  |  | S/4 only entity — no ECC CDC mapping |
| `CapacityUsage` |  |  |  | `Decimal(11,3)` |  | Capacity usage |  |  | S/4 only entity — no ECC CDC mapping |
| `CapacityConsumptionUnit` |  |  |  | `String(3)` |  | Cap.consumption unit |  |  | S/4 only entity — no ECC CDC mapping |
| `ProdWrhsPickingStorageType` |  |  |  | `String(3)` |  | Picking storage type |  |  | S/4 only entity — no ECC CDC mapping |
| `ProdWrhsMatlMasterDefaultUnit` |  |  |  | `String(1)` |  | Proposed UoM frm mat |  |  | S/4 only entity — no ECC CDC mapping |
| `ProdIsRlvtForTwoStepPicking` |  |  |  | `String(1)` |  | 2-step picking |  |  | S/4 only entity — no ECC CDC mapping |
