# PurchaseOrder

> Source file: `sap-s4com-PurchaseOrder-v1.json`


## Entity: `PurOrdSupplierConfirmation`

- **ABAP CDS Name:** `C_POSupplierConfirmationDEX`
- **Label:** Purchase Order Supplier Confirmation DEX
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `PurchaseOrder` |  |  |  |  |  | `String(10)` | Y | Purchase Order |  | S/4 only entity |
| `PurchaseOrderItem` |  |  |  |  |  | `String(5)` | Y | Purchase Order Item |  | S/4 only entity |
| `SequentialNmbrOfSuplrConf` |  |  |  |  |  | `String(4)` | Y | Sequential Number |  | S/4 only entity |
| `SupplierConfirmationCategory` |  |  |  |  |  | `String(2)` |  | Confirm. Category |  | S/4 only entity |
| `DeliveryDate` |  |  |  |  |  | `Date` |  | Delivery Date |  | S/4 only entity |
| `DelivDateCategory` |  |  |  |  |  | `String(1)` |  | Deliv. Date Category |  | S/4 only entity |
| `DeliveryTime` |  |  |  |  |  | `String(6)` |  | Time |  | S/4 only entity |
| `CreationDate` |  |  |  |  |  | `Date` |  | Creation Date |  | S/4 only entity |
| `CreationTime` |  |  |  |  |  | `String(6)` |  | Creation Time |  | S/4 only entity |
| `ConfirmedQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Quantity | OrderQuantityUnit | S/4 only entity |
| `MRPRelevantQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Qty Reduced (MRP) | OrderQuantityUnit | S/4 only entity |
| `SuplrConfCreationCategory` |  |  |  |  |  | `String(1)` |  | Creation Indicator |  | S/4 only entity |
| `IsDeleted` |  |  |  |  |  | `String(1)` |  | Deletion Indicator |  | S/4 only entity |
| `ConfIsRelevantToMRP` |  |  |  |  |  | `Boolean` |  | MRP-Relevant |  | S/4 only entity |
| `SupplierConfirmationExtNumber` |  |  |  |  |  | `String(35)` |  | Reference |  | S/4 only entity |
| `DeliveryDocument` |  |  |  |  |  | `String(10)` |  | Delivery |  | S/4 only entity |
| `DeliveryDocumentItem` |  |  |  |  |  | `String(6)` |  | Item |  | S/4 only entity |
| `ManufacturerPartProfile` |  |  |  |  |  | `String(4)` |  | Mfr Part Profile |  | S/4 only entity |
| `ManufacturerMaterial` |  |  |  |  |  | `String(40)` |  | MPN: Material |  | S/4 only entity |
| `NumberOfReminders` |  |  |  |  |  | `Decimal(3,0)` |  | No. Rem./Expediters |  | S/4 only entity |
| `Batch` |  |  |  |  |  | `String(10)` |  | Batch |  | S/4 only entity |
| `DeliveryIsInPlant` |  |  |  |  |  | `Boolean` |  | In Plant |  | S/4 only entity |
| `HandoverDate` |  |  |  |  |  | `Date` |  | Handover Date |  | S/4 only entity |
| `HandoverTime` |  |  |  |  |  | `String(6)` |  | Handover Time |  | S/4 only entity |
| `PerformancePeriodStartDate` |  |  |  |  |  | `Date` |  | Start Date |  | S/4 only entity |
| `PerformancePeriodEndDate` |  |  |  |  |  | `Date` |  | End Date |  | S/4 only entity |
| `ServicePerformer` |  |  |  |  |  | `String(10)` |  | Service Performer |  | S/4 only entity |
| `OrderQuantityUnit` |  |  |  |  |  | `String(3)` |  | Order Unit |  | S/4 only entity |
| `SupplierConfirmation` |  |  |  |  |  | `String(10)` |  | Confirmation |  | S/4 only entity |
| `SupplierConfirmationItem` |  |  |  |  |  | `String(5)` |  | Confirmation Item |  | S/4 only entity |
| `PurchaseOrderType` |  |  |  |  |  | `String(4)` |  | Purchasing Doc. Type |  | S/4 only entity |
| `PurchasingOrganization` |  |  |  |  |  | `String(4)` |  | Purch. Organization |  | S/4 only entity |
| `PurchasingGroup` |  |  |  |  |  | `String(3)` |  | Purchasing Group |  | S/4 only entity |
| `Plant` |  |  |  |  |  | `String(4)` |  | Plant |  | S/4 only entity |


## Entity: `PurchaseOrder`

