# Product

> Source file: `sap-s4com-Product-v1.json`


## Entity: `ProdIntlTradeClassification`

- **ABAP CDS Name:** `I_ProdCommodityCodeDEX`
- **Label:** Data Extraction for Product Commodity Code by Country/Region
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** MARC

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `TrdClassfctnNmbrSchm` |  |  |  |  |  | `String(10)` | Y | Numbering Scheme |  |  |
| `Product` |  |  |  |  |  | `String(40)` | Y | Product |  |  |
| `CommodityCode` |  |  |  |  |  | `String(30)` | Y | Commodity Code |  |  |
| `ValidityStartDate` |  |  |  |  |  | `Date` | Y | Valid From |  |  |
| `Country` |  |  |  |  |  | `String(3)` | Y | Country/Region |  |  |
| `ValidityEndDate` |  |  |  |  |  | `Date` |  | Valid To |  |  |
| `TrdClassfctnNmbrUUID` |  |  |  |  |  | `UUID` |  |  |  |  |


## Entity: `ProdWhseManagementStorageType`

- **ABAP CDS Name:** `I_ProdWrhsMgmtStorageType`
- **Label:** Product Data For Each Storage Type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** MLGT

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Product |  |  |
| `WarehouseNumber` |  |  |  |  |  | `String(3)` | Y | Warehouse Number |  |  |
| `StorageType` |  |  |  |  |  | `String(3)` | Y | Storage Type |  |  |
| `ProdStorTypeMatlIsMrkdForDeltn` |  |  |  |  |  | `Boolean` |  | Del. flag: stge type |  |  |
| `StorageBin` |  |  |  |  |  | `String(10)` |  | Storage Bin |  |  |
| `ProdWrhsMaxStorageBinQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Maximum bin quantity | BaseUnit |  |
| `ProdWrhsMinStorageBinQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Minimum bin quantity | BaseUnit |  |
| `ProdWrhsStorTypeCtrlQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Control quantity | BaseUnit |  |
| `ProdWrhsStorTypeReplnmtQty` |  |  |  |  |  | `Decimal(13,3)` |  | Replenishment qty | BaseUnit |  |
| `LeanWrhsManagementPickingArea` |  |  |  |  |  | `String(3)` |  | Picking Area |  |  |
| `ProdWrhsStorTypeRoundingQty` |  |  |  |  |  | `Decimal(13,3)` |  | Rounding qty | BaseUnit |  |
| `BaseUnit` |  |  |  |  |  | `String(3)` |  | Base Unit of Measure |  |  |


## Entity: `Product`

- **ABAP CDS Name:** `I_Product`
- **Label:** Product
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** MARA, MAKT

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  | `MARA` | `MATNR` |  |  | `String(40)` | Y | Product |  |  |
| `ProductExternalID` |  |  |  |  |  | `String(40)` |  | Material |  |  |
| `ProductOID` |  |  |  |  |  | `String(128)` |  | Product OID |  |  |
| `ProductType` |  | `MARA` | `MTART` |  |  | `String(4)` |  | Product Type |  |  |
| `CreationDate` |  | `MARA` | `ERSDA` |  |  | `Date` |  | Created On |  |  |
| `CreationTime` |  |  |  |  |  | `String(6)` |  | Created At Time |  |  |
| `CreationDateTime` |  |  |  |  |  | `Timestamp` |  | Created On |  |  |
| `CreatedByUser` |  |  |  |  |  | `String(12)` |  | Created By |  |  |
| `LastChangeDate` |  |  |  |  |  | `Date` |  | Last Change |  |  |
| `LastChangedByUser` |  |  |  |  |  | `String(12)` |  | Changed By |  |  |
| `IsMarkedForDeletion` |  | `MARA` | `LVORM` |  |  | `Boolean` |  | Marked for Deletion |  |  |
| `CrossPlantStatus` |  |  |  |  |  | `String(2)` |  | CrossPlantProdStatus |  |  |
| `CrossPlantStatusValidityDate` |  |  |  |  |  | `Date` |  | Valid from |  |  |
| `ProductOldID` |  |  |  |  |  | `String(40)` |  | Old Product Number |  |  |
| `GrossWeight` |  | `MARA` | `BRGEW` |  |  | `Decimal(13,3)` |  | Gross Weight | WeightUnit |  |
| `PurchaseOrderQuantityUnit` |  |  |  |  |  | `String(3)` |  | Order Unit |  |  |
| `SourceOfSupply` |  |  |  |  |  | `String(1)` |  | Source of supply |  |  |
| `WeightUnit` |  | `MARA` | `GEWEI` |  |  | `String(3)` |  | Unit of Weight |  |  |
| `CountryOfOrigin` |  |  |  |  |  | `String(3)` |  | Cntry/Reg of Origin |  |  |
| `CompetitorID` |  |  |  |  |  | `String(10)` |  | Competitor |  |  |
| `ProductGroup` |  | `MARA` | `MATKL` |  |  | `String(9)` |  | Product Group |  |  |
| `BaseUnit` |  | `MARA` | `MEINS` |  |  | `String(3)` |  | Base Unit of Measure |  |  |
| `ItemCategoryGroup` |  |  |  |  |  | `String(4)` |  | Gen. item cat. grp |  |  |
| `NetWeight` |  | `MARA` | `NTGEW` |  |  | `Decimal(13,3)` |  | Net Weight | WeightUnit |  |
| `ProductHierarchy` |  |  |  |  |  | `String(18)` |  | Product Hierarchy |  |  |
| `Division` |  |  |  |  |  | `String(2)` |  | Division |  |  |
| `VarblPurOrdUnitIsActive` |  |  |  |  |  | `String(1)` |  | Var. Order Unit |  |  |
| `VolumeUnit` |  |  |  |  |  | `String(3)` |  | Volume Unit |  |  |
| `MaterialVolume` |  |  |  |  |  | `Decimal(13,3)` |  | Volume | VolumeUnit |  |
| `SalesStatus` |  |  |  |  |  | `String(2)` |  | X-DChain Status |  |  |
| `TransportationGroup` |  |  |  |  |  | `String(4)` |  | Transportation Group |  |  |
| `SalesStatusValidityDate` |  |  |  |  |  | `Date` |  | Valid from |  |  |
| `AuthorizationGroup` |  |  |  |  |  | `String(4)` |  | Authorization Group |  |  |
| `ANPCode` |  |  |  |  |  | `String(9)` |  | ANP Code |  |  |
| `ProductCategory` |  |  |  |  |  | `String(2)` |  | Product Category |  |  |
| `Brand` |  |  |  |  |  | `String(4)` |  | Brand |  |  |
| `ProcurementRule` |  |  |  |  |  | `String(1)` |  | Procurement rule |  |  |
| `ValidityStartDate` |  |  |  |  |  | `Date` |  | Valid From |  |  |
| `LowLevelCode` |  |  |  |  |  | `String(3)` |  | Low-Level Code |  |  |
| `ProdNoInGenProdInPrepackProd` |  |  |  |  |  | `String(40)` |  | Generic Material |  |  |
| `SerialIdentifierAssgmtProfile` |  |  |  |  |  | `String(4)` |  | Serial No. Profile |  |  |
| `SizeOrDimensionText` |  |  |  |  |  | `String(32)` |  | Size/dimensions |  |  |
| `IndustryStandardName` |  |  |  |  |  | `String(18)` |  | Industry Std Desc. |  |  |
| `ProductStandardID` |  |  |  |  |  | `String(18)` |  | GTIN |  |  |
| `InternationalArticleNumberCat` |  |  |  |  |  | `String(2)` |  | EAN Category |  |  |
| `ProductIsConfigurable` |  |  |  |  |  | `Boolean` |  | Configurable |  |  |
| `IsBatchManagementRequired` |  |  |  |  |  | `Boolean` |  | Batch Management |  |  |
| `HasEmptiesBOM` |  |  |  |  |  | `Boolean` |  | With Empties BOM |  |  |
| `ExternalProductGroup` |  |  |  |  |  | `String(18)` |  | Ext. Product Group |  |  |
| `CrossPlantConfigurableProduct` |  |  |  |  |  | `String(40)` |  | Cross-plant CP |  |  |
| `SerialNoExplicitnessLevel` |  |  |  |  |  | `String(1)` |  | Serialization Level |  |  |
| `ProductManufacturerNumber` |  |  |  |  |  | `String(40)` |  | Mfr Part Number |  |  |
| `ManufacturerNumber` |  |  |  |  |  | `String(10)` |  | Manufacturer |  |  |
| `ManufacturerPartProfile` |  |  |  |  |  | `String(4)` |  | Mfr Part Profile |  |  |
| `QltyMgmtInProcmtIsActive` |  |  |  |  |  | `Boolean` |  | QM in Procur. Active |  |  |
| `IsApprovedBatchRecordReqd` |  |  |  |  |  | `Boolean` |  | Appr.Batch Recd Req. |  |  |
| `HandlingIndicator` |  |  |  |  |  | `String(4)` |  | Handling Indicator |  |  |
| `WarehouseProductGroup` |  |  |  |  |  | `String(4)` |  | WH Material Group |  |  |
| `WarehouseStorageCondition` |  |  |  |  |  | `String(2)` |  | Whse Stor. Condition |  |  |
| `StandardHandlingUnitType` |  |  |  |  |  | `String(4)` |  | Standard HU Type |  |  |
| `SerialNumberProfile` |  |  |  |  |  | `String(4)` |  | Serial No. Profile |  |  |
| `AdjustmentProfile` |  |  |  |  |  | `String(3)` |  | Adjust. Profile |  |  |
| `PreferredUnitOfMeasure` |  |  |  |  |  | `String(3)` |  | Preferred UoM |  |  |
| `IsPilferable` |  |  |  |  |  | `Boolean` |  | Pilferable |  |  |
| `IsRelevantForHzdsSubstances` |  |  |  |  |  | `Boolean` |  | Relevant for HS |  |  |
| `QuarantinePeriod` |  |  |  |  |  | `Decimal(3,0)` |  | Quarant. Per. | TimeUnitForQuarantinePeriod |  |
| `TimeUnitForQuarantinePeriod` |  |  |  |  |  | `String(3)` |  | Time Unit |  |  |
| `QualityInspectionGroup` |  |  |  |  |  | `String(4)` |  | Quality Inspec. Grp |  |  |
| `HandlingUnitType` |  |  |  |  |  | `String(4)` |  | Handling Unit Type |  |  |
| `HasVariableTareWeight` |  |  |  |  |  | `Boolean` |  | Varb. Tare Weight |  |  |
| `MaximumPackagingLength` |  |  |  |  |  | `Decimal(15,3)` |  | Max. Pack. Length | UnitForMaxPackagingDimensions |  |
| `MaximumPackagingWidth` |  |  |  |  |  | `Decimal(15,3)` |  | Max. Pack. Width | UnitForMaxPackagingDimensions |  |
| `MaximumPackagingHeight` |  |  |  |  |  | `Decimal(15,3)` |  | Max. Pack. Height | UnitForMaxPackagingDimensions |  |
| `MaximumCapacity` |  |  |  |  |  | `Decimal(15,3)` |  | Maximum Capacity |  |  |
| `OvercapacityTolerance` |  |  |  |  |  | `Decimal(3,1)` |  | Overcapacity Toler. |  |  |
| `UnitForMaxPackagingDimensions` |  |  |  |  |  | `String(3)` |  | Unit of Measurement |  |  |
| `BaseUnitSpecificProductLength` |  |  |  |  |  | `Decimal(13,3)` |  | Length | ProductMeasurementUnit |  |
| `BaseUnitSpecificProductWidth` |  |  |  |  |  | `Decimal(13,3)` |  | Width | ProductMeasurementUnit |  |
| `BaseUnitSpecificProductHeight` |  |  |  |  |  | `Decimal(13,3)` |  | Height | ProductMeasurementUnit |  |
| `ProductMeasurementUnit` |  |  |  |  |  | `String(3)` |  | Unit of Dimension |  |  |
| `ProductValidStartDate` |  |  |  |  |  | `Date` |  | Valid From |  |  |
| `ArticleCategory` |  |  |  |  |  | `String(2)` |  | Product Category |  |  |
| `ContentUnit` |  |  |  |  |  | `String(3)` |  | Content Unit |  |  |
| `NetContent` |  |  |  |  |  | `Decimal(13,3)` |  | Net Contents | ContentUnit |  |
| `ComparisonPriceQuantity` |  |  |  |  |  | `Decimal(5,0)` |  | Comparison Price Unit | ContentUnit |  |
| `GrossContent` |  |  |  |  |  | `Decimal(13,3)` |  | Gross Contents | ContentUnit |  |
| `ProductValidEndDate` |  |  |  |  |  | `Date` |  | Valid To |  |  |
| `AssortmentListType` |  |  |  |  |  | `String(1)` |  | Assortment List Type |  |  |
| `HasTextilePartsWthAnimalOrigin` |  |  |  |  |  | `Boolean` |  | Animal Origin |  |  |
| `ProductSeasonUsageCategory` |  |  |  |  |  | `String(1)` |  | Season Usage |  |  |
| `IndustrySector` |  |  |  |  |  | `String(1)` |  | Industry |  |  |
| `ChangeNumber` |  |  |  |  |  | `String(12)` |  | Change Number |  |  |
| `MaterialRevisionLevel` |  |  |  |  |  | `String(2)` |  | Revision Level |  |  |
| `IsActiveEntity` |  |  |  |  |  | `Boolean` |  | Is active |  |  |
| `LastChangeDateTime` |  |  |  |  |  | `Timestamp` |  | Last Changed |  |  |
| `LastChangeTime` |  |  |  |  |  | `String(6)` |  | Last Changed Time |  |  |
| `DangerousGoodsIndProfile` |  |  |  |  |  | `String(3)` |  | DG indicator profile |  |  |
| `ProductUUID` |  |  |  |  |  | `UUID` |  | Product |  |  |
| `ProdSupChnMgmtUUID22` |  |  |  |  |  | `String(22)` |  | Product ID |  |  |
| `ProductDocumentChangeNumber` |  |  |  |  |  | `String(6)` |  | Document Change No. |  |  |
| `ProductDocumentPageCount` |  |  |  |  |  | `String(3)` |  | Number Of Sheets |  |  |
| `ProductDocumentPageNumber` |  |  |  |  |  | `String(3)` |  | Page Number |  |  |
| `OwnInventoryManagedProduct` |  |  |  |  |  | `String(40)` |  | Int. material number |  |  |
| `DocumentIsCreatedByCAD` |  |  |  |  |  | `Boolean` |  | CAD Indicator |  |  |
| `ProductionOrInspectionMemoTxt` |  |  |  |  |  | `String(18)` |  | Prod./insp. memo |  |  |
| `ProductionMemoPageFormat` |  |  |  |  |  | `String(4)` |  | Page format |  |  |
| `GlobalTradeItemNumberVariant` |  |  |  |  |  | `String(2)` |  | EAN Variant |  |  |
| `ProductIsHighlyViscous` |  |  |  |  |  | `Boolean` |  | Highly viscous |  |  |
| `TransportIsInBulk` |  |  |  |  |  | `Boolean` |  | In bulk/liquid |  |  |
| `ProdAllocDetnProcedure` |  |  |  |  |  | `String(18)` |  | Product allocation |  |  |
| `ProdEffctyParamValsAreAssigned` |  |  |  |  |  | `Boolean` |  | Assign effect. vals |  |  |
| `ProdIsEnvironmentallyRelevant` |  |  |  |  |  | `Boolean` |  | Environmentally rlvt |  |  |
| `LaboratoryOrDesignOffice` |  |  |  |  |  | `String(3)` |  | Lab/Office |  |  |
| `PackagingMaterialGroup` |  |  |  |  |  | `String(4)` |  | Matl Grp Pack.Matls |  |  |
| `ProductIsLocked` |  |  |  |  |  | `Boolean` |  | Product locked |  |  |
| `DiscountInKindEligibility` |  |  |  |  |  | `String(1)` |  | Qual.f.FreeGoodsDis. |  |  |
| `SmartFormName` |  |  |  |  |  | `String(30)` |  | Form Name |  |  |
| `PackingReferenceProduct` |  |  |  |  |  | `String(40)` |  | Ref. Mat. for Pckg |  |  |
| `BasicMaterial` |  |  |  |  |  | `String(48)` |  | Basic Material |  |  |
| `ProductDocumentNumber` |  |  |  |  |  | `String(22)` |  | Document |  |  |
| `ProductDocumentVersion` |  |  |  |  |  | `String(2)` |  | Document Version |  |  |
| `ProductDocumentType` |  |  |  |  |  | `String(3)` |  | Document Type |  |  |
| `ProductDocumentPageFormat` |  |  |  |  |  | `String(4)` |  | Page Format |  |  |
| `ProductConfiguration` |  |  |  |  |  | `String(18)` |  | Internal object no. |  |  |
| `SegmentationStrategy` |  |  |  |  |  | `String(8)` |  | Seg. Strategy |  |  |
| `SegmentationIsRelevant` |  |  |  |  |  | `Boolean` |  | Seg. Relevant |  |  |
| `ProductCompositionIsRelevant` |  |  |  |  |  | `Boolean` |  | Product Composition |  |  |
| `IsChemicalComplianceRelevant` |  |  |  |  |  | `String(1)` |  | Chemical Compliance Relevance Indicator |  |  |
| `ManufacturerBookPartNumber` |  |  |  |  |  | `String(40)` |  | MS Book Part No |  |  |
| `LogisticalProductCategory` |  |  |  |  |  | `String(1)` |  | Logl Material Cat. |  |  |
| `SalesProduct` |  |  |  |  |  | `String(40)` |  | Sales Material No. |  |  |
| `ProdCharc1InternalNumber` |  |  |  |  |  | `String(10)` |  | Int. Char. Number |  |  |
| `ProdCharc2InternalNumber` |  |  |  |  |  | `String(10)` |  | Int. Char. Number |  |  |
| `ProdCharc3InternalNumber` |  |  |  |  |  | `String(10)` |  | Int. Char. Number |  |  |
| `ProductCharacteristic1` |  |  |  |  |  | `String(18)` |  | Color |  |  |
| `ProductCharacteristic2` |  |  |  |  |  | `String(18)` |  | Main Size |  |  |
| `ProductCharacteristic3` |  |  |  |  |  | `String(18)` |  | Second Size |  |  |
| `MaintenanceStatus` |  |  |  |  |  | `String(15)` |  | Maintenance Status |  |  |
| `FashionProdInformationField1` |  |  |  |  |  | `String(10)` |  | Fsh. Attribute1 |  |  |
| `FashionProdInformationField2` |  |  |  |  |  | `String(10)` |  | Fsh. Attribute2 |  |  |
| `FashionProdInformationField3` |  |  |  |  |  | `String(6)` |  | Fsh. Attribute3 |  |  |
| `DfsAmmunitionGroupCode` |  |  |  |  |  | `String(8)` |  | Ammunition Code |  |  |
| `DfsRICIdentifier` |  |  |  |  |  | `Integer64` |  | RIC ID |  |  |
| `DfsProductSensitivity` |  |  |  |  |  | `String(4)` |  | Sensitivity for Char |  |  |
| `DfsManufacturerPartLongNumber` |  |  |  |  |  | `String(60)` |  | Long Mfr Part No. |  |  |
| `DfsMatlConditionMgmt` |  |  |  |  |  | `String(1)` |  | Condition Mgmt |  |  |
| `DfsReturnDelivery` |  |  |  |  |  | `String(1)` |  | Return Code |  |  |
| `DfsLogisticsLevel` |  |  |  |  |  | `String(1)` |  | Return to Log.Level |  |  |
| `DfsNationalItemIdnNumber` |  |  |  |  |  | `String(9)` |  | NATO Item ID Number |  |  |
| `LstMiProductToleranceType` |  |  |  |  |  | `String(4)` |  | Tolerance Type |  |  |


## Entity: `ProductConsumption`

- **ABAP CDS Name:** `I_ProductConsumption`
- **Label:** Product Consumption
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** MVER

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Product |  |  |
| `Plant` |  |  |  |  |  | `String(4)` | Y | Plant |  |  |
| `PostingFiscalYear` |  |  |  |  |  | `String(4)` | Y | Fiscal Year |  |  |
| `PeriodType` |  |  |  |  |  | `String(1)` | Y | Period Indicator |  |  |
| `NumberOfFollowOnRecords` |  |  |  |  |  | `String(2)` | Y | Follow-on records |  |  |
| `TotalConsumption1Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Tot.consumption 1 | BaseUnit |  |
| `TotalConsumption2Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Tot.consumption 2 | BaseUnit |  |
| `TotalConsumption3Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Tot.consumption 3 | BaseUnit |  |
| `TotalConsumption4Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Tot.consumption 4 | BaseUnit |  |
| `TotalConsumption5Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Tot.consumption 5 | BaseUnit |  |
| `TotalConsumption6Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Tot.consumption 6 | BaseUnit |  |
| `TotalConsumption7Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Tot.consumption 7 | BaseUnit |  |
| `TotalConsumption8Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Tot.consumption 8 | BaseUnit |  |
| `TotalConsumption9Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Tot.consumption 9 | BaseUnit |  |
| `TotalConsumption10Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Tot.consumption 10 | BaseUnit |  |
| `TotalConsumption11Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Tot.consumption 11 | BaseUnit |  |
| `TotalConsumption12Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Tot.consumption 12 | BaseUnit |  |
| `TotalConsumption13Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Tot.consumption 13 | BaseUnit |  |
| `UnplannedConsumption1Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Unplnd consump. 1 | BaseUnit |  |
| `UnplannedConsumption2Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Unplnd consump. 2 | BaseUnit |  |
| `UnplannedConsumption3Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Unplnd consump. 3 | BaseUnit |  |
| `UnplannedConsumption4Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Unplnd consump. 4 | BaseUnit |  |
| `UnplannedConsumption5Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Unplnd consump. 5 | BaseUnit |  |
| `UnplannedConsumption6Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Unplnd consump. 6 | BaseUnit |  |
| `UnplannedConsumption7Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Unplnd consump. 7 | BaseUnit |  |
| `UnplannedConsumption8Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Unplnd consump. 8 | BaseUnit |  |
| `UnplannedConsumption9Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Unplnd consump. 9 | BaseUnit |  |
| `UnplannedConsumption10Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Unplnd consump. 10 | BaseUnit |  |
| `UnplannedConsumption11Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Unplnd consump. 11 | BaseUnit |  |
| `UnplannedConsumption12Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Unplnd consump. 12 | BaseUnit |  |
| `UnplannedConsumption13Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Unplnd consump. 13 | BaseUnit |  |
| `MnllyCrrtdTotCnsmpn1Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.tot.consum 1 | BaseUnit |  |
| `MnllyCrrtdTotCnsmpn2Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.tot.consum 2 | BaseUnit |  |
| `MnllyCrrtdTotCnsmpn3Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.tot.consum 3 | BaseUnit |  |
| `MnllyCrrtdTotCnsmpn4Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.tot.consum 4 | BaseUnit |  |
| `MnllyCrrtdTotCnsmpn5Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.tot.consum 5 | BaseUnit |  |
| `MnllyCrrtdTotCnsmpn6Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.tot.consum 6 | BaseUnit |  |
| `MnllyCrrtdTotCnsmpn7Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.tot.consum 7 | BaseUnit |  |
| `MnllyCrrtdTotCnsmpn8Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.tot.consum 8 | BaseUnit |  |
| `MnllyCrrtdTotCnsmpn9Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.tot.consum 9 | BaseUnit |  |
| `MnllyCrrtdTotCnsmpn10Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.tot.consum 10 | BaseUnit |  |
| `MnllyCrrtdTotCnsmpn11Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.tot.consum 11 | BaseUnit |  |
| `MnllyCrrtdTotCnsmpn12Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.tot.consum 12 | BaseUnit |  |
| `MnllyCrrtdTotCnsmpn13Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.tot.consum 13 | BaseUnit |  |
| `MnllyCrrtdUnplndCnsmpn1Qty` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.unpl.cons. 1 | BaseUnit |  |
| `MnllyCrrtdUnplndCnsmpn2Qty` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.unpl.cons. 2 | BaseUnit |  |
| `MnllyCrrtdUnplndCnsmpn3Qty` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.unpl.cons. 3 | BaseUnit |  |
| `MnllyCrrtdUnplndCnsmpn4Qty` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.unpl.cons. 4 | BaseUnit |  |
| `MnllyCrrtdUnplndCnsmpn5Qty` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.unpl.cons. 5 | BaseUnit |  |
| `MnllyCrrtdUnplndCnsmpn6Qty` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.unpl.cons. 6 | BaseUnit |  |
| `MnllyCrrtdUnplndCnsmpn7Qty` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.unpl.cons. 7 | BaseUnit |  |
| `MnllyCrrtdUnplndCnsmpn8Qty` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.unpl.cons. 8 | BaseUnit |  |
| `MnllyCrrtdUnplndCnsmpn9Qty` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.unpl.cons. 9 | BaseUnit |  |
| `MnllyCrrtdUnplndCnsmpn10Qty` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.unpl.cons. 10 | BaseUnit |  |
| `MnllyCrrtdUnplndCnsmpn11Qty` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.unpl.cons. 11 | BaseUnit |  |
| `MnllyCrrtdUnplndCnsmpn12Qty` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.unpl.cons. 12 | BaseUnit |  |
| `MnllyCrrtdUnplndCnsmpn13Qty` |  |  |  |  |  | `Decimal(13,3)` |  | Corr.unpl.cons. 13 | BaseUnit |  |
| `BaseUnit` |  |  |  |  |  | `String(3)` |  | Base Unit of Measure |  |  |


