# Product

> Source file: `sap-s4com-Product-v1.json`


## Entity: `ProdIntlTradeClassification`

- **ABAP CDS Name:** `I_ProdCommodityCodeDEX`
- **Label:** Data Extraction for Product Commodity Code by Country/Region
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `TrdClassfctnNmbrSchm` |  |  |  |  |  | `String(10)` | Y | Numbering Scheme |  | S/4 only entity |
| `Product` |  |  |  |  |  | `String(40)` | Y | Product |  | S/4 only entity |
| `CommodityCode` |  |  |  |  |  | `String(30)` | Y | Commodity Code |  | S/4 only entity |
| `ValidityStartDate` |  |  |  |  |  | `Date` | Y | Valid From |  | S/4 only entity |
| `Country` |  |  |  |  |  | `String(3)` | Y | Country/Region |  | S/4 only entity |
| `ValidityEndDate` |  |  |  |  |  | `Date` |  | Valid To |  | S/4 only entity |
| `TrdClassfctnNmbrUUID` |  |  |  |  |  | `UUID` |  |  |  | S/4 only entity |


## Entity: `ProdWhseManagementStorageType`

- **ABAP CDS Name:** `I_ProdWrhsMgmtStorageType`
- **Label:** Product Data For Each Storage Type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Product |  | S/4 only entity |
| `WarehouseNumber` |  |  |  |  |  | `String(3)` | Y | Warehouse Number |  | S/4 only entity |
| `StorageType` |  |  |  |  |  | `String(3)` | Y | Storage Type |  | S/4 only entity |
| `ProdStorTypeMatlIsMrkdForDeltn` |  |  |  |  |  | `Boolean` |  | Del. flag: stge type |  | S/4 only entity |
| `StorageBin` |  |  |  |  |  | `String(10)` |  | Storage Bin |  | S/4 only entity |
| `ProdWrhsMaxStorageBinQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Maximum bin quantity | BaseUnit | S/4 only entity |
| `ProdWrhsMinStorageBinQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Minimum bin quantity | BaseUnit | S/4 only entity |
| `ProdWrhsStorTypeCtrlQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Control quantity | BaseUnit | S/4 only entity |
| `ProdWrhsStorTypeReplnmtQty` |  |  |  |  |  | `Decimal(13,3)` |  | Replenishment qty | BaseUnit | S/4 only entity |
| `LeanWrhsManagementPickingArea` |  |  |  |  |  | `String(3)` |  | Picking Area |  | S/4 only entity |
| `ProdWrhsStorTypeRoundingQty` |  |  |  |  |  | `Decimal(13,3)` |  | Rounding qty | BaseUnit | S/4 only entity |
| `BaseUnit` |  |  |  |  |  | `String(3)` |  | Base Unit of Measure |  | S/4 only entity |


## Entity: `Product`

- **ABAP CDS Name:** `I_Product`
- **Label:** Product
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  | `MARA` | `MATNR` |  |  | `String(40)` | Y | Product |  |  |
| `ProductExternalID` |  |  |  |  |  | `String(40)` |  | Material |  | S/4 only entity |
| `ProductOID` |  |  |  |  |  | `String(128)` |  | Product OID |  | S/4 only entity |
| `ProductType` |  | `MARA` | `MTART` |  |  | `String(4)` |  | Product Type |  |  |
| `CreationDate` |  | `MARA` | `ERSDA` |  |  | `Date` |  | Created On |  |  |
| `CreationTime` |  |  |  |  |  | `String(6)` |  | Created At Time |  | S/4 only entity |
| `CreationDateTime` |  |  |  |  |  | `Timestamp` |  | Created On |  | S/4 only entity |
| `CreatedByUser` |  |  |  |  |  | `String(12)` |  | Created By |  | S/4 only entity |
| `LastChangeDate` |  |  |  |  |  | `Date` |  | Last Change |  | S/4 only entity |
| `LastChangedByUser` |  |  |  |  |  | `String(12)` |  | Changed By |  | S/4 only entity |
| `IsMarkedForDeletion` |  | `MARA` | `LVORM` |  |  | `Boolean` |  | Marked for Deletion |  |  |
| `CrossPlantStatus` |  |  |  |  |  | `String(2)` |  | CrossPlantProdStatus |  | S/4 only entity |
| `CrossPlantStatusValidityDate` |  |  |  |  |  | `Date` |  | Valid from |  | S/4 only entity |
| `ProductOldID` |  |  |  |  |  | `String(40)` |  | Old Product Number |  | S/4 only entity |
| `GrossWeight` |  | `MARA` | `BRGEW` |  |  | `Decimal(13,3)` |  | Gross Weight | WeightUnit |  |
| `PurchaseOrderQuantityUnit` |  |  |  |  |  | `String(3)` |  | Order Unit |  | S/4 only entity |
| `SourceOfSupply` |  |  |  |  |  | `String(1)` |  | Source of supply |  | S/4 only entity |
| `WeightUnit` |  | `MARA` | `GEWEI` |  |  | `String(3)` |  | Unit of Weight |  |  |
| `CountryOfOrigin` |  |  |  |  |  | `String(3)` |  | Cntry/Reg of Origin |  | S/4 only entity |
| `CompetitorID` |  |  |  |  |  | `String(10)` |  | Competitor |  | S/4 only entity |
| `ProductGroup` |  | `MARA` | `MATKL` |  |  | `String(9)` |  | Product Group |  |  |
| `BaseUnit` |  | `MARA` | `MEINS` |  |  | `String(3)` |  | Base Unit of Measure |  |  |
| `ItemCategoryGroup` |  |  |  |  |  | `String(4)` |  | Gen. item cat. grp |  | S/4 only entity |
| `NetWeight` |  | `MARA` | `NTGEW` |  |  | `Decimal(13,3)` |  | Net Weight | WeightUnit |  |
| `ProductHierarchy` |  |  |  |  |  | `String(18)` |  | Product Hierarchy |  | S/4 only entity |
| `Division` |  |  |  |  |  | `String(2)` |  | Division |  | S/4 only entity |
| `VarblPurOrdUnitIsActive` |  |  |  |  |  | `String(1)` |  | Var. Order Unit |  | S/4 only entity |
| `VolumeUnit` |  |  |  |  |  | `String(3)` |  | Volume Unit |  | S/4 only entity |
| `MaterialVolume` |  |  |  |  |  | `Decimal(13,3)` |  | Volume | VolumeUnit | S/4 only entity |
| `SalesStatus` |  |  |  |  |  | `String(2)` |  | X-DChain Status |  | S/4 only entity |
| `TransportationGroup` |  |  |  |  |  | `String(4)` |  | Transportation Group |  | S/4 only entity |
| `SalesStatusValidityDate` |  |  |  |  |  | `Date` |  | Valid from |  | S/4 only entity |
| `AuthorizationGroup` |  |  |  |  |  | `String(4)` |  | Authorization Group |  | S/4 only entity |
| `ANPCode` |  |  |  |  |  | `String(9)` |  | ANP Code |  | S/4 only entity |
| `ProductCategory` |  |  |  |  |  | `String(2)` |  | Product Category |  | S/4 only entity |
| `Brand` |  |  |  |  |  | `String(4)` |  | Brand |  | S/4 only entity |
| `ProcurementRule` |  |  |  |  |  | `String(1)` |  | Procurement rule |  | S/4 only entity |
| `ValidityStartDate` |  |  |  |  |  | `Date` |  | Valid From |  | S/4 only entity |
| `LowLevelCode` |  |  |  |  |  | `String(3)` |  | Low-Level Code |  | S/4 only entity |
| `ProdNoInGenProdInPrepackProd` |  |  |  |  |  | `String(40)` |  | Generic Material |  | S/4 only entity |
| `SerialIdentifierAssgmtProfile` |  |  |  |  |  | `String(4)` |  | Serial No. Profile |  | S/4 only entity |
| `SizeOrDimensionText` |  |  |  |  |  | `String(32)` |  | Size/dimensions |  | S/4 only entity |
| `IndustryStandardName` |  |  |  |  |  | `String(18)` |  | Industry Std Desc. |  | S/4 only entity |
| `ProductStandardID` |  |  |  |  |  | `String(18)` |  | GTIN |  | S/4 only entity |
| `InternationalArticleNumberCat` |  |  |  |  |  | `String(2)` |  | EAN Category |  | S/4 only entity |
| `ProductIsConfigurable` |  |  |  |  |  | `Boolean` |  | Configurable |  | S/4 only entity |
| `IsBatchManagementRequired` |  |  |  |  |  | `Boolean` |  | Batch Management |  | S/4 only entity |
| `HasEmptiesBOM` |  |  |  |  |  | `Boolean` |  | With Empties BOM |  | S/4 only entity |
| `ExternalProductGroup` |  |  |  |  |  | `String(18)` |  | Ext. Product Group |  | S/4 only entity |
| `CrossPlantConfigurableProduct` |  |  |  |  |  | `String(40)` |  | Cross-plant CP |  | S/4 only entity |
| `SerialNoExplicitnessLevel` |  |  |  |  |  | `String(1)` |  | Serialization Level |  | S/4 only entity |
| `ProductManufacturerNumber` |  |  |  |  |  | `String(40)` |  | Mfr Part Number |  | S/4 only entity |
| `ManufacturerNumber` |  |  |  |  |  | `String(10)` |  | Manufacturer |  | S/4 only entity |
| `ManufacturerPartProfile` |  |  |  |  |  | `String(4)` |  | Mfr Part Profile |  | S/4 only entity |
| `QltyMgmtInProcmtIsActive` |  |  |  |  |  | `Boolean` |  | QM in Procur. Active |  | S/4 only entity |
| `IsApprovedBatchRecordReqd` |  |  |  |  |  | `Boolean` |  | Appr.Batch Recd Req. |  | S/4 only entity |
| `HandlingIndicator` |  |  |  |  |  | `String(4)` |  | Handling Indicator |  | S/4 only entity |
| `WarehouseProductGroup` |  |  |  |  |  | `String(4)` |  | WH Material Group |  | S/4 only entity |
| `WarehouseStorageCondition` |  |  |  |  |  | `String(2)` |  | Whse Stor. Condition |  | S/4 only entity |
| `StandardHandlingUnitType` |  |  |  |  |  | `String(4)` |  | Standard HU Type |  | S/4 only entity |
| `SerialNumberProfile` |  |  |  |  |  | `String(4)` |  | Serial No. Profile |  | S/4 only entity |
| `AdjustmentProfile` |  |  |  |  |  | `String(3)` |  | Adjust. Profile |  | S/4 only entity |
| `PreferredUnitOfMeasure` |  |  |  |  |  | `String(3)` |  | Preferred UoM |  | S/4 only entity |
| `IsPilferable` |  |  |  |  |  | `Boolean` |  | Pilferable |  | S/4 only entity |
| `IsRelevantForHzdsSubstances` |  |  |  |  |  | `Boolean` |  | Relevant for HS |  | S/4 only entity |
| `QuarantinePeriod` |  |  |  |  |  | `Decimal(3,0)` |  | Quarant. Per. | TimeUnitForQuarantinePeriod | S/4 only entity |
| `TimeUnitForQuarantinePeriod` |  |  |  |  |  | `String(3)` |  | Time Unit |  | S/4 only entity |
| `QualityInspectionGroup` |  |  |  |  |  | `String(4)` |  | Quality Inspec. Grp |  | S/4 only entity |
| `HandlingUnitType` |  |  |  |  |  | `String(4)` |  | Handling Unit Type |  | S/4 only entity |
| `HasVariableTareWeight` |  |  |  |  |  | `Boolean` |  | Varb. Tare Weight |  | S/4 only entity |
| `MaximumPackagingLength` |  |  |  |  |  | `Decimal(15,3)` |  | Max. Pack. Length | UnitForMaxPackagingDimensions | S/4 only entity |
| `MaximumPackagingWidth` |  |  |  |  |  | `Decimal(15,3)` |  | Max. Pack. Width | UnitForMaxPackagingDimensions | S/4 only entity |
| `MaximumPackagingHeight` |  |  |  |  |  | `Decimal(15,3)` |  | Max. Pack. Height | UnitForMaxPackagingDimensions | S/4 only entity |
| `MaximumCapacity` |  |  |  |  |  | `Decimal(15,3)` |  | Maximum Capacity |  | S/4 only entity |
| `OvercapacityTolerance` |  |  |  |  |  | `Decimal(3,1)` |  | Overcapacity Toler. |  | S/4 only entity |
| `UnitForMaxPackagingDimensions` |  |  |  |  |  | `String(3)` |  | Unit of Measurement |  | S/4 only entity |
| `BaseUnitSpecificProductLength` |  |  |  |  |  | `Decimal(13,3)` |  | Length | ProductMeasurementUnit | S/4 only entity |
| `BaseUnitSpecificProductWidth` |  |  |  |  |  | `Decimal(13,3)` |  | Width | ProductMeasurementUnit | S/4 only entity |
| `BaseUnitSpecificProductHeight` |  |  |  |  |  | `Decimal(13,3)` |  | Height | ProductMeasurementUnit | S/4 only entity |
| `ProductMeasurementUnit` |  |  |  |  |  | `String(3)` |  | Unit of Dimension |  | S/4 only entity |
| `ProductValidStartDate` |  |  |  |  |  | `Date` |  | Valid From |  | S/4 only entity |
| `ArticleCategory` |  |  |  |  |  | `String(2)` |  | Product Category |  | S/4 only entity |
| `ContentUnit` |  |  |  |  |  | `String(3)` |  | Content Unit |  | S/4 only entity |
| `NetContent` |  |  |  |  |  | `Decimal(13,3)` |  | Net Contents | ContentUnit | S/4 only entity |
| `ComparisonPriceQuantity` |  |  |  |  |  | `Decimal(5,0)` |  | Comparison Price Unit | ContentUnit | S/4 only entity |
| `GrossContent` |  |  |  |  |  | `Decimal(13,3)` |  | Gross Contents | ContentUnit | S/4 only entity |
| `ProductValidEndDate` |  |  |  |  |  | `Date` |  | Valid To |  | S/4 only entity |
| `AssortmentListType` |  |  |  |  |  | `String(1)` |  | Assortment List Type |  | S/4 only entity |
| `HasTextilePartsWthAnimalOrigin` |  |  |  |  |  | `Boolean` |  | Animal Origin |  | S/4 only entity |
| `ProductSeasonUsageCategory` |  |  |  |  |  | `String(1)` |  | Season Usage |  | S/4 only entity |
| `IndustrySector` |  |  |  |  |  | `String(1)` |  | Industry |  | S/4 only entity |
| `ChangeNumber` |  |  |  |  |  | `String(12)` |  | Change Number |  | S/4 only entity |
| `MaterialRevisionLevel` |  |  |  |  |  | `String(2)` |  | Revision Level |  | S/4 only entity |
| `IsActiveEntity` |  |  |  |  |  | `Boolean` |  | Is active |  | S/4 only entity |
| `LastChangeDateTime` |  |  |  |  |  | `Timestamp` |  | Last Changed |  | S/4 only entity |
| `LastChangeTime` |  |  |  |  |  | `String(6)` |  | Last Changed Time |  | S/4 only entity |
| `DangerousGoodsIndProfile` |  |  |  |  |  | `String(3)` |  | DG indicator profile |  | S/4 only entity |
| `ProductUUID` |  |  |  |  |  | `UUID` |  | Product |  | S/4 only entity |
| `ProdSupChnMgmtUUID22` |  |  |  |  |  | `String(22)` |  | Product ID |  | S/4 only entity |
| `ProductDocumentChangeNumber` |  |  |  |  |  | `String(6)` |  | Document Change No. |  | S/4 only entity |
| `ProductDocumentPageCount` |  |  |  |  |  | `String(3)` |  | Number Of Sheets |  | S/4 only entity |
| `ProductDocumentPageNumber` |  |  |  |  |  | `String(3)` |  | Page Number |  | S/4 only entity |
| `OwnInventoryManagedProduct` |  |  |  |  |  | `String(40)` |  | Int. material number |  | S/4 only entity |
| `DocumentIsCreatedByCAD` |  |  |  |  |  | `Boolean` |  | CAD Indicator |  | S/4 only entity |
| `ProductionOrInspectionMemoTxt` |  |  |  |  |  | `String(18)` |  | Prod./insp. memo |  | S/4 only entity |
| `ProductionMemoPageFormat` |  |  |  |  |  | `String(4)` |  | Page format |  | S/4 only entity |
| `GlobalTradeItemNumberVariant` |  |  |  |  |  | `String(2)` |  | EAN Variant |  | S/4 only entity |
| `ProductIsHighlyViscous` |  |  |  |  |  | `Boolean` |  | Highly viscous |  | S/4 only entity |
| `TransportIsInBulk` |  |  |  |  |  | `Boolean` |  | In bulk/liquid |  | S/4 only entity |
| `ProdAllocDetnProcedure` |  |  |  |  |  | `String(18)` |  | Product allocation |  | S/4 only entity |
| `ProdEffctyParamValsAreAssigned` |  |  |  |  |  | `Boolean` |  | Assign effect. vals |  | S/4 only entity |
| `ProdIsEnvironmentallyRelevant` |  |  |  |  |  | `Boolean` |  | Environmentally rlvt |  | S/4 only entity |
| `LaboratoryOrDesignOffice` |  |  |  |  |  | `String(3)` |  | Lab/Office |  | S/4 only entity |
| `PackagingMaterialGroup` |  |  |  |  |  | `String(4)` |  | Matl Grp Pack.Matls |  | S/4 only entity |
| `ProductIsLocked` |  |  |  |  |  | `Boolean` |  | Product locked |  | S/4 only entity |
| `DiscountInKindEligibility` |  |  |  |  |  | `String(1)` |  | Qual.f.FreeGoodsDis. |  | S/4 only entity |
| `SmartFormName` |  |  |  |  |  | `String(30)` |  | Form Name |  | S/4 only entity |
| `PackingReferenceProduct` |  |  |  |  |  | `String(40)` |  | Ref. Mat. for Pckg |  | S/4 only entity |
| `BasicMaterial` |  |  |  |  |  | `String(48)` |  | Basic Material |  | S/4 only entity |
| `ProductDocumentNumber` |  |  |  |  |  | `String(22)` |  | Document |  | S/4 only entity |
| `ProductDocumentVersion` |  |  |  |  |  | `String(2)` |  | Document Version |  | S/4 only entity |
| `ProductDocumentType` |  |  |  |  |  | `String(3)` |  | Document Type |  | S/4 only entity |
| `ProductDocumentPageFormat` |  |  |  |  |  | `String(4)` |  | Page Format |  | S/4 only entity |
| `ProductConfiguration` |  |  |  |  |  | `String(18)` |  | Internal object no. |  | S/4 only entity |
| `SegmentationStrategy` |  |  |  |  |  | `String(8)` |  | Seg. Strategy |  | S/4 only entity |
| `SegmentationIsRelevant` |  |  |  |  |  | `Boolean` |  | Seg. Relevant |  | S/4 only entity |
| `ProductCompositionIsRelevant` |  |  |  |  |  | `Boolean` |  | Product Composition |  | S/4 only entity |
| `IsChemicalComplianceRelevant` |  |  |  |  |  | `String(1)` |  | Chemical Compliance Relevance Indicator |  | S/4 only entity |
| `ManufacturerBookPartNumber` |  |  |  |  |  | `String(40)` |  | MS Book Part No |  | S/4 only entity |
| `LogisticalProductCategory` |  |  |  |  |  | `String(1)` |  | Logl Material Cat. |  | S/4 only entity |
| `SalesProduct` |  |  |  |  |  | `String(40)` |  | Sales Material No. |  | S/4 only entity |
| `ProdCharc1InternalNumber` |  |  |  |  |  | `String(10)` |  | Int. Char. Number |  | S/4 only entity |
| `ProdCharc2InternalNumber` |  |  |  |  |  | `String(10)` |  | Int. Char. Number |  | S/4 only entity |
| `ProdCharc3InternalNumber` |  |  |  |  |  | `String(10)` |  | Int. Char. Number |  | S/4 only entity |
| `ProductCharacteristic1` |  |  |  |  |  | `String(18)` |  | Color |  | S/4 only entity |
| `ProductCharacteristic2` |  |  |  |  |  | `String(18)` |  | Main Size |  | S/4 only entity |
| `ProductCharacteristic3` |  |  |  |  |  | `String(18)` |  | Second Size |  | S/4 only entity |
| `MaintenanceStatus` |  |  |  |  |  | `String(15)` |  | Maintenance Status |  | S/4 only entity |
| `FashionProdInformationField1` |  |  |  |  |  | `String(10)` |  | Fsh. Attribute1 |  | S/4 only entity |
| `FashionProdInformationField2` |  |  |  |  |  | `String(10)` |  | Fsh. Attribute2 |  | S/4 only entity |
| `FashionProdInformationField3` |  |  |  |  |  | `String(6)` |  | Fsh. Attribute3 |  | S/4 only entity |
| `DfsAmmunitionGroupCode` |  |  |  |  |  | `String(8)` |  | Ammunition Code |  | S/4 only entity |
| `DfsRICIdentifier` |  |  |  |  |  | `Integer64` |  | RIC ID |  | S/4 only entity |
| `DfsProductSensitivity` |  |  |  |  |  | `String(4)` |  | Sensitivity for Char |  | S/4 only entity |
| `DfsManufacturerPartLongNumber` |  |  |  |  |  | `String(60)` |  | Long Mfr Part No. |  | S/4 only entity |
| `DfsMatlConditionMgmt` |  |  |  |  |  | `String(1)` |  | Condition Mgmt |  | S/4 only entity |
| `DfsReturnDelivery` |  |  |  |  |  | `String(1)` |  | Return Code |  | S/4 only entity |
| `DfsLogisticsLevel` |  |  |  |  |  | `String(1)` |  | Return to Log.Level |  | S/4 only entity |
| `DfsNationalItemIdnNumber` |  |  |  |  |  | `String(9)` |  | NATO Item ID Number |  | S/4 only entity |
| `LstMiProductToleranceType` |  |  |  |  |  | `String(4)` |  | Tolerance Type |  | S/4 only entity |


## Entity: `ProductConsumption`

- **ABAP CDS Name:** `I_ProductConsumption`
- **Label:** Product Consumption
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Product |  | S/4 only entity |
| `Plant` |  |  |  |  |  | `String(4)` | Y | Plant |  | S/4 only entity |
| `PostingFiscalYear` |  |  |  |  |  | `String(4)` | Y | Fiscal Year |  | S/4 only entity |
| `PeriodType` |  |  |  |  |  | `String(1)` | Y | Period Indicator |  | S/4 only entity |
| `NumberOfFollowOnRecords` |  |  |  |  |  | `String(2)` | Y | Follow-on records |  | S/4 only entity |
| `TotalConsumption1Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Tot.consumption 1 | BaseUnit | S/4 only entity |
| `TotalConsumption2Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Tot.consumption 2 | BaseUnit | S/4 only entity |
| `TotalConsumption3Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Tot.consumption 3 | BaseUnit | S/4 only entity |
| `TotalConsumption4Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Tot.consumption 4 | BaseUnit | S/4 only entity |
| `TotalConsumption5Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Tot.consumption 5 | BaseUnit | S/4 only entity |
| `TotalConsumption6Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Tot.consumption 6 | BaseUnit | S/4 only entity |
| `TotalConsumption7Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Tot.consumption 7 | BaseUnit | S/4 only entity |
| `TotalConsumption8Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Tot.consumption 8 | BaseUnit | S/4 only entity |
| `TotalConsumption9Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Tot.consumption 9 | BaseUnit | S/4 only entity |
| `TotalConsumption10Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Tot.consumption 10 | BaseUnit | S/4 only entity |
| `TotalConsumption11Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Tot.consumption 11 | BaseUnit | S/4 only entity |
| `TotalConsumption12Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Tot.consumption 12 | BaseUnit | S/4 only entity |
| `TotalConsumption13Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Tot.consumption 13 | BaseUnit | S/4 only entity |
| `UnplannedConsumption1Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Unplnd consump. 1 | BaseUnit | S/4 only entity |
| `UnplannedConsumption2Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Unplnd consump. 2 | BaseUnit | S/4 only entity |
| `UnplannedConsumption3Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Unplnd consump. 3 | BaseUnit | S/4 only entity |
| `UnplannedConsumption4Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Unplnd consump. 4 | BaseUnit | S/4 only entity |
| `UnplannedConsumption5Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Unplnd consump. 5 | BaseUnit | S/4 only entity |
| `UnplannedConsumption6Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Unplnd consump. 6 | BaseUnit | S/4 only entity |
| `UnplannedConsumption7Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Unplnd consump. 7 | BaseUnit | S/4 only entity |
| `UnplannedConsumption8Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Unplnd consump. 8 | BaseUnit | S/4 only entity |
| `UnplannedConsumption9Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Unplnd consump. 9 | BaseUnit | S/4 only entity |
| `UnplannedConsumption10Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Unplnd consump. 10 | BaseUnit | S/4 only entity |
| `UnplannedConsumption11Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Unplnd consump. 11 | BaseUnit | S/4 only entity |
| `UnplannedConsumption12Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Unplnd consump. 12 | BaseUnit | S/4 only entity |
| `UnplannedConsumption13Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Unplnd consump. 13 | BaseUnit | S/4 only entity |
| `MnllyCrrtdTotCnsmpn1Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.tot.consum 1 | BaseUnit | S/4 only entity |
| `MnllyCrrtdTotCnsmpn2Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.tot.consum 2 | BaseUnit | S/4 only entity |
| `MnllyCrrtdTotCnsmpn3Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.tot.consum 3 | BaseUnit | S/4 only entity |
| `MnllyCrrtdTotCnsmpn4Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.tot.consum 4 | BaseUnit | S/4 only entity |
| `MnllyCrrtdTotCnsmpn5Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.tot.consum 5 | BaseUnit | S/4 only entity |
| `MnllyCrrtdTotCnsmpn6Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.tot.consum 6 | BaseUnit | S/4 only entity |
| `MnllyCrrtdTotCnsmpn7Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.tot.consum 7 | BaseUnit | S/4 only entity |
| `MnllyCrrtdTotCnsmpn8Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.tot.consum 8 | BaseUnit | S/4 only entity |
| `MnllyCrrtdTotCnsmpn9Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.tot.consum 9 | BaseUnit | S/4 only entity |
| `MnllyCrrtdTotCnsmpn10Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.tot.consum 10 | BaseUnit | S/4 only entity |
| `MnllyCrrtdTotCnsmpn11Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.tot.consum 11 | BaseUnit | S/4 only entity |
| `MnllyCrrtdTotCnsmpn12Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.tot.consum 12 | BaseUnit | S/4 only entity |
| `MnllyCrrtdTotCnsmpn13Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.tot.consum 13 | BaseUnit | S/4 only entity |
| `MnllyCrrtdUnplndCnsmpn1Qty` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.unpl.cons. 1 | BaseUnit | S/4 only entity |
| `MnllyCrrtdUnplndCnsmpn2Qty` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.unpl.cons. 2 | BaseUnit | S/4 only entity |
| `MnllyCrrtdUnplndCnsmpn3Qty` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.unpl.cons. 3 | BaseUnit | S/4 only entity |
| `MnllyCrrtdUnplndCnsmpn4Qty` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.unpl.cons. 4 | BaseUnit | S/4 only entity |
| `MnllyCrrtdUnplndCnsmpn5Qty` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.unpl.cons. 5 | BaseUnit | S/4 only entity |
| `MnllyCrrtdUnplndCnsmpn6Qty` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.unpl.cons. 6 | BaseUnit | S/4 only entity |
| `MnllyCrrtdUnplndCnsmpn7Qty` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.unpl.cons. 7 | BaseUnit | S/4 only entity |
| `MnllyCrrtdUnplndCnsmpn8Qty` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.unpl.cons. 8 | BaseUnit | S/4 only entity |
| `MnllyCrrtdUnplndCnsmpn9Qty` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.unpl.cons. 9 | BaseUnit | S/4 only entity |
| `MnllyCrrtdUnplndCnsmpn10Qty` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.unpl.cons. 10 | BaseUnit | S/4 only entity |
| `MnllyCrrtdUnplndCnsmpn11Qty` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.unpl.cons. 11 | BaseUnit | S/4 only entity |
| `MnllyCrrtdUnplndCnsmpn12Qty` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.unpl.cons. 12 | BaseUnit | S/4 only entity |
| `MnllyCrrtdUnplndCnsmpn13Qty` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.unpl.cons. 13 | BaseUnit | S/4 only entity |
| `BaseUnit` |  |  |  |  |  | `String(3)` |  | Base Unit of Measure |  | S/4 only entity |