- **ABAP CDS Name:** `C_PurchaseOrderDEX`
- **Label:** Data Extraction for Purchase Order
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `PurchaseOrder` |  | `EKKO` | `EBELN` |  |  | `String(10)` | Y | Purchase Order |  |  |
| `PurchaseOrderType` |  | `EKKO` | `BSART` |  |  | `String(4)` |  | Purchasing Doc. Type |  |  |
| `PurchaseOrderSubtype` |  |  |  |  |  | `String(1)` |  | Control indicator |  | S/4 only entity |
| `PurchasingDocumentOrigin` |  |  |  |  |  | `String(1)` |  | Status |  | S/4 only entity |
| `CreatedByUser` |  | `EKKO` | `ERNAM` |  |  | `String(12)` |  | Created By |  |  |
| `CreationDate` |  | `EKKO` | `AEDAT` |  |  | `Date` |  | Created On |  |  |
| `PurchaseOrderDate` |  | `EKKO` | `BEDAT` |  |  | `Date` |  | Purchase Order Date |  |  |
| `Language` |  | `EKKO` | `SPRAS` |  |  | `String(2)` |  | Language Key |  |  |
| `CorrespncExternalReference` |  |  |  |  |  | `String(12)` |  | Your Reference |  | S/4 only entity |
| `CorrespncInternalReference` |  |  |  |  |  | `String(12)` |  | Our Reference |  | S/4 only entity |
| `PurchasingDocumentDeletionCode` |  |  |  |  |  | `String(1)` |  | Deletion Code |  | S/4 only entity |
| `ReleaseIsNotCompleted` |  |  |  |  |  | `Boolean` |  | Subject to Release |  | S/4 only entity |
| `PurchasingCompletenessStatus` |  |  |  |  |  | `Boolean` |  | Incomplete |  | S/4 only entity |
| `PurchasingProcessingStatus` |  |  |  |  |  | `String(2)` |  | Proc. State |  | S/4 only entity |
| `PurgReleaseSequenceStatus` |  |  |  |  |  | `String(8)` |  | Release Status |  | S/4 only entity |
| `ReleaseCode` |  |  |  |  |  | `String(1)` |  | Release indicator |  | S/4 only entity |
| `CompanyCode` |  | `EKKO` | `BUKRS` |  |  | `String(4)` |  | Company Code |  |  |
| `PurchasingOrganization` |  | `EKKO` | `EKORG` |  |  | `String(4)` |  | Purch. Organization |  |  |
| `PurchasingGroup` |  | `EKKO` | `EKGRP` |  |  | `String(3)` |  | Purchasing Group |  |  |
| `Supplier` |  | `EKKO` | `LIFNR` |  |  | `String(10)` |  | Supplier |  |  |
| `ManualSupplierAddressID` |  |  |  |  |  | `String(10)` |  | Address Number |  | S/4 only entity |
| `SupplierRespSalesPersonName` |  |  |  |  |  | `String(30)` |  | Salesperson |  | S/4 only entity |
| `SupplierPhoneNumber` |  |  |  |  |  | `String(16)` |  | Supplier Phone |  | S/4 only entity |
| `SupplyingSupplier` |  |  |  |  |  | `String(10)` |  | Goods Supplier |  | S/4 only entity |
| `SupplyingPlant` |  |  |  |  |  | `String(4)` |  | Supplying Plant |  | S/4 only entity |
| `InvoicingParty` |  |  |  |  |  | `String(10)` |  | Invoicing Party |  | S/4 only entity |
| `Customer` |  |  |  |  |  | `String(10)` |  | Customer |  | S/4 only entity |
| `SupplierQuotationExternalID` |  |  |  |  |  | `String(10)` |  | Quotation |  | S/4 only entity |
| `PaymentTerms` |  |  |  |  |  | `String(4)` |  | Payment Terms |  | S/4 only entity |
| `CashDiscount1Days` |  |  |  |  |  | `Decimal(3,0)` |  | Days 1 |  | S/4 only entity |
| `CashDiscount2Days` |  |  |  |  |  | `Decimal(3,0)` |  | Days 2 |  | S/4 only entity |
| `NetPaymentDays` |  |  |  |  |  | `Decimal(3,0)` |  | Days Net |  | S/4 only entity |
| `CashDiscount1Percent` |  |  |  |  |  | `Decimal(5,3)` |  | CD Percentage 1 |  | S/4 only entity |
| `CashDiscount2Percent` |  |  |  |  |  | `Decimal(5,3)` |  | CD Percentage 2 |  | S/4 only entity |
| `DownPaymentType` |  |  |  |  |  | `String(4)` |  | Down Payment |  | S/4 only entity |
| `DownPaymentPercentageOfTotAmt` |  |  |  |  |  | `Decimal(5,2)` |  | Down Payment % |  | S/4 only entity |
| `DownPaymentAmount` |  |  |  |  |  | `Decimal(34,4)` |  | Down Payment Amount | DocumentCurrency | S/4 only entity |
| `DownPaymentDueDate` |  |  |  |  |  | `Date` |  | Due Date for DP |  | S/4 only entity |
| `IncotermsClassification` |  |  |  |  |  | `String(3)` |  | Incoterms |  | S/4 only entity |
| `IncotermsTransferLocation` |  |  |  |  |  | `String(28)` |  | Incoterms (Part 2) |  | S/4 only entity |
| `IncotermsVersion` |  |  |  |  |  | `String(4)` |  | Incoterms Version |  | S/4 only entity |
| `IncotermsLocation1` |  |  |  |  |  | `String(70)` |  | Incoterms Location 1 |  | S/4 only entity |
| `IncotermsLocation2` |  |  |  |  |  | `String(70)` |  | Incoterms Location 2 |  | S/4 only entity |
| `IsIntrastatReportingRelevant` |  |  |  |  |  | `Boolean` |  | Intrastat Relevance |  | S/4 only entity |
| `IsIntrastatReportingExcluded` |  |  |  |  |  | `Boolean` |  | Intrastat Exclusion |  | S/4 only entity |
| `PricingDocument` |  |  |  |  |  | `String(10)` |  | Doc. Condition No. |  | S/4 only entity |
| `PricingProcedure` |  |  |  |  |  | `String(6)` |  | Procedure |  | S/4 only entity |
| `DocumentCurrency` |  | `EKKO` | `WAERS` |  |  | `String(5)` |  | Currency |  |  |
| `ValidityStartDate` |  |  |  |  |  | `Date` |  | Validity Per. Start |  | S/4 only entity |
| `ValidityEndDate` |  |  |  |  |  | `Date` |  | Validity Period End |  | S/4 only entity |
| `ExchangeRate` |  | `EKKO` | `WKURS` |  |  | `Decimal(9,5)` |  | Exchange Rate |  |  |
| `ExchangeRateIsFixed` |  |  |  |  |  | `Boolean` |  | Fixed Exchange Rate |  | S/4 only entity |
| `LastChangeDateTime` |  |  |  |  |  | `Timestamp` |  | Last Changed |  | S/4 only entity |
| `TaxReturnCountry` |  |  |  |  |  | `String(3)` |  | Reporting C/R |  | S/4 only entity |
| `VATRegistrationCountry` |  |  |  |  |  | `String(3)` |  | Ctry/Rgn Sls Tax No. |  | S/4 only entity |
| `PurgReasonForDocCancellation` |  |  |  |  |  | `String(2)` |  | Reason for Canc. |  | S/4 only entity |
| `PurgReleaseTimeTotalAmount` |  |  |  |  |  | `Decimal(34,4)` |  | Tot. val. rel. | DocumentCurrency | S/4 only entity |


