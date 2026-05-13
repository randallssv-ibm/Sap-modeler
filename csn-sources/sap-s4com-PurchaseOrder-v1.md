# PurchaseOrder

> Source file: `sap-s4com-PurchaseOrder-v1.json`


## Entity: `PurOrdSupplierConfirmation`

- **ABAP CDS Name:** `C_POSupplierConfirmationDEX`
- **Label:** Purchase Order Supplier Confirmation DEX
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** EKAB

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `PurchaseOrder` |  |  |  |  |  | `String(10)` | Y | Purchase Order |  |  |
| `PurchaseOrderItem` |  |  |  |  |  | `String(5)` | Y | Purchase Order Item |  |  |
| `SequentialNmbrOfSuplrConf` |  |  |  |  |  | `String(4)` | Y | Sequential Number |  |  |
| `SupplierConfirmationCategory` |  |  |  |  |  | `String(2)` |  | Confirm. Category |  |  |
| `DeliveryDate` |  |  |  |  |  | `Date` |  | Delivery Date |  |  |
| `DelivDateCategory` |  |  |  |  |  | `String(1)` |  | Deliv. Date Category |  |  |
| `DeliveryTime` |  |  |  |  |  | `String(6)` |  | Time |  |  |
| `CreationDate` |  |  |  |  |  | `Date` |  | Creation Date |  |  |
| `CreationTime` |  |  |  |  |  | `String(6)` |  | Creation Time |  |  |
| `ConfirmedQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Quantity | OrderQuantityUnit |  |
| `MRPRelevantQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Qty Reduced (MRP) | OrderQuantityUnit |  |
| `SuplrConfCreationCategory` |  |  |  |  |  | `String(1)` |  | Creation Indicator |  |  |
| `IsDeleted` |  |  |  |  |  | `String(1)` |  | Deletion Indicator |  |  |
| `ConfIsRelevantToMRP` |  |  |  |  |  | `Boolean` |  | MRP-Relevant |  |  |
| `SupplierConfirmationExtNumber` |  |  |  |  |  | `String(35)` |  | Reference |  |  |
| `DeliveryDocument` |  |  |  |  |  | `String(10)` |  | Delivery |  |  |
| `DeliveryDocumentItem` |  |  |  |  |  | `String(6)` |  | Item |  |  |
| `ManufacturerPartProfile` |  |  |  |  |  | `String(4)` |  | Mfr Part Profile |  |  |
| `ManufacturerMaterial` |  |  |  |  |  | `String(40)` |  | MPN: Material |  |  |
| `NumberOfReminders` |  |  |  |  |  | `Decimal(3,0)` |  | No. Rem./Expediters |  |  |
| `Batch` |  |  |  |  |  | `String(10)` |  | Batch |  |  |
| `DeliveryIsInPlant` |  |  |  |  |  | `Boolean` |  | In Plant |  |  |
| `HandoverDate` |  |  |  |  |  | `Date` |  | Handover Date |  |  |
| `HandoverTime` |  |  |  |  |  | `String(6)` |  | Handover Time |  |  |
| `PerformancePeriodStartDate` |  |  |  |  |  | `Date` |  | Start Date |  |  |
| `PerformancePeriodEndDate` |  |  |  |  |  | `Date` |  | End Date |  |  |
| `ServicePerformer` |  |  |  |  |  | `String(10)` |  | Service Performer |  |  |
| `OrderQuantityUnit` |  |  |  |  |  | `String(3)` |  | Order Unit |  |  |
| `SupplierConfirmation` |  |  |  |  |  | `String(10)` |  | Confirmation |  |  |
| `SupplierConfirmationItem` |  |  |  |  |  | `String(5)` |  | Confirmation Item |  |  |
| `PurchaseOrderType` |  |  |  |  |  | `String(4)` |  | Purchasing Doc. Type |  |  |
| `PurchasingOrganization` |  |  |  |  |  | `String(4)` |  | Purch. Organization |  |  |
| `PurchasingGroup` |  |  |  |  |  | `String(3)` |  | Purchasing Group |  |  |
| `Plant` |  |  |  |  |  | `String(4)` |  | Plant |  |  |


## Entity: `PurchaseOrder`