## Entity: `ProductDescription`

- **ABAP CDS Name:** `I_ProductDescription_2`
- **Label:** Product Descriptions
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Product |  | S/4 only entity |
| `Language` |  |  |  |  |  | `String(2)` | Y | Language Key |  | S/4 only entity |
| `ProductDescription` |  |  |  |  |  | `String(40)` |  | Product Description |  | S/4 only entity |
| `LanguageISOCode` |  |  |  |  |  | `String(2)` |  | Language |  | S/4 only entity |


## Entity: `ProductGroup`

- **ABAP CDS Name:** `I_ProductGroup_2`
- **Label:** Product Group
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `ProductGroup` |  |  |  |  |  | `String(9)` | Y | Product Group |  | S/4 only entity |
| `AuthorizationGroup` |  |  |  |  |  | `String(4)` |  | Authorization Group |  | S/4 only entity |
| `ValuationClass` |  |  |  |  |  | `String(4)` |  | Valuation Class |  | S/4 only entity |
| `PurchasingAcknProfile` |  |  |  |  |  | `String(4)` |  | Purchasing value key |  | S/4 only entity |


## Entity: `ProductGroupText`

- **ABAP CDS Name:** `I_ProductGroupText_2`
- **Label:** Product Group - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `ProductGroup` |  |  |  |  |  | `String(9)` | Y | Product Group |  | S/4 only entity |
| `Language` |  |  |  |  |  | `String(2)` | Y | Language Key |  | S/4 only entity |
| `ProductGroupName` |  |  |  |  |  | `String(20)` |  | Product Group Description |  | S/4 only entity |
| `ProductGroupText` |  |  |  |  |  | `String(60)` |  | Mat.Grp Desc. 2 |  | S/4 only entity |