## Entity: `PurchaseOrderAccountAssignment`

- **ABAP CDS Name:** `C_PurOrdAccountAssignmentDEX`
- **Label:** Data Extraction for Purchase Order Account Assignments
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `PurchaseOrder` |  | `EKKO` | `EBELN` |  |  | `String(10)` | Y | Purchasing Document |  |  |
| `PurchaseOrderItem` |  | `EKPO` | `EBELP` |  |  | `String(5)` | Y | Item |  |  |
| `AccountAssignmentNumber` |  | `EKKN` | `ZEKKN` |  |  | `String(2)` | Y | Account Assgmt No. |  |  |
| `CostCenter` |  | `EKKN` | `KOSTL` |  |  | `String(10)` |  | Cost Center |  |  |
| `MasterFixedAsset` |  |  |  |  |  | `String(12)` |  | Asset |  | S/4 only entity |
| `ProjectNetwork` |  |  |  |  |  | `String(12)` |  | Network |  | S/4 only entity |
| `Quantity` |  |  |  |  |  | `Decimal(13,3)` |  | Quantity | PurchaseOrderQuantityUnit | S/4 only entity |
| `PurchaseOrderQuantityUnit` |  | `EKPO` | `MEINS` |  |  | `String(3)` |  | Order Unit |  |  |
| `MultipleAcctAssgmtDistrPercent` |  |  |  |  |  | `Decimal(3,1)` |  | Distribution (%) |  | S/4 only entity |
| `PurgDocNetAmount` |  |  |  |  |  | `Decimal(34,4)` |  | Net Order Value | DocumentCurrency | S/4 only entity |
| `DocumentCurrency` |  | `EKKO` | `WAERS` |  |  | `String(5)` |  | Currency |  |  |
| `IsDeleted` |  |  |  |  |  | `Boolean` |  | Deletion Indicator |  | S/4 only entity |
| `GLAccount` |  | `EKKN` | `SAKTO` |  |  | `String(10)` |  | G/L Account |  |  |
| `BusinessArea` |  |  |  |  |  | `String(4)` |  | Business Area |  | S/4 only entity |
| `SalesOrder` |  |  |  |  |  | `String(10)` |  | SD Document |  | S/4 only entity |
| `SalesOrderItem` |  |  |  |  |  | `String(6)` |  | Item |  | S/4 only entity |
| `SalesOrderScheduleLine` |  |  |  |  |  | `String(4)` |  | Schedule Line Number |  | S/4 only entity |
| `FixedAsset` |  |  |  |  |  | `String(4)` |  | Subnumber |  | S/4 only entity |
| `OrderID` |  |  |  |  |  | `String(12)` |  | Order |  | S/4 only entity |
| `UnloadingPointName` |  |  |  |  |  | `String(25)` |  | Unloading Point |  | S/4 only entity |
| `ControllingArea` |  | `EKKN` | `KOKRS` |  |  | `String(4)` |  | Controlling Area |  |  |
| `CostObject` |  |  |  |  |  | `String(12)` |  | Cost Object |  | S/4 only entity |
| `ProfitabilitySegment` |  |  |  |  |  | `String(10)` |  | Profitability Segment (Deprecated) |  | S/4 only entity |
| `ProfitabilitySegment_2` |  |  |  |  |  | `String(10)` |  | Profitability Segment |  | S/4 only entity |
| `ProfitCenter` |  | `EKKN` | `PRCTR` |  |  | `String(10)` |  | Profit Center |  |  |
| `WBSElementInternalID` |  |  |  |  |  | `String(8)` |  | WBS Internal ID |  | S/4 only entity |
| `ProjectNetworkInternalID` |  |  |  |  |  | `String(10)` |  | Opertn Task List No. |  | S/4 only entity |
| `CommitmentItem` |  |  |  |  |  | `String(24)` |  |  |  | S/4 only entity |
| `FundsCenter` |  |  |  |  |  | `String(16)` |  | Funds Center |  | S/4 only entity |
| `Fund` |  |  |  |  |  | `String(10)` |  | Fund |  | S/4 only entity |
| `FunctionalArea` |  | `EKKN` | `FKBER` |  |  | `String(16)` |  | Functional Area |  |  |
| `GoodsRecipientName` |  |  |  |  |  | `String(12)` |  | Goods Recipient |  | S/4 only entity |
| `IsFinallyInvoiced` |  |  |  |  |  | `Boolean` |  | Final Invoice |  | S/4 only entity |
| `RealEstateObject` |  |  |  |  |  | `String(8)` |  | Real Estate Key |  | S/4 only entity |
| `NetworkActivityInternalID` |  |  |  |  |  | `String(8)` |  | Counter |  | S/4 only entity |
| `PartnerAccountNumber` |  |  |  |  |  | `String(10)` |  | Partner |  | S/4 only entity |
| `JointVentureRecoveryCode` |  |  |  |  |  | `String(2)` |  | Recovery Indicator |  | S/4 only entity |
| `SettlementReferenceDate` |  |  |  |  |  | `Date` |  | Reference Date |  | S/4 only entity |
| `OrderInternalID` |  |  |  |  |  | `String(10)` |  | Opertn Task List No. |  | S/4 only entity |
| `OrderIntBillOfOperationsItem` |  |  |  |  |  | `String(8)` |  | Counter |  | S/4 only entity |
| `TaxCode` |  |  |  |  |  | `String(2)` |  | Tax Code |  | S/4 only entity |
| `TaxJurisdiction` |  |  |  |  |  | `String(15)` |  | Tax Jurisdiction |  | S/4 only entity |
| `NonDeductibleInputTaxAmount` |  |  |  |  |  | `Decimal(34,4)` |  | Non-deductible | DocumentCurrency | S/4 only entity |
| `CostCtrActivityType` |  |  |  |  |  | `String(6)` |  | Activity Type |  | S/4 only entity |
| `BusinessProcess` |  |  |  |  |  | `String(12)` |  | Business Process |  | S/4 only entity |
| `GrantID` |  |  |  |  |  | `String(20)` |  | Grant |  | S/4 only entity |
| `BudgetPeriod` |  |  |  |  |  | `String(10)` |  | Budget Period |  | S/4 only entity |
| `EarmarkedFundsDocument` |  |  |  |  |  | `String(10)` |  | Earmarked Funds |  | S/4 only entity |
| `EarmarkedFundsDocumentItem` |  |  |  |  |  | `String(3)` |  | Document Item |  | S/4 only entity |
| `ServiceDocumentType` |  |  |  |  |  | `String(4)` |  | Service Doc. Type |  | S/4 only entity |
| `ServiceDocument` |  |  |  |  |  | `String(10)` |  | Service Document |  | S/4 only entity |
| `ServiceDocumentItem` |  |  |  |  |  | `String(6)` |  | Service Doc. Item |  | S/4 only entity |
| `PurchaseOrderType` |  | `EKKO` | `BSART` |  |  | `String(4)` |  | Purchasing Doc. Type |  |  |
| `PurchasingOrganization` |  | `EKKO` | `EKORG` |  |  | `String(4)` |  | Purch. Organization |  |  |
| `PurchasingGroup` |  | `EKKO` | `EKGRP` |  |  | `String(3)` |  | Purchasing Group |  |  |
| `CreationDate` |  | `EKKO` | `AEDAT` |  |  | `Date` |  | Created On |  |  |
| `LastChangeDateTime` |  |  |  |  |  | `Timestamp` |  | Last Changed |  | S/4 only entity |
| `Plant` |  | `EKPO` | `WERKS` |  |  | `String(4)` |  | Plant |  |  |
| `AccountAssignmentCategory` |  | `EKPO` | `KNTTP` |  |  | `String(1)` |  | Acct Assignment Cat. |  |  |
| `CompanyCode` |  | `EKKO` | `BUKRS` |  |  | `String(4)` |  | Company Code |  |  |
| `IsReturnsItem` |  |  |  |  |  | `Boolean` |  | Returns Item |  | S/4 only entity |
| `SupplyingPlant` |  |  |  |  |  | `String(4)` |  | Supplying Plant |  | S/4 only entity |
| `PurchaseOrderItemCategory` |  |  |  |  |  | `String(1)` |  | Item Category |  | S/4 only entity |
| `Material` |  | `EKPO` | `MATNR` |  |  | `String(40)` |  | Material |  |  |
| `MaterialGroup` |  | `EKPO` | `MATKL` |  |  | `String(9)` |  | Material Group |  |  |
| `PurchaseOrderDate` |  | `EKKO` | `BEDAT` |  |  | `Date` |  | Purchase Order Date |  |  |
| `StorageLocation` |  | `EKPO` | `LGORT` |  |  | `String(4)` |  | Storage Location |  |  |
| `IsCompletelyDelivered` |  |  |  |  |  | `Boolean` |  | Delivery Completed |  | S/4 only entity |
| `PurchasingInfoRecord` |  |  |  |  |  | `String(10)` |  | Purchasing Info Rec. |  | S/4 only entity |
| `RequirementTracking` |  |  |  |  |  | `String(10)` |  | Req. Tracking Number |  | S/4 only entity |
| `PurchaseOrderItemText` |  | `EKPO` | `TXZ01` |  |  | `String(40)` |  | Short Text |  |  |
| `PurgDocumentItemDeletionCode` |  |  |  |  |  | `String(1)` |  | Deletion Indicator |  | S/4 only entity |
| `PurchasingDocumentDeletionCode` |  |  |  |  |  | `String(1)` |  | Deletion Code |  | S/4 only entity |
| `InvoiceIsExpected` |  | `EKPO` | `REPOS` |  |  | `Boolean` |  | Invoice Receipt |  |  |
| `GoodsReceiptIsExpected` |  | `EKPO` | `WEPOS` |  |  | `Boolean` |  | Goods Receipt |  |  |
| `ProductTypeCode` |  |  |  |  |  | `String(2)` |  | Product Type Group |  | S/4 only entity |
| `IsStatisticalItem` |  |  |  |  |  | `Boolean` |  | Statistical |  | S/4 only entity |
| `ReleaseIsNotCompleted` |  |  |  |  |  | `Boolean` |  | Subject to Release |  | S/4 only entity |
| `PurchasingCompletenessStatus` |  |  |  |  |  | `Boolean` |  | Incomplete |  | S/4 only entity |
| `PurchaseContract` |  |  |  |  |  | `String(10)` |  | Outline agreement |  | S/4 only entity |
| `PurchaseContractItem` |  |  |  |  |  | `String(5)` |  | Agreement Item |  | S/4 only entity |