## Entity: `ProductDescription`

- **ABAP CDS Name:** `I_ProductDescription_2`
- **Label:** Product Descriptions
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** MAKT

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Product |  |  |
| `Language` |  |  |  |  |  | `String(2)` | Y | Language Key |  |  |
| `ProductDescription` |  |  |  |  |  | `String(40)` |  | Product Description |  |  |
| `LanguageISOCode` |  |  |  |  |  | `String(2)` |  | Language |  |  |


## Entity: `ProductGroup`

- **ABAP CDS Name:** `I_ProductGroup_2`
- **Label:** Product Group
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** T023

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `ProductGroup` |  |  |  |  |  | `String(9)` | Y | Product Group |  |  |
| `AuthorizationGroup` |  |  |  |  |  | `String(4)` |  | Authorization Group |  |  |
| `ValuationClass` |  |  |  |  |  | `String(4)` |  | Valuation Class |  |  |
| `PurchasingAcknProfile` |  |  |  |  |  | `String(4)` |  | Purchasing value key |  |  |


## Entity: `ProductGroupText`

- **ABAP CDS Name:** `I_ProductGroupText_2`
- **Label:** Product Group - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** T023T

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `ProductGroup` |  |  |  |  |  | `String(9)` | Y | Product Group |  |  |
| `Language` |  |  |  |  |  | `String(2)` | Y | Language Key |  |  |
| `ProductGroupName` |  |  |  |  |  | `String(20)` |  | Product Group Description |  |  |
| `ProductGroupText` |  |  |  |  |  | `String(60)` |  | Mat.Grp Desc. 2 |  |  |