## Entity: `ProductMRPArea`

- **ABAP CDS Name:** `I_ProductMRPArea`
- **Label:** MRP Area Details of a Product
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Product |  | S/4 only entity |
| `MRPArea` |  |  |  |  |  | `String(10)` | Y | MRP Area |  | S/4 only entity |
| `MRPPlant` |  |  |  |  |  | `String(4)` |  | MRP Area Plant |  | S/4 only entity |
| `MRPGroup` |  |  |  |  |  | `String(4)` |  | MRP Group |  | S/4 only entity |
| `MRPType` |  |  |  |  |  | `String(2)` |  | MRP Type |  | S/4 only entity |
| `MRPController` |  |  |  |  |  | `String(3)` |  | MRP Controller |  | S/4 only entity |
| `MRPProfile` |  |  |  |  |  | `String(4)` |  | MRP Profile |  | S/4 only entity |
| `LotSizingProcedure` |  |  |  |  |  | `String(2)` |  | Lot Sizing Procedure |  | S/4 only entity |
| `MRPPlanningCalendar` |  |  |  |  |  | `String(3)` |  | Planning Calendar |  | S/4 only entity |
| `MRPPlanningCycle` |  |  |  |  |  | `String(3)` |  | Planning Cycle |  | S/4 only entity |
| `MRPSafetyStockMethod` |  |  |  |  |  | `String(2)` |  | Safety Stock Method |  | S/4 only entity |
| `MaterialProcurementProfile` |  |  |  |  |  | `String(2)` |  | Procurement Profile |  | S/4 only entity |
| `ProductionStorageLocation` |  |  |  |  |  | `String(4)` |  | Production Storage Location |  | S/4 only entity |
| `DfltStorLocForExtProcmt` |  |  |  |  |  | `String(4)` |  | External Procurement Storage Location |  | S/4 only entity |
| `RangeOfCoverageProfile` |  |  |  |  |  | `String(3)` |  | Range-of-Coverage Profile |  | S/4 only entity |
| `SafetyTimePeriodProfile` |  |  |  |  |  | `String(3)` |  | Period Profile for Safety Time |  | S/4 only entity |
| `ProductSafetyTimeMRPRelevance` |  |  |  |  |  | `String(1)` |  | Safety Time MRP Relevance |  | S/4 only entity |
| `DependentRqmtMRPRelevance` |  |  |  |  |  | `String(1)` |  | Dependent Requirements MRP Relevance |  | S/4 only entity |
| `StorageCostsPercentageCode` |  |  |  |  |  | `String(1)` |  | Storage Costs Code |  | S/4 only entity |
| `RoundingProfile` |  |  |  |  |  | `String(4)` |  | Rounding Profile |  | S/4 only entity |
| `IsMarkedForDeletion` |  |  |  |  |  | `Boolean` |  | Deletion Indicator |  | S/4 only entity |
| `LastChangedByUser` |  |  |  |  |  | `String(12)` |  | Changed By |  | S/4 only entity |
| `LastChangeDate` |  |  |  |  |  | `Date` |  | Changed On |  | S/4 only entity |
| `LastChangeTime` |  |  |  |  |  | `String(6)` |  | Time of Change |  | S/4 only entity |
| `PlannedDeliveryDurationInDays` |  |  |  |  |  | `Decimal(3,0)` |  | Planned Deliv. Time |  | S/4 only entity |
| `PlanningTimeFenceInDays` |  |  |  |  |  | `String(3)` |  | Planning Time Fence |  | S/4 only entity |
| `RqmtQtyRcptTaktTmeInWrkgDays` |  |  |  |  |  | `Decimal(3,0)` |  | Takt time |  | S/4 only entity |
| `AssemblyScrapPercent` |  |  |  |  |  | `Decimal(5,2)` |  | Assembly scrap (%) |  | S/4 only entity |
| `BaseUnit` |  |  |  |  |  | `String(3)` |  | Base Unit of Measure |  | S/4 only entity |
| `MinimumLotSizeQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Minimum Lot Size | BaseUnit | S/4 only entity |
| `MaximumLotSizeQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Maximum Lot Size | BaseUnit | S/4 only entity |
| `MaterialMaxStockLevelQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Maximum Stock Level | BaseUnit | S/4 only entity |
| `SafetyStockQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Safety Stock | BaseUnit | S/4 only entity |
| `LotSizeRoundingQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Rounding Quantity | BaseUnit | S/4 only entity |
| `ReorderThresholdQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Reorder Point | BaseUnit | S/4 only entity |


## Entity: `ProductPlant`

