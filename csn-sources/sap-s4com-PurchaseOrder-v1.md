# PurchaseOrder

> Source file: `sap-s4com-PurchaseOrder-v1.json`


## Entity: `PurOrdSupplierConfirmation`

- **ABAP Name:** `C_POSupplierConfirmationDEX`
- **Label:** Purchase Order Supplier Confirmation DEX
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `PurchaseOrder` |  |  |  | `String(10)` | Y | Purchase Order |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchaseOrderItem` |  |  |  | `String(5)` | Y | Purchase Order Item |  |  | S/4 only entity — no ECC CDC mapping |
| `SequentialNmbrOfSuplrConf` |  |  |  | `String(4)` | Y | Sequential Number |  |  | S/4 only entity — no ECC CDC mapping |
| `SupplierConfirmationCategory` |  |  |  | `String(2)` |  | Confirm. Category |  |  | S/4 only entity — no ECC CDC mapping |
| `DeliveryDate` |  |  |  | `Date` |  | Delivery Date |  |  | S/4 only entity — no ECC CDC mapping |
| `DelivDateCategory` |  |  |  | `String(1)` |  | Deliv. Date Category |  |  | S/4 only entity — no ECC CDC mapping |
| `DeliveryTime` |  |  |  | `String(6)` |  | Time |  |  | S/4 only entity — no ECC CDC mapping |
| `CreationDate` |  |  |  | `Date` |  | Creation Date |  |  | S/4 only entity — no ECC CDC mapping |
| `CreationTime` |  |  |  | `String(6)` |  | Creation Time |  |  | S/4 only entity — no ECC CDC mapping |
| `ConfirmedQuantity` |  |  |  | `Decimal(13,3)` |  | Quantity | OrderQuantityUnit |  | S/4 only entity — no ECC CDC mapping |
| `MRPRelevantQuantity` |  |  |  | `Decimal(13,3)` |  | Qty Reduced (MRP) | OrderQuantityUnit |  | S/4 only entity — no ECC CDC mapping |
| `SuplrConfCreationCategory` |  |  |  | `String(1)` |  | Creation Indicator |  |  | S/4 only entity — no ECC CDC mapping |
| `IsDeleted` |  |  |  | `String(1)` |  | Deletion Indicator |  |  | S/4 only entity — no ECC CDC mapping |
| `ConfIsRelevantToMRP` |  |  |  | `Boolean` |  | MRP-Relevant |  |  | S/4 only entity — no ECC CDC mapping |
| `SupplierConfirmationExtNumber` |  |  |  | `String(35)` |  | Reference |  |  | S/4 only entity — no ECC CDC mapping |
| `DeliveryDocument` |  |  |  | `String(10)` |  | Delivery |  |  | S/4 only entity — no ECC CDC mapping |
| `DeliveryDocumentItem` |  |  |  | `String(6)` |  | Item |  |  | S/4 only entity — no ECC CDC mapping |
| `ManufacturerPartProfile` |  |  |  | `String(4)` |  | Mfr Part Profile |  |  | S/4 only entity — no ECC CDC mapping |
| `ManufacturerMaterial` |  |  |  | `String(40)` |  | MPN: Material |  |  | S/4 only entity — no ECC CDC mapping |
| `NumberOfReminders` |  |  |  | `Decimal(3,0)` |  | No. Rem./Expediters |  |  | S/4 only entity — no ECC CDC mapping |
| `Batch` |  |  |  | `String(10)` |  | Batch |  |  | S/4 only entity — no ECC CDC mapping |
| `DeliveryIsInPlant` |  |  |  | `Boolean` |  | In Plant |  |  | S/4 only entity — no ECC CDC mapping |
| `HandoverDate` |  |  |  | `Date` |  | Handover Date |  |  | S/4 only entity — no ECC CDC mapping |
| `HandoverTime` |  |  |  | `String(6)` |  | Handover Time |  |  | S/4 only entity — no ECC CDC mapping |
| `PerformancePeriodStartDate` |  |  |  | `Date` |  | Start Date |  |  | S/4 only entity — no ECC CDC mapping |
| `PerformancePeriodEndDate` |  |  |  | `Date` |  | End Date |  |  | S/4 only entity — no ECC CDC mapping |
| `ServicePerformer` |  |  |  | `String(10)` |  | Service Performer |  |  | S/4 only entity — no ECC CDC mapping |
| `OrderQuantityUnit` |  |  |  | `String(3)` |  | Order Unit |  |  | S/4 only entity — no ECC CDC mapping |
| `SupplierConfirmation` |  |  |  | `String(10)` |  | Confirmation |  |  | S/4 only entity — no ECC CDC mapping |
| `SupplierConfirmationItem` |  |  |  | `String(5)` |  | Confirmation Item |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchaseOrderType` |  |  |  | `String(4)` |  | Purchasing Doc. Type |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchasingOrganization` |  |  |  | `String(4)` |  | Purch. Organization |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchasingGroup` |  |  |  | `String(3)` |  | Purchasing Group |  |  | S/4 only entity — no ECC CDC mapping |
| `Plant` |  |  |  | `String(4)` |  | Plant |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `PurchaseOrder`