## Entity: `ProductMRPArea`

- **ABAP CDS Name:** `I_ProductMRPArea`
- **Label:** MRP Area Details of a Product
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** MDMA

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Product |  |  |
| `MRPArea` |  |  |  |  |  | `String(10)` | Y | MRP Area |  |  |
| `MRPPlant` |  |  |  |  |  | `String(4)` |  | MRP Area Plant |  |  |
| `MRPGroup` |  |  |  |  |  | `String(4)` |  | MRP Group |  |  |
| `MRPType` |  |  |  |  |  | `String(2)` |  | MRP Type |  |  |
| `MRPController` |  |  |  |  |  | `String(3)` |  | MRP Controller |  |  |
| `MRPProfile` |  |  |  |  |  | `String(4)` |  | MRP Profile |  |  |
| `LotSizingProcedure` |  |  |  |  |  | `String(2)` |  | Lot Sizing Procedure |  |  |
| `MRPPlanningCalendar` |  |  |  |  |  | `String(3)` |  | Planning Calendar |  |  |
| `MRPPlanningCycle` |  |  |  |  |  | `String(3)` |  | Planning Cycle |  |  |
| `MRPSafetyStockMethod` |  |  |  |  |  | `String(2)` |  | Safety Stock Method |  |  |
| `MaterialProcurementProfile` |  |  |  |  |  | `String(2)` |  | Procurement Profile |  |  |
| `ProductionStorageLocation` |  |  |  |  |  | `String(4)` |  | Production Storage Location |  |  |
| `DfltStorLocForExtProcmt` |  |  |  |  |  | `String(4)` |  | External Procurement Storage Location |  |  |
| `RangeOfCoverageProfile` |  |  |  |  |  | `String(3)` |  | Range-of-Coverage Profile |  |  |
| `SafetyTimePeriodProfile` |  |  |  |  |  | `String(3)` |  | Period Profile for Safety Time |  |  |
| `ProductSafetyTimeMRPRelevance` |  |  |  |  |  | `String(1)` |  | Safety Time MRP Relevance |  |  |
| `DependentRqmtMRPRelevance` |  |  |  |  |  | `String(1)` |  | Dependent Requirements MRP Relevance |  |  |
| `StorageCostsPercentageCode` |  |  |  |  |  | `String(1)` |  | Storage Costs Code |  |  |
| `RoundingProfile` |  |  |  |  |  | `String(4)` |  | Rounding Profile |  |  |
| `IsMarkedForDeletion` |  |  |  |  |  | `Boolean` |  | Deletion Indicator |  |  |
| `LastChangedByUser` |  |  |  |  |  | `String(12)` |  | Changed By |  |  |
| `LastChangeDate` |  |  |  |  |  | `Date` |  | Changed On |  |  |
| `LastChangeTime` |  |  |  |  |  | `String(6)` |  | Time of Change |  |  |
| `PlannedDeliveryDurationInDays` |  |  |  |  |  | `Decimal(3,0)` |  | Planned Deliv. Time |  |  |
| `PlanningTimeFenceInDays` |  |  |  |  |  | `String(3)` |  | Planning Time Fence |  |  |
| `RqmtQtyRcptTaktTmeInWrkgDays` |  |  |  |  |  | `Decimal(3,0)` |  | Takt time |  |  |
| `AssemblyScrapPercent` |  |  |  |  |  | `Decimal(5,2)` |  | Assembly scrap (%) |  |  |
| `BaseUnit` |  |  |  |  |  | `String(3)` |  | Base Unit of Measure |  |  |
| `MinimumLotSizeQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Minimum Lot Size | BaseUnit |  |
| `MaximumLotSizeQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Maximum Lot Size | BaseUnit |  |
| `MaterialMaxStockLevelQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Maximum Stock Level | BaseUnit |  |
| `SafetyStockQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Safety Stock | BaseUnit |  |
| `LotSizeRoundingQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Rounding Quantity | BaseUnit |  |
| `ReorderThresholdQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Reorder Point | BaseUnit |  |


## Entity: `ProductPlant`