- **ABAP CDS Name:** `I_ProductPlantBasic`
- **Label:** Product Plant
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Product |  | S/4 only entity |
| `Plant` |  |  |  |  |  | `String(4)` | Y | Plant |  | S/4 only entity |
| `PurchasingGroup` |  |  |  |  |  | `String(3)` |  | Purchasing Group |  | S/4 only entity |
| `CountryOfOrigin` |  |  |  |  |  | `String(3)` |  | Country/Region of Origin |  | S/4 only entity |
| `RegionOfOrigin` |  |  |  |  |  | `String(3)` |  | Region of Origin |  | S/4 only entity |
| `ProductionInvtryManagedLoc` |  |  |  |  |  | `String(4)` |  | Storage Location |  | S/4 only entity |
| `ProfileCode` |  |  |  |  |  | `String(2)` |  | Material Status |  | S/4 only entity |
| `ProfileValidityStartDate` |  |  |  |  |  | `Date` |  | Valid From |  | S/4 only entity |
| `AvailabilityCheckType` |  |  |  |  |  | `String(2)` |  | Availability check |  | S/4 only entity |
| `FiscalYearVariant` |  |  |  |  |  | `String(2)` |  | Fiscal Year Variant |  | S/4 only entity |
| `PeriodType` |  |  |  |  |  | `String(1)` |  | Period Indicator |  | S/4 only entity |
| `ProfitCenter` |  |  |  |  |  | `String(10)` |  | Profit Center |  | S/4 only entity |
| `GoodsReceiptDuration` |  |  |  |  |  | `Decimal(3,0)` |  | GR processing time |  | S/4 only entity |
| `MaintenanceStatusName` |  |  |  |  |  | `String(15)` |  | Maintenance Status |  | S/4 only entity |
| `IsMarkedForDeletion` |  |  |  |  |  | `Boolean` |  | DF at plant level |  | S/4 only entity |
| `MRPType` |  |  |  |  |  | `String(2)` |  | MRP Type |  | S/4 only entity |
| `MRPResponsible` |  |  |  |  |  | `String(3)` |  | MRP Controller |  | S/4 only entity |
| `ABCIndicator` |  |  |  |  |  | `String(1)` |  | ABC Indicator |  | S/4 only entity |
| `MinimumLotSizeQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Minimum Lot Size | BaseUnit | S/4 only entity |
| `MaximumLotSizeQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Maximum Lot Size | BaseUnit | S/4 only entity |
| `FixedLotSizeQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Fixed lot size | BaseUnit | S/4 only entity |
| `ConsumptionTaxCtrlCode` |  |  |  |  |  | `String(16)` |  | Control Code |  | S/4 only entity |
| `IsCoProduct` |  |  |  |  |  | `Boolean` |  | Co-Product |  | S/4 only entity |
| `ConfigurableProduct` |  |  |  |  |  | `String(40)` |  | Conf. Material |  | S/4 only entity |
| `StockDeterminationGroup` |  |  |  |  |  | `String(4)` |  | Stock Determ. Group |  | S/4 only entity |
| `HasPostToInspectionStock` |  |  |  |  |  | `Boolean` |  | Post to insp. stock |  | S/4 only entity |
| `IsBatchManagementRequired` |  |  |  |  |  | `Boolean` |  | Batch Mgmt Rqt(Plnt) |  | S/4 only entity |
| `SerialNumberProfile` |  |  |  |  |  | `String(4)` |  | Serial No. Profile |  | S/4 only entity |
| `IsNegativeStockAllowed` |  |  |  |  |  | `Boolean` |  | Neg. Stocks In Plant |  | S/4 only entity |
| `HasConsignmentCtrl` |  |  |  |  |  | `String(1)` |  | Consign.Control |  | S/4 only entity |
| `IsPurgAcrossPurgGroup` |  |  |  |  |  | `Boolean` |  | Across Purch.Group |  | S/4 only entity |
| `IsInternalBatchManaged` |  |  |  |  |  | `Boolean` |  | Batch Management |  | S/4 only entity |
| `ProductCFOPCategory` |  |  |  |  |  | `String(2)` |  | Matl. CFOP Category |  | S/4 only entity |
| `ProductIsExciseTaxRelevant` |  |  |  |  |  | `Boolean` |  | Is Excise Tax Relevant |  | S/4 only entity |
| `UnderDelivToleranceLimit` |  |  |  |  |  | `Decimal(3,1)` |  | Underdelivery Toler. |  | S/4 only entity |
| `OverDelivToleranceLimit` |  |  |  |  |  | `Decimal(3,1)` |  | Overdelivery Toler. |  | S/4 only entity |
| `ProcurementType` |  |  |  |  |  | `String(1)` |  | Procurement Type |  | S/4 only entity |
| `SpecialProcurementType` |  |  |  |  |  | `String(2)` |  | Special Procurement |  | S/4 only entity |
| `ProductionSchedulingProfile` |  |  |  |  |  | `String(6)` |  | Production Scheduling Profile |  | S/4 only entity |
| `ProductionSupervisor` |  |  |  |  |  | `String(3)` |  | Prodn Supervisor |  | S/4 only entity |
| `SafetyStockQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Safety Stock | BaseUnit | S/4 only entity |
| `GoodsIssueUnit` |  |  |  |  |  | `String(3)` |  | Unit of Issue |  | S/4 only entity |
| `SourceOfSupplyCategory` |  |  |  |  |  | `String(1)` |  | Source of supply |  | S/4 only entity |
| `ConsumptionReferenceProduct` |  |  |  |  |  | `String(40)` |  | RefMatl: consumption |  | S/4 only entity |
| `ConsumptionReferencePlant` |  |  |  |  |  | `String(4)` |  | RefPlant:consumption |  | S/4 only entity |
| `ConsumptionRefUsageEndDate` |  |  |  |  |  | `Date` |  | Date to |  | S/4 only entity |
| `ConsumptionQtyMultiplier` |  |  |  |  |  | `Decimal(4,2)` |  | Multiplier |  | S/4 only entity |
| `ProductUnitGroup` |  |  |  |  |  | `String(4)` |  | Unit of Measure Group |  | S/4 only entity |
| `DistrCntrDistributionProfile` |  |  |  |  |  | `String(3)` |  | Distr. profile |  | S/4 only entity |
| `ConsignmentControl` |  |  |  |  |  | `String(1)` |  | Consign.Control |  | S/4 only entity |
| `GoodIssueProcessingDays` |  |  |  |  |  | `Decimal(3,0)` |  | GI Proc. Time |  | S/4 only entity |
| `PlannedDeliveryDurationInDays` |  |  |  |  |  | `Decimal(3,0)` |  | Planned Deliv. Time |  | S/4 only entity |
| `ProductIsCriticalPrt` |  |  |  |  |  | `Boolean` |  | Critical Part |  | S/4 only entity |
| `ProductLogisticsHandlingGroup` |  |  |  |  |  | `String(4)` |  | Log. handling group |  | S/4 only entity |
| `MaterialFreightGroup` |  |  |  |  |  | `String(8)` |  | Material Freight Grp |  | S/4 only entity |
| `OriginalBatchReferenceMaterial` |  |  |  |  |  | `String(40)` |  | OB Reference Materl |  | S/4 only entity |
| `OriglBatchManagementIsRequired` |  |  |  |  |  | `String(1)` |  | OB Management |  | S/4 only entity |
| `ProductConfiguration` |  |  |  |  |  | `String(18)` |  | Internal object no. |  | S/4 only entity |
| `ProductMinControlTemperature` |  |  |  |  |  | `Decimal(7,2)` |  | Min. Temperature | ProductControlTemperatureUnit | S/4 only entity |
| `ProductMaxControlTemperature` |  |  |  |  |  | `Decimal(7,2)` |  | Max. Temperature | ProductControlTemperatureUnit | S/4 only entity |
| `ProductControlTemperatureUnit` |  |  |  |  |  | `String(3)` |  | Temperature UoM |  | S/4 only entity |
| `ValuationCategory` |  |  |  |  |  | `String(1)` |  | Valuation Category |  | S/4 only entity |
| `BaseUnit` |  |  |  |  |  | `String(3)` |  | Base Unit of Measure |  | S/4 only entity |
| `ItemUniqueIdentifierIsRelevant` |  |  |  |  |  | `Boolean` |  | IUID-Relevant |  | S/4 only entity |
| `ItemUniqueIdentifierType` |  |  |  |  |  | `String(10)` |  | IUID Type |  | S/4 only entity |
| `ExtAllocOfItmUnqIdtIsRelevant` |  |  |  |  |  | `Boolean` |  | Ext. Allocation |  | S/4 only entity |


## Entity: `ProductPlantCosting`

- **ABAP CDS Name:** `I_ProductPlantCosting`
- **Label:** Product Plant Costing
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Product |  | S/4 only entity |
| `Plant` |  |  |  |  |  | `String(4)` | Y | Plant |  | S/4 only entity |
| `IsCoProduct` |  |  |  |  |  | `Boolean` |  | Co-Product |  | S/4 only entity |
| `CostingLotSize` |  |  |  |  |  | `Decimal(13,3)` |  | Costing Lot Size | BaseUnit | S/4 only entity |
| `TaskListGroup` |  |  |  |  |  | `String(8)` |  | Group |  | S/4 only entity |
| `TaskListType` |  |  |  |  |  | `String(1)` |  | Task List Type |  | S/4 only entity |
| `CostingSpecialProcurementType` |  |  |  |  |  | `String(2)` |  | Special Procurement Type |  | S/4 only entity |
| `SourceBOMAlternative` |  |  |  |  |  | `String(2)` |  | Alternative BOM |  | S/4 only entity |
| `ProductBOMUsage` |  |  |  |  |  | `String(1)` |  | BOM Usage |  | S/4 only entity |
| `ProductIsCostingRelevant` |  |  |  |  |  | `Boolean` |  | Do Not Cost |  | S/4 only entity |
| `TaskListGroupCounter` |  |  |  |  |  | `String(2)` |  | Group Counter |  | S/4 only entity |
| `VarianceKey` |  |  |  |  |  | `String(6)` |  | Variance Key |  | S/4 only entity |
| `CostingProductionVersion` |  |  |  |  |  | `String(4)` |  | Production Version |  | S/4 only entity |
| `IsFixedPriceCoProduct` |  |  |  |  |  | `Boolean` |  | Fixed-Price Co-Prod. |  | S/4 only entity |
| `BaseUnit` |  |  |  |  |  | `String(3)` |  | Base Unit of Measure |  | S/4 only entity |


## Entity: `ProductPlantForecast`

- **ABAP CDS Name:** `I_ProductPlantForecast`
- **Label:** Product Plant Forecast
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Product |  | S/4 only entity |
| `Plant` |  |  |  |  |  | `String(4)` | Y | Plant |  | S/4 only entity |
| `ConsumptionRefUsageEndDate` |  |  |  |  |  | `Date` |  | Date to |  | S/4 only entity |
| `ConsumptionQtyMultiplier` |  |  |  |  |  | `Decimal(4,2)` |  | Multiplier |  | S/4 only entity |
| `ConsumptionReferenceProduct` |  |  |  |  |  | `String(40)` |  | RefMatl: consumption |  | S/4 only entity |
| `ConsumptionReferencePlant` |  |  |  |  |  | `String(4)` |  | RefPlant:consumption |  | S/4 only entity |
| `CorrectionFactorIsRequired` |  |  |  |  |  | `Boolean` |  | Correction factors |  | S/4 only entity |
| `ForecastModelIsReset` |  |  |  |  |  | `Boolean` |  | Reset automatically |  | S/4 only entity |


## Entity: `ProductPlantInternationalTrade`

- **ABAP CDS Name:** `I_ProductPlantIntlTrd`
- **Label:** Product Plant Intrntionl Trade
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Product |  | S/4 only entity |
| `Plant` |  |  |  |  |  | `String(4)` | Y | Plant |  | S/4 only entity |
| `CountryOfOrigin` |  |  |  |  |  | `String(3)` |  | Country/Region of Origin |  | S/4 only entity |
| `RegionOfOrigin` |  |  |  |  |  | `String(3)` |  | Region of Origin |  | S/4 only entity |
| `ConsumptionTaxCtrlCode` |  |  |  |  |  | `String(16)` |  | Control Code |  | S/4 only entity |
| `ExportAndImportProductGroup` |  |  |  |  |  | `String(4)` |  | Intrastat Group |  | S/4 only entity |
| `ProductCASNumber` |  |  |  |  |  | `String(15)` |  | CAS number (pharm.) |  | S/4 only entity |
| `CommoditiyCodeNumberUnit` |  |  |  |  |  | `String(3)` |  | Commodity code unit |  | S/4 only entity |
| `ProdIntlTradeClassification` |  |  |  |  |  | `String(9)` |  | PRODCOM no. |  | S/4 only entity |


## Entity: `ProductPlantProcurement`

- **ABAP CDS Name:** `I_Productplantprocurement`
- **Label:** Product Plant Procurement
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Product |  | S/4 only entity |
| `Plant` |  |  |  |  |  | `String(4)` | Y | Plant |  | S/4 only entity |
| `IsAutoPurOrdCreationAllowed` |  |  |  |  |  | `Boolean` |  | Automatic PO |  | S/4 only entity |
| `IsSourceListRequired` |  |  |  |  |  | `Boolean` |  | Source list |  | S/4 only entity |
| `IsPurgAcrossPurgGroup` |  |  |  |  |  | `Boolean` |  | Across Purch.Group |  | S/4 only entity |
| `SourceOfSupplyCategory` |  |  |  |  |  | `String(1)` |  | Source of supply |  | S/4 only entity |
| `PurchasingGroup` |  |  |  |  |  | `String(3)` |  | Purchasing Group |  | S/4 only entity |
| `IsActiveEntity` |  |  |  |  |  | `Boolean` |  | Is active |  | S/4 only entity |
| `ProposedProductSupplyArea` |  |  |  |  |  | `String(10)` |  | Proposed Supply Area |  | S/4 only entity |
| `ItmIsRlvtToJITDelivSchedules` |  |  |  |  |  | `String(1)` |  | JIT Delivery |  | S/4 only entity |


## Entity: `ProductPlantPurchaseTax`