- **ABAP Name:** `C_PurchaseOrderDEX`
- **Label:** Data Extraction for Purchase Order
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `PurchaseOrder` |  |  |  | `String(10)` | Y | Purchase Order |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchaseOrderType` |  |  |  | `String(4)` |  | Purchasing Doc. Type |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchaseOrderSubtype` |  |  |  | `String(1)` |  | Control indicator |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchasingDocumentOrigin` |  |  |  | `String(1)` |  | Status |  |  | S/4 only entity — no ECC CDC mapping |
| `CreatedByUser` |  |  |  | `String(12)` |  | Created By |  |  | S/4 only entity — no ECC CDC mapping |
| `CreationDate` |  |  |  | `Date` |  | Created On |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchaseOrderDate` |  |  |  | `Date` |  | Purchase Order Date |  |  | S/4 only entity — no ECC CDC mapping |
| `Language` |  |  |  | `String(2)` |  | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `CorrespncExternalReference` |  |  |  | `String(12)` |  | Your Reference |  |  | S/4 only entity — no ECC CDC mapping |
| `CorrespncInternalReference` |  |  |  | `String(12)` |  | Our Reference |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchasingDocumentDeletionCode` |  |  |  | `String(1)` |  | Deletion Code |  |  | S/4 only entity — no ECC CDC mapping |
| `ReleaseIsNotCompleted` |  |  |  | `Boolean` |  | Subject to Release |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchasingCompletenessStatus` |  |  |  | `Boolean` |  | Incomplete |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchasingProcessingStatus` |  |  |  | `String(2)` |  | Proc. State |  |  | S/4 only entity — no ECC CDC mapping |
| `PurgReleaseSequenceStatus` |  |  |  | `String(8)` |  | Release Status |  |  | S/4 only entity — no ECC CDC mapping |
| `ReleaseCode` |  |  |  | `String(1)` |  | Release indicator |  |  | S/4 only entity — no ECC CDC mapping |
| `CompanyCode` |  |  |  | `String(4)` |  | Company Code |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchasingOrganization` |  |  |  | `String(4)` |  | Purch. Organization |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchasingGroup` |  |  |  | `String(3)` |  | Purchasing Group |  |  | S/4 only entity — no ECC CDC mapping |
| `Supplier` |  |  |  | `String(10)` |  | Supplier |  |  | S/4 only entity — no ECC CDC mapping |
| `ManualSupplierAddressID` |  |  |  | `String(10)` |  | Address Number |  |  | S/4 only entity — no ECC CDC mapping |
| `SupplierRespSalesPersonName` |  |  |  | `String(30)` |  | Salesperson |  |  | S/4 only entity — no ECC CDC mapping |
| `SupplierPhoneNumber` |  |  |  | `String(16)` |  | Supplier Phone |  |  | S/4 only entity — no ECC CDC mapping |
| `SupplyingSupplier` |  |  |  | `String(10)` |  | Goods Supplier |  |  | S/4 only entity — no ECC CDC mapping |
| `SupplyingPlant` |  |  |  | `String(4)` |  | Supplying Plant |  |  | S/4 only entity — no ECC CDC mapping |
| `InvoicingParty` |  |  |  | `String(10)` |  | Invoicing Party |  |  | S/4 only entity — no ECC CDC mapping |
| `Customer` |  |  |  | `String(10)` |  | Customer |  |  | S/4 only entity — no ECC CDC mapping |
| `SupplierQuotationExternalID` |  |  |  | `String(10)` |  | Quotation |  |  | S/4 only entity — no ECC CDC mapping |
| `PaymentTerms` |  |  |  | `String(4)` |  | Payment Terms |  |  | S/4 only entity — no ECC CDC mapping |
| `CashDiscount1Days` |  |  |  | `Decimal(3,0)` |  | Days 1 |  |  | S/4 only entity — no ECC CDC mapping |
| `CashDiscount2Days` |  |  |  | `Decimal(3,0)` |  | Days 2 |  |  | S/4 only entity — no ECC CDC mapping |
| `NetPaymentDays` |  |  |  | `Decimal(3,0)` |  | Days Net |  |  | S/4 only entity — no ECC CDC mapping |
| `CashDiscount1Percent` |  |  |  | `Decimal(5,3)` |  | CD Percentage 1 |  |  | S/4 only entity — no ECC CDC mapping |
| `CashDiscount2Percent` |  |  |  | `Decimal(5,3)` |  | CD Percentage 2 |  |  | S/4 only entity — no ECC CDC mapping |
| `DownPaymentType` |  |  |  | `String(4)` |  | Down Payment |  |  | S/4 only entity — no ECC CDC mapping |
| `DownPaymentPercentageOfTotAmt` |  |  |  | `Decimal(5,2)` |  | Down Payment % |  |  | S/4 only entity — no ECC CDC mapping |
| `DownPaymentAmount` |  |  |  | `Decimal(34,4)` |  | Down Payment Amount | DocumentCurrency |  | S/4 only entity — no ECC CDC mapping |
| `DownPaymentDueDate` |  |  |  | `Date` |  | Due Date for DP |  |  | S/4 only entity — no ECC CDC mapping |
| `IncotermsClassification` |  |  |  | `String(3)` |  | Incoterms |  |  | S/4 only entity — no ECC CDC mapping |
| `IncotermsTransferLocation` |  |  |  | `String(28)` |  | Incoterms (Part 2) |  |  | S/4 only entity — no ECC CDC mapping |
| `IncotermsVersion` |  |  |  | `String(4)` |  | Incoterms Version |  |  | S/4 only entity — no ECC CDC mapping |
| `IncotermsLocation1` |  |  |  | `String(70)` |  | Incoterms Location 1 |  |  | S/4 only entity — no ECC CDC mapping |
| `IncotermsLocation2` |  |  |  | `String(70)` |  | Incoterms Location 2 |  |  | S/4 only entity — no ECC CDC mapping |
| `IsIntrastatReportingRelevant` |  |  |  | `Boolean` |  | Intrastat Relevance |  |  | S/4 only entity — no ECC CDC mapping |
| `IsIntrastatReportingExcluded` |  |  |  | `Boolean` |  | Intrastat Exclusion |  |  | S/4 only entity — no ECC CDC mapping |
| `PricingDocument` |  |  |  | `String(10)` |  | Doc. Condition No. |  |  | S/4 only entity — no ECC CDC mapping |
| `PricingProcedure` |  |  |  | `String(6)` |  | Procedure |  |  | S/4 only entity — no ECC CDC mapping |
| `DocumentCurrency` |  |  |  | `String(5)` |  | Currency |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityStartDate` |  |  |  | `Date` |  | Validity Per. Start |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityEndDate` |  |  |  | `Date` |  | Validity Period End |  |  | S/4 only entity — no ECC CDC mapping |
| `ExchangeRate` |  |  |  | `Decimal(9,5)` |  | Exchange Rate |  |  | S/4 only entity — no ECC CDC mapping |
| `ExchangeRateIsFixed` |  |  |  | `Boolean` |  | Fixed Exchange Rate |  |  | S/4 only entity — no ECC CDC mapping |
| `LastChangeDateTime` |  |  |  | `Timestamp` |  | Last Changed |  |  | S/4 only entity — no ECC CDC mapping |
| `TaxReturnCountry` |  |  |  | `String(3)` |  | Reporting C/R |  |  | S/4 only entity — no ECC CDC mapping |
| `VATRegistrationCountry` |  |  |  | `String(3)` |  | Ctry/Rgn Sls Tax No. |  |  | S/4 only entity — no ECC CDC mapping |
| `PurgReasonForDocCancellation` |  |  |  | `String(2)` |  | Reason for Canc. |  |  | S/4 only entity — no ECC CDC mapping |
| `PurgReleaseTimeTotalAmount` |  |  |  | `Decimal(34,4)` |  | Tot. val. rel. | DocumentCurrency |  | S/4 only entity — no ECC CDC mapping |


## Entity: `PurchaseOrderAccountAssignment`

- **ABAP Name:** `C_PurOrdAccountAssignmentDEX`
- **Label:** Data Extraction for Purchase Order Account Assignments
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `PurchaseOrder` |  |  |  | `String(10)` | Y | Purchasing Document |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchaseOrderItem` |  |  |  | `String(5)` | Y | Item |  |  | S/4 only entity — no ECC CDC mapping |
| `AccountAssignmentNumber` |  |  |  | `String(2)` | Y | Account Assgmt No. |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCenter` |  |  |  | `String(10)` |  | Cost Center |  |  | S/4 only entity — no ECC CDC mapping |
| `MasterFixedAsset` |  |  |  | `String(12)` |  | Asset |  |  | S/4 only entity — no ECC CDC mapping |
| `ProjectNetwork` |  |  |  | `String(12)` |  | Network |  |  | S/4 only entity — no ECC CDC mapping |
| `Quantity` |  |  |  | `Decimal(13,3)` |  | Quantity | PurchaseOrderQuantityUnit |  | S/4 only entity — no ECC CDC mapping |
| `PurchaseOrderQuantityUnit` |  |  |  | `String(3)` |  | Order Unit |  |  | S/4 only entity — no ECC CDC mapping |
| `MultipleAcctAssgmtDistrPercent` |  |  |  | `Decimal(3,1)` |  | Distribution (%) |  |  | S/4 only entity — no ECC CDC mapping |
| `PurgDocNetAmount` |  |  |  | `Decimal(34,4)` |  | Net Order Value | DocumentCurrency |  | S/4 only entity — no ECC CDC mapping |
| `DocumentCurrency` |  |  |  | `String(5)` |  | Currency |  |  | S/4 only entity — no ECC CDC mapping |
| `IsDeleted` |  |  |  | `Boolean` |  | Deletion Indicator |  |  | S/4 only entity — no ECC CDC mapping |
| `GLAccount` |  |  |  | `String(10)` |  | G/L Account |  |  | S/4 only entity — no ECC CDC mapping |
| `BusinessArea` |  |  |  | `String(4)` |  | Business Area |  |  | S/4 only entity — no ECC CDC mapping |
| `SalesOrder` |  |  |  | `String(10)` |  | SD Document |  |  | S/4 only entity — no ECC CDC mapping |
| `SalesOrderItem` |  |  |  | `String(6)` |  | Item |  |  | S/4 only entity — no ECC CDC mapping |
| `SalesOrderScheduleLine` |  |  |  | `String(4)` |  | Schedule Line Number |  |  | S/4 only entity — no ECC CDC mapping |
| `FixedAsset` |  |  |  | `String(4)` |  | Subnumber |  |  | S/4 only entity — no ECC CDC mapping |
| `OrderID` |  |  |  | `String(12)` |  | Order |  |  | S/4 only entity — no ECC CDC mapping |
| `UnloadingPointName` |  |  |  | `String(25)` |  | Unloading Point |  |  | S/4 only entity — no ECC CDC mapping |
| `ControllingArea` |  |  |  | `String(4)` |  | Controlling Area |  |  | S/4 only entity — no ECC CDC mapping |
| `CostObject` |  |  |  | `String(12)` |  | Cost Object |  |  | S/4 only entity — no ECC CDC mapping |
| `ProfitabilitySegment` |  |  |  | `String(10)` |  | Profitability Segment (Deprecated) |  |  | S/4 only entity — no ECC CDC mapping |
| `ProfitabilitySegment_2` |  |  |  | `String(10)` |  | Profitability Segment |  |  | S/4 only entity — no ECC CDC mapping |
| `ProfitCenter` |  |  |  | `String(10)` |  | Profit Center |  |  | S/4 only entity — no ECC CDC mapping |
| `WBSElementInternalID` |  |  |  | `String(8)` |  | WBS Internal ID |  |  | S/4 only entity — no ECC CDC mapping |
| `ProjectNetworkInternalID` |  |  |  | `String(10)` |  | Opertn Task List No. |  |  | S/4 only entity — no ECC CDC mapping |
| `CommitmentItem` |  |  |  | `String(24)` |  |  |  |  | S/4 only entity — no ECC CDC mapping |
| `FundsCenter` |  |  |  | `String(16)` |  | Funds Center |  |  | S/4 only entity — no ECC CDC mapping |
| `Fund` |  |  |  | `String(10)` |  | Fund |  |  | S/4 only entity — no ECC CDC mapping |
| `FunctionalArea` |  |  |  | `String(16)` |  | Functional Area |  |  | S/4 only entity — no ECC CDC mapping |
| `GoodsRecipientName` |  |  |  | `String(12)` |  | Goods Recipient |  |  | S/4 only entity — no ECC CDC mapping |
| `IsFinallyInvoiced` |  |  |  | `Boolean` |  | Final Invoice |  |  | S/4 only entity — no ECC CDC mapping |
| `RealEstateObject` |  |  |  | `String(8)` |  | Real Estate Key |  |  | S/4 only entity — no ECC CDC mapping |
| `NetworkActivityInternalID` |  |  |  | `String(8)` |  | Counter |  |  | S/4 only entity — no ECC CDC mapping |
| `PartnerAccountNumber` |  |  |  | `String(10)` |  | Partner |  |  | S/4 only entity — no ECC CDC mapping |
| `JointVentureRecoveryCode` |  |  |  | `String(2)` |  | Recovery Indicator |  |  | S/4 only entity — no ECC CDC mapping |
| `SettlementReferenceDate` |  |  |  | `Date` |  | Reference Date |  |  | S/4 only entity — no ECC CDC mapping |
| `OrderInternalID` |  |  |  | `String(10)` |  | Opertn Task List No. |  |  | S/4 only entity — no ECC CDC mapping |
| `OrderIntBillOfOperationsItem` |  |  |  | `String(8)` |  | Counter |  |  | S/4 only entity — no ECC CDC mapping |
| `TaxCode` |  |  |  | `String(2)` |  | Tax Code |  |  | S/4 only entity — no ECC CDC mapping |
| `TaxJurisdiction` |  |  |  | `String(15)` |  | Tax Jurisdiction |  |  | S/4 only entity — no ECC CDC mapping |
| `NonDeductibleInputTaxAmount` |  |  |  | `Decimal(34,4)` |  | Non-deductible | DocumentCurrency |  | S/4 only entity — no ECC CDC mapping |
| `CostCtrActivityType` |  |  |  | `String(6)` |  | Activity Type |  |  | S/4 only entity — no ECC CDC mapping |
| `BusinessProcess` |  |  |  | `String(12)` |  | Business Process |  |  | S/4 only entity — no ECC CDC mapping |
| `GrantID` |  |  |  | `String(20)` |  | Grant |  |  | S/4 only entity — no ECC CDC mapping |
| `BudgetPeriod` |  |  |  | `String(10)` |  | Budget Period |  |  | S/4 only entity — no ECC CDC mapping |
| `EarmarkedFundsDocument` |  |  |  | `String(10)` |  | Earmarked Funds |  |  | S/4 only entity — no ECC CDC mapping |
| `EarmarkedFundsDocumentItem` |  |  |  | `String(3)` |  | Document Item |  |  | S/4 only entity — no ECC CDC mapping |
| `ServiceDocumentType` |  |  |  | `String(4)` |  | Service Doc. Type |  |  | S/4 only entity — no ECC CDC mapping |
| `ServiceDocument` |  |  |  | `String(10)` |  | Service Document |  |  | S/4 only entity — no ECC CDC mapping |
| `ServiceDocumentItem` |  |  |  | `String(6)` |  | Service Doc. Item |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchaseOrderType` |  |  |  | `String(4)` |  | Purchasing Doc. Type |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchasingOrganization` |  |  |  | `String(4)` |  | Purch. Organization |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchasingGroup` |  |  |  | `String(3)` |  | Purchasing Group |  |  | S/4 only entity — no ECC CDC mapping |
| `CreationDate` |  |  |  | `Date` |  | Created On |  |  | S/4 only entity — no ECC CDC mapping |
| `LastChangeDateTime` |  |  |  | `Timestamp` |  | Last Changed |  |  | S/4 only entity — no ECC CDC mapping |
| `Plant` |  |  |  | `String(4)` |  | Plant |  |  | S/4 only entity — no ECC CDC mapping |
| `AccountAssignmentCategory` |  |  |  | `String(1)` |  | Acct Assignment Cat. |  |  | S/4 only entity — no ECC CDC mapping |
| `CompanyCode` |  |  |  | `String(4)` |  | Company Code |  |  | S/4 only entity — no ECC CDC mapping |
| `IsReturnsItem` |  |  |  | `Boolean` |  | Returns Item |  |  | S/4 only entity — no ECC CDC mapping |
| `SupplyingPlant` |  |  |  | `String(4)` |  | Supplying Plant |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchaseOrderItemCategory` |  |  |  | `String(1)` |  | Item Category |  |  | S/4 only entity — no ECC CDC mapping |
| `Material` |  |  |  | `String(40)` |  | Material |  |  | S/4 only entity — no ECC CDC mapping |
| `MaterialGroup` |  |  |  | `String(9)` |  | Material Group |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchaseOrderDate` |  |  |  | `Date` |  | Purchase Order Date |  |  | S/4 only entity — no ECC CDC mapping |
| `StorageLocation` |  |  |  | `String(4)` |  | Storage Location |  |  | S/4 only entity — no ECC CDC mapping |
| `IsCompletelyDelivered` |  |  |  | `Boolean` |  | Delivery Completed |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchasingInfoRecord` |  |  |  | `String(10)` |  | Purchasing Info Rec. |  |  | S/4 only entity — no ECC CDC mapping |
| `RequirementTracking` |  |  |  | `String(10)` |  | Req. Tracking Number |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchaseOrderItemText` |  |  |  | `String(40)` |  | Short Text |  |  | S/4 only entity — no ECC CDC mapping |
| `PurgDocumentItemDeletionCode` |  |  |  | `String(1)` |  | Deletion Indicator |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchasingDocumentDeletionCode` |  |  |  | `String(1)` |  | Deletion Code |  |  | S/4 only entity — no ECC CDC mapping |
| `InvoiceIsExpected` |  |  |  | `Boolean` |  | Invoice Receipt |  |  | S/4 only entity — no ECC CDC mapping |
| `GoodsReceiptIsExpected` |  |  |  | `Boolean` |  | Goods Receipt |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductTypeCode` |  |  |  | `String(2)` |  | Product Type Group |  |  | S/4 only entity — no ECC CDC mapping |
| `IsStatisticalItem` |  |  |  | `Boolean` |  | Statistical |  |  | S/4 only entity — no ECC CDC mapping |
| `ReleaseIsNotCompleted` |  |  |  | `Boolean` |  | Subject to Release |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchasingCompletenessStatus` |  |  |  | `Boolean` |  | Incomplete |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchaseContract` |  |  |  | `String(10)` |  | Outline agreement |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchaseContractItem` |  |  |  | `String(5)` |  | Agreement Item |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `PurchaseOrderItem`

- **ABAP Name:** `C_PurchaseOrderItemDEX`
- **Label:** Data Extraction View for PO Item
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `PurchaseOrder` |  |  |  | `String(10)` | Y | Purchase Order |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchaseOrderItem` |  |  |  | `String(5)` | Y | Purchase Order Item |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchaseOrderType` |  |  |  | `String(4)` |  | Purchasing Doc. Type |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchasingGroup` |  |  |  | `String(3)` |  | Purchasing Group |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchasingOrganization` |  |  |  | `String(4)` |  | Purch. Organization |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchasingDocumentOrigin` |  |  |  | `String(1)` |  | Status |  |  | S/4 only entity — no ECC CDC mapping |
| `Supplier` |  |  |  | `String(10)` |  | Supplier |  |  | S/4 only entity — no ECC CDC mapping |
| `SupplyingSupplier` |  |  |  | `String(10)` |  | Goods Supplier |  |  | S/4 only entity — no ECC CDC mapping |
| `SupplyingPlant` |  |  |  | `String(4)` |  | Supplying Plant |  |  | S/4 only entity — no ECC CDC mapping |
| `DocumentCurrency` |  |  |  | `String(5)` |  | Currency |  |  | S/4 only entity — no ECC CDC mapping |
| `ExchangeRate` |  |  |  | `Decimal(9,5)` |  | Exchange Rate |  |  | S/4 only entity — no ECC CDC mapping |
| `InvoicingParty` |  |  |  | `String(10)` |  | Invoicing Party |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchaseOrderDate` |  |  |  | `Date` |  | Purchase Order Date |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityStartDate` |  |  |  | `Date` |  | Validity Per. Start |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityEndDate` |  |  |  | `Date` |  | Validity Period End |  |  | S/4 only entity — no ECC CDC mapping |
| `CreationDate` |  |  |  | `Date` |  | Created On |  |  | S/4 only entity — no ECC CDC mapping |
| `LastChangeDateTime` |  |  |  | `Timestamp` |  | Last Changed |  |  | S/4 only entity — no ECC CDC mapping |
| `PurgDocumentItemDeletionCode` |  |  |  | `String(1)` |  | Deletion Indicator |  |  | S/4 only entity — no ECC CDC mapping |
| `MaterialGroup` |  |  |  | `String(9)` |  | Material Group |  |  | S/4 only entity — no ECC CDC mapping |
| `Material` |  |  |  | `String(40)` |  | Material |  |  | S/4 only entity — no ECC CDC mapping |
| `ManufacturerMaterial` |  |  |  | `String(40)` |  | Material |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchaseOrderCategory` |  |  |  | `String(1)` |  | Purch. Doc. Category |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchasingOrderReason` |  |  |  | `String(3)` |  | Reason for Ordering |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchaseOrderItemText` |  |  |  | `String(40)` |  | Short Text |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchaseOrderItemCategory` |  |  |  | `String(1)` |  | Item Category |  |  | S/4 only entity — no ECC CDC mapping |
| `CompanyCode` |  |  |  | `String(4)` |  | Company Code |  |  | S/4 only entity — no ECC CDC mapping |
| `Plant` |  |  |  | `String(4)` |  | Plant |  |  | S/4 only entity — no ECC CDC mapping |
| `StorageLocation` |  |  |  | `String(4)` |  | Storage Location |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchaseContract` |  |  |  | `String(10)` |  | Outline agreement |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchaseContractItem` |  |  |  | `String(5)` |  | Agreement Item |  |  | S/4 only entity — no ECC CDC mapping |
| `BaseUnit` |  |  |  | `String(3)` |  | Base Unit of Measure |  |  | S/4 only entity — no ECC CDC mapping |
| `OrderQuantity` |  |  |  | `Decimal(13,3)` |  | Order Quantity | PurchaseOrderQuantityUnit |  | S/4 only entity — no ECC CDC mapping |
| `PurchaseOrderQuantityUnit` |  |  |  | `String(3)` |  | Order Unit |  |  | S/4 only entity — no ECC CDC mapping |
| `NetPriceAmount` |  |  |  | `Decimal(34,4)` |  | Net Order Price | DocumentCurrency |  | S/4 only entity — no ECC CDC mapping |
| `NetAmount` |  |  |  | `Decimal(34,4)` |  | Net Order Value | DocumentCurrency |  | S/4 only entity — no ECC CDC mapping |
| `LocalCurrency` |  |  |  | `String(5)` |  | Currency |  |  | S/4 only entity — no ECC CDC mapping |
| `NetPriceQuantity` |  |  |  | `Decimal(5,0)` |  | Price Unit | OrderPriceUnit |  | S/4 only entity — no ECC CDC mapping |
| `OrderPriceUnit` |  |  |  | `String(3)` |  | Order Price Unit |  |  | S/4 only entity — no ECC CDC mapping |
| `RequisitionerName` |  |  |  | `String(12)` |  | Requisitioner |  |  | S/4 only entity — no ECC CDC mapping |
| `RetailPromotion` |  |  |  | `String(10)` |  | Retail Promotion |  |  | S/4 only entity — no ECC CDC mapping |
| `IsCompletelyDelivered` |  |  |  | `Boolean` |  | Delivery Completed |  |  | S/4 only entity — no ECC CDC mapping |
| `IsReturnsItem` |  |  |  | `Boolean` |  | Returns Item |  |  | S/4 only entity — no ECC CDC mapping |
| `IsFinallyInvoiced` |  |  |  | `Boolean` |  | Final Invoice |  |  | S/4 only entity — no ECC CDC mapping |
| `InvoiceIsExpected` |  |  |  | `Boolean` |  | Invoice Receipt |  |  | S/4 only entity — no ECC CDC mapping |
| `OrderItemQtyToBaseQtyDnmntr` |  |  |  | `Decimal(5,0)` |  | Denominator |  |  | S/4 only entity — no ECC CDC mapping |
| `OrderItemQtyToBaseQtyNmrtr` |  |  |  | `Decimal(5,0)` |  | Numerator |  |  | S/4 only entity — no ECC CDC mapping |
| `InvoiceIsGoodsReceiptBased` |  |  |  | `Boolean` |  | GR-Based Inv. Verif. |  |  | S/4 only entity — no ECC CDC mapping |
| `GoodsReceiptIsExpected` |  |  |  | `Boolean` |  | Goods Receipt |  |  | S/4 only entity — no ECC CDC mapping |
| `EvaldRcptSettlmtIsAllowed` |  |  |  | `Boolean` |  | Eval. Receipt Sett. |  |  | S/4 only entity — no ECC CDC mapping |
| `AccountAssignmentCategory` |  |  |  | `String(1)` |  | Acct Assignment Cat. |  |  | S/4 only entity — no ECC CDC mapping |
| `GoodsReceiptIsNonValuated` |  |  |  | `Boolean` |  | GR Non-Valuated |  |  | S/4 only entity — no ECC CDC mapping |
| `MaterialType` |  |  |  | `String(4)` |  | Material Type |  |  | S/4 only entity — no ECC CDC mapping |
| `OverdelivTolrtdLmtRatioInPct` |  |  |  | `Decimal(3,1)` |  | Overdeliv. Tolerance |  |  | S/4 only entity — no ECC CDC mapping |
| `ServicePerformer` |  |  |  | `String(10)` |  | Service Performer |  |  | S/4 only entity — no ECC CDC mapping |
| `TaxCode` |  |  |  | `String(2)` |  | Tax Code |  |  | S/4 only entity — no ECC CDC mapping |
| `UnderdelivTolrtdLmtRatioInPct` |  |  |  | `Decimal(3,1)` |  | Underdel. Tolerance |  |  | S/4 only entity — no ECC CDC mapping |
| `UnlimitedOverdeliveryIsAllowed` |  |  |  | `Boolean` |  | Unltd Overdelivery |  |  | S/4 only entity — no ECC CDC mapping |
| `SupplierMaterialNumber` |  |  |  | `String(35)` |  | Supplier Mat. No. |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductTypeCode` |  |  |  | `String(2)` |  | Product Type Group |  |  | S/4 only entity — no ECC CDC mapping |
| `CreatedByUser` |  |  |  | `String(12)` |  | Created By |  |  | S/4 only entity — no ECC CDC mapping |
| `ExpectedOverallLimitAmount` |  |  |  | `Decimal(34,4)` |  | Expected Value | DocumentCurrency |  | S/4 only entity — no ECC CDC mapping |
| `OverallLimitAmount` |  |  |  | `Decimal(34,4)` |  | Overall Limit | DocumentCurrency |  | S/4 only entity — no ECC CDC mapping |
| `RequirementSegment` |  |  |  | `String(40)` |  | Requirement Segment |  |  | S/4 only entity — no ECC CDC mapping |
| `ReleaseIsNotCompleted` |  |  |  | `Boolean` |  | Subject to Release |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchasingCompletenessStatus` |  |  |  | `Boolean` |  | Incomplete |  |  | S/4 only entity — no ECC CDC mapping |
| `IsStatisticalItem` |  |  |  | `Boolean` |  | Statistical |  |  | S/4 only entity — no ECC CDC mapping |
| `MultipleAcctAssgmtDistribution` |  |  |  | `String(1)` |  | Distribut. Indicator |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchaseRequisition` |  |  |  | `String(10)` |  | Purchase Requisition |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchaseRequisitionItem` |  |  |  | `String(5)` |  | Item of requisition |  |  | S/4 only entity — no ECC CDC mapping |
| `SupplierConfirmationControlKey` |  |  |  | `String(4)` |  | Confirmation Control |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchasingDocumentDeletionCode` |  |  |  | `String(1)` |  | Deletion Code |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `PurchaseOrderScheduleLine`