## Entity: `PurchaseOrderItem`

- **ABAP CDS Name:** `C_PurchaseOrderItemDEX`
- **Label:** Data Extraction View for PO Item
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `PurchaseOrder` |  | `EKKO` | `EBELN` |  |  | `String(10)` | Y | Purchase Order |  |  |
| `PurchaseOrderItem` |  | `EKPO` | `EBELP` |  |  | `String(5)` | Y | Purchase Order Item |  |  |
| `PurchaseOrderType` |  | `EKKO` | `BSART` |  |  | `String(4)` |  | Purchasing Doc. Type |  |  |
| `PurchasingGroup` |  | `EKKO` | `EKGRP` |  |  | `String(3)` |  | Purchasing Group |  |  |
| `PurchasingOrganization` |  | `EKKO` | `EKORG` |  |  | `String(4)` |  | Purch. Organization |  |  |
| `PurchasingDocumentOrigin` |  |  |  |  |  | `String(1)` |  | Status |  | S/4 only entity |
| `Supplier` |  | `EKKO` | `LIFNR` |  |  | `String(10)` |  | Supplier |  |  |
| `SupplyingSupplier` |  |  |  |  |  | `String(10)` |  | Goods Supplier |  | S/4 only entity |
| `SupplyingPlant` |  |  |  |  |  | `String(4)` |  | Supplying Plant |  | S/4 only entity |
| `DocumentCurrency` |  | `EKKO` | `WAERS` |  |  | `String(5)` |  | Currency |  |  |
| `ExchangeRate` |  | `EKKO` | `WKURS` |  |  | `Decimal(9,5)` |  | Exchange Rate |  |  |
| `InvoicingParty` |  |  |  |  |  | `String(10)` |  | Invoicing Party |  | S/4 only entity |
| `PurchaseOrderDate` |  | `EKKO` | `BEDAT` |  |  | `Date` |  | Purchase Order Date |  |  |
| `ValidityStartDate` |  |  |  |  |  | `Date` |  | Validity Per. Start |  | S/4 only entity |
| `ValidityEndDate` |  |  |  |  |  | `Date` |  | Validity Period End |  | S/4 only entity |
| `CreationDate` |  | `EKKO` | `AEDAT` |  |  | `Date` |  | Created On |  |  |
| `LastChangeDateTime` |  |  |  |  |  | `Timestamp` |  | Last Changed |  | S/4 only entity |
| `PurgDocumentItemDeletionCode` |  |  |  |  |  | `String(1)` |  | Deletion Indicator |  | S/4 only entity |
| `MaterialGroup` |  | `EKPO` | `MATKL` |  |  | `String(9)` |  | Material Group |  |  |
| `Material` |  | `EKPO` | `MATNR` |  |  | `String(40)` |  | Material |  |  |
| `ManufacturerMaterial` |  |  |  |  |  | `String(40)` |  | Material |  | S/4 only entity |
| `PurchaseOrderCategory` |  |  |  |  |  | `String(1)` |  | Purch. Doc. Category |  | S/4 only entity |
| `PurchasingOrderReason` |  |  |  |  |  | `String(3)` |  | Reason for Ordering |  | S/4 only entity |
| `PurchaseOrderItemText` |  | `EKPO` | `TXZ01` |  |  | `String(40)` |  | Short Text |  |  |
| `PurchaseOrderItemCategory` |  |  |  |  |  | `String(1)` |  | Item Category |  | S/4 only entity |
| `CompanyCode` |  | `EKKO` | `BUKRS` |  |  | `String(4)` |  | Company Code |  |  |
| `Plant` |  | `EKPO` | `WERKS` |  |  | `String(4)` |  | Plant |  |  |
| `StorageLocation` |  | `EKPO` | `LGORT` |  |  | `String(4)` |  | Storage Location |  |  |
| `PurchaseContract` |  |  |  |  |  | `String(10)` |  | Outline agreement |  | S/4 only entity |
| `PurchaseContractItem` |  |  |  |  |  | `String(5)` |  | Agreement Item |  | S/4 only entity |
| `BaseUnit` |  |  |  |  |  | `String(3)` |  | Base Unit of Measure |  | S/4 only entity |
| `OrderQuantity` |  | `EKPO` | `MENGE` |  |  | `Decimal(13,3)` |  | Order Quantity | PurchaseOrderQuantityUnit |  |
| `PurchaseOrderQuantityUnit` |  | `EKPO` | `MEINS` |  |  | `String(3)` |  | Order Unit |  |  |
| `NetPriceAmount` |  | `EKPO` | `NETWR` |  |  | `Decimal(34,4)` |  | Net Order Price | DocumentCurrency |  |
| `NetAmount` |  |  |  |  |  | `Decimal(34,4)` |  | Net Order Value | DocumentCurrency | S/4 only entity |
| `LocalCurrency` |  |  |  |  |  | `String(5)` |  | Currency |  | S/4 only entity |
| `NetPriceQuantity` |  |  |  |  |  | `Decimal(5,0)` |  | Price Unit | OrderPriceUnit | S/4 only entity |
| `OrderPriceUnit` |  |  |  |  |  | `String(3)` |  | Order Price Unit |  | S/4 only entity |
| `RequisitionerName` |  |  |  |  |  | `String(12)` |  | Requisitioner |  | S/4 only entity |
| `RetailPromotion` |  |  |  |  |  | `String(10)` |  | Retail Promotion |  | S/4 only entity |
| `IsCompletelyDelivered` |  |  |  |  |  | `Boolean` |  | Delivery Completed |  | S/4 only entity |
| `IsReturnsItem` |  |  |  |  |  | `Boolean` |  | Returns Item |  | S/4 only entity |
| `IsFinallyInvoiced` |  |  |  |  |  | `Boolean` |  | Final Invoice |  | S/4 only entity |
| `InvoiceIsExpected` |  | `EKPO` | `REPOS` |  |  | `Boolean` |  | Invoice Receipt |  |  |
| `OrderItemQtyToBaseQtyDnmntr` |  |  |  |  |  | `Decimal(5,0)` |  | Denominator |  | S/4 only entity |
| `OrderItemQtyToBaseQtyNmrtr` |  |  |  |  |  | `Decimal(5,0)` |  | Numerator |  | S/4 only entity |
| `InvoiceIsGoodsReceiptBased` |  |  |  |  |  | `Boolean` |  | GR-Based Inv. Verif. |  | S/4 only entity |
| `GoodsReceiptIsExpected` |  | `EKPO` | `WEPOS` |  |  | `Boolean` |  | Goods Receipt |  |  |
| `EvaldRcptSettlmtIsAllowed` |  |  |  |  |  | `Boolean` |  | Eval. Receipt Sett. |  | S/4 only entity |
| `AccountAssignmentCategory` |  | `EKPO` | `KNTTP` |  |  | `String(1)` |  | Acct Assignment Cat. |  |  |
| `GoodsReceiptIsNonValuated` |  |  |  |  |  | `Boolean` |  | GR Non-Valuated |  | S/4 only entity |
| `MaterialType` |  |  |  |  |  | `String(4)` |  | Material Type |  | S/4 only entity |
| `OverdelivTolrtdLmtRatioInPct` |  |  |  |  |  | `Decimal(3,1)` |  | Overdeliv. Tolerance |  | S/4 only entity |
| `ServicePerformer` |  |  |  |  |  | `String(10)` |  | Service Performer |  | S/4 only entity |
| `TaxCode` |  |  |  |  |  | `String(2)` |  | Tax Code |  | S/4 only entity |
| `UnderdelivTolrtdLmtRatioInPct` |  |  |  |  |  | `Decimal(3,1)` |  | Underdel. Tolerance |  | S/4 only entity |
| `UnlimitedOverdeliveryIsAllowed` |  |  |  |  |  | `Boolean` |  | Unltd Overdelivery |  | S/4 only entity |
| `SupplierMaterialNumber` |  |  |  |  |  | `String(35)` |  | Supplier Mat. No. |  | S/4 only entity |
| `ProductTypeCode` |  |  |  |  |  | `String(2)` |  | Product Type Group |  | S/4 only entity |
| `CreatedByUser` |  | `EKKO` | `ERNAM` |  |  | `String(12)` |  | Created By |  |  |
| `ExpectedOverallLimitAmount` |  |  |  |  |  | `Decimal(34,4)` |  | Expected Value | DocumentCurrency | S/4 only entity |
| `OverallLimitAmount` |  |  |  |  |  | `Decimal(34,4)` |  | Overall Limit | DocumentCurrency | S/4 only entity |
| `RequirementSegment` |  |  |  |  |  | `String(40)` |  | Requirement Segment |  | S/4 only entity |
| `ReleaseIsNotCompleted` |  |  |  |  |  | `Boolean` |  | Subject to Release |  | S/4 only entity |
| `PurchasingCompletenessStatus` |  |  |  |  |  | `Boolean` |  | Incomplete |  | S/4 only entity |
| `IsStatisticalItem` |  |  |  |  |  | `Boolean` |  | Statistical |  | S/4 only entity |
| `MultipleAcctAssgmtDistribution` |  |  |  |  |  | `String(1)` |  | Distribut. Indicator |  | S/4 only entity |
| `PurchaseRequisition` |  |  |  |  |  | `String(10)` |  | Purchase Requisition |  | S/4 only entity |
| `PurchaseRequisitionItem` |  |  |  |  |  | `String(5)` |  | Item of requisition |  | S/4 only entity |
| `SupplierConfirmationControlKey` |  |  |  |  |  | `String(4)` |  | Confirmation Control |  | S/4 only entity |
| `PurchasingDocumentDeletionCode` |  |  |  |  |  | `String(1)` |  | Deletion Code |  | S/4 only entity |