- **ABAP CDS Name:** `C_PurchaseOrderDEX`
- **Label:** Data Extraction for Purchase Order
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** EKKO

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `PurchaseOrder` |  | `EKKO` | `EBELN` |  |  | `String(10)` | Y | Purchase Order |  |  |
| `PurchaseOrderType` |  | `EKKO` | `BSART` |  |  | `String(4)` |  | Purchasing Doc. Type |  |  |
| `PurchaseOrderSubtype` |  |  |  |  |  | `String(1)` |  | Control indicator |  |  |
| `PurchasingDocumentOrigin` |  |  |  |  |  | `String(1)` |  | Status |  |  |
| `CreatedByUser` |  | `EKKO` | `ERNAM` |  |  | `String(12)` |  | Created By |  |  |
| `CreationDate` |  | `EKKO` | `AEDAT` |  |  | `Date` |  | Created On |  |  |
| `PurchaseOrderDate` |  | `EKKO` | `BEDAT` |  |  | `Date` |  | Purchase Order Date |  |  |
| `Language` |  | `EKKO` | `SPRAS` |  |  | `String(2)` |  | Language Key |  |  |
| `CorrespncExternalReference` |  |  |  |  |  | `String(12)` |  | Your Reference |  |  |
| `CorrespncInternalReference` |  |  |  |  |  | `String(12)` |  | Our Reference |  |  |
| `PurchasingDocumentDeletionCode` |  |  |  |  |  | `String(1)` |  | Deletion Code |  |  |
| `ReleaseIsNotCompleted` |  |  |  |  |  | `Boolean` |  | Subject to Release |  |  |
| `PurchasingCompletenessStatus` |  |  |  |  |  | `Boolean` |  | Incomplete |  |  |
| `PurchasingProcessingStatus` |  |  |  |  |  | `String(2)` |  | Proc. State |  |  |
| `PurgReleaseSequenceStatus` |  |  |  |  |  | `String(8)` |  | Release Status |  |  |
| `ReleaseCode` |  |  |  |  |  | `String(1)` |  | Release indicator |  |  |
| `CompanyCode` |  | `EKKO` | `BUKRS` |  |  | `String(4)` |  | Company Code |  |  |
| `PurchasingOrganization` |  | `EKKO` | `EKORG` |  |  | `String(4)` |  | Purch. Organization |  |  |
| `PurchasingGroup` |  | `EKKO` | `EKGRP` |  |  | `String(3)` |  | Purchasing Group |  |  |
| `Supplier` |  | `EKKO` | `LIFNR` |  |  | `String(10)` |  | Supplier |  |  |
| `ManualSupplierAddressID` |  |  |  |  |  | `String(10)` |  | Address Number |  |  |
| `SupplierRespSalesPersonName` |  |  |  |  |  | `String(30)` |  | Salesperson |  |  |
| `SupplierPhoneNumber` |  |  |  |  |  | `String(16)` |  | Supplier Phone |  |  |
| `SupplyingSupplier` |  |  |  |  |  | `String(10)` |  | Goods Supplier |  |  |
| `SupplyingPlant` |  |  |  |  |  | `String(4)` |  | Supplying Plant |  |  |
| `InvoicingParty` |  |  |  |  |  | `String(10)` |  | Invoicing Party |  |  |
| `Customer` |  |  |  |  |  | `String(10)` |  | Customer |  |  |
| `SupplierQuotationExternalID` |  |  |  |  |  | `String(10)` |  | Quotation |  |  |
| `PaymentTerms` |  |  |  |  |  | `String(4)` |  | Payment Terms |  |  |
| `CashDiscount1Days` |  |  |  |  |  | `Decimal(3,0)` |  | Days 1 |  |  |
| `CashDiscount2Days` |  |  |  |  |  | `Decimal(3,0)` |  | Days 2 |  |  |
| `NetPaymentDays` |  |  |  |  |  | `Decimal(3,0)` |  | Days Net |  |  |
| `CashDiscount1Percent` |  |  |  |  |  | `Decimal(5,3)` |  | CD Percentage 1 |  |  |
| `CashDiscount2Percent` |  |  |  |  |  | `Decimal(5,3)` |  | CD Percentage 2 |  |  |
| `DownPaymentType` |  |  |  |  |  | `String(4)` |  | Down Payment |  |  |
| `DownPaymentPercentageOfTotAmt` |  |  |  |  |  | `Decimal(5,2)` |  | Down Payment % |  |  |
| `DownPaymentAmount` |  |  |  |  |  | `Decimal(34,4)` |  | Down Payment Amount | DocumentCurrency |  |
| `DownPaymentDueDate` |  |  |  |  |  | `Date` |  | Due Date for DP |  |  |
| `IncotermsClassification` |  |  |  |  |  | `String(3)` |  | Incoterms |  |  |
| `IncotermsTransferLocation` |  |  |  |  |  | `String(28)` |  | Incoterms (Part 2) |  |  |
| `IncotermsVersion` |  |  |  |  |  | `String(4)` |  | Incoterms Version |  |  |
| `IncotermsLocation1` |  |  |  |  |  | `String(70)` |  | Incoterms Location 1 |  |  |
| `IncotermsLocation2` |  |  |  |  |  | `String(70)` |  | Incoterms Location 2 |  |  |
| `IsIntrastatReportingRelevant` |  |  |  |  |  | `Boolean` |  | Intrastat Relevance |  |  |
| `IsIntrastatReportingExcluded` |  |  |  |  |  | `Boolean` |  | Intrastat Exclusion |  |  |
| `PricingDocument` |  |  |  |  |  | `String(10)` |  | Doc. Condition No. |  |  |
| `PricingProcedure` |  |  |  |  |  | `String(6)` |  | Procedure |  |  |
| `DocumentCurrency` |  | `EKKO` | `WAERS` |  |  | `String(5)` |  | Currency |  |  |
| `ValidityStartDate` |  |  |  |  |  | `Date` |  | Validity Per. Start |  |  |
| `ValidityEndDate` |  |  |  |  |  | `Date` |  | Validity Period End |  |  |
| `ExchangeRate` |  | `EKKO` | `WKURS` |  |  | `Decimal(9,5)` |  | Exchange Rate |  |  |
| `ExchangeRateIsFixed` |  |  |  |  |  | `Boolean` |  | Fixed Exchange Rate |  |  |
| `LastChangeDateTime` |  |  |  |  |  | `Timestamp` |  | Last Changed |  |  |
| `TaxReturnCountry` |  |  |  |  |  | `String(3)` |  | Reporting C/R |  |  |
| `VATRegistrationCountry` |  |  |  |  |  | `String(3)` |  | Ctry/Rgn Sls Tax No. |  |  |
| `PurgReasonForDocCancellation` |  |  |  |  |  | `String(2)` |  | Reason for Canc. |  |  |
| `PurgReleaseTimeTotalAmount` |  |  |  |  |  | `Decimal(34,4)` |  | Tot. val. rel. | DocumentCurrency |  |