- **ABAP CDS Name:** `I_ProductPlantBasic`
- **Label:** Product Plant
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** MARC

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Product |  |  |
| `Plant` |  |  |  |  |  | `String(4)` | Y | Plant |  |  |
| `PurchasingGroup` |  |  |  |  |  | `String(3)` |  | Purchasing Group |  |  |
| `CountryOfOrigin` |  |  |  |  |  | `String(3)` |  | Country/Region of Origin |  |  |
| `RegionOfOrigin` |  |  |  |  |  | `String(3)` |  | Region of Origin |  |  |
| `ProductionInvtryManagedLoc` |  |  |  |  |  | `String(4)` |  | Storage Location |  |  |
| `ProfileCode` |  |  |  |  |  | `String(2)` |  | Material Status |  |  |
| `ProfileValidityStartDate` |  |  |  |  |  | `Date` |  | Valid From |  |  |
| `AvailabilityCheckType` |  |  |  |  |  | `String(2)` |  | Availability check |  |  |
| `FiscalYearVariant` |  |  |  |  |  | `String(2)` |  | Fiscal Year Variant |  |  |
| `PeriodType` |  |  |  |  |  | `String(1)` |  | Period Indicator |  |  |
| `ProfitCenter` |  |  |  |  |  | `String(10)` |  | Profit Center |  |  |
| `GoodsReceiptDuration` |  |  |  |  |  | `Decimal(3,0)` |  | GR processing time |  |  |
| `MaintenanceStatusName` |  |  |  |  |  | `String(15)` |  | Maintenance Status |  |  |
| `IsMarkedForDeletion` |  |  |  |  |  | `Boolean` |  | DF at plant level |  |  |
| `MRPType` |  |  |  |  |  | `String(2)` |  | MRP Type |  |  |
| `MRPResponsible` |  |  |  |  |  | `String(3)` |  | MRP Controller |  |  |
| `ABCIndicator` |  |  |  |  |  | `String(1)` |  | ABC Indicator |  |  |
| `MinimumLotSizeQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Minimum Lot Size | BaseUnit |  |
| `MaximumLotSizeQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Maximum Lot Size | BaseUnit |  |
| `FixedLotSizeQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Fixed lot size | BaseUnit |  |
| `ConsumptionTaxCtrlCode` |  |  |  |  |  | `String(16)` |  | Control Code |  |  |
| `IsCoProduct` |  |  |  |  |  | `Boolean` |  | Co-Product |  |  |
| `ConfigurableProduct` |  |  |  |  |  | `String(40)` |  | Conf. Material |  |  |
| `StockDeterminationGroup` |  |  |  |  |  | `String(4)` |  | Stock Determ. Group |  |  |
| `HasPostToInspectionStock` |  |  |  |  |  | `Boolean` |  | Post to insp. stock |  |  |
| `IsBatchManagementRequired` |  |  |  |  |  | `Boolean` |  | Batch Mgmt Rqt(Plnt) |  |  |
| `SerialNumberProfile` |  |  |  |  |  | `String(4)` |  | Serial No. Profile |  |  |
| `IsNegativeStockAllowed` |  |  |  |  |  | `Boolean` |  | Neg. Stocks In Plant |  |  |
| `HasConsignmentCtrl` |  |  |  |  |  | `String(1)` |  | Consign.Control |  |  |
| `IsPurgAcrossPurgGroup` |  |  |  |  |  | `Boolean` |  | Across Purch.Group |  |  |
| `IsInternalBatchManaged` |  |  |  |  |  | `Boolean` |  | Batch Management |  |  |
| `ProductCFOPCategory` |  |  |  |  |  | `String(2)` |  | Matl. CFOP Category |  |  |
| `ProductIsExciseTaxRelevant` |  |  |  |  |  | `Boolean` |  | Is Excise Tax Relevant |  |  |
| `UnderDelivToleranceLimit` |  |  |  |  |  | `Decimal(3,1)` |  | Underdelivery Toler. |  |  |
| `OverDelivToleranceLimit` |  |  |  |  |  | `Decimal(3,1)` |  | Overdelivery Toler. |  |  |
| `ProcurementType` |  |  |  |  |  | `String(1)` |  | Procurement Type |  |  |
| `SpecialProcurementType` |  |  |  |  |  | `String(2)` |  | Special Procurement |  |  |
| `ProductionSchedulingProfile` |  |  |  |  |  | `String(6)` |  | Production Scheduling Profile |  |  |
| `ProductionSupervisor` |  |  |  |  |  | `String(3)` |  | Prodn Supervisor |  |  |
| `SafetyStockQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Safety Stock | BaseUnit |  |
| `GoodsIssueUnit` |  |  |  |  |  | `String(3)` |  | Unit of Issue |  |  |
| `SourceOfSupplyCategory` |  |  |  |  |  | `String(1)` |  | Source of supply |  |  |
| `ConsumptionReferenceProduct` |  |  |  |  |  | `String(40)` |  | RefMatl: consumption |  |  |
| `ConsumptionReferencePlant` |  |  |  |  |  | `String(4)` |  | RefPlant:consumption |  |  |
| `ConsumptionRefUsageEndDate` |  |  |  |  |  | `Date` |  | Date to |  |  |
| `ConsumptionQtyMultiplier` |  |  |  |  |  | `Decimal(4,2)` |  | Multiplier |  |  |
| `ProductUnitGroup` |  |  |  |  |  | `String(4)` |  | Unit of Measure Group |  |  |
| `DistrCntrDistributionProfile` |  |  |  |  |  | `String(3)` |  | Distr. profile |  |  |
| `ConsignmentControl` |  |  |  |  |  | `String(1)` |  | Consign.Control |  |  |
| `GoodIssueProcessingDays` |  |  |  |  |  | `Decimal(3,0)` |  | GI Proc. Time |  |  |
| `PlannedDeliveryDurationInDays` |  |  |  |  |  | `Decimal(3,0)` |  | Planned Deliv. Time |  |  |
| `ProductIsCriticalPrt` |  |  |  |  |  | `Boolean` |  | Critical Part |  |  |
| `ProductLogisticsHandlingGroup` |  |  |  |  |  | `String(4)` |  | Log. handling group |  |  |
| `MaterialFreightGroup` |  |  |  |  |  | `String(8)` |  | Material Freight Grp |  |  |
| `OriginalBatchReferenceMaterial` |  |  |  |  |  | `String(40)` |  | OB Reference Materl |  |  |
| `OriglBatchManagementIsRequired` |  |  |  |  |  | `String(1)` |  | OB Management |  |  |
| `ProductConfiguration` |  |  |  |  |  | `String(18)` |  | Internal object no. |  |  |
| `ProductMinControlTemperature` |  |  |  |  |  | `Decimal(7,2)` |  | Min. Temperature | ProductControlTemperatureUnit |  |
| `ProductMaxControlTemperature` |  |  |  |  |  | `Decimal(7,2)` |  | Max. Temperature | ProductControlTemperatureUnit |  |
| `ProductControlTemperatureUnit` |  |  |  |  |  | `String(3)` |  | Temperature UoM |  |  |
| `ValuationCategory` |  |  |  |  |  | `String(1)` |  | Valuation Category |  |  |
| `BaseUnit` |  |  |  |  |  | `String(3)` |  | Base Unit of Measure |  |  |
| `ItemUniqueIdentifierIsRelevant` |  |  |  |  |  | `Boolean` |  | IUID-Relevant |  |  |
| `ItemUniqueIdentifierType` |  |  |  |  |  | `String(10)` |  | IUID Type |  |  |
| `ExtAllocOfItmUnqIdtIsRelevant` |  |  |  |  |  | `Boolean` |  | Ext. Allocation |  |  |


## Entity: `ProductPlantCosting`

- **ABAP CDS Name:** `I_ProductPlantCosting`
- **Label:** Product Plant Costing
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** CKMLMV, MBEW

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Product |  |  |
| `Plant` |  |  |  |  |  | `String(4)` | Y | Plant |  |  |
| `IsCoProduct` |  |  |  |  |  | `Boolean` |  | Co-Product |  |  |
| `CostingLotSize` |  |  |  |  |  | `Decimal(13,3)` |  | Costing Lot Size | BaseUnit |  |
| `TaskListGroup` |  |  |  |  |  | `String(8)` |  | Group |  |  |
| `TaskListType` |  |  |  |  |  | `String(1)` |  | Task List Type |  |  |
| `CostingSpecialProcurementType` |  |  |  |  |  | `String(2)` |  | Special Procurement Type |  |  |
| `SourceBOMAlternative` |  |  |  |  |  | `String(2)` |  | Alternative BOM |  |  |
| `ProductBOMUsage` |  |  |  |  |  | `String(1)` |  | BOM Usage |  |  |
| `ProductIsCostingRelevant` |  |  |  |  |  | `Boolean` |  | Do Not Cost |  |  |
| `TaskListGroupCounter` |  |  |  |  |  | `String(2)` |  | Group Counter |  |  |
| `VarianceKey` |  |  |  |  |  | `String(6)` |  | Variance Key |  |  |
| `CostingProductionVersion` |  |  |  |  |  | `String(4)` |  | Production Version |  |  |
| `IsFixedPriceCoProduct` |  |  |  |  |  | `Boolean` |  | Fixed-Price Co-Prod. |  |  |
| `BaseUnit` |  |  |  |  |  | `String(3)` |  | Base Unit of Measure |  |  |


## Entity: `ProductPlantForecast`

- **ABAP CDS Name:** `I_ProductPlantForecast`
- **Label:** Product Plant Forecast
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** MPOP

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Product |  |  |
| `Plant` |  |  |  |  |  | `String(4)` | Y | Plant |  |  |
| `ConsumptionRefUsageEndDate` |  |  |  |  |  | `Date` |  | Date to |  |  |
| `ConsumptionQtyMultiplier` |  |  |  |  |  | `Decimal(4,2)` |  | Multiplier |  |  |
| `ConsumptionReferenceProduct` |  |  |  |  |  | `String(40)` |  | RefMatl: consumption |  |  |
| `ConsumptionReferencePlant` |  |  |  |  |  | `String(4)` |  | RefPlant:consumption |  |  |
| `CorrectionFactorIsRequired` |  |  |  |  |  | `Boolean` |  | Correction factors |  |  |
| `ForecastModelIsReset` |  |  |  |  |  | `Boolean` |  | Reset automatically |  |  |


## Entity: `ProductPlantInternationalTrade`

- **ABAP CDS Name:** `I_ProductPlantIntlTrd`
- **Label:** Product Plant Intrntionl Trade
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** MARC

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Product |  |  |
| `Plant` |  |  |  |  |  | `String(4)` | Y | Plant |  |  |
| `CountryOfOrigin` |  |  |  |  |  | `String(3)` |  | Country/Region of Origin |  |  |
| `RegionOfOrigin` |  |  |  |  |  | `String(3)` |  | Region of Origin |  |  |
| `ConsumptionTaxCtrlCode` |  |  |  |  |  | `String(16)` |  | Control Code |  |  |
| `ExportAndImportProductGroup` |  |  |  |  |  | `String(4)` |  | Intrastat Group |  |  |
| `ProductCASNumber` |  |  |  |  |  | `String(15)` |  | CAS number (pharm.) |  |  |
| `CommoditiyCodeNumberUnit` |  |  |  |  |  | `String(3)` |  | Commodity code unit |  |  |
| `ProdIntlTradeClassification` |  |  |  |  |  | `String(9)` |  | PRODCOM no. |  |  |


## Entity: `ProductPlantProcurement`

- **ABAP CDS Name:** `I_Productplantprocurement`
- **Label:** Product Plant Procurement
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** MARC

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Product |  |  |
| `Plant` |  |  |  |  |  | `String(4)` | Y | Plant |  |  |
| `IsAutoPurOrdCreationAllowed` |  |  |  |  |  | `Boolean` |  | Automatic PO |  |  |
| `IsSourceListRequired` |  |  |  |  |  | `Boolean` |  | Source list |  |  |
| `IsPurgAcrossPurgGroup` |  |  |  |  |  | `Boolean` |  | Across Purch.Group |  |  |
| `SourceOfSupplyCategory` |  |  |  |  |  | `String(1)` |  | Source of supply |  |  |
| `PurchasingGroup` |  |  |  |  |  | `String(3)` |  | Purchasing Group |  |  |
| `IsActiveEntity` |  |  |  |  |  | `Boolean` |  | Is active |  |  |
| `ProposedProductSupplyArea` |  |  |  |  |  | `String(10)` |  | Proposed Supply Area |  |  |
| `ItmIsRlvtToJITDelivSchedules` |  |  |  |  |  | `String(1)` |  | JIT Delivery |  |  |


## Entity: `ProductPlantPurchaseTax`

- **ABAP CDS Name:** `I_ProductPurchaseTax`
- **Label:** Product Purchase Tax
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** MARC

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Product |  |  |
| `SourceLocationCountry` |  |  |  |  |  | `String(3)` | Y | Departure Ctry/Reg. |  |  |
| `TaxIndicator` |  |  |  |  |  | `String(1)` |  | Tax ind. f. material |  |  |