## Entity: `PurchaseOrderScheduleLine`

- **ABAP CDS Name:** `C_PurOrdScheduleLineDEX`
- **Label:** Data Extraction for Purchase Order Schedule Lines
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `PurchaseOrder` |  |  |  |  |  | `String(10)` | Y | Purchasing Document |  | S/4 only entity |
| `PurchaseOrderItem` |  |  |  |  |  | `String(5)` | Y | Item |  | S/4 only entity |
| `PurchaseOrderScheduleLine` |  |  |  |  |  | `String(4)` | Y | Schedule Line |  | S/4 only entity |
| `ScheduleLineDeliveryDate` |  |  |  |  |  | `Date` |  | Delivery Date |  | S/4 only entity |
| `SchedLineStscDeliveryDate` |  |  |  |  |  | `Date` |  | Stat.-Rel. Del. Date |  | S/4 only entity |
| `ScheduleLineDeliveryTime` |  |  |  |  |  | `String(6)` |  | Time |  | S/4 only entity |
| `PurchaseRequisition` |  |  |  |  |  | `String(10)` |  | Purchase Requisition |  | S/4 only entity |
| `PurchaseRequisitionItem` |  |  |  |  |  | `String(5)` |  | Item of requisition |  | S/4 only entity |
| `Batch` |  |  |  |  |  | `String(10)` |  | Batch |  | S/4 only entity |
| `PurchasingSchdLnNrOfReminders` |  |  |  |  |  | `Decimal(3,0)` |  | No. Rem./Expediters |  | S/4 only entity |
| `RequisitionerName` |  |  |  |  |  | `String(12)` |  | Requisitioner |  | S/4 only entity |
| `RetailPromotion` |  |  |  |  |  | `String(10)` |  | Retail Promotion |  | S/4 only entity |
| `ArticleCategory` |  |  |  |  |  | `String(2)` |  | Material Category |  | S/4 only entity |
| `PurchasingOrderReason` |  |  |  |  |  | `String(3)` |  | Reason for Ordering |  | S/4 only entity |
| `IsCompletelyDelivered` |  |  |  |  |  | `Boolean` |  | Delivery Completed |  | S/4 only entity |
| `ManufacturerMaterial` |  |  |  |  |  | `String(40)` |  | Material |  | S/4 only entity |
| `IsFinallyInvoiced` |  |  |  |  |  | `Boolean` |  | Final Invoice |  | S/4 only entity |
| `PurchaseContract` |  |  |  |  |  | `String(10)` |  | Outline agreement |  | S/4 only entity |
| `PurchaseContractItem` |  |  |  |  |  | `String(5)` |  | Agreement Item |  | S/4 only entity |
| `StorageLocation` |  |  |  |  |  | `String(4)` |  | Storage Location |  | S/4 only entity |
| `BaseUnit` |  |  |  |  |  | `String(3)` |  | Base Unit of Measure |  | S/4 only entity |
| `MaterialGroup` |  |  |  |  |  | `String(9)` |  | Material Group |  | S/4 only entity |
| `Material` |  |  |  |  |  | `String(40)` |  | Material |  | S/4 only entity |
| `PurchaseOrderQuantityUnit` |  |  |  |  |  | `String(3)` |  | Order Unit |  | S/4 only entity |
| `PurchaseOrderItemCategory` |  |  |  |  |  | `String(1)` |  | Item Category |  | S/4 only entity |
| `IssuingStorageLocation` |  |  |  |  |  | `String(4)` |  | Issuing Storage Loc. |  | S/4 only entity |
| `PurchaseOrderItemText` |  |  |  |  |  | `String(40)` |  | Short Text |  | S/4 only entity |
| `PurchasingParentItem` |  |  |  |  |  | `String(5)` |  | Higher-Level Item |  | S/4 only entity |
| `OrderItemQtyToBaseQtyDnmntr` |  |  |  |  |  | `Decimal(5,0)` |  | Denominator |  | S/4 only entity |
| `OrderItemQtyToBaseQtyNmrtr` |  |  |  |  |  | `Decimal(5,0)` |  | Numerator |  | S/4 only entity |
| `InvoiceIsGoodsReceiptBased` |  |  |  |  |  | `Boolean` |  | GR-Based Inv. Verif. |  | S/4 only entity |
| `GoodsReceiptIsExpected` |  |  |  |  |  | `Boolean` |  | Goods Receipt |  | S/4 only entity |
| `Plant` |  |  |  |  |  | `String(4)` |  | Plant |  | S/4 only entity |
| `EvaldRcptSettlmtIsAllowed` |  |  |  |  |  | `Boolean` |  | Eval. Receipt Sett. |  | S/4 only entity |
| `PurchaseOrderDate` |  |  |  |  |  | `Date` |  | Purchase Order Date |  | S/4 only entity |
| `PurchaseOrderType` |  |  |  |  |  | `String(4)` |  | Purchasing Doc. Type |  | S/4 only entity |
| `PurchasingGroup` |  |  |  |  |  | `String(3)` |  | Purchasing Group |  | S/4 only entity |
| `PurchasingOrganization` |  |  |  |  |  | `String(4)` |  | Purch. Organization |  | S/4 only entity |
| `ValidityStartDate` |  |  |  |  |  | `Date` |  | Validity Per. Start |  | S/4 only entity |
| `ValidityEndDate` |  |  |  |  |  | `Date` |  | Validity Period End |  | S/4 only entity |
| `Supplier` |  |  |  |  |  | `String(10)` |  | Supplier |  | S/4 only entity |
| `InvoicingParty` |  |  |  |  |  | `String(10)` |  | Invoicing Party |  | S/4 only entity |
| `SupplyingSupplier` |  |  |  |  |  | `String(10)` |  | Goods Supplier |  | S/4 only entity |
| `SupplyingPlant` |  |  |  |  |  | `String(4)` |  | Supplying Plant |  | S/4 only entity |
| `PurchasingDocumentOrigin` |  |  |  |  |  | `String(1)` |  | Status |  | S/4 only entity |
| `DocumentCurrency` |  |  |  |  |  | `String(5)` |  | Currency |  | S/4 only entity |
| `ExchangeRate` |  |  |  |  |  | `Decimal(9,5)` |  | Exchange Rate |  | S/4 only entity |
| `DelivDateCategory` |  |  |  |  |  | `String(1)` |  | Deliv. date category |  | S/4 only entity |
| `ScheduleLineOrderQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Scheduled Quantity | PurchaseOrderQuantityUnit | S/4 only entity |
| `PrevDelivQtyOfScheduleLine` |  |  |  |  |  | `Decimal(13,3)` |  | Previous Quantity | PurchaseOrderQuantityUnit | S/4 only entity |
| `RoughGoodsReceiptQty` |  |  |  |  |  | `Decimal(13,3)` |  | Quantity Delivered | PurchaseOrderQuantityUnit | S/4 only entity |
| `ScheduleLineIssuedQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Issued Quantity | PurchaseOrderQuantityUnit | S/4 only entity |
| `SourceOfCreation` |  |  |  |  |  | `String(1)` |  | Creation indicator |  | S/4 only entity |
| `Reservation` |  |  |  |  |  | `String(10)` |  | Reservation |  | S/4 only entity |
| `ScheduleLineIsFixed` |  |  |  |  |  | `Boolean` |  | Fixing Indicator |  | S/4 only entity |
| `StockTransferDeliveredQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Qty Delivered | PurchaseOrderQuantityUnit | S/4 only entity |
| `ScheduleLineCommittedQuantity` |  |  |  |  |  | `Decimal(13,3)` |  | Committed Quantity | PurchaseOrderQuantityUnit | S/4 only entity |
| `ProductAvailabilityDate` |  |  |  |  |  | `Date` |  | Material Avail. Date |  | S/4 only entity |
| `ProductAvailabilityTime` |  |  |  |  |  | `String(6)` |  | Matl Staging Time |  | S/4 only entity |
| `LoadingDate` |  |  |  |  |  | `Date` |  | Loading Date |  | S/4 only entity |
| `LoadingTime` |  |  |  |  |  | `String(6)` |  | Loading Time |  | S/4 only entity |
| `TransportationPlanningDate` |  |  |  |  |  | `Date` |  | Transptn Plang Date |  | S/4 only entity |
| `TransportationPlanningTime` |  |  |  |  |  | `String(6)` |  | Transp. Plan. Time |  | S/4 only entity |
| `GoodsIssueDate` |  |  |  |  |  | `Date` |  | Goods Issue Date |  | S/4 only entity |
| `GoodsIssueTime` |  |  |  |  |  | `String(6)` |  | Goods Issue Time |  | S/4 only entity |
| `STOLatestPossibleGRDate` |  |  |  |  |  | `Date` |  | GR End Date |  | S/4 only entity |
| `STOLatestPossibleGRTime` |  |  |  |  |  | `String(6)` |  | GR End Time |  | S/4 only entity |
| `OpenPurchaseOrderNetAmount` |  |  |  |  |  | `Decimal(34,4)` |  |  | DocumentCurrency | S/4 only entity |
| `IsReturnsItem` |  |  |  |  |  | `Boolean` |  | Returns Item |  | S/4 only entity |
| `CompanyCode` |  |  |  |  |  | `String(4)` |  | Company Code |  | S/4 only entity |
| `ProductTypeCode` |  |  |  |  |  | `String(2)` |  | Product Type Group |  | S/4 only entity |
| `PurchasingDocumentDeletionCode` |  |  |  |  |  | `String(1)` |  | Deletion Code |  | S/4 only entity |
| `PurgDocumentItemDeletionCode` |  |  |  |  |  | `String(1)` |  | Deletion Indicator |  | S/4 only entity |
| `ReleaseIsNotCompleted` |  |  |  |  |  | `Boolean` |  | Subject to Release |  | S/4 only entity |
| `PurchasingCompletenessStatus` |  |  |  |  |  | `Boolean` |  | Incomplete |  | S/4 only entity |
| `SupplierConfirmationControlKey` |  |  |  |  |  | `String(4)` |  | Confirmation Control |  | S/4 only entity |
| `IsStatisticalItem` |  |  |  |  |  | `Boolean` |  | Statistical |  | S/4 only entity |
| `ScheduleLineOpenQuantity` |  |  |  |  |  | `Decimal(14,3)` |  |  | PurchaseOrderQuantityUnit | S/4 only entity |