## Entity: `PurchaseOrderAccountAssignment`

- **ABAP CDS Name:** `C_PurOrdAccountAssignmentDEX`
- **Label:** Data Extraction for Purchase Order Account Assignments
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** EKKN

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `PurchaseOrder` |  | `EKKO` | `EBELN` |  |  | `String(10)` | Y | Purchasing Document |  |  |
| `PurchaseOrderItem` |  | `EKPO` | `EBELP` |  |  | `String(5)` | Y | Item |  |  |
| `AccountAssignmentNumber` |  | `EKKN` | `ZEKKN` |  |  | `String(2)` | Y | Account Assgmt No. |  |  |
| `CostCenter` |  | `EKKN` | `KOSTL` |  |  | `String(10)` |  | Cost Center |  |  |
| `MasterFixedAsset` |  |  |  |  |  | `String(12)` |  | Asset |  |  |
| `ProjectNetwork` |  |  |  |  |  | `String(12)` |  | Network |  |  |
| `Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Quantity | PurchaseOrderQuantityUnit |  |
| `PurchaseOrderQuantityUnit` |  | `EKPO` | `MEINS` |  |  | `String(3)` |  | Order Unit |  |  |
| `MultipleAcctAssgmtDistrPercent` |  |  |  |  |  | `Decimal(3,1)` |  | Distribution (%) |  |  |
| `PurgDocNetAmount` |  |  |  |  |  | `Decimal(34,4)` |  | Net Order Value | DocumentCurrency |  |
| `DocumentCurrency` |  | `EKKO` | `WAERS` |  |  | `String(5)` |  | Currency |  |  |
| `IsDeleted` |  |  |  |  |  | `Boolean` |  | Deletion Indicator |  |  |
| `GLAccount` |  | `EKKN` | `SAKTO` |  |  | `String(10)` |  | G/L Account |  |  |
| `BusinessArea` |  |  |  |  |  | `String(4)` |  | Business Area |  |  |
| `SalesOrder` |  |  |  |  |  | `String(10)` |  | SD Document |  |  |
| `SalesOrderItem` |  |  |  |  |  | `String(6)` |  | Item |  |  |
| `SalesOrderScheduleLine` |  |  |  |  |  | `String(4)` |  | Schedule Line Number |  |  |
| `FixedAsset` |  |  |  |  |  | `String(4)` |  | Subnumber |  |  |
| `OrderID` |  |  |  |  |  | `String(12)` |  | Order |  |  |
| `UnloadingPointName` |  |  |  |  |  | `String(25)` |  | Unloading Point |  |  |
| `ControllingArea` |  | `EKKN` | `KOKRS` |  |  | `String(4)` |  | Controlling Area |  |  |
| `CostObject` |  |  |  |  |  | `String(12)` |  | Cost Object |  |  |
| `ProfitabilitySegment` |  |  |  |  |  | `String(10)` |  | Profitability Segment (Deprecated) |  |  |
| `ProfitabilitySegment_2` |  |  |  |  |  | `String(10)` |  | Profitability Segment |  |  |
| `ProfitCenter` |  | `EKKN` | `PRCTR` |  |  | `String(10)` |  | Profit Center |  |  |
| `WBSElementInternalID` |  |  |  |  |  | `String(8)` |  | WBS Internal ID |  |  |
| `ProjectNetworkInternalID` |  |  |  |  |  | `String(10)` |  | Opertn Task List No. |  |  |
| `CommitmentItem` |  |  |  |  |  | `String(24)` |  |  |  |  |
| `FundsCenter` |  |  |  |  |  | `String(16)` |  | Funds Center |  |  |
| `Fund` |  |  |  |  |  | `String(10)` |  | Fund |  |  |
| `FunctionalArea` |  | `EKKN` | `FKBER` |  |  | `String(16)` |  | Functional Area |  |  |
| `GoodsRecipientName` |  |  |  |  |  | `String(12)` |  | Goods Recipient |  |  |
| `IsFinallyInvoiced` |  |  |  |  |  | `Boolean` |  | Final Invoice |  |  |
| `RealEstateObject` |  |  |  |  |  | `String(8)` |  | Real Estate Key |  |  |
| `NetworkActivityInternalID` |  |  |  |  |  | `String(8)` |  | Counter |  |  |
| `PartnerAccountNumber` |  |  |  |  |  | `String(10)` |  | Partner |  |  |
| `JointVentureRecoveryCode` |  |  |  |  |  | `String(2)` |  | Recovery Indicator |  |  |
| `SettlementReferenceDate` |  |  |  |  |  | `Date` |  | Reference Date |  |  |
| `OrderInternalID` |  |  |  |  |  | `String(10)` |  | Opertn Task List No. |  |  |
| `OrderIntBillOfOperationsItem` |  |  |  |  |  | `String(8)` |  | Counter |  |  |
| `TaxCode` |  |  |  |  |  | `String(2)` |  | Tax Code |  |  |
| `TaxJurisdiction` |  |  |  |  |  | `String(15)` |  | Tax Jurisdiction |  |  |
| `NonDeductibleInputTaxAmount` |  |  |  |  |  | `Decimal(34,4)` |  | Non-deductible | DocumentCurrency |  |
| `CostCtrActivityType` |  |  |  |  |  | `String(6)` |  | Activity Type |  |  |
| `BusinessProcess` |  |  |  |  |  | `String(12)` |  | Business Process |  |  |
| `GrantID` |  |  |  |  |  | `String(20)` |  | Grant |  |  |
| `BudgetPeriod` |  |  |  |  |  | `String(10)` |  | Budget Period |  |  |
| `EarmarkedFundsDocument` |  |  |  |  |  | `String(10)` |  | Earmarked Funds |  |  |
| `EarmarkedFundsDocumentItem` |  |  |  |  |  | `String(3)` |  | Document Item |  |  |
| `ServiceDocumentType` |  |  |  |  |  | `String(4)` |  | Service Doc. Type |  |  |
| `ServiceDocument` |  |  |  |  |  | `String(10)` |  | Service Document |  |  |
| `ServiceDocumentItem` |  |  |  |  |  | `String(6)` |  | Service Doc. Item |  |  |
| `PurchaseOrderType` |  | `EKKO` | `BSART` |  |  | `String(4)` |  | Purchasing Doc. Type |  |  |
| `PurchasingOrganization` |  | `EKKO` | `EKORG` |  |  | `String(4)` |  | Purch. Organization |  |  |
| `PurchasingGroup` |  | `EKKO` | `EKGRP` |  |  | `String(3)` |  | Purchasing Group |  |  |
| `CreationDate` |  | `EKKO` | `AEDAT` |  |  | `Date` |  | Created On |  |  |
| `LastChangeDateTime` |  |  |  |  |  | `Timestamp` |  | Last Changed |  |  |
| `Plant` |  | `EKPO` | `WERKS` |  |  | `String(4)` |  | Plant |  |  |
| `AccountAssignmentCategory` |  | `EKPO` | `KNTTP` |  |  | `String(1)` |  | Acct Assignment Cat. |  |  |
| `CompanyCode` |  | `EKKO` | `BUKRS` |  |  | `String(4)` |  | Company Code |  |  |
| `IsReturnsItem` |  |  |  |  |  | `Boolean` |  | Returns Item |  |  |
| `SupplyingPlant` |  |  |  |  |  | `String(4)` |  | Supplying Plant |  |  |
| `PurchaseOrderItemCategory` |  |  |  |  |  | `String(1)` |  | Item Category |  |  |
| `Material` |  | `EKPO` | `MATNR` |  |  | `String(40)` |  | Material |  |  |
| `MaterialGroup` |  | `EKPO` | `MATKL` |  |  | `String(9)` |  | Material Group |  |  |
| `PurchaseOrderDate` |  | `EKKO` | `BEDAT` |  |  | `Date` |  | Purchase Order Date |  |  |
| `StorageLocation` |  | `EKPO` | `LGORT` |  |  | `String(4)` |  | Storage Location |  |  |
| `IsCompletelyDelivered` |  |  |  |  |  | `Boolean` |  | Delivery Completed |  |  |
| `PurchasingInfoRecord` |  |  |  |  |  | `String(10)` |  | Purchasing Info Rec. |  |  |
| `RequirementTracking` |  |  |  |  |  | `String(10)` |  | Req. Tracking Number |  |  |
| `PurchaseOrderItemText` |  | `EKPO` | `TXZ01` |  |  | `String(40)` |  | Short Text |  |  |
| `PurgDocumentItemDeletionCode` |  |  |  |  |  | `String(1)` |  | Deletion Indicator |  |  |
| `PurchasingDocumentDeletionCode` |  |  |  |  |  | `String(1)` |  | Deletion Code |  |  |
| `InvoiceIsExpected` |  | `EKPO` | `REPOS` |  |  | `Boolean` |  | Invoice Receipt |  |  |
| `GoodsReceiptIsExpected` |  | `EKPO` | `WEPOS` |  |  | `Boolean` |  | Goods Receipt |  |  |
| `ProductTypeCode` |  |  |  |  |  | `String(2)` |  | Product Type Group |  |  |
| `IsStatisticalItem` |  |  |  |  |  | `Boolean` |  | Statistical |  |  |
| `ReleaseIsNotCompleted` |  |  |  |  |  | `Boolean` |  | Subject to Release |  |  |
| `PurchasingCompletenessStatus` |  |  |  |  |  | `Boolean` |  | Incomplete |  |  |
| `PurchaseContract` |  |  |  |  |  | `String(10)` |  | Outline agreement |  |  |
| `PurchaseContractItem` |  |  |  |  |  | `String(5)` |  | Agreement Item |  |  |


## Entity: `PurchaseOrderItem`

- **ABAP CDS Name:** `C_PurchaseOrderItemDEX`
- **Label:** Data Extraction View for PO Item
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** EKPO

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `PurchaseOrder` |  | `EKKO` | `EBELN` |  |  | `String(10)` | Y | Purchase Order |  |  |
| `PurchaseOrderItem` |  | `EKPO` | `EBELP` |  |  | `String(5)` | Y | Purchase Order Item |  |  |
| `PurchaseOrderType` |  | `EKKO` | `BSART` |  |  | `String(4)` |  | Purchasing Doc. Type |  |  |
| `PurchasingGroup` |  | `EKKO` | `EKGRP` |  |  | `String(3)` |  | Purchasing Group |  |  |
| `PurchasingOrganization` |  | `EKKO` | `EKORG` |  |  | `String(4)` |  | Purch. Organization |  |  |
| `PurchasingDocumentOrigin` |  |  |  |  |  | `String(1)` |  | Status |  |  |
| `Supplier` |  | `EKKO` | `LIFNR` |  |  | `String(10)` |  | Supplier |  |  |
| `SupplyingSupplier` |  |  |  |  |  | `String(10)` |  | Goods Supplier |  |  |
| `SupplyingPlant` |  |  |  |  |  | `String(4)` |  | Supplying Plant |  |  |
| `DocumentCurrency` |  | `EKKO` | `WAERS` |  |  | `String(5)` |  | Currency |  |  |
| `ExchangeRate` |  | `EKKO` | `WKURS` |  |  | `Decimal(9,5)` |  | Exchange Rate |  |  |
| `InvoicingParty` |  |  |  |  |  | `String(10)` |  | Invoicing Party |  |  |
| `PurchaseOrderDate` |  | `EKKO` | `BEDAT` |  |  | `Date` |  | Purchase Order Date |  |  |
| `ValidityStartDate` |  |  |  |  |  | `Date` |  | Validity Per. Start |  |  |
| `ValidityEndDate` |  |  |  |  |  | `Date` |  | Validity Period End |  |  |
| `CreationDate` |  | `EKKO` | `AEDAT` |  |  | `Date` |  | Created On |  |  |
| `LastChangeDateTime` |  |  |  |  |  | `Timestamp` |  | Last Changed |  |  |
| `PurgDocumentItemDeletionCode` |  |  |  |  |  | `String(1)` |  | Deletion Indicator |  |  |
| `MaterialGroup` |  | `EKPO` | `MATKL` |  |  | `String(9)` |  | Material Group |  |  |
| `Material` |  | `EKPO` | `MATNR` |  |  | `String(40)` |  | Material |  |  |
| `ManufacturerMaterial` |  |  |  |  |  | `String(40)` |  | Material |  |  |
| `PurchaseOrderCategory` |  |  |  |  |  | `String(1)` |  | Purch. Doc. Category |  |  |
| `PurchasingOrderReason` |  |  |  |  |  | `String(3)` |  | Reason for Ordering |  |  |
| `PurchaseOrderItemText` |  | `EKPO` | `TXZ01` |  |  | `String(40)` |  | Short Text |  |  |
| `PurchaseOrderItemCategory` |  |  |  |  |  | `String(1)` |  | Item Category |  |  |
| `CompanyCode` |  | `EKKO` | `BUKRS` |  |  | `String(4)` |  | Company Code |  |  |
| `Plant` |  | `EKPO` | `WERKS` |  |  | `String(4)` |  | Plant |  |  |
| `StorageLocation` |  | `EKPO` | `LGORT` |  |  | `String(4)` |  | Storage Location |  |  |
| `PurchaseContract` |  |  |  |  |  | `String(10)` |  | Outline agreement |  |  |
| `PurchaseContractItem` |  |  |  |  |  | `String(5)` |  | Agreement Item |  |  |
| `BaseUnit` |  |  |  |  |  | `String(3)` |  | Base Unit of Measure |  |  |
| `OrderQuantity` |  | `EKPO` | `MENGE` |  |  | `Decimal(13,3)` |  | Order Quantity | PurchaseOrderQuantityUnit |  |
| `PurchaseOrderQuantityUnit` |  | `EKPO` | `MEINS` |  |  | `String(3)` |  | Order Unit |  |  |
| `NetPriceAmount` |  | `EKPO` | `NETWR` |  |  | `Decimal(34,4)` |  | Net Order Price | DocumentCurrency |  |
| `NetAmount` |  |  |  |  |  | `Decimal(34,4)` |  | Net Order Value | DocumentCurrency |  |
| `LocalCurrency` |  |  |  |  |  | `String(5)` |  | Currency |  |  |
| `NetPriceQuantity` |  |  |  |  |  | `Decimal(5,0)` |  | Price Unit | OrderPriceUnit |  |
| `OrderPriceUnit` |  |  |  |  |  | `String(3)` |  | Order Price Unit |  |  |
| `RequisitionerName` |  |  |  |  |  | `String(12)` |  | Requisitioner |  |  |
| `RetailPromotion` |  |  |  |  |  | `String(10)` |  | Retail Promotion |  |  |
| `IsCompletelyDelivered` |  |  |  |  |  | `Boolean` |  | Delivery Completed |  |  |
| `IsReturnsItem` |  |  |  |  |  | `Boolean` |  | Returns Item |  |  |
| `IsFinallyInvoiced` |  |  |  |  |  | `Boolean` |  | Final Invoice |  |  |
| `InvoiceIsExpected` |  | `EKPO` | `REPOS` |  |  | `Boolean` |  | Invoice Receipt |  |  |
| `OrderItemQtyToBaseQtyDnmntr` |  |  |  |  |  | `Decimal(5,0)` |  | Denominator |  |  |
| `OrderItemQtyToBaseQtyNmrtr` |  |  |  |  |  | `Decimal(5,0)` |  | Numerator |  |  |
| `InvoiceIsGoodsReceiptBased` |  |  |  |  |  | `Boolean` |  | GR-Based Inv. Verif. |  |  |
| `GoodsReceiptIsExpected` |  | `EKPO` | `WEPOS` |  |  | `Boolean` |  | Goods Receipt |  |  |
| `EvaldRcptSettlmtIsAllowed` |  |  |  |  |  | `Boolean` |  | Eval. Receipt Sett. |  |  |
| `AccountAssignmentCategory` |  | `EKPO` | `KNTTP` |  |  | `String(1)` |  | Acct Assignment Cat. |  |  |
| `GoodsReceiptIsNonValuated` |  |  |  |  |  | `Boolean` |  | GR Non-Valuated |  |  |
| `MaterialType` |  |  |  |  |  | `String(4)` |  | Material Type |  |  |
| `OverdelivTolrtdLmtRatioInPct` |  |  |  |  |  | `Decimal(3,1)` |  | Overdeliv. Tolerance |  |  |
| `ServicePerformer` |  |  |  |  |  | `String(10)` |  | Service Performer |  |  |
| `TaxCode` |  |  |  |  |  | `String(2)` |  | Tax Code |  |  |
| `UnderdelivTolrtdLmtRatioInPct` |  |  |  |  |  | `Decimal(3,1)` |  | Underdel. Tolerance |  |  |
| `UnlimitedOverdeliveryIsAllowed` |  |  |  |  |  | `Boolean` |  | Unltd Overdelivery |  |  |
| `SupplierMaterialNumber` |  |  |  |  |  | `String(35)` |  | Supplier Mat. No. |  |  |
| `ProductTypeCode` |  |  |  |  |  | `String(2)` |  | Product Type Group |  |  |
| `CreatedByUser` |  | `EKKO` | `ERNAM` |  |  | `String(12)` |  | Created By |  |  |
| `ExpectedOverallLimitAmount` |  |  |  |  |  | `Decimal(34,4)` |  | Expected Value | DocumentCurrency |  |
| `OverallLimitAmount` |  |  |  |  |  | `Decimal(34,4)` |  | Overall Limit | DocumentCurrency |  |
| `RequirementSegment` |  |  |  |  |  | `String(40)` |  | Requirement Segment |  |  |
| `ReleaseIsNotCompleted` |  |  |  |  |  | `Boolean` |  | Subject to Release |  |  |
| `PurchasingCompletenessStatus` |  |  |  |  |  | `Boolean` |  | Incomplete |  |  |
| `IsStatisticalItem` |  |  |  |  |  | `Boolean` |  | Statistical |  |  |
| `MultipleAcctAssgmtDistribution` |  |  |  |  |  | `String(1)` |  | Distribut. Indicator |  |  |
| `PurchaseRequisition` |  |  |  |  |  | `String(10)` |  | Purchase Requisition |  |  |
| `PurchaseRequisitionItem` |  |  |  |  |  | `String(5)` |  | Item of requisition |  |  |
| `SupplierConfirmationControlKey` |  |  |  |  |  | `String(4)` |  | Confirmation Control |  |  |
| `PurchasingDocumentDeletionCode` |  |  |  |  |  | `String(1)` |  | Deletion Code |  |  |


## Entity: `PurchaseOrderScheduleLine`

- **ABAP CDS Name:** `C_PurOrdScheduleLineDEX`
- **Label:** Data Extraction for Purchase Order Schedule Lines
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** EKET

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `PurchaseOrder` |  |  |  |  |  | `String(10)` | Y | Purchasing Document |  |  |
| `PurchaseOrderItem` |  |  |  |  |  | `String(5)` | Y | Item |  |  |
| `PurchaseOrderScheduleLine` |  |  |  |  |  | `String(4)` | Y | Schedule Line |  |  |
| `ScheduleLineDeliveryDate` |  |  |  |  |  | `Date` |  | Delivery Date |  |  |
| `SchedLineStscDeliveryDate` |  |  |  |  |  | `Date` |  | Stat.-Rel. Del. Date |  |  |
| `ScheduleLineDeliveryTime` |  |  |  |  |  | `String(6)` |  | Time |  |  |
| `PurchaseRequisition` |  |  |  |  |  | `String(10)` |  | Purchase Requisition |  |  |
| `PurchaseRequisitionItem` |  |  |  |  |  | `String(5)` |  | Item of requisition |  |  |
| `Batch` |  |  |  |  |  | `String(10)` |  | Batch |  |  |
| `PurchasingSchdLnNrOfReminders` |  |  |  |  |  | `Decimal(3,0)` |  | No. Rem./Expediters |  |  |
| `RequisitionerName` |  |  |  |  |  | `String(12)` |  | Requisitioner |  |  |
| `RetailPromotion` |  |  |  |  |  | `String(10)` |  | Retail Promotion |  |  |
| `ArticleCategory` |  |  |  |  |  | `String(2)` |  | Material Category |  |  |
| `PurchasingOrderReason` |  |  |  |  |  | `String(3)` |  | Reason for Ordering |  |  |
| `IsCompletelyDelivered` |  |  |  |  |  | `Boolean` |  | Delivery Completed |  |  |
| `ManufacturerMaterial` |  |  |  |  |  | `String(40)` |  | Material |  |  |
| `IsFinallyInvoiced` |  |  |  |  |  | `Boolean` |  | Final Invoice |  |  |
| `PurchaseContract` |  |  |  |  |  | `String(10)` |  | Outline agreement |  |  |
| `PurchaseContractItem` |  |  |  |  |  | `String(5)` |  | Agreement Item |  |  |
| `StorageLocation` |  |  |  |  |  | `String(4)` |  | Storage Location |  |  |
| `BaseUnit` |  |  |  |  |  | `String(3)` |  | Base Unit of Measure |  |  |
| `MaterialGroup` |  |  |  |  |  | `String(9)` |  | Material Group |  |  |
| `Material` |  |  |  |  |  | `String(40)` |  | Material |  |  |
| `PurchaseOrderQuantityUnit` |  |  |  |  |  | `String(3)` |  | Order Unit |  |  |
| `PurchaseOrderItemCategory` |  |  |  |  |  | `String(1)` |  | Item Category |  |  |
| `IssuingStorageLocation` |  |  |  |  |  | `String(4)` |  | Issuing Storage Loc. |  |  |
| `PurchaseOrderItemText` |  |  |  |  |  | `String(40)` |  | Short Text |  |  |
| `PurchasingParentItem` |  |  |  |  |  | `String(5)` |  | Higher-Level Item |  |  |
| `OrderItemQtyToBaseQtyDnmntr` |  |  |  |  |  | `Decimal(5,0)` |  | Denominator |  |  |
| `OrderItemQtyToBaseQtyNmrtr` |  |  |  |  |  | `Decimal(5,0)` |  | Numerator |  |  |
| `InvoiceIsGoodsReceiptBased` |  |  |  |  |  | `Boolean` |  | GR-Based Inv. Verif. |  |  |
| `GoodsReceiptIsExpected` |  |  |  |  |  | `Boolean` |  | Goods Receipt |  |  |
| `Plant` |  |  |  |  |  | `String(4)` |  | Plant |  |  |
| `EvaldRcptSettlmtIsAllowed` |  |  |  |  |  | `Boolean` |  | Eval. Receipt Sett. |  |  |
| `PurchaseOrderDate` |  |  |  |  |  | `Date` |  | Purchase Order Date |  |  |
| `PurchaseOrderType` |  |  |  |  |  | `String(4)` |  | Purchasing Doc. Type |  |  |
| `PurchasingGroup` |  |  |  |  |  | `String(3)` |  | Purchasing Group |  |  |
| `PurchasingOrganization` |  |  |  |  |  | `String(4)` |  | Purch. Organization |  |  |
| `ValidityStartDate` |  |  |  |  |  | `Date` |  | Validity Per. Start |  |  |
| `ValidityEndDate` |  |  |  |  |  | `Date` |  | Validity Period End |  |  |
| `Supplier` |  |  |  |  |  | `String(10)` |  | Supplier |  |  |
| `InvoicingParty` |  |  |  |  |  | `String(10)` |  | Invoicing Party |  |  |
| `SupplyingSupplier` |  |  |  |  |  | `String(10)` |  | Goods Supplier |  |  |
| `SupplyingPlant` |  |  |  |  |  | `String(4)` |  | Supplying Plant |  |  |
| `PurchasingDocumentOrigin` |  |  |  |  |  | `String(1)` |  | Status |  |  |
| `DocumentCurrency` |  |  |  |  |  | `String(5)` |  | Currency |  |  |
| `ExchangeRate` |  |  |  |  |  | `Decimal(9,5)` |  | Exchange Rate |  |  |
| `DelivDateCategory` |  |  |  |  |  | `String(1)` |  | Deliv. date category |  |  |
| `ScheduleLineOrderQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Scheduled Quantity | PurchaseOrderQuantityUnit |  |
| `PrevDelivQtyOfScheduleLine` |  |  |  |  |  | `Decimal(13,3)` |  | Previous Quantity | PurchaseOrderQuantityUnit |  |
| `RoughGoodsReceiptQty` |  |  |  |  |  | `Decimal(13,3)` |  | Quantity Delivered | PurchaseOrderQuantityUnit |  |
| `ScheduleLineIssuedQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Issued Quantity | PurchaseOrderQuantityUnit |  |
| `SourceOfCreation` |  |  |  |  |  | `String(1)` |  | Creation indicator |  |  |
| `Reservation` |  |  |  |  |  | `String(10)` |  | Reservation |  |  |
| `ScheduleLineIsFixed` |  |  |  |  |  | `Boolean` |  | Fixing Indicator |  |  |
| `StockTransferDeliveredQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Qty Delivered | PurchaseOrderQuantityUnit |  |
| `ScheduleLineCommittedQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Committed Quantity | PurchaseOrderQuantityUnit |  |
| `ProductAvailabilityDate` |  |  |  |  |  | `Date` |  | Material Avail. Date |  |  |
| `ProductAvailabilityTime` |  |  |  |  |  | `String(6)` |  | Matl Staging Time |  |  |
| `LoadingDate` |  |  |  |  |  | `Date` |  | Loading Date |  |  |
| `LoadingTime` |  |  |  |  |  | `String(6)` |  | Loading Time |  |  |
| `TransportationPlanningDate` |  |  |  |  |  | `Date` |  | Transptn Plang Date |  |  |
| `TransportationPlanningTime` |  |  |  |  |  | `String(6)` |  | Transp. Plan. Time |  |  |
| `GoodsIssueDate` |  |  |  |  |  | `Date` |  | Goods Issue Date |  |  |
| `GoodsIssueTime` |  |  |  |  |  | `String(6)` |  | Goods Issue Time |  |  |
| `STOLatestPossibleGRDate` |  |  |  |  |  | `Date` |  | GR End Date |  |  |
| `STOLatestPossibleGRTime` |  |  |  |  |  | `String(6)` |  | GR End Time |  |  |
| `OpenPurchaseOrderNetAmount` |  |  |  |  |  | `Decimal(34,4)` |  |  | DocumentCurrency |  |
| `IsReturnsItem` |  |  |  |  |  | `Boolean` |  | Returns Item |  |  |
| `CompanyCode` |  |  |  |  |  | `String(4)` |  | Company Code |  |  |
| `ProductTypeCode` |  |  |  |  |  | `String(2)` |  | Product Type Group |  |  |
| `PurchasingDocumentDeletionCode` |  |  |  |  |  | `String(1)` |  | Deletion Code |  |  |
| `PurgDocumentItemDeletionCode` |  |  |  |  |  | `String(1)` |  | Deletion Indicator |  |  |
| `ReleaseIsNotCompleted` |  |  |  |  |  | `Boolean` |  | Subject to Release |  |  |
| `PurchasingCompletenessStatus` |  |  |  |  |  | `Boolean` |  | Incomplete |  |  |
| `SupplierConfirmationControlKey` |  |  |  |  |  | `String(4)` |  | Confirmation Control |  |  |
| `IsStatisticalItem` |  |  |  |  |  | `Boolean` |  | Statistical |  |  |
| `ScheduleLineOpenQuantity` |  |  |  |  |  | `Decimal(14,3)` |  |  | PurchaseOrderQuantityUnit |  |