## Entity: `ProductPlantQualityManagement`

- **ABAP CDS Name:** `I_Productplantqtmanagement`
- **Label:** Product Plant QM
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** MARC

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Product |  |  |
| `Plant` |  |  |  |  |  | `String(4)` | Y | Plant |  |  |
| `MaximumStoragePeriod` |  |  |  |  |  | `Decimal(5,0)` |  | Max. Storage Period |  |  |
| `QualityMgmtCtrlKey` |  |  |  |  |  | `String(8)` |  | QM Control Key |  |  |
| `MatlQualityAuthorizationGroup` |  |  |  |  |  | `String(6)` |  | QM Material Auth. |  |  |
| `HasPostToInspectionStock` |  |  |  |  |  | `Boolean` |  | Post to insp. stock |  |  |
| `IsActiveEntity` |  |  |  |  |  | `Boolean` |  | Is active |  |  |
| `InspLotDocumentationIsRequired` |  |  |  |  |  | `Boolean` |  | Documentation reqd |  |  |
| `SuplrQualityManagementSystem` |  |  |  |  |  | `String(4)` |  | Target QM System |  |  |
| `RecrrgInspIntervalTimeInDays` |  |  |  |  |  | `Decimal(5,0)` |  | Inspection Interval |  |  |
| `ProductQualityCertificateType` |  |  |  |  |  | `String(4)` |  | Certificate Type |  |  |
| `ProductPlantHasInspectionSetup` |  |  |  |  |  | `Boolean` |  | Inspection Setup |  |  |


## Entity: `ProductPlantStorage`

- **ABAP CDS Name:** `I_Productplantstorage`
- **Label:** Product plant storage
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** MARC, MARD

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Product |  |  |
| `Plant` |  |  |  |  |  | `String(4)` | Y | Plant |  |  |
| `InventoryForCycleCountInd` |  |  |  |  |  | `String(1)` |  | CC Phys. Inv. Ind. |  |  |
| `MaximumStoragePeriod` |  |  |  |  |  | `Decimal(5,0)` |  | Max. Storage Period |  |  |
| `ProvisioningServiceLevel` |  |  |  |  |  | `String(1)` |  | Service Level |  |  |
| `IsActiveEntity` |  |  |  |  |  | `Boolean` |  | Is active |  |  |
| `ProdMaximumStoragePeriodUnit` |  |  |  |  |  | `String(3)` |  | Time unit |  |  |
| `WrhsMgmtPtwyAndStkRemovalStrgy` |  |  |  |  |  | `String(1)` |  | Putaway/StkRmvl |  |  |
| `CycleCountingIndicatorIsFixed` |  |  |  |  |  | `Boolean` |  | CC indicator fixed |  |  |
| `SegmentationStrategyForPlant` |  |  |  |  |  | `String(8)` |  | Segment. Strategy |  |  |
| `DefaultSegmentValue` |  |  |  |  |  | `String(40)` |  | Stock Segment |  |  |
| `SgmtHasPrioInProductStockSort` |  |  |  |  |  | `Boolean` |  | Sort Stock |  |  |


## Entity: `ProductPlantSupplyPlanning`

- **ABAP CDS Name:** `I_ProductPlantSupplyPlanning`
- **Label:** Product Plant Supply Planning
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** MARC

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Product |  |  |
| `Plant` |  |  |  |  |  | `String(4)` | Y | Plant |  |  |
| `FixedLotSizeQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Fixed lot size | BaseUnit |  |
| `MaximumLotSizeQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Maximum Lot Size | BaseUnit |  |
| `MinimumLotSizeQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Minimum Lot Size | BaseUnit |  |
| `LotSizeRoundingQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Rounding value | BaseUnit |  |
| `LotSizingProcedure` |  |  |  |  |  | `String(2)` |  | Lot Sizing Procedure |  |  |
| `MRPType` |  |  |  |  |  | `String(2)` |  | MRP Type |  |  |
| `MRPResponsible` |  |  |  |  |  | `String(3)` |  | MRP Controller |  |  |
| `SafetyStockQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Safety Stock | BaseUnit |  |
| `MinimumSafetyStockQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Min. Saf. Stock | BaseUnit |  |
| `PlanningTimeFence` |  |  |  |  |  | `String(3)` |  | Planning time fence |  |  |
| `ConsumptionValueCategory` |  |  |  |  |  | `String(1)` |  | ABC Indicator |  |  |
| `MaximumStockQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Maximum Stock Level | BaseUnit |  |
| `ReorderThresholdQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Reorder Point | BaseUnit |  |
| `PlannedDeliveryDurationInDays` |  |  |  |  |  | `Decimal(3,0)` |  | Planned Deliv. Time |  |  |
| `SafetySupplyDurationInDays` |  |  |  |  |  | `String(2)` |  | Safety Time |  |  |
| `PlanningStrategyGroup` |  |  |  |  |  | `String(2)` |  | Strategy Group |  |  |
| `TotalReplenishmentLeadTime` |  |  |  |  |  | `Decimal(3,0)` |  | Tot. repl. lead time |  |  |
| `ProcurementType` |  |  |  |  |  | `String(1)` |  | Procurement Type |  |  |
| `ProcurementSubType` |  |  |  |  |  | `String(2)` |  | Special Procurement |  |  |
| `AssemblyScrapPercent` |  |  |  |  |  | `Decimal(5,2)` |  | Assembly scrap (%) |  |  |
| `AvailabilityCheckType` |  |  |  |  |  | `String(2)` |  | Availability check |  |  |
| `GoodsReceiptDuration` |  |  |  |  |  | `Decimal(3,0)` |  | GR processing time |  |  |
| `PlanAndOrderDayDetermination` |  |  |  |  |  | `String(3)` |  | Planning Cycle |  |  |
| `RoundingProfile` |  |  |  |  |  | `String(4)` |  | Rounding Profile |  |  |
| `DfltStorageLocationExtProcmt` |  |  |  |  |  | `String(4)` |  | Storage Location |  |  |
| `GoodIssueProcessingDays` |  |  |  |  |  | `Decimal(3,0)` |  | GI Proc. Time |  |  |
| `ConsignmentControl` |  |  |  |  |  | `String(1)` |  | Consign.Control |  |  |
| `IsActiveEntity` |  |  |  |  |  | `Boolean` |  | Is active |  |  |
| `MRPGroup` |  |  |  |  |  | `String(4)` |  | MRP Group |  |  |
| `LotSizeIndependentCosts` |  |  |  |  |  | `Decimal(34,4)` |  | LS-Independent Costs | Currency |  |
| `StorageCostsPercentageCode` |  |  |  |  |  | `String(1)` |  | Storage Costs Code |  |  |
| `RqmtQtyRcptTaktTmeInWrkgDays` |  |  |  |  |  | `Decimal(3,0)` |  | Takt time |  |  |
| `MRPPlanningCalendar` |  |  |  |  |  | `String(3)` |  | Planning Calendar |  |  |
| `RangeOfCvrgPrflCode` |  |  |  |  |  | `String(3)` |  | Coverage Profile |  |  |
| `ProductSafetyTimeMRPRelevance` |  |  |  |  |  | `String(1)` |  | Safety Time Ind |  |  |
| `SafetyTimePeriodProfile` |  |  |  |  |  | `String(3)` |  | Time Profile |  |  |
| `DependentRqmtMRPRelevance` |  |  |  |  |  | `String(1)` |  | MRP Relevant |  |  |
| `ProductServiceLevelInPercent` |  |  |  |  |  | `Decimal(3,1)` |  | Service level (%) |  |  |
| `ProdInhProdnDurationInWorkDays` |  |  |  |  |  | `Decimal(3,0)` |  | In-house production |  |  |
| `MRPAvailabilityType` |  |  |  |  |  | `String(1)` |  | Mixed MRP |  |  |
| `CrossProjectProduct` |  |  |  |  |  | `String(1)` |  | Cross-Project |  |  |
| `ProdnPlngAndControlCalendar` |  |  |  |  |  | `String(3)` |  | Planning Calendar |  |  |
| `FollowUpProduct` |  |  |  |  |  | `String(40)` |  | Follow-Up Material |  |  |
| `RepetitiveManufacturingIsAllwd` |  |  |  |  |  | `Boolean` |  | Repetitive Manufacturing Enabled |  |  |
| `DependentRequirementsType` |  |  |  |  |  | `String(1)` |  | Indiv./ Coll. |  |  |
| `ProductIsBulkComponent` |  |  |  |  |  | `Boolean` |  | Bulk Material |  |  |
| `RepetitiveManufacturingProfile` |  |  |  |  |  | `String(4)` |  | Repetitive Manufacturing Profile |  |  |
| `BackwardCnsmpnPeriodInWorkDays` |  |  |  |  |  | `String(3)` |  | Backward Consumption Period |  |  |
| `FwdConsumptionPeriodInWorkDays` |  |  |  |  |  | `String(3)` |  | Forward Consumption Period |  |  |
| `ProdRqmtsConsumptionMode` |  |  |  |  |  | `String(1)` |  | Consumption mode |  |  |
| `ProdFcstRequirementsSplitCode` |  |  |  |  |  | `String(1)` |  | Splitting Indicator |  |  |
| `EffectiveOutDate` |  |  |  |  |  | `Date` |  | Effective-Out Date |  |  |
| `MRPProfile` |  |  |  |  |  | `String(4)` |  | MRP profile |  |  |
| `SchedulingFloatProfile` |  |  |  |  |  | `String(3)` |  | Scheduling Float Profile |  |  |
| `ComponentScrapInPercent` |  |  |  |  |  | `Decimal(5,2)` |  | Component Scrap (%) |  |  |
| `ProductDiscontinuationCode` |  |  |  |  |  | `String(1)` |  | Discontinuation ind. |  |  |
| `ProductRequirementsGrouping` |  |  |  |  |  | `String(1)` |  | Requirements group |  |  |
| `ProductionInvtryManagedLoc` |  |  |  |  |  | `String(4)` |  | Storage Location |  |  |
| `ProductComponentBackflushCode` |  |  |  |  |  | `String(1)` |  | Backflush |  |  |
| `ProposedProductSupplyArea` |  |  |  |  |  | `String(10)` |  | Proposed Supply Area |  |  |
| `PlannedOrderActionControl` |  |  |  |  |  | `String(2)` |  | Action Control |  |  |
| `ProductUnitGroup` |  |  |  |  |  | `String(4)` |  | Unit of Measure Group |  |  |
| `MRPSafetyStockMethod` |  |  |  |  |  | `String(2)` |  | Safety Stock Method |  |  |
| `JITProdnConfProfile` |  |  |  |  |  | `String(4)` |  | JIT Production Confirmation Profile |  |  |
| `Currency` |  |  |  |  |  | `String(5)` |  | Currency |  |  |
| `CompanyCode` |  |  |  |  |  | `String(4)` |  | Company Code |  |  |
| `ValuationArea` |  |  |  |  |  | `String(4)` |  | Valuation Area |  |  |
| `BaseUnit` |  |  |  |  |  | `String(3)` |  | Base Unit of Measure |  |  |