- **ABAP CDS Name:** `I_ProductPurchaseTax`
- **Label:** Product Purchase Tax
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Product |  | S/4 only entity |
| `SourceLocationCountry` |  |  |  |  |  | `String(3)` | Y | Departure Ctry/Reg. |  | S/4 only entity |
| `TaxIndicator` |  |  |  |  |  | `String(1)` |  | Tax ind. f. material |  | S/4 only entity |


## Entity: `ProductPlantQualityManagement`

- **ABAP CDS Name:** `I_Productplantqtmanagement`
- **Label:** Product Plant QM
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Product |  | S/4 only entity |
| `Plant` |  |  |  |  |  | `String(4)` | Y | Plant |  | S/4 only entity |
| `MaximumStoragePeriod` |  |  |  |  |  | `Decimal(5,0)` |  | Max. Storage Period |  | S/4 only entity |
| `QualityMgmtCtrlKey` |  |  |  |  |  | `String(8)` |  | QM Control Key |  | S/4 only entity |
| `MatlQualityAuthorizationGroup` |  |  |  |  |  | `String(6)` |  | QM Material Auth. |  | S/4 only entity |
| `HasPostToInspectionStock` |  |  |  |  |  | `Boolean` |  | Post to insp. stock |  | S/4 only entity |
| `IsActiveEntity` |  |  |  |  |  | `Boolean` |  | Is active |  | S/4 only entity |
| `InspLotDocumentationIsRequired` |  |  |  |  |  | `Boolean` |  | Documentation reqd |  | S/4 only entity |
| `SuplrQualityManagementSystem` |  |  |  |  |  | `String(4)` |  | Target QM System |  | S/4 only entity |
| `RecrrgInspIntervalTimeInDays` |  |  |  |  |  | `Decimal(5,0)` |  | Inspection Interval |  | S/4 only entity |
| `ProductQualityCertificateType` |  |  |  |  |  | `String(4)` |  | Certificate Type |  | S/4 only entity |
| `ProductPlantHasInspectionSetup` |  |  |  |  |  | `Boolean` |  | Inspection Setup |  | S/4 only entity |


## Entity: `ProductPlantStorage`

- **ABAP CDS Name:** `I_Productplantstorage`
- **Label:** Product plant storage
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Product |  | S/4 only entity |
| `Plant` |  |  |  |  |  | `String(4)` | Y | Plant |  | S/4 only entity |
| `InventoryForCycleCountInd` |  |  |  |  |  | `String(1)` |  | CC Phys. Inv. Ind. |  | S/4 only entity |
| `MaximumStoragePeriod` |  |  |  |  |  | `Decimal(5,0)` |  | Max. Storage Period |  | S/4 only entity |
| `ProvisioningServiceLevel` |  |  |  |  |  | `String(1)` |  | Service Level |  | S/4 only entity |
| `IsActiveEntity` |  |  |  |  |  | `Boolean` |  | Is active |  | S/4 only entity |
| `ProdMaximumStoragePeriodUnit` |  |  |  |  |  | `String(3)` |  | Time unit |  | S/4 only entity |
| `WrhsMgmtPtwyAndStkRemovalStrgy` |  |  |  |  |  | `String(1)` |  | Putaway/StkRmvl |  | S/4 only entity |
| `CycleCountingIndicatorIsFixed` |  |  |  |  |  | `Boolean` |  | CC indicator fixed |  | S/4 only entity |
| `SegmentationStrategyForPlant` |  |  |  |  |  | `String(8)` |  | Segment. Strategy |  | S/4 only entity |
| `DefaultSegmentValue` |  |  |  |  |  | `String(40)` |  | Stock Segment |  | S/4 only entity |
| `SgmtHasPrioInProductStockSort` |  |  |  |  |  | `Boolean` |  | Sort Stock |  | S/4 only entity |


## Entity: `ProductPlantSupplyPlanning`

- **ABAP CDS Name:** `I_ProductPlantSupplyPlanning`
- **Label:** Product Plant Supply Planning
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Product |  | S/4 only entity |
| `Plant` |  |  |  |  |  | `String(4)` | Y | Plant |  | S/4 only entity |
| `FixedLotSizeQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Fixed lot size | BaseUnit | S/4 only entity |
| `MaximumLotSizeQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Maximum Lot Size | BaseUnit | S/4 only entity |
| `MinimumLotSizeQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Minimum Lot Size | BaseUnit | S/4 only entity |
| `LotSizeRoundingQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Rounding value | BaseUnit | S/4 only entity |
| `LotSizingProcedure` |  |  |  |  |  | `String(2)` |  | Lot Sizing Procedure |  | S/4 only entity |
| `MRPType` |  |  |  |  |  | `String(2)` |  | MRP Type |  | S/4 only entity |
| `MRPResponsible` |  |  |  |  |  | `String(3)` |  | MRP Controller |  | S/4 only entity |
| `SafetyStockQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Safety Stock | BaseUnit | S/4 only entity |
| `MinimumSafetyStockQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Min. Saf. Stock | BaseUnit | S/4 only entity |
| `PlanningTimeFence` |  |  |  |  |  | `String(3)` |  | Planning time fence |  | S/4 only entity |
| `ConsumptionValueCategory` |  |  |  |  |  | `String(1)` |  | ABC Indicator |  | S/4 only entity |
| `MaximumStockQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Maximum Stock Level | BaseUnit | S/4 only entity |
| `ReorderThresholdQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Reorder Point | BaseUnit | S/4 only entity |
| `PlannedDeliveryDurationInDays` |  |  |  |  |  | `Decimal(3,0)` |  | Planned Deliv. Time |  | S/4 only entity |
| `SafetySupplyDurationInDays` |  |  |  |  |  | `String(2)` |  | Safety Time |  | S/4 only entity |
| `PlanningStrategyGroup` |  |  |  |  |  | `String(2)` |  | Strategy Group |  | S/4 only entity |
| `TotalReplenishmentLeadTime` |  |  |  |  |  | `Decimal(3,0)` |  | Tot. repl. lead time |  | S/4 only entity |
| `ProcurementType` |  |  |  |  |  | `String(1)` |  | Procurement Type |  | S/4 only entity |
| `ProcurementSubType` |  |  |  |  |  | `String(2)` |  | Special Procurement |  | S/4 only entity |
| `AssemblyScrapPercent` |  |  |  |  |  | `Decimal(5,2)` |  | Assembly scrap (%) |  | S/4 only entity |
| `AvailabilityCheckType` |  |  |  |  |  | `String(2)` |  | Availability check |  | S/4 only entity |
| `GoodsReceiptDuration` |  |  |  |  |  | `Decimal(3,0)` |  | GR processing time |  | S/4 only entity |
| `PlanAndOrderDayDetermination` |  |  |  |  |  | `String(3)` |  | Planning Cycle |  | S/4 only entity |
| `RoundingProfile` |  |  |  |  |  | `String(4)` |  | Rounding Profile |  | S/4 only entity |
| `DfltStorageLocationExtProcmt` |  |  |  |  |  | `String(4)` |  | Storage Location |  | S/4 only entity |
| `GoodIssueProcessingDays` |  |  |  |  |  | `Decimal(3,0)` |  | GI Proc. Time |  | S/4 only entity |
| `ConsignmentControl` |  |  |  |  |  | `String(1)` |  | Consign.Control |  | S/4 only entity |
| `IsActiveEntity` |  |  |  |  |  | `Boolean` |  | Is active |  | S/4 only entity |
| `MRPGroup` |  |  |  |  |  | `String(4)` |  | MRP Group |  | S/4 only entity |
| `LotSizeIndependentCosts` |  |  |  |  |  | `Decimal(34,4)` |  | LS-Independent Costs | Currency | S/4 only entity |
| `StorageCostsPercentageCode` |  |  |  |  |  | `String(1)` |  | Storage Costs Code |  | S/4 only entity |
| `RqmtQtyRcptTaktTmeInWrkgDays` |  |  |  |  |  | `Decimal(3,0)` |  | Takt time |  | S/4 only entity |
| `MRPPlanningCalendar` |  |  |  |  |  | `String(3)` |  | Planning Calendar |  | S/4 only entity |
| `RangeOfCvrgPrflCode` |  |  |  |  |  | `String(3)` |  | Coverage Profile |  | S/4 only entity |
| `ProductSafetyTimeMRPRelevance` |  |  |  |  |  | `String(1)` |  | Safety Time Ind |  | S/4 only entity |
| `SafetyTimePeriodProfile` |  |  |  |  |  | `String(3)` |  | Time Profile |  | S/4 only entity |
| `DependentRqmtMRPRelevance` |  |  |  |  |  | `String(1)` |  | MRP Relevant |  | S/4 only entity |
| `ProductServiceLevelInPercent` |  |  |  |  |  | `Decimal(3,1)` |  | Service level (%) |  | S/4 only entity |
| `ProdInhProdnDurationInWorkDays` |  |  |  |  |  | `Decimal(3,0)` |  | In-house production |  | S/4 only entity |
| `MRPAvailabilityType` |  |  |  |  |  | `String(1)` |  | Mixed MRP |  | S/4 only entity |
| `CrossProjectProduct` |  |  |  |  |  | `String(1)` |  | Cross-Project |  | S/4 only entity |
| `ProdnPlngAndControlCalendar` |  |  |  |  |  | `String(3)` |  | Planning Calendar |  | S/4 only entity |
| `FollowUpProduct` |  |  |  |  |  | `String(40)` |  | Follow-Up Material |  | S/4 only entity |
| `RepetitiveManufacturingIsAllwd` |  |  |  |  |  | `Boolean` |  | Repetitive Manufacturing Enabled |  | S/4 only entity |
| `DependentRequirementsType` |  |  |  |  |  | `String(1)` |  | Indiv./ Coll. |  | S/4 only entity |
| `ProductIsBulkComponent` |  |  |  |  |  | `Boolean` |  | Bulk Material |  | S/4 only entity |
| `RepetitiveManufacturingProfile` |  |  |  |  |  | `String(4)` |  | Repetitive Manufacturing Profile |  | S/4 only entity |
| `BackwardCnsmpnPeriodInWorkDays` |  |  |  |  |  | `String(3)` |  | Backward Consumption Period |  | S/4 only entity |
| `FwdConsumptionPeriodInWorkDays` |  |  |  |  |  | `String(3)` |  | Forward Consumption Period |  | S/4 only entity |
| `ProdRqmtsConsumptionMode` |  |  |  |  |  | `String(1)` |  | Consumption mode |  | S/4 only entity |
| `ProdFcstRequirementsSplitCode` |  |  |  |  |  | `String(1)` |  | Splitting Indicator |  | S/4 only entity |
| `EffectiveOutDate` |  |  |  |  |  | `Date` |  | Effective-Out Date |  | S/4 only entity |
| `MRPProfile` |  |  |  |  |  | `String(4)` |  | MRP profile |  | S/4 only entity |
| `SchedulingFloatProfile` |  |  |  |  |  | `String(3)` |  | Scheduling Float Profile |  | S/4 only entity |
| `ComponentScrapInPercent` |  |  |  |  |  | `Decimal(5,2)` |  | Component Scrap (%) |  | S/4 only entity |
| `ProductDiscontinuationCode` |  |  |  |  |  | `String(1)` |  | Discontinuation ind. |  | S/4 only entity |
| `ProductRequirementsGrouping` |  |  |  |  |  | `String(1)` |  | Requirements group |  | S/4 only entity |
| `ProductionInvtryManagedLoc` |  |  |  |  |  | `String(4)` |  | Storage Location |  | S/4 only entity |
| `ProductComponentBackflushCode` |  |  |  |  |  | `String(1)` |  | Backflush |  | S/4 only entity |
| `ProposedProductSupplyArea` |  |  |  |  |  | `String(10)` |  | Proposed Supply Area |  | S/4 only entity |
| `PlannedOrderActionControl` |  |  |  |  |  | `String(2)` |  | Action Control |  | S/4 only entity |
| `ProductUnitGroup` |  |  |  |  |  | `String(4)` |  | Unit of Measure Group |  | S/4 only entity |
| `MRPSafetyStockMethod` |  |  |  |  |  | `String(2)` |  | Safety Stock Method |  | S/4 only entity |
| `JITProdnConfProfile` |  |  |  |  |  | `String(4)` |  | JIT Production Confirmation Profile |  | S/4 only entity |
| `Currency` |  |  |  |  |  | `String(5)` |  | Currency |  | S/4 only entity |
| `CompanyCode` |  |  |  |  |  | `String(4)` |  | Company Code |  | S/4 only entity |
| `ValuationArea` |  |  |  |  |  | `String(4)` |  | Valuation Area |  | S/4 only entity |
| `BaseUnit` |  |  |  |  |  | `String(3)` |  | Base Unit of Measure |  | S/4 only entity |