- **ABAP Name:** `C_PurOrdScheduleLineDEX`
- **Label:** Data Extraction for Purchase Order Schedule Lines
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `PurchaseOrder` |  |  |  | `String(10)` | Y | Purchasing Document |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchaseOrderItem` |  |  |  | `String(5)` | Y | Item |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchaseOrderScheduleLine` |  |  |  | `String(4)` | Y | Schedule Line |  |  | S/4 only entity — no ECC CDC mapping |
| `ScheduleLineDeliveryDate` |  |  |  | `Date` |  | Delivery Date |  |  | S/4 only entity — no ECC CDC mapping |
| `SchedLineStscDeliveryDate` |  |  |  | `Date` |  | Stat.-Rel. Del. Date |  |  | S/4 only entity — no ECC CDC mapping |
| `ScheduleLineDeliveryTime` |  |  |  | `String(6)` |  | Time |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchaseRequisition` |  |  |  | `String(10)` |  | Purchase Requisition |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchaseRequisitionItem` |  |  |  | `String(5)` |  | Item of requisition |  |  | S/4 only entity — no ECC CDC mapping |
| `Batch` |  |  |  | `String(10)` |  | Batch |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchasingSchdLnNrOfReminders` |  |  |  | `Decimal(3,0)` |  | No. Rem./Expediters |  |  | S/4 only entity — no ECC CDC mapping |
| `RequisitionerName` |  |  |  | `String(12)` |  | Requisitioner |  |  | S/4 only entity — no ECC CDC mapping |
| `RetailPromotion` |  |  |  | `String(10)` |  | Retail Promotion |  |  | S/4 only entity — no ECC CDC mapping |
| `ArticleCategory` |  |  |  | `String(2)` |  | Material Category |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchasingOrderReason` |  |  |  | `String(3)` |  | Reason for Ordering |  |  | S/4 only entity — no ECC CDC mapping |
| `IsCompletelyDelivered` |  |  |  | `Boolean` |  | Delivery Completed |  |  | S/4 only entity — no ECC CDC mapping |
| `ManufacturerMaterial` |  |  |  | `String(40)` |  | Material |  |  | S/4 only entity — no ECC CDC mapping |
| `IsFinallyInvoiced` |  |  |  | `Boolean` |  | Final Invoice |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchaseContract` |  |  |  | `String(10)` |  | Outline agreement |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchaseContractItem` |  |  |  | `String(5)` |  | Agreement Item |  |  | S/4 only entity — no ECC CDC mapping |
| `StorageLocation` |  |  |  | `String(4)` |  | Storage Location |  |  | S/4 only entity — no ECC CDC mapping |
| `BaseUnit` |  |  |  | `String(3)` |  | Base Unit of Measure |  |  | S/4 only entity — no ECC CDC mapping |
| `MaterialGroup` |  |  |  | `String(9)` |  | Material Group |  |  | S/4 only entity — no ECC CDC mapping |
| `Material` |  |  |  | `String(40)` |  | Material |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchaseOrderQuantityUnit` |  |  |  | `String(3)` |  | Order Unit |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchaseOrderItemCategory` |  |  |  | `String(1)` |  | Item Category |  |  | S/4 only entity — no ECC CDC mapping |
| `IssuingStorageLocation` |  |  |  | `String(4)` |  | Issuing Storage Loc. |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchaseOrderItemText` |  |  |  | `String(40)` |  | Short Text |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchasingParentItem` |  |  |  | `String(5)` |  | Higher-Level Item |  |  | S/4 only entity — no ECC CDC mapping |
| `OrderItemQtyToBaseQtyDnmntr` |  |  |  | `Decimal(5,0)` |  | Denominator |  |  | S/4 only entity — no ECC CDC mapping |
| `OrderItemQtyToBaseQtyNmrtr` |  |  |  | `Decimal(5,0)` |  | Numerator |  |  | S/4 only entity — no ECC CDC mapping |
| `InvoiceIsGoodsReceiptBased` |  |  |  | `Boolean` |  | GR-Based Inv. Verif. |  |  | S/4 only entity — no ECC CDC mapping |
| `GoodsReceiptIsExpected` |  |  |  | `Boolean` |  | Goods Receipt |  |  | S/4 only entity — no ECC CDC mapping |
| `Plant` |  |  |  | `String(4)` |  | Plant |  |  | S/4 only entity — no ECC CDC mapping |
| `EvaldRcptSettlmtIsAllowed` |  |  |  | `Boolean` |  | Eval. Receipt Sett. |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchaseOrderDate` |  |  |  | `Date` |  | Purchase Order Date |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchaseOrderType` |  |  |  | `String(4)` |  | Purchasing Doc. Type |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchasingGroup` |  |  |  | `String(3)` |  | Purchasing Group |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchasingOrganization` |  |  |  | `String(4)` |  | Purch. Organization |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityStartDate` |  |  |  | `Date` |  | Validity Per. Start |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityEndDate` |  |  |  | `Date` |  | Validity Period End |  |  | S/4 only entity — no ECC CDC mapping |
| `Supplier` |  |  |  | `String(10)` |  | Supplier |  |  | S/4 only entity — no ECC CDC mapping |
| `InvoicingParty` |  |  |  | `String(10)` |  | Invoicing Party |  |  | S/4 only entity — no ECC CDC mapping |
| `SupplyingSupplier` |  |  |  | `String(10)` |  | Goods Supplier |  |  | S/4 only entity — no ECC CDC mapping |
| `SupplyingPlant` |  |  |  | `String(4)` |  | Supplying Plant |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchasingDocumentOrigin` |  |  |  | `String(1)` |  | Status |  |  | S/4 only entity — no ECC CDC mapping |
| `DocumentCurrency` |  |  |  | `String(5)` |  | Currency |  |  | S/4 only entity — no ECC CDC mapping |
| `ExchangeRate` |  |  |  | `Decimal(9,5)` |  | Exchange Rate |  |  | S/4 only entity — no ECC CDC mapping |
| `DelivDateCategory` |  |  |  | `String(1)` |  | Deliv. date category |  |  | S/4 only entity — no ECC CDC mapping |
| `ScheduleLineOrderQuantity` |  |  |  | `Decimal(13,3)` |  | Scheduled Quantity | PurchaseOrderQuantityUnit |  | S/4 only entity — no ECC CDC mapping |
| `PrevDelivQtyOfScheduleLine` |  |  |  | `Decimal(13,3)` |  | Previous Quantity | PurchaseOrderQuantityUnit |  | S/4 only entity — no ECC CDC mapping |
| `RoughGoodsReceiptQty` |  |  |  | `Decimal(13,3)` |  | Quantity Delivered | PurchaseOrderQuantityUnit |  | S/4 only entity — no ECC CDC mapping |
| `ScheduleLineIssuedQuantity` |  |  |  | `Decimal(13,3)` |  | Issued Quantity | PurchaseOrderQuantityUnit |  | S/4 only entity — no ECC CDC mapping |
| `SourceOfCreation` |  |  |  | `String(1)` |  | Creation indicator |  |  | S/4 only entity — no ECC CDC mapping |
| `Reservation` |  |  |  | `String(10)` |  | Reservation |  |  | S/4 only entity — no ECC CDC mapping |
| `ScheduleLineIsFixed` |  |  |  | `Boolean` |  | Fixing Indicator |  |  | S/4 only entity — no ECC CDC mapping |
| `StockTransferDeliveredQuantity` |  |  |  | `Decimal(13,3)` |  | Qty Delivered | PurchaseOrderQuantityUnit |  | S/4 only entity — no ECC CDC mapping |
| `ScheduleLineCommittedQuantity` |  |  |  | `Decimal(13,3)` |  | Committed Quantity | PurchaseOrderQuantityUnit |  | S/4 only entity — no ECC CDC mapping |
| `ProductAvailabilityDate` |  |  |  | `Date` |  | Material Avail. Date |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductAvailabilityTime` |  |  |  | `String(6)` |  | Matl Staging Time |  |  | S/4 only entity — no ECC CDC mapping |
| `LoadingDate` |  |  |  | `Date` |  | Loading Date |  |  | S/4 only entity — no ECC CDC mapping |
| `LoadingTime` |  |  |  | `String(6)` |  | Loading Time |  |  | S/4 only entity — no ECC CDC mapping |
| `TransportationPlanningDate` |  |  |  | `Date` |  | Transptn Plang Date |  |  | S/4 only entity — no ECC CDC mapping |
| `TransportationPlanningTime` |  |  |  | `String(6)` |  | Transp. Plan. Time |  |  | S/4 only entity — no ECC CDC mapping |
| `GoodsIssueDate` |  |  |  | `Date` |  | Goods Issue Date |  |  | S/4 only entity — no ECC CDC mapping |
| `GoodsIssueTime` |  |  |  | `String(6)` |  | Goods Issue Time |  |  | S/4 only entity — no ECC CDC mapping |
| `STOLatestPossibleGRDate` |  |  |  | `Date` |  | GR End Date |  |  | S/4 only entity — no ECC CDC mapping |
| `STOLatestPossibleGRTime` |  |  |  | `String(6)` |  | GR End Time |  |  | S/4 only entity — no ECC CDC mapping |
| `OpenPurchaseOrderNetAmount` |  |  |  | `Decimal(34,4)` |  |  | DocumentCurrency |  | S/4 only entity — no ECC CDC mapping |
| `IsReturnsItem` |  |  |  | `Boolean` |  | Returns Item |  |  | S/4 only entity — no ECC CDC mapping |
| `CompanyCode` |  |  |  | `String(4)` |  | Company Code |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductTypeCode` |  |  |  | `String(2)` |  | Product Type Group |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchasingDocumentDeletionCode` |  |  |  | `String(1)` |  | Deletion Code |  |  | S/4 only entity — no ECC CDC mapping |
| `PurgDocumentItemDeletionCode` |  |  |  | `String(1)` |  | Deletion Indicator |  |  | S/4 only entity — no ECC CDC mapping |
| `ReleaseIsNotCompleted` |  |  |  | `Boolean` |  | Subject to Release |  |  | S/4 only entity — no ECC CDC mapping |
| `PurchasingCompletenessStatus` |  |  |  | `Boolean` |  | Incomplete |  |  | S/4 only entity — no ECC CDC mapping |
| `SupplierConfirmationControlKey` |  |  |  | `String(4)` |  | Confirmation Control |  |  | S/4 only entity — no ECC CDC mapping |
| `IsStatisticalItem` |  |  |  | `Boolean` |  | Statistical |  |  | S/4 only entity — no ECC CDC mapping |
| `ScheduleLineOpenQuantity` |  |  |  | `Decimal(14,3)` |  |  | PurchaseOrderQuantityUnit |  | S/4 only entity — no ECC CDC mapping |