## Entity: `ProductPlantWorkScheduling`

- **ABAP CDS Name:** `I_ProductWorkScheduling`
- **Label:** Product WorkScheduling core entity
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** MARC

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Product |  |  |
| `Plant` |  |  |  |  |  | `String(4)` | Y | Plant |  |  |
| `MaterialBaseQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Base quantity | BaseUnit |  |
| `UnlimitedOverDelivIsAllowed` |  |  |  |  |  | `Boolean` |  | Unltd Overdelivery |  |  |
| `OverDelivToleranceLimit` |  |  |  |  |  | `Decimal(3,1)` |  | Overdelivery Toler. |  |  |
| `UnderDelivToleranceLimit` |  |  |  |  |  | `Decimal(3,1)` |  | Underdelivery Toler. |  |  |
| `ProductionInvtryManagedLoc` |  |  |  |  |  | `String(4)` |  | Storage Location |  |  |
| `IsActiveEntity` |  |  |  |  |  | `Boolean` |  | Is active |  |  |
| `ProdnOrderIsBatchRequired` |  |  |  |  |  | `String(1)` |  | Batch entry |  |  |
| `ProdIsWithdrawnFrmProdnBin` |  |  |  |  |  | `Boolean` |  | Withdr.from prod.bin |  |  |
| `TransitionMatrixProductsGroup` |  |  |  |  |  | `String(20)` |  | Material Grouping |  |  |
| `OrderChangeManagementProfile` |  |  |  |  |  | `String(6)` |  | Change overall prof. |  |  |
| `MatlCompIsMarkedForBackflush` |  |  |  |  |  | `String(1)` |  | Backflush |  |  |
| `SetupAndTeardownTime` |  |  |  |  |  | `Decimal(5,2)` |  | Setup time |  |  |
| `ProductionSchedulingProfile` |  |  |  |  |  | `String(6)` |  | Production Scheduling Profile |  |  |
| `TransitionTime` |  |  |  |  |  | `Decimal(5,2)` |  | Interoperation |  |  |
| `ProcessingTimeInDays` |  |  |  |  |  | `Decimal(5,2)` |  | Processing time |  |  |
| `ProductionSupervisor` |  |  |  |  |  | `String(3)` |  | Prodn Supervisor |  |  |
| `ProductProductionQuantityUnit` |  |  |  |  |  | `String(3)` |  | Production unit |  |  |
| `HasProductionVersion` |  |  |  |  |  | `Boolean` |  | Version Indicator |  |  |
| `BaseUnit` |  |  |  |  |  | `String(3)` |  | Base Unit of Measure |  |  |


## Entity: `ProductProcurement`

- **ABAP CDS Name:** `I_Productprocurement`
- **Label:** Product Procurement
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** MARA

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Material |  |  |
| `PurchaseOrderQuantityUnit` |  |  |  |  |  | `String(3)` |  | Order Unit |  |  |
| `VarblPurOrdUnitStatus` |  |  |  |  |  | `String(1)` |  | Var. Order Unit |  |  |
| `PurchasingAcknProfile` |  |  |  |  |  | `String(4)` |  | Purchasing value key |  |  |
| `ProcurementRule` |  |  |  |  |  | `String(1)` |  | Procurement rule |  |  |
| `SourceOfSupplyCategory` |  |  |  |  |  | `String(1)` |  | Source of supply |  |  |
| `PurchasingGroup` |  |  |  |  |  | `String(3)` |  | Purchasing Group |  |  |
| `IsActiveEntity` |  |  |  |  |  | `Boolean` |  | Is active |  |  |
| `AuthorizationGroup` |  |  |  |  |  | `String(4)` |  | Authorization Group |  |  |


## Entity: `ProductQualityManagement`

- **ABAP CDS Name:** `I_Productqm`
- **Label:** Product QM active core entity
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** MARA

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Product |  |  |
| `QltyMgmtInProcmtIsActive` |  |  |  |  |  | `Boolean` |  | QM in Procur. Active |  |  |
| `AuthorizationGroup` |  |  |  |  |  | `String(4)` |  | Authorization Group |  |  |
| `CatalogProfile` |  |  |  |  |  | `String(9)` |  | Catalog Profile |  |  |


## Entity: `ProductSales`

- **ABAP CDS Name:** `I_ProductSales`
- **Label:** Product Sales
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** MVKE

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Material |  |  |
| `SalesStatus` |  |  |  |  |  | `String(2)` |  | X-DChain Status |  |  |
| `SalesStatusValidityDate` |  |  |  |  |  | `Date` |  | Cross-Distr. Chain Product Validity |  |  |
| `TaxClassification` |  |  |  |  |  | `String(1)` |  | Tax classification |  |  |
| `TransportationGroup` |  |  |  |  |  | `String(4)` |  | Transportation Group |  |  |
| `AllowedPackagingWeightQty` |  |  |  |  |  | `Decimal(13,3)` |  | Allowed Pkg wt | AllowedPackagingWeightQtyUnit |  |
| `AllowedPackagingWeightQtyUnit` |  |  |  |  |  | `String(3)` |  | Allowed Packaging Unit of Weight |  |  |
| `AllowedPackagingVolumeQty` |  |  |  |  |  | `Decimal(13,3)` |  | Allowed Volume | AllowedPackagingVolumeQtyUnit |  |
| `AllowedPackagingVolumeQtyUnit` |  |  |  |  |  | `String(3)` |  | Allowed Packaging Unit of Volume |  |  |
| `PricingReferenceProduct` |  |  |  |  |  | `String(40)` |  | Pricing Ref. Matl |  |  |
| `VariantsPricingProfile` |  |  |  |  |  | `String(1)` |  | Pricing profile |  |  |
| `IsVariantPriceAllowed` |  |  |  |  |  | `Boolean` |  | Var. Price Allowed |  |  |
| `LoadingGroup` |  |  |  |  |  | `String(4)` |  | Loading Group |  |  |
| `IsActiveEntity` |  |  |  |  |  | `Boolean` |  | Is active |  |  |
| `ExcessWeightTolerance` |  |  |  |  |  | `Decimal(3,1)` |  | Excess Weight Tolerance |  |  |
| `ExcessVolumeTolerance` |  |  |  |  |  | `Decimal(3,1)` |  | Excess Volume Tolerance |  |  |
| `PackagingMaterialType` |  |  |  |  |  | `String(4)` |  | Packaging Material Type |  |  |
| `IsClosedPackagingMaterial` |  |  |  |  |  | `Boolean` |  | Closed |  |  |
| `VolumeMaximumLevel` |  |  |  |  |  | `Decimal(3,0)` |  | Maximum level |  |  |
| `AuthorizationGroup` |  |  |  |  |  | `String(4)` |  | Authorization Group |  |  |
| `MaterialFreightGroup` |  |  |  |  |  | `String(8)` |  | Material Freight Grp |  |  |
| `StackingFactor` |  |  |  |  |  | `Integer` |  | Stackability factor |  |  |
| `ServiceDuration` |  |  |  |  |  | `Decimal(13,3)` |  | Duration of Work |  |  |
| `ServiceDurationUnit` |  |  |  |  |  | `String(3)` |  | Unit |  |  |
| `ServiceProfile` |  |  |  |  |  | `String(10)` |  | Service Profile |  |  |
| `ResponseProfile` |  |  |  |  |  | `String(10)` |  | Response Prof. |  |  |
| `CABillgCycle` |  |  |  |  |  | `String(4)` |  | Billing Cycle |  |  |
| `SubscrpnProdBillgCycDetn` |  |  |  |  |  | `String(4)` |  | Billing Cycle Determ |  |  |
| `SubscrpnProdTechRsceSchema` |  |  |  |  |  | `String(2)` |  | Assignment Schema |  |  |
| `ContractAutoRenewalType` |  |  |  |  |  | `String(1)` |  | Ctr. Auto Renew Ind. |  |  |


## Entity: `ProductSalesDelivery`

- **ABAP CDS Name:** `I_ProductSalesDelivery`
- **Label:** Product Sales Delivery
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** MVKE

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Product |  |  |
| `ProductSalesOrg` |  |  |  |  |  | `String(4)` | Y | Sales Organization |  |  |
| `ProductDistributionChnl` |  |  |  |  |  | `String(2)` | Y | Distribution Channel |  |  |
| `MinimumOrderQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Minimum order qty | BaseUnit |  |
| `SupplyingPlant` |  |  |  |  |  | `String(4)` |  | Delivering Plant |  |  |
| `PriceSpecificationProductGroup` |  |  |  |  |  | `String(2)` |  | Product Price Group |  |  |
| `AccountDetnProductGroup` |  |  |  |  |  | `String(2)` |  | Acct Assmt Grp Mat. |  |  |
| `DeliveryNoteProcMinDelivQty` |  |  |  |  |  | `Decimal(13,3)` |  | Minimum Delivery Qty | BaseUnit |  |
| `ItemCategoryGroup` |  |  |  |  |  | `String(4)` |  | Item Category Group |  |  |
| `DeliveryQuantityUnit` |  |  |  |  |  | `String(3)` |  | Unit Of Measure |  |  |
| `DeliveryQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Delivery unit | DeliveryQuantityUnit |  |
| `ProductSalesStatus` |  |  |  |  |  | `String(2)` |  | DChain-spec. status |  |  |
| `ProductSalesStatusValidityDate` |  |  |  |  |  | `Date` |  | Valid from |  |  |
| `SalesMeasureUnit` |  |  |  |  |  | `String(3)` |  | Sales Unit |  |  |
| `IsMarkedForDeletion` |  |  |  |  |  | `Boolean` |  | DF distr. chain lvl |  |  |
| `ProductHierarchy` |  |  |  |  |  | `String(18)` |  | Product Hierarchy |  |  |
| `FirstSalesSpecProductGroup` |  |  |  |  |  | `String(3)` |  | Product Group 1 |  |  |
| `SecondSalesSpecProductGroup` |  |  |  |  |  | `String(3)` |  | Product Group 2 |  |  |
| `ThirdSalesSpecProductGroup` |  |  |  |  |  | `String(3)` |  | Product Group 3 |  |  |
| `FourthSalesSpecProductGroup` |  |  |  |  |  | `String(3)` |  | Product Group 4 |  |  |
| `FifthSalesSpecProductGroup` |  |  |  |  |  | `String(3)` |  | Product Group 5 |  |  |
| `MinimumMakeToOrderOrderQty` |  |  |  |  |  | `Decimal(13,3)` |  | Min. MtO quantity | BaseUnit |  |
| `LogisticsStatisticsGroup` |  |  |  |  |  | `String(1)` |  | Matl statistics grp |  |  |
| `VolumeRebateGroup` |  |  |  |  |  | `String(2)` |  | Volume Rebate Group |  |  |
| `ProductCommissionGroup` |  |  |  |  |  | `String(2)` |  | Commission Group |  |  |
| `CashDiscountIsDeductible` |  |  |  |  |  | `Boolean` |  | Cash Discount |  |  |
| `PricingReferenceProduct` |  |  |  |  |  | `String(40)` |  | Pricing Ref. Matl |  |  |
| `AssortmentGrade` |  |  |  |  |  | `String(2)` |  | Assortment Grade |  |  |
| `StoreListingProcedure` |  |  |  |  |  | `String(2)` |  | LP for Stores |  |  |
| `DistrCntrListingProcedure` |  |  |  |  |  | `String(2)` |  | LP distr. ctrs |  |  |
| `StoreListingStartDate` |  |  |  |  |  | `Date` |  | Store Listed from |  |  |
| `StoreListingEndDate` |  |  |  |  |  | `Date` |  | Store Listed to |  |  |
| `DistrCntrListingStartDate` |  |  |  |  |  | `Date` |  | DC Listed from |  |  |
| `DistrCntrListingEndDate` |  |  |  |  |  | `Date` |  | DC Listed to |  |  |
| `StoreSaleStartDate` |  |  |  |  |  | `Date` |  | For sale from (str) |  |  |
| `StoreSaleEndDate` |  |  |  |  |  | `Date` |  | For sale till (str) |  |  |
| `DistrCntrSaleStartDate` |  |  |  |  |  | `Date` |  | For sale from (DC) |  |  |
| `DistrCntrSaleEndDate` |  |  |  |  |  | `Date` |  | For sale till (DC) |  |  |
| `RoundingProfile` |  |  |  |  |  | `String(4)` |  | Rounding Profile |  |  |
| `ProductUnitGroup` |  |  |  |  |  | `String(4)` |  | Unit of Measure Grp |  |  |
| `MaxDeliveryQtyStoreOrder` |  |  |  |  |  | `Decimal(13,3)` |  | Max. delivery qty | BaseUnit |  |
| `PriceFixingCategory` |  |  |  |  |  | `String(1)` |  | Price fixing |  |  |
| `VariableSalesUnitIsNotAllowed` |  |  |  |  |  | `Boolean` |  | Sales unit not var. |  |  |
| `CompetitionPressureCategory` |  |  |  |  |  | `String(1)` |  | Competition charactn |  |  |
| `ProductHasAttributeID01` |  |  |  |  |  | `Boolean` |  | Product Attribute 1 |  |  |
| `ProductHasAttributeID02` |  |  |  |  |  | `Boolean` |  | Product Attribute 2 |  |  |
| `ProductHasAttributeID03` |  |  |  |  |  | `Boolean` |  | Product Attribute 3 |  |  |
| `ProductHasAttributeID04` |  |  |  |  |  | `Boolean` |  | Product Attribute 4 |  |  |
| `ProductHasAttributeID05` |  |  |  |  |  | `Boolean` |  | Product Attribute 5 |  |  |
| `ProductHasAttributeID06` |  |  |  |  |  | `Boolean` |  | Product Attribute 6 |  |  |
| `ProductHasAttributeID07` |  |  |  |  |  | `Boolean` |  | Product Attribute 7 |  |  |
| `ProductHasAttributeID08` |  |  |  |  |  | `Boolean` |  | Product Attribute 8 |  |  |
| `ProductHasAttributeID09` |  |  |  |  |  | `Boolean` |  | Product Attribute 9 |  |  |
| `ProductHasAttributeID10` |  |  |  |  |  | `Boolean` |  | Product Attribute 10 |  |  |
| `IsActiveEntity` |  |  |  |  |  | `Boolean` |  | Is active |  |  |
| `ProdExtAssortmentPriority` |  |  |  |  |  | `String(1)` |  | Ext. asst priority |  |  |
| `ProdIsEntlmntRlvt` |  |  |  |  |  | `Boolean` |  | Rel. Entitlement Gen |  |  |
| `BaseUnit` |  |  |  |  |  | `String(3)` |  | Base Unit of Measure |  |  |
| `SubscrpnContrDfltDuration` |  |  |  |  |  | `String(3)` |  | Def Contract Term |  |  |
| `SubscrpnContrAltvDuration1` |  |  |  |  |  | `String(3)` |  | Contract Term 1 |  |  |
| `SubscrpnContrAltvDuration2` |  |  |  |  |  | `String(3)` |  | Contract Term 2 |  |  |
| `SubscrpnContrDurationUnit` |  |  |  |  |  | `String(1)` |  | Unit Contract Term |  |  |
| `SubscrpnContrDfltExtnDurn` |  |  |  |  |  | `String(3)` |  | Def Extension Period |  |  |
| `SubscrpnContrAltvExtnDurn1` |  |  |  |  |  | `String(3)` |  | Extension Period 1 |  |  |
| `SubscrpnContrAltvExtnDurn2` |  |  |  |  |  | `String(3)` |  | Extension Period 2 |  |  |
| `SubscrpnContrExtnDurnUnit` |  |  |  |  |  | `String(1)` |  | Unit for Extension |  |  |
| `LstMiProductPackageSizeCode` |  |  |  |  |  | `String(3)` |  | Package Size |  |  |
| `LstMiProductPackageType` |  |  |  |  |  | `String(3)` |  | Package Type |  |  |


## Entity: `ProductStorage`

- **ABAP CDS Name:** `I_ProductStorage_2`
- **Label:** Product Storage
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** MARA

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Material |  |  |
| `StorageConditions` |  |  |  |  |  | `String(2)` |  | Storage conditions |  |  |
| `TemperatureConditionInd` |  |  |  |  |  | `String(2)` |  | Temp. conditions |  |  |
| `HazardousMaterialNumber` |  |  |  |  |  | `String(40)` |  | Haz. material number |  |  |
| `NmbrOfGROrGISlipsToPrintQty` |  |  |  |  |  | `Decimal(13,3)` |  | GR slips quantity | BaseUnit |  |
| `LabelType` |  |  |  |  |  | `String(2)` |  | Label type |  |  |
| `LabelForm` |  |  |  |  |  | `String(2)` |  | Label form |  |  |
| `MinRemainingShelfLife` |  |  |  |  |  | `Decimal(4,0)` |  | Min. Rem. Shelf Life |  |  |
| `ProductExpirationDateCode` |  |  |  |  |  | `String(1)` |  | Expiration Date |  |  |
| `StorageBinInstruction` |  |  |  |  |  | `String(2)` |  | Container reqmts |  |  |
| `TotalShelfLifeStoragePercent` |  |  |  |  |  | `Decimal(3,0)` |  | Storage percentage |  |  |
| `ShelfLifeExpirationDatePeriod` |  |  |  |  |  | `String(1)` |  | Period Ind. for SLED |  |  |
| `ShelfLifeExprtnDateRndngRule` |  |  |  |  |  | `String(1)` |  | Rounding rule SLED |  |  |
| `AuthorizationGroup` |  |  |  |  |  | `String(4)` |  | Authorization Group |  |  |
| `IsActiveEntity` |  |  |  |  |  | `Boolean` |  | Is active |  |  |
| `TotalShelfLife` |  |  |  |  |  | `Decimal(4,0)` |  | Total Shelf Life |  |  |
| `BaseUnit` |  |  |  |  |  | `String(3)` |  | Base Unit of Measure |  |  |


## Entity: `ProductUnitOfMeasure`

- **ABAP CDS Name:** `I_ProductUnitsOfMeasure`
- **Label:** Units of Measure of Product
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** MARM

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Product |  |  |
| `AlternativeUnit` |  |  |  |  |  | `String(3)` | Y | AlternativeUnit |  |  |
| `QuantityNumerator` |  |  |  |  |  | `Decimal(5,0)` |  | Units / Quantity - Base Unit of Measure | BaseUnit |  |
| `QuantityDenominator` |  |  |  |  |  | `Decimal(5,0)` |  | Units / Quantity - Alt Unit of Measure | AlternativeUnit |  |
| `MaterialVolume` |  |  |  |  |  | `Decimal(13,3)` |  | Volume | VolumeUnit |  |
| `VolumeUnit` |  |  |  |  |  | `String(3)` |  | Volume Unit |  |  |
| `GrossWeight` |  |  |  |  |  | `Decimal(13,3)` |  | Gross Weight | WeightUnit |  |
| `WeightUnit` |  |  |  |  |  | `String(3)` |  | Unit of Weight |  |  |
| `GlobalTradeItemNumber` |  |  |  |  |  | `String(18)` |  | EAN/UPC |  |  |
| `GlobalTradeItemNumberCategory` |  |  |  |  |  | `String(2)` |  | GTIN Category |  |  |
| `UnitSpecificProductLength` |  |  |  |  |  | `Decimal(13,3)` |  | Length | ProductMeasurementUnit |  |
| `UnitSpecificProductWidth` |  |  |  |  |  | `Decimal(13,3)` |  | Width | ProductMeasurementUnit |  |
| `UnitSpecificProductHeight` |  |  |  |  |  | `Decimal(13,3)` |  | Height | ProductMeasurementUnit |  |
| `ProductMeasurementUnit` |  |  |  |  |  | `String(3)` |  | Unit of Dimension |  |  |
| `LowerLevelPackagingUnit` |  |  |  |  |  | `String(3)` |  | Lower-level unit |  |  |
| `RemainingVolumeAfterNesting` |  |  |  |  |  | `Decimal(3,0)` |  | Rem.Vol.After Nestng |  |  |
| `MaximumStackingFactor` |  |  |  |  |  | `Integer` |  | Max. Stacking Factor |  |  |
| `CapacityUsage` |  |  |  |  |  | `Decimal(15,3)` |  | Capacity Usage |  |  |
| `IsActiveEntity` |  |  |  |  |  | `Boolean` |  | Is active |  |  |
| `UnitOfMeasureCategory` |  |  |  |  |  | `String(1)` |  | UoM Category |  |  |
| `ProductGTINVariant` |  |  |  |  |  | `String(2)` |  | EAN Variant |  |  |
| `BaseUnit` |  |  |  |  |  | `String(3)` |  | Base Unit of Measure |  |  |


## Entity: `ProductUnitOfMeasureEAN`

- **ABAP CDS Name:** `I_ProductUnitOfMeasureEAN`
- **Label:** International Article Number of Product
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** MEAN

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Material |  |  |
| `AlternativeUnit` |  |  |  |  |  | `String(3)` | Y | Display Unit/Measure |  |  |
| `ConsecutiveNumber` |  |  |  |  |  | `String(5)` | Y | Consecutive number |  |  |
| `ProductStandardID` |  |  |  |  |  | `String(18)` |  | EAN/UPC |  |  |
| `InternationalArticleNumberCat` |  |  |  |  |  | `String(2)` |  | GTIN Category |  |  |
| `IsMainGlobalTradeItemNumber` |  |  |  |  |  | `Boolean` |  | Main EAN |  |  |


## Entity: `ProductValuation`

- **ABAP CDS Name:** `I_ProductValuationBasic`
- **Label:** Product Valuation
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** MBEW

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Product |  |  |
| `ValuationArea` |  |  |  |  |  | `String(4)` | Y | Valuation Area |  |  |
| `ValuationType` |  |  |  |  |  | `String(10)` | Y | Valuation Type |  |  |
| `ValuationClass` |  |  |  |  |  | `String(4)` |  | Valuation Class |  |  |
| `PriceDeterminationControl` |  |  |  |  |  | `String(1)` |  | Price Determ. |  |  |
| `FiscalMonthCurrentPeriod` |  |  |  |  |  | `String(2)` |  | Current Period |  |  |
| `FiscalYearCurrentPeriod` |  |  |  |  |  | `String(4)` |  | Year Current Period |  |  |
| `StandardPrice` |  |  |  |  |  | `Decimal(34,4)` |  | Standard price | Currency |  |
| `PriceUnitQty` |  |  |  |  |  | `Decimal(5,0)` |  | Price unit |  |  |
| `InventoryValuationProcedure` |  |  |  |  |  | `String(1)` |  | Price Control |  |  |
| `FuturePriceValidityStartDate` |  |  |  |  |  | `Date` |  | Valid from |  |  |
| `PrevInvtryPriceInCoCodeCrcy` |  |  |  |  |  | `Decimal(34,4)` |  | Previous Price | Currency |  |
| `MovingAveragePrice` |  |  |  |  |  | `Decimal(34,4)` |  | Moving price | Currency |  |
| `ValuationCategory` |  |  |  |  |  | `String(1)` |  | Valuation Category |  |  |
| `ProductUsageType` |  |  |  |  |  | `String(1)` |  | Product Usage |  |  |
| `ProductOriginType` |  |  |  |  |  | `String(1)` |  | Product Origin |  |  |
| `IsProducedInhouse` |  |  |  |  |  | `Boolean` |  | In-House Production |  |  |
| `ProdCostEstNumber` |  |  |  |  |  | `String(12)` |  | ProdCostEst.No. |  |  |
| `IsMarkedForDeletion` |  |  |  |  |  | `Boolean` |  | Del. flag val. type |  |  |
| `ValuationMargin` |  |  |  |  |  | `Decimal(6,2)` |  | Valuation Margin |  |  |
| `IsActiveEntity` |  |  |  |  |  | `Boolean` |  | Is active |  |  |
| `CompanyCode` |  |  |  |  |  | `String(4)` |  | Company Code |  |  |
| `ValuationClassSalesOrderStock` |  |  |  |  |  | `String(4)` |  | VC: Sales Order Stk |  |  |
| `ProjectStockValuationClass` |  |  |  |  |  | `String(4)` |  | Proj. stk val. class |  |  |
| `TaxBasedPricesPriceUnitQty` |  |  |  |  |  | `Decimal(5,0)` |  | Price Unit | BaseUnit |  |
| `PriceLastChangeDate` |  |  |  |  |  | `Date` |  | Last Price Change |  |  |
| `FuturePrice` |  |  |  |  |  | `Decimal(34,4)` |  | Future Price | Currency |  |
| `MaintenanceStatus` |  |  |  |  |  | `String(15)` |  | Maintenance Status |  |  |
| `Currency` |  |  |  |  |  | `String(5)` |  | Currency |  |  |
| `BaseUnit` |  |  |  |  |  | `String(3)` |  | Base Unit of Measure |  |  |
| `MLIsActiveAtProductLevel` |  |  |  |  |  | `Boolean` |  | ML Act. |  |  |


## Entity: `ProductValuationAccounting`

- **ABAP CDS Name:** `I_ProductValuationAccounting_2`
- **Label:** Product Valuation Account
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** MBEW

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Product |  |  |
| `ValuationArea` |  |  |  |  |  | `String(4)` | Y | Valuation Area |  |  |
| `ValuationType` |  |  |  |  |  | `String(10)` | Y | Valuation Type |  |  |
| `CommercialPrice1InCoCodeCrcy` |  |  |  |  |  | `Decimal(34,4)` |  | Commercial price 1 | Currency |  |
| `CommercialPrice2InCoCodeCrcy` |  |  |  |  |  | `Decimal(34,4)` |  | Commercial price 2 | Currency |  |
| `CommercialPrice3InCoCodeCrcy` |  |  |  |  |  | `Decimal(34,4)` |  | Commercial price 3 | Currency |  |
| `DevaluationYearCount` |  |  |  |  |  | `String(2)` |  | Devaluation Ind. |  |  |
| `FuturePrice` |  |  |  |  |  | `Decimal(34,4)` |  | Future Price | Currency |  |
| `FuturePriceValidityStartDate` |  |  |  |  |  | `Date` |  | Valid from |  |  |
| `IsLIFOAndFIFORelevant` |  |  |  |  |  | `Boolean` |  | TRUE |  |  |
| `LIFOValuationPoolNumber` |  |  |  |  |  | `String(4)` |  | LIFO Pool |  |  |
| `StandardPricePrevYear` |  |  |  |  |  | `Decimal(34,4)` |  | Standard price | Currency |  |
| `TaxPricel1InCoCodeCrcy` |  |  |  |  |  | `Decimal(34,4)` |  | Tax price 1 | Currency |  |
| `TaxPrice2InCoCodeCrcy` |  |  |  |  |  | `Decimal(34,4)` |  | Tax price 2 | Currency |  |
| `TaxPrice3InCoCodeCrcy` |  |  |  |  |  | `Decimal(34,4)` |  | Tax price 3 | Currency |  |
| `TaxBasedPricesPriceUnitQty` |  |  |  |  |  | `Decimal(5,0)` |  | Price Unit | BaseUnit |  |
| `CompanyCode` |  |  |  |  |  | `String(4)` |  | Company Code |  |  |
| `Currency` |  |  |  |  |  | `String(5)` |  | Currency |  |  |
| `BaseUnit` |  |  |  |  |  | `String(3)` |  | Base Unit of Measure |  |  |


## Entity: `ProductValuationCosting`

- **ABAP CDS Name:** `I_ProductValuationCosting`
- **Label:** Product Valuation Costing Core Entity
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** MBEW

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Product |  |  |
| `ValuationArea` |  |  |  |  |  | `String(4)` | Y | Valuation Area |  |  |
| `ValuationType` |  |  |  |  |  | `String(10)` | Y | Valuation Type |  |  |
| `IsMaterialCostedWithQtyStruc` |  |  |  |  |  | `Boolean` |  | With Qty Structure |  |  |
| `IsMaterialRelatedOrigin` |  |  |  |  |  | `Boolean` |  | Material origin |  |  |
| `CostOriginGroup` |  |  |  |  |  | `String(4)` |  | Origin Group |  |  |
| `CostingOverheadGroup` |  |  |  |  |  | `String(10)` |  | Overhead Group |  |  |
| `PlannedPrice1InCoCodeCrcy` |  |  |  |  |  | `Decimal(34,4)` |  | Planned price 1 | Currency |  |
| `PlannedPrice2InCoCodeCrcy` |  |  |  |  |  | `Decimal(34,4)` |  | Planned price 2 | Currency |  |
| `PlannedPrice3InCoCodeCrcy` |  |  |  |  |  | `Decimal(34,4)` |  | Planned price 3 | Currency |  |
| `FuturePlndPrice1ValdtyDate` |  |  |  |  |  | `Date` |  | Planned price date 1 |  |  |
| `FuturePlndPrice2ValdtyDate` |  |  |  |  |  | `Date` |  | Planned price date 2 |  |  |
| `FuturePlndPrice3ValdtyDate` |  |  |  |  |  | `Date` |  | Planned price date 3 |  |  |
| `PlannedPrice` |  |  |  |  |  | `Decimal(34,4)` |  | Future Planned Price | Currency |  |
| `Currency` |  |  |  |  |  | `String(5)` |  | Currency |  |  |
| `CompanyCode` |  |  |  |  |  | `String(4)` |  | Company Code |  |  |


## Entity: `ProductWarehouseManagement`

- **ABAP CDS Name:** `I_ProductWrhsMgmt`
- **Label:** Product Warehouse Management
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** MLGN, MLGT

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Product` |  |  |  |  |  | `String(40)` | Y | Product |  |  |
| `WarehouseNumber` |  |  |  |  |  | `String(3)` | Y | Warehouse Number |  |  |
| `ProdWrhsMatlDataIsMrkdForDeltn` |  |  |  |  |  | `Boolean` |  | Del.flag:warehse no. |  |  |
| `ProdStorageSectionMethod` |  |  |  |  |  | `String(3)` |  | Storage Section Ind. |  |  |
| `ProdWrhsStkPlacementStorType` |  |  |  |  |  | `String(3)` |  | Stock placement |  |  |
| `ProdWrhsStkRemovalStorageType` |  |  |  |  |  | `String(3)` |  | Stock removal |  |  |
| `ProdWrhs1stLoadgEquipQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Loading equip. qty 1 | ProdWrhs1stLoadgEquipQtyUnit |  |
| `ProdWrhs2ndLoadgEquipQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Loading equip. qty 2 | ProdWrhs2ndLoadgEquipQtyUnit |  |
| `ProdWrhs3rdLoadgEquipQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Loading equip. qty 3 | ProdWrhs3rdLoadgEquipQtyUnit |  |
| `ProdWrhs1stLoadgEquipQtyUnit` |  |  |  |  |  | `String(3)` |  | Unit of measure 1 |  |  |
| `ProdWrhs2ndLoadgEquipQtyUnit` |  |  |  |  |  | `String(3)` |  | Unit of measure 2 |  |  |
| `ProdWrhs3rdLoadgEquipQtyUnit` |  |  |  |  |  | `String(3)` |  | Unit of measure 3 |  |  |
| `ProductStorageUnitType1` |  |  |  |  |  | `String(3)` |  | Storage Unit Type 1 |  |  |
| `ProductStorageUnitType2` |  |  |  |  |  | `String(3)` |  | Storage Unit Type 2 |  |  |
| `ProductStorageUnitType3` |  |  |  |  |  | `String(3)` |  | Storage Unit Type 3 |  |  |
| `ProdWarehouseManagementUnit` |  |  |  |  |  | `String(3)` |  | WM unit |  |  |
| `AdditionToExistingStkIsAllowed` |  |  |  |  |  | `Boolean` |  | Allow addn to stock |  |  |
| `ProductBulkStorageMethod` |  |  |  |  |  | `String(2)` |  | Bulk storage |  |  |
| `WrhsMgmtMsgToInvtryMgmtIsRqd` |  |  |  |  |  | `Boolean` |  | Message to inv. mgmt |  |  |
| `WrhsMgmtHasSpecialMovement` |  |  |  |  |  | `String(1)` |  | Special movement |  |  |
| `CapacityUsage` |  |  |  |  |  | `Decimal(11,3)` |  | Capacity usage |  |  |
| `CapacityConsumptionUnit` |  |  |  |  |  | `String(3)` |  | Cap.consumption unit |  |  |
| `ProdWrhsPickingStorageType` |  |  |  |  |  | `String(3)` |  | Picking storage type |  |  |
| `ProdWrhsMatlMasterDefaultUnit` |  |  |  |  |  | `String(1)` |  | Proposed UoM frm mat |  |  |
| `ProdIsRlvtForTwoStepPicking` |  |  |  |  |  | `String(1)` |  | 2-step picking |  |  |