## Entity: `ProductPlantWorkScheduling`

- **ABAP CDS Name:** `I_ProductWorkScheduling`
- **Label:** Product WorkScheduling core entity
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Product |  | S/4 only entity |
| `Plant` |  |  |  |  |  | `String(4)` | Y | Plant |  | S/4 only entity |
| `MaterialBaseQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Base quantity | BaseUnit | S/4 only entity |
| `UnlimitedOverDelivIsAllowed` |  |  |  |  |  | `Boolean` |  | Unltd Overdelivery |  | S/4 only entity |
| `OverDelivToleranceLimit` |  |  |  |  |  | `Decimal(3,1)` |  | Overdelivery Toler. |  | S/4 only entity |
| `UnderDelivToleranceLimit` |  |  |  |  |  | `Decimal(3,1)` |  | Underdelivery Toler. |  | S/4 only entity |
| `ProductionInvtryManagedLoc` |  |  |  |  |  | `String(4)` |  | Storage Location |  | S/4 only entity |
| `IsActiveEntity` |  |  |  |  |  | `Boolean` |  | Is active |  | S/4 only entity |
| `ProdnOrderIsBatchRequired` |  |  |  |  |  | `String(1)` |  | Batch entry |  | S/4 only entity |
| `ProdIsWithdrawnFrmProdnBin` |  |  |  |  |  | `Boolean` |  | Withdr.from prod.bin |  | S/4 only entity |
| `TransitionMatrixProductsGroup` |  |  |  |  |  | `String(20)` |  | Material Grouping |  | S/4 only entity |
| `OrderChangeManagementProfile` |  |  |  |  |  | `String(6)` |  | Change overall prof. |  | S/4 only entity |
| `MatlCompIsMarkedForBackflush` |  |  |  |  |  | `String(1)` |  | Backflush |  | S/4 only entity |
| `SetupAndTeardownTime` |  |  |  |  |  | `Decimal(5,2)` |  | Setup time |  | S/4 only entity |
| `ProductionSchedulingProfile` |  |  |  |  |  | `String(6)` |  | Production Scheduling Profile |  | S/4 only entity |
| `TransitionTime` |  |  |  |  |  | `Decimal(5,2)` |  | Interoperation |  | S/4 only entity |
| `ProcessingTimeInDays` |  |  |  |  |  | `Decimal(5,2)` |  | Processing time |  | S/4 only entity |
| `ProductionSupervisor` |  |  |  |  |  | `String(3)` |  | Prodn Supervisor |  | S/4 only entity |
| `ProductProductionQuantityUnit` |  |  |  |  |  | `String(3)` |  | Production unit |  | S/4 only entity |
| `HasProductionVersion` |  |  |  |  |  | `Boolean` |  | Version Indicator |  | S/4 only entity |
| `BaseUnit` |  |  |  |  |  | `String(3)` |  | Base Unit of Measure |  | S/4 only entity |


## Entity: `ProductProcurement`

- **ABAP CDS Name:** `I_Productprocurement`
- **Label:** Product Procurement
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Material |  | S/4 only entity |
| `PurchaseOrderQuantityUnit` |  |  |  |  |  | `String(3)` |  | Order Unit |  | S/4 only entity |
| `VarblPurOrdUnitStatus` |  |  |  |  |  | `String(1)` |  | Var. Order Unit |  | S/4 only entity |
| `PurchasingAcknProfile` |  |  |  |  |  | `String(4)` |  | Purchasing value key |  | S/4 only entity |
| `ProcurementRule` |  |  |  |  |  | `String(1)` |  | Procurement rule |  | S/4 only entity |
| `SourceOfSupplyCategory` |  |  |  |  |  | `String(1)` |  | Source of supply |  | S/4 only entity |
| `PurchasingGroup` |  |  |  |  |  | `String(3)` |  | Purchasing Group |  | S/4 only entity |
| `IsActiveEntity` |  |  |  |  |  | `Boolean` |  | Is active |  | S/4 only entity |
| `AuthorizationGroup` |  |  |  |  |  | `String(4)` |  | Authorization Group |  | S/4 only entity |


## Entity: `ProductQualityManagement`

- **ABAP CDS Name:** `I_Productqm`
- **Label:** Product QM active core entity
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Product |  | S/4 only entity |
| `QltyMgmtInProcmtIsActive` |  |  |  |  |  | `Boolean` |  | QM in Procur. Active |  | S/4 only entity |
| `AuthorizationGroup` |  |  |  |  |  | `String(4)` |  | Authorization Group |  | S/4 only entity |
| `CatalogProfile` |  |  |  |  |  | `String(9)` |  | Catalog Profile |  | S/4 only entity |


## Entity: `ProductSales`

- **ABAP CDS Name:** `I_ProductSales`
- **Label:** Product Sales
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Material |  | S/4 only entity |
| `SalesStatus` |  |  |  |  |  | `String(2)` |  | X-DChain Status |  | S/4 only entity |
| `SalesStatusValidityDate` |  |  |  |  |  | `Date` |  | Cross-Distr. Chain Product Validity |  | S/4 only entity |
| `TaxClassification` |  |  |  |  |  | `String(1)` |  | Tax classification |  | S/4 only entity |
| `TransportationGroup` |  |  |  |  |  | `String(4)` |  | Transportation Group |  | S/4 only entity |
| `AllowedPackagingWeightQty` |  |  |  |  |  | `Decimal(13,3)` |  | Allowed Pkg wt | AllowedPackagingWeightQtyUnit | S/4 only entity |
| `AllowedPackagingWeightQtyUnit` |  |  |  |  |  | `String(3)` |  | Allowed Packaging Unit of Weight |  | S/4 only entity |
| `AllowedPackagingVolumeQty` |  |  |  |  |  | `Decimal(13,3)` |  | Allowed Volume | AllowedPackagingVolumeQtyUnit | S/4 only entity |
| `AllowedPackagingVolumeQtyUnit` |  |  |  |  |  | `String(3)` |  | Allowed Packaging Unit of Volume |  | S/4 only entity |
| `PricingReferenceProduct` |  |  |  |  |  | `String(40)` |  | Pricing Ref. Matl |  | S/4 only entity |
| `VariantsPricingProfile` |  |  |  |  |  | `String(1)` |  | Pricing profile |  | S/4 only entity |
| `IsVariantPriceAllowed` |  |  |  |  |  | `Boolean` |  | Var. Price Allowed |  | S/4 only entity |
| `LoadingGroup` |  |  |  |  |  | `String(4)` |  | Loading Group |  | S/4 only entity |
| `IsActiveEntity` |  |  |  |  |  | `Boolean` |  | Is active |  | S/4 only entity |
| `ExcessWeightTolerance` |  |  |  |  |  | `Decimal(3,1)` |  | Excess Weight Tolerance |  | S/4 only entity |
| `ExcessVolumeTolerance` |  |  |  |  |  | `Decimal(3,1)` |  | Excess Volume Tolerance |  | S/4 only entity |
| `PackagingMaterialType` |  |  |  |  |  | `String(4)` |  | Packaging Material Type |  | S/4 only entity |
| `IsClosedPackagingMaterial` |  |  |  |  |  | `Boolean` |  | Closed |  | S/4 only entity |
| `VolumeMaximumLevel` |  |  |  |  |  | `Decimal(3,0)` |  | Maximum level |  | S/4 only entity |
| `AuthorizationGroup` |  |  |  |  |  | `String(4)` |  | Authorization Group |  | S/4 only entity |
| `MaterialFreightGroup` |  |  |  |  |  | `String(8)` |  | Material Freight Grp |  | S/4 only entity |
| `StackingFactor` |  |  |  |  |  | `Integer` |  | Stackability factor |  | S/4 only entity |
| `ServiceDuration` |  |  |  |  |  | `Decimal(13,3)` |  | Duration of Work |  | S/4 only entity |
| `ServiceDurationUnit` |  |  |  |  |  | `String(3)` |  | Unit |  | S/4 only entity |
| `ServiceProfile` |  |  |  |  |  | `String(10)` |  | Service Profile |  | S/4 only entity |
| `ResponseProfile` |  |  |  |  |  | `String(10)` |  | Response Prof. |  | S/4 only entity |
| `CABillgCycle` |  |  |  |  |  | `String(4)` |  | Billing Cycle |  | S/4 only entity |
| `SubscrpnProdBillgCycDetn` |  |  |  |  |  | `String(4)` |  | Billing Cycle Determ |  | S/4 only entity |
| `SubscrpnProdTechRsceSchema` |  |  |  |  |  | `String(2)` |  | Assignment Schema |  | S/4 only entity |
| `ContractAutoRenewalType` |  |  |  |  |  | `String(1)` |  | Ctr. Auto Renew Ind. |  | S/4 only entity |


## Entity: `ProductSalesDelivery`

- **ABAP CDS Name:** `I_ProductSalesDelivery`
- **Label:** Product Sales Delivery
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Product |  | S/4 only entity |
| `ProductSalesOrg` |  |  |  |  |  | `String(4)` | Y | Sales Organization |  | S/4 only entity |
| `ProductDistributionChnl` |  |  |  |  |  | `String(2)` | Y | Distribution Channel |  | S/4 only entity |
| `MinimumOrderQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Minimum order qty | BaseUnit | S/4 only entity |
| `SupplyingPlant` |  |  |  |  |  | `String(4)` |  | Delivering Plant |  | S/4 only entity |
| `PriceSpecificationProductGroup` |  |  |  |  |  | `String(2)` |  | Product Price Group |  | S/4 only entity |
| `AccountDetnProductGroup` |  |  |  |  |  | `String(2)` |  | Acct Assmt Grp Mat. |  | S/4 only entity |
| `DeliveryNoteProcMinDelivQty` |  |  |  |  |  | `Decimal(13,3)` |  | Minimum Delivery Qty | BaseUnit | S/4 only entity |
| `ItemCategoryGroup` |  |  |  |  |  | `String(4)` |  | Item Category Group |  | S/4 only entity |
| `DeliveryQuantityUnit` |  |  |  |  |  | `String(3)` |  | Unit Of Measure |  | S/4 only entity |
| `DeliveryQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Delivery unit | DeliveryQuantityUnit | S/4 only entity |
| `ProductSalesStatus` |  |  |  |  |  | `String(2)` |  | DChain-spec. status |  | S/4 only entity |
| `ProductSalesStatusValidityDate` |  |  |  |  |  | `Date` |  | Valid from |  | S/4 only entity |
| `SalesMeasureUnit` |  |  |  |  |  | `String(3)` |  | Sales Unit |  | S/4 only entity |
| `IsMarkedForDeletion` |  |  |  |  |  | `Boolean` |  | DF distr. chain lvl |  | S/4 only entity |
| `ProductHierarchy` |  |  |  |  |  | `String(18)` |  | Product Hierarchy |  | S/4 only entity |
| `FirstSalesSpecProductGroup` |  |  |  |  |  | `String(3)` |  | Product Group 1 |  | S/4 only entity |
| `SecondSalesSpecProductGroup` |  |  |  |  |  | `String(3)` |  | Product Group 2 |  | S/4 only entity |
| `ThirdSalesSpecProductGroup` |  |  |  |  |  | `String(3)` |  | Product Group 3 |  | S/4 only entity |
| `FourthSalesSpecProductGroup` |  |  |  |  |  | `String(3)` |  | Product Group 4 |  | S/4 only entity |
| `FifthSalesSpecProductGroup` |  |  |  |  |  | `String(3)` |  | Product Group 5 |  | S/4 only entity |
| `MinimumMakeToOrderOrderQty` |  |  |  |  |  | `Decimal(13,3)` |  | Min. MtO quantity | BaseUnit | S/4 only entity |
| `LogisticsStatisticsGroup` |  |  |  |  |  | `String(1)` |  | Matl statistics grp |  | S/4 only entity |
| `VolumeRebateGroup` |  |  |  |  |  | `String(2)` |  | Volume Rebate Group |  | S/4 only entity |
| `ProductCommissionGroup` |  |  |  |  |  | `String(2)` |  | Commission Group |  | S/4 only entity |
| `CashDiscountIsDeductible` |  |  |  |  |  | `Boolean` |  | Cash Discount |  | S/4 only entity |
| `PricingReferenceProduct` |  |  |  |  |  | `String(40)` |  | Pricing Ref. Matl |  | S/4 only entity |
| `AssortmentGrade` |  |  |  |  |  | `String(2)` |  | Assortment Grade |  | S/4 only entity |
| `StoreListingProcedure` |  |  |  |  |  | `String(2)` |  | LP for Stores |  | S/4 only entity |
| `DistrCntrListingProcedure` |  |  |  |  |  | `String(2)` |  | LP distr. ctrs |  | S/4 only entity |
| `StoreListingStartDate` |  |  |  |  |  | `Date` |  | Store Listed from |  | S/4 only entity |
| `StoreListingEndDate` |  |  |  |  |  | `Date` |  | Store Listed to |  | S/4 only entity |
| `DistrCntrListingStartDate` |  |  |  |  |  | `Date` |  | DC Listed from |  | S/4 only entity |
| `DistrCntrListingEndDate` |  |  |  |  |  | `Date` |  | DC Listed to |  | S/4 only entity |
| `StoreSaleStartDate` |  |  |  |  |  | `Date` |  | For sale from (str) |  | S/4 only entity |
| `StoreSaleEndDate` |  |  |  |  |  | `Date` |  | For sale till (str) |  | S/4 only entity |
| `DistrCntrSaleStartDate` |  |  |  |  |  | `Date` |  | For sale from (DC) |  | S/4 only entity |
| `DistrCntrSaleEndDate` |  |  |  |  |  | `Date` |  | For sale till (DC) |  | S/4 only entity |
| `RoundingProfile` |  |  |  |  |  | `String(4)` |  | Rounding Profile |  | S/4 only entity |
| `ProductUnitGroup` |  |  |  |  |  | `String(4)` |  | Unit of Measure Grp |  | S/4 only entity |
| `MaxDeliveryQtyStoreOrder` |  |  |  |  |  | `Decimal(13,3)` |  | Max. delivery qty | BaseUnit | S/4 only entity |
| `PriceFixingCategory` |  |  |  |  |  | `String(1)` |  | Price fixing |  | S/4 only entity |
| `VariableSalesUnitIsNotAllowed` |  |  |  |  |  | `Boolean` |  | Sales unit not var. |  | S/4 only entity |
| `CompetitionPressureCategory` |  |  |  |  |  | `String(1)` |  | Competition charactn |  | S/4 only entity |
| `ProductHasAttributeID01` |  |  |  |  |  | `Boolean` |  | Product Attribute 1 |  | S/4 only entity |
| `ProductHasAttributeID02` |  |  |  |  |  | `Boolean` |  | Product Attribute 2 |  | S/4 only entity |
| `ProductHasAttributeID03` |  |  |  |  |  | `Boolean` |  | Product Attribute 3 |  | S/4 only entity |
| `ProductHasAttributeID04` |  |  |  |  |  | `Boolean` |  | Product Attribute 4 |  | S/4 only entity |
| `ProductHasAttributeID05` |  |  |  |  |  | `Boolean` |  | Product Attribute 5 |  | S/4 only entity |
| `ProductHasAttributeID06` |  |  |  |  |  | `Boolean` |  | Product Attribute 6 |  | S/4 only entity |
| `ProductHasAttributeID07` |  |  |  |  |  | `Boolean` |  | Product Attribute 7 |  | S/4 only entity |
| `ProductHasAttributeID08` |  |  |  |  |  | `Boolean` |  | Product Attribute 8 |  | S/4 only entity |
| `ProductHasAttributeID09` |  |  |  |  |  | `Boolean` |  | Product Attribute 9 |  | S/4 only entity |
| `ProductHasAttributeID10` |  |  |  |  |  | `Boolean` |  | Product Attribute 10 |  | S/4 only entity |
| `IsActiveEntity` |  |  |  |  |  | `Boolean` |  | Is active |  | S/4 only entity |
| `ProdExtAssortmentPriority` |  |  |  |  |  | `String(1)` |  | Ext. asst priority |  | S/4 only entity |
| `ProdIsEntlmntRlvt` |  |  |  |  |  | `Boolean` |  | Rel. Entitlement Gen |  | S/4 only entity |
| `BaseUnit` |  |  |  |  |  | `String(3)` |  | Base Unit of Measure |  | S/4 only entity |
| `SubscrpnContrDfltDuration` |  |  |  |  |  | `String(3)` |  | Def Contract Term |  | S/4 only entity |
| `SubscrpnContrAltvDuration1` |  |  |  |  |  | `String(3)` |  | Contract Term 1 |  | S/4 only entity |
| `SubscrpnContrAltvDuration2` |  |  |  |  |  | `String(3)` |  | Contract Term 2 |  | S/4 only entity |
| `SubscrpnContrDurationUnit` |  |  |  |  |  | `String(1)` |  | Unit Contract Term |  | S/4 only entity |
| `SubscrpnContrDfltExtnDurn` |  |  |  |  |  | `String(3)` |  | Def Extension Period |  | S/4 only entity |
| `SubscrpnContrAltvExtnDurn1` |  |  |  |  |  | `String(3)` |  | Extension Period 1 |  | S/4 only entity |
| `SubscrpnContrAltvExtnDurn2` |  |  |  |  |  | `String(3)` |  | Extension Period 2 |  | S/4 only entity |
| `SubscrpnContrExtnDurnUnit` |  |  |  |  |  | `String(1)` |  | Unit for Extension |  | S/4 only entity |
| `LstMiProductPackageSizeCode` |  |  |  |  |  | `String(3)` |  | Package Size |  | S/4 only entity |
| `LstMiProductPackageType` |  |  |  |  |  | `String(3)` |  | Package Type |  | S/4 only entity |


## Entity: `ProductStorage`

- **ABAP CDS Name:** `I_ProductStorage_2`
- **Label:** Product Storage
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Material |  | S/4 only entity |
| `StorageConditions` |  |  |  |  |  | `String(2)` |  | Storage conditions |  | S/4 only entity |
| `TemperatureConditionInd` |  |  |  |  |  | `String(2)` |  | Temp. conditions |  | S/4 only entity |
| `HazardousMaterialNumber` |  |  |  |  |  | `String(40)` |  | Haz. material number |  | S/4 only entity |
| `NmbrOfGROrGISlipsToPrintQty` |  |  |  |  |  | `Decimal(13,3)` |  | GR slips quantity | BaseUnit | S/4 only entity |
| `LabelType` |  |  |  |  |  | `String(2)` |  | Label type |  | S/4 only entity |
| `LabelForm` |  |  |  |  |  | `String(2)` |  | Label form |  | S/4 only entity |
| `MinRemainingShelfLife` |  |  |  |  |  | `Decimal(4,0)` |  | Min. Rem. Shelf Life |  | S/4 only entity |
| `ProductExpirationDateCode` |  |  |  |  |  | `String(1)` |  | Expiration Date |  | S/4 only entity |
| `StorageBinInstruction` |  |  |  |  |  | `String(2)` |  | Container reqmts |  | S/4 only entity |
| `TotalShelfLifeStoragePercent` |  |  |  |  |  | `Decimal(3,0)` |  | Storage percentage |  | S/4 only entity |
| `ShelfLifeExpirationDatePeriod` |  |  |  |  |  | `String(1)` |  | Period Ind. for SLED |  | S/4 only entity |
| `ShelfLifeExprtnDateRndngRule` |  |  |  |  |  | `String(1)` |  | Rounding rule SLED |  | S/4 only entity |
| `AuthorizationGroup` |  |  |  |  |  | `String(4)` |  | Authorization Group |  | S/4 only entity |
| `IsActiveEntity` |  |  |  |  |  | `Boolean` |  | Is active |  | S/4 only entity |
| `TotalShelfLife` |  |  |  |  |  | `Decimal(4,0)` |  | Total Shelf Life |  | S/4 only entity |
| `BaseUnit` |  |  |  |  |  | `String(3)` |  | Base Unit of Measure |  | S/4 only entity |


## Entity: `ProductUnitOfMeasure`

- **ABAP CDS Name:** `I_ProductUnitsOfMeasure`
- **Label:** Units of Measure of Product
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Product |  | S/4 only entity |
| `AlternativeUnit` |  |  |  |  |  | `String(3)` | Y | AlternativeUnit |  | S/4 only entity |
| `QuantityNumerator` |  |  |  |  |  | `Decimal(5,0)` |  | Units / Quantity - Base Unit of Measure | BaseUnit | S/4 only entity |
| `QuantityDenominator` |  |  |  |  |  | `Decimal(5,0)` |  | Units / Quantity - Alt Unit of Measure | AlternativeUnit | S/4 only entity |
| `MaterialVolume` |  |  |  |  |  | `Decimal(13,3)` |  | Volume | VolumeUnit | S/4 only entity |
| `VolumeUnit` |  |  |  |  |  | `String(3)` |  | Volume Unit |  | S/4 only entity |
| `GrossWeight` |  |  |  |  |  | `Decimal(13,3)` |  | Gross Weight | WeightUnit | S/4 only entity |
| `WeightUnit` |  |  |  |  |  | `String(3)` |  | Unit of Weight |  | S/4 only entity |
| `GlobalTradeItemNumber` |  |  |  |  |  | `String(18)` |  | EAN/UPC |  | S/4 only entity |
| `GlobalTradeItemNumberCategory` |  |  |  |  |  | `String(2)` |  | GTIN Category |  | S/4 only entity |
| `UnitSpecificProductLength` |  |  |  |  |  | `Decimal(13,3)` |  | Length | ProductMeasurementUnit | S/4 only entity |
| `UnitSpecificProductWidth` |  |  |  |  |  | `Decimal(13,3)` |  | Width | ProductMeasurementUnit | S/4 only entity |
| `UnitSpecificProductHeight` |  |  |  |  |  | `Decimal(13,3)` |  | Height | ProductMeasurementUnit | S/4 only entity |
| `ProductMeasurementUnit` |  |  |  |  |  | `String(3)` |  | Unit of Dimension |  | S/4 only entity |
| `LowerLevelPackagingUnit` |  |  |  |  |  | `String(3)` |  | Lower-level unit |  | S/4 only entity |
| `RemainingVolumeAfterNesting` |  |  |  |  |  | `Decimal(3,0)` |  | Rem.Vol.After Nestng |  | S/4 only entity |
| `MaximumStackingFactor` |  |  |  |  |  | `Integer` |  | Max. Stacking Factor |  | S/4 only entity |
| `CapacityUsage` |  |  |  |  |  | `Decimal(15,3)` |  | Capacity Usage |  | S/4 only entity |
| `IsActiveEntity` |  |  |  |  |  | `Boolean` |  | Is active |  | S/4 only entity |
| `UnitOfMeasureCategory` |  |  |  |  |  | `String(1)` |  | UoM Category |  | S/4 only entity |
| `ProductGTINVariant` |  |  |  |  |  | `String(2)` |  | EAN Variant |  | S/4 only entity |
| `BaseUnit` |  |  |  |  |  | `String(3)` |  | Base Unit of Measure |  | S/4 only entity |


## Entity: `ProductUnitOfMeasureEAN`

- **ABAP CDS Name:** `I_ProductUnitOfMeasureEAN`
- **Label:** International Article Number of Product
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Material |  | S/4 only entity |
| `AlternativeUnit` |  |  |  |  |  | `String(3)` | Y | Display Unit/Measure |  | S/4 only entity |
| `ConsecutiveNumber` |  |  |  |  |  | `String(5)` | Y | Consecutive number |  | S/4 only entity |
| `ProductStandardID` |  |  |  |  |  | `String(18)` |  | EAN/UPC |  | S/4 only entity |
| `InternationalArticleNumberCat` |  |  |  |  |  | `String(2)` |  | GTIN Category |  | S/4 only entity |
| `IsMainGlobalTradeItemNumber` |  |  |  |  |  | `Boolean` |  | Main EAN |  | S/4 only entity |


## Entity: `ProductValuation`

- **ABAP CDS Name:** `I_ProductValuationBasic`
- **Label:** Product Valuation
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Product |  | S/4 only entity |
| `ValuationArea` |  |  |  |  |  | `String(4)` | Y | Valuation Area |  | S/4 only entity |
| `ValuationType` |  |  |  |  |  | `String(10)` | Y | Valuation Type |  | S/4 only entity |
| `ValuationClass` |  |  |  |  |  | `String(4)` |  | Valuation Class |  | S/4 only entity |
| `PriceDeterminationControl` |  |  |  |  |  | `String(1)` |  | Price Determ. |  | S/4 only entity |
| `FiscalMonthCurrentPeriod` |  |  |  |  |  | `String(2)` |  | Current Period |  | S/4 only entity |
| `FiscalYearCurrentPeriod` |  |  |  |  |  | `String(4)` |  | Year Current Period |  | S/4 only entity |
| `StandardPrice` |  |  |  |  |  | `Decimal(34,4)` |  | Standard price | Currency | S/4 only entity |
| `PriceUnitQty` |  |  |  |  |  | `Decimal(5,0)` |  | Price unit |  | S/4 only entity |
| `InventoryValuationProcedure` |  |  |  |  |  | `String(1)` |  | Price Control |  | S/4 only entity |
| `FuturePriceValidityStartDate` |  |  |  |  |  | `Date` |  | Valid from |  | S/4 only entity |
| `PrevInvtryPriceInCoCodeCrcy` |  |  |  |  |  | `Decimal(34,4)` |  | Previous Price | Currency | S/4 only entity |
| `MovingAveragePrice` |  |  |  |  |  | `Decimal(34,4)` |  | Moving price | Currency | S/4 only entity |
| `ValuationCategory` |  |  |  |  |  | `String(1)` |  | Valuation Category |  | S/4 only entity |
| `ProductUsageType` |  |  |  |  |  | `String(1)` |  | Product Usage |  | S/4 only entity |
| `ProductOriginType` |  |  |  |  |  | `String(1)` |  | Product Origin |  | S/4 only entity |
| `IsProducedInhouse` |  |  |  |  |  | `Boolean` |  | In-House Production |  | S/4 only entity |
| `ProdCostEstNumber` |  |  |  |  |  | `String(12)` |  | ProdCostEst.No. |  | S/4 only entity |
| `IsMarkedForDeletion` |  |  |  |  |  | `Boolean` |  | Del. flag val. type |  | S/4 only entity |
| `ValuationMargin` |  |  |  |  |  | `Decimal(6,2)` |  | Valuation Margin |  | S/4 only entity |
| `IsActiveEntity` |  |  |  |  |  | `Boolean` |  | Is active |  | S/4 only entity |
| `CompanyCode` |  |  |  |  |  | `String(4)` |  | Company Code |  | S/4 only entity |
| `ValuationClassSalesOrderStock` |  |  |  |  |  | `String(4)` |  | VC: Sales Order Stk |  | S/4 only entity |
| `ProjectStockValuationClass` |  |  |  |  |  | `String(4)` |  | Proj. stk val. class |  | S/4 only entity |
| `TaxBasedPricesPriceUnitQty` |  |  |  |  |  | `Decimal(5,0)` |  | Price Unit | BaseUnit | S/4 only entity |
| `PriceLastChangeDate` |  |  |  |  |  | `Date` |  | Last Price Change |  | S/4 only entity |
| `FuturePrice` |  |  |  |  |  | `Decimal(34,4)` |  | Future Price | Currency | S/4 only entity |
| `MaintenanceStatus` |  |  |  |  |  | `String(15)` |  | Maintenance Status |  | S/4 only entity |
| `Currency` |  |  |  |  |  | `String(5)` |  | Currency |  | S/4 only entity |
| `BaseUnit` |  |  |  |  |  | `String(3)` |  | Base Unit of Measure |  | S/4 only entity |
| `MLIsActiveAtProductLevel` |  |  |  |  |  | `Boolean` |  | ML Act. |  | S/4 only entity |


## Entity: `ProductValuationAccounting`

- **ABAP CDS Name:** `I_ProductValuationAccounting_2`
- **Label:** Product Valuation Account
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Product |  | S/4 only entity |
| `ValuationArea` |  |  |  |  |  | `String(4)` | Y | Valuation Area |  | S/4 only entity |
| `ValuationType` |  |  |  |  |  | `String(10)` | Y | Valuation Type |  | S/4 only entity |
| `CommercialPrice1InCoCodeCrcy` |  |  |  |  |  | `Decimal(34,4)` |  | Commercial price 1 | Currency | S/4 only entity |
| `CommercialPrice2InCoCodeCrcy` |  |  |  |  |  | `Decimal(34,4)` |  | Commercial price 2 | Currency | S/4 only entity |
| `CommercialPrice3InCoCodeCrcy` |  |  |  |  |  | `Decimal(34,4)` |  | Commercial price 3 | Currency | S/4 only entity |
| `DevaluationYearCount` |  |  |  |  |  | `String(2)` |  | Devaluation Ind. |  | S/4 only entity |
| `FuturePrice` |  |  |  |  |  | `Decimal(34,4)` |  | Future Price | Currency | S/4 only entity |
| `FuturePriceValidityStartDate` |  |  |  |  |  | `Date` |  | Valid from |  | S/4 only entity |
| `IsLIFOAndFIFORelevant` |  |  |  |  |  | `Boolean` |  | TRUE |  | S/4 only entity |
| `LIFOValuationPoolNumber` |  |  |  |  |  | `String(4)` |  | LIFO Pool |  | S/4 only entity |
| `StandardPricePrevYear` |  |  |  |  |  | `Decimal(34,4)` |  | Standard price | Currency | S/4 only entity |
| `TaxPricel1InCoCodeCrcy` |  |  |  |  |  | `Decimal(34,4)` |  | Tax price 1 | Currency | S/4 only entity |
| `TaxPrice2InCoCodeCrcy` |  |  |  |  |  | `Decimal(34,4)` |  | Tax price 2 | Currency | S/4 only entity |
| `TaxPrice3InCoCodeCrcy` |  |  |  |  |  | `Decimal(34,4)` |  | Tax price 3 | Currency | S/4 only entity |
| `TaxBasedPricesPriceUnitQty` |  |  |  |  |  | `Decimal(5,0)` |  | Price Unit | BaseUnit | S/4 only entity |
| `CompanyCode` |  |  |  |  |  | `String(4)` |  | Company Code |  | S/4 only entity |
| `Currency` |  |  |  |  |  | `String(5)` |  | Currency |  | S/4 only entity |
| `BaseUnit` |  |  |  |  |  | `String(3)` |  | Base Unit of Measure |  | S/4 only entity |


## Entity: `ProductValuationCosting`

- **ABAP CDS Name:** `I_ProductValuationCosting`
- **Label:** Product Valuation Costing Core Entity
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Product |  | S/4 only entity |
| `ValuationArea` |  |  |  |  |  | `String(4)` | Y | Valuation Area |  | S/4 only entity |
| `ValuationType` |  |  |  |  |  | `String(10)` | Y | Valuation Type |  | S/4 only entity |
| `IsMaterialCostedWithQtyStruc` |  |  |  |  |  | `Boolean` |  | With Qty Structure |  | S/4 only entity |
| `IsMaterialRelatedOrigin` |  |  |  |  |  | `Boolean` |  | Material origin |  | S/4 only entity |
| `CostOriginGroup` |  |  |  |  |  | `String(4)` |  | Origin Group |  | S/4 only entity |
| `CostingOverheadGroup` |  |  |  |  |  | `String(10)` |  | Overhead Group |  | S/4 only entity |
| `PlannedPrice1InCoCodeCrcy` |  |  |  |  |  | `Decimal(34,4)` |  | Planned price 1 | Currency | S/4 only entity |
| `PlannedPrice2InCoCodeCrcy` |  |  |  |  |  | `Decimal(34,4)` |  | Planned price 2 | Currency | S/4 only entity |
| `PlannedPrice3InCoCodeCrcy` |  |  |  |  |  | `Decimal(34,4)` |  | Planned price 3 | Currency | S/4 only entity |
| `FuturePlndPrice1ValdtyDate` |  |  |  |  |  | `Date` |  | Planned price date 1 |  | S/4 only entity |
| `FuturePlndPrice2ValdtyDate` |  |  |  |  |  | `Date` |  | Planned price date 2 |  | S/4 only entity |
| `FuturePlndPrice3ValdtyDate` |  |  |  |  |  | `Date` |  | Planned price date 3 |  | S/4 only entity |
| `PlannedPrice` |  |  |  |  |  | `Decimal(34,4)` |  | Future Planned Price | Currency | S/4 only entity |
| `Currency` |  |  |  |  |  | `String(5)` |  | Currency |  | S/4 only entity |
| `CompanyCode` |  |  |  |  |  | `String(4)` |  | Company Code |  | S/4 only entity |


## Entity: `ProductWarehouseManagement`

- **ABAP CDS Name:** `I_ProductWrhsMgmt`
- **Label:** Product Warehouse Management
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Product |  | S/4 only entity |
| `WarehouseNumber` |  |  |  |  |  | `String(3)` | Y | Warehouse Number |  | S/4 only entity |
| `ProdWrhsMatlDataIsMrkdForDeltn` |  |  |  |  |  | `Boolean` |  | Del.flag:warehse no. |  | S/4 only entity |
| `ProdStorageSectionMethod` |  |  |  |  |  | `String(3)` |  | Storage Section Ind. |  | S/4 only entity |
| `ProdWrhsStkPlacementStorType` |  |  |  |  |  | `String(3)` |  | Stock placement |  | S/4 only entity |
| `ProdWrhsStkRemovalStorageType` |  |  |  |  |  | `String(3)` |  | Stock removal |  | S/4 only entity |
| `ProdWrhs1stLoadgEquipQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Loading equip. qty 1 | ProdWrhs1stLoadgEquipQtyUnit | S/4 only entity |
| `ProdWrhs2ndLoadgEquipQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Loading equip. qty 2 | ProdWrhs2ndLoadgEquipQtyUnit | S/4 only entity |
| `ProdWrhs3rdLoadgEquipQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Loading equip. qty 3 | ProdWrhs3rdLoadgEquipQtyUnit | S/4 only entity |
| `ProdWrhs1stLoadgEquipQtyUnit` |  |  |  |  |  | `String(3)` |  | Unit of measure 1 |  | S/4 only entity |
| `ProdWrhs2ndLoadgEquipQtyUnit` |  |  |  |  |  | `String(3)` |  | Unit of measure 2 |  | S/4 only entity |
| `ProdWrhs3rdLoadgEquipQtyUnit` |  |  |  |  |  | `String(3)` |  | Unit of measure 3 |  | S/4 only entity |
| `ProductStorageUnitType1` |  |  |  |  |  | `String(3)` |  | Storage Unit Type 1 |  | S/4 only entity |
| `ProductStorageUnitType2` |  |  |  |  |  | `String(3)` |  | Storage Unit Type 2 |  | S/4 only entity |
| `ProductStorageUnitType3` |  |  |  |  |  | `String(3)` |  | Storage Unit Type 3 |  | S/4 only entity |
| `ProdWarehouseManagementUnit` |  |  |  |  |  | `String(3)` |  | WM unit |  | S/4 only entity |
| `AdditionToExistingStkIsAllowed` |  |  |  |  |  | `Boolean` |  | Allow addn to stock |  | S/4 only entity |
| `ProductBulkStorageMethod` |  |  |  |  |  | `String(2)` |  | Bulk storage |  | S/4 only entity |
| `WrhsMgmtMsgToInvtryMgmtIsRqd` |  |  |  |  |  | `Boolean` |  | Message to inv. mgmt |  | S/4 only entity |
| `WrhsMgmtHasSpecialMovement` |  |  |  |  |  | `String(1)` |  | Special movement |  | S/4 only entity |
| `CapacityUsage` |  |  |  |  |  | `Decimal(11,3)` |  | Capacity usage |  | S/4 only entity |
| `CapacityConsumptionUnit` |  |  |  |  |  | `String(3)` |  | Cap.consumption unit |  | S/4 only entity |
| `ProdWrhsPickingStorageType` |  |  |  |  |  | `String(3)` |  | Picking storage type |  | S/4 only entity |
| `ProdWrhsMatlMasterDefaultUnit` |  |  |  |  |  | `String(1)` |  | Proposed UoM frm mat |  | S/4 only entity |
| `ProdIsRlvtForTwoStepPicking` |  |  |  |  |  | `String(1)` |  | 2-step picking |  | S/4 only entity |
