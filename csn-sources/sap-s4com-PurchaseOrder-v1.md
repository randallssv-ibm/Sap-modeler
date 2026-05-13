# PurchaseOrder

> Source file: `sap-s4com-PurchaseOrder-v1.json`


## Entity: `PurOrdSupplierConfirmation`

- **ABAP Name:** `C_POSupplierConfirmationDEX`
- **Label:** Purchase Order Supplier Confirmation DEX
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `PurchaseOrder` | `PurchaseOrder` | `String(10)` | Y | Purchase Order |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchaseOrderItem` | `PurchaseOrderItem` | `String(5)` | Y | Purchase Order Item |  |  | S/4 only entity (no ECC CDC mapping) |
| `SequentialNmbrOfSuplrConf` | `SequentialNmbrOfSuplrConf` | `String(4)` | Y | Sequential Number |  |  | S/4 only entity (no ECC CDC mapping) |
| `SupplierConfirmationCategory` | `SupplierConfirmationCategory` | `String(2)` |  | Confirm. Category |  |  | S/4 only entity (no ECC CDC mapping) |
| `DeliveryDate` | `DeliveryDate` | `Date` |  | Delivery Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `DelivDateCategory` | `DelivDateCategory` | `String(1)` |  | Deliv. Date Category |  |  | S/4 only entity (no ECC CDC mapping) |
| `DeliveryTime` | `DeliveryTime` | `String(6)` |  | Time |  |  | S/4 only entity (no ECC CDC mapping) |
| `CreationDate` | `CreationDate` | `Date` |  | Creation Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `CreationTime` | `CreationTime` | `String(6)` |  | Creation Time |  |  | S/4 only entity (no ECC CDC mapping) |
| `ConfirmedQuantity` | `ConfirmedQuantity` | `Decimal(13,3)` |  | Quantity | OrderQuantityUnit |  | S/4 only entity (no ECC CDC mapping) |
| `MRPRelevantQuantity` | `MRPRelevantQuantity` | `Decimal(13,3)` |  | Qty Reduced (MRP) | OrderQuantityUnit |  | S/4 only entity (no ECC CDC mapping) |
| `SuplrConfCreationCategory` | `SuplrConfCreationCategory` | `String(1)` |  | Creation Indicator |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsDeleted` | `IsDeleted` | `String(1)` |  | Deletion Indicator |  |  | S/4 only entity (no ECC CDC mapping) |
| `ConfIsRelevantToMRP` | `ConfIsRelevantToMRP` | `Boolean` |  | MRP-Relevant |  |  | S/4 only entity (no ECC CDC mapping) |
| `SupplierConfirmationExtNumber` | `SupplierConfirmationExtNumber` | `String(35)` |  | Reference |  |  | S/4 only entity (no ECC CDC mapping) |
| `DeliveryDocument` | `DeliveryDocument` | `String(10)` |  | Delivery |  |  | S/4 only entity (no ECC CDC mapping) |
| `DeliveryDocumentItem` | `DeliveryDocumentItem` | `String(6)` |  | Item |  |  | S/4 only entity (no ECC CDC mapping) |
| `ManufacturerPartProfile` | `ManufacturerPartProfile` | `String(4)` |  | Mfr Part Profile |  |  | S/4 only entity (no ECC CDC mapping) |
| `ManufacturerMaterial` | `ManufacturerMaterial` | `String(40)` |  | MPN: Material |  |  | S/4 only entity (no ECC CDC mapping) |
| `NumberOfReminders` | `NumberOfReminders` | `Decimal(3,0)` |  | No. Rem./Expediters |  |  | S/4 only entity (no ECC CDC mapping) |
| `Batch` | `Batch` | `String(10)` |  | Batch |  |  | S/4 only entity (no ECC CDC mapping) |
| `DeliveryIsInPlant` | `DeliveryIsInPlant` | `Boolean` |  | In Plant |  |  | S/4 only entity (no ECC CDC mapping) |
| `HandoverDate` | `HandoverDate` | `Date` |  | Handover Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `HandoverTime` | `HandoverTime` | `String(6)` |  | Handover Time |  |  | S/4 only entity (no ECC CDC mapping) |
| `PerformancePeriodStartDate` | `PerformancePeriodStartDate` | `Date` |  | Start Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `PerformancePeriodEndDate` | `PerformancePeriodEndDate` | `Date` |  | End Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `ServicePerformer` | `ServicePerformer` | `String(10)` |  | Service Performer |  |  | S/4 only entity (no ECC CDC mapping) |
| `OrderQuantityUnit` | `OrderQuantityUnit` | `String(3)` |  | Order Unit |  |  | S/4 only entity (no ECC CDC mapping) |
| `SupplierConfirmation` | `SupplierConfirmation` | `String(10)` |  | Confirmation |  |  | S/4 only entity (no ECC CDC mapping) |
| `SupplierConfirmationItem` | `SupplierConfirmationItem` | `String(5)` |  | Confirmation Item |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchaseOrderType` | `PurchaseOrderType` | `String(4)` |  | Purchasing Doc. Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchasingOrganization` | `PurchasingOrganization` | `String(4)` |  | Purch. Organization |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchasingGroup` | `PurchasingGroup` | `String(3)` |  | Purchasing Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `Plant` | `Plant` | `String(4)` |  | Plant |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `PurchaseOrder`

- **ABAP Name:** `C_PurchaseOrderDEX`
- **Label:** Data Extraction for Purchase Order
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `PurchaseOrder` | `PurchaseOrder` | `String(10)` | Y | Purchase Order |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchaseOrderType` | `PurchaseOrderType` | `String(4)` |  | Purchasing Doc. Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchaseOrderSubtype` | `PurchaseOrderSubtype` | `String(1)` |  | Control indicator |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchasingDocumentOrigin` | `PurchasingDocumentOrigin` | `String(1)` |  | Status |  |  | S/4 only entity (no ECC CDC mapping) |
| `CreatedByUser` | `CreatedByUser` | `String(12)` |  | Created By |  |  | S/4 only entity (no ECC CDC mapping) |
| `CreationDate` | `CreationDate` | `Date` |  | Created On |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchaseOrderDate` | `PurchaseOrderDate` | `Date` |  | Purchase Order Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `Language` | `Language` | `String(2)` |  | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `CorrespncExternalReference` | `CorrespncExternalReference` | `String(12)` |  | Your Reference |  |  | S/4 only entity (no ECC CDC mapping) |
| `CorrespncInternalReference` | `CorrespncInternalReference` | `String(12)` |  | Our Reference |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchasingDocumentDeletionCode` | `PurchasingDocumentDeletionCode` | `String(1)` |  | Deletion Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `ReleaseIsNotCompleted` | `ReleaseIsNotCompleted` | `Boolean` |  | Subject to Release |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchasingCompletenessStatus` | `PurchasingCompletenessStatus` | `Boolean` |  | Incomplete |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchasingProcessingStatus` | `PurchasingProcessingStatus` | `String(2)` |  | Proc. State |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurgReleaseSequenceStatus` | `PurgReleaseSequenceStatus` | `String(8)` |  | Release Status |  |  | S/4 only entity (no ECC CDC mapping) |
| `ReleaseCode` | `ReleaseCode` | `String(1)` |  | Release indicator |  |  | S/4 only entity (no ECC CDC mapping) |
| `CompanyCode` | `CompanyCode` | `String(4)` |  | Company Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchasingOrganization` | `PurchasingOrganization` | `String(4)` |  | Purch. Organization |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchasingGroup` | `PurchasingGroup` | `String(3)` |  | Purchasing Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `Supplier` | `Supplier` | `String(10)` |  | Supplier |  |  | S/4 only entity (no ECC CDC mapping) |
| `ManualSupplierAddressID` | `ManualSupplierAddressID` | `String(10)` |  | Address Number |  |  | S/4 only entity (no ECC CDC mapping) |
| `SupplierRespSalesPersonName` | `SupplierRespSalesPersonName` | `String(30)` |  | Salesperson |  |  | S/4 only entity (no ECC CDC mapping) |
| `SupplierPhoneNumber` | `SupplierPhoneNumber` | `String(16)` |  | Supplier Phone |  |  | S/4 only entity (no ECC CDC mapping) |
| `SupplyingSupplier` | `SupplyingSupplier` | `String(10)` |  | Goods Supplier |  |  | S/4 only entity (no ECC CDC mapping) |
| `SupplyingPlant` | `SupplyingPlant` | `String(4)` |  | Supplying Plant |  |  | S/4 only entity (no ECC CDC mapping) |
| `InvoicingParty` | `InvoicingParty` | `String(10)` |  | Invoicing Party |  |  | S/4 only entity (no ECC CDC mapping) |
| `Customer` | `Customer` | `String(10)` |  | Customer |  |  | S/4 only entity (no ECC CDC mapping) |
| `SupplierQuotationExternalID` | `SupplierQuotationExternalID` | `String(10)` |  | Quotation |  |  | S/4 only entity (no ECC CDC mapping) |
| `PaymentTerms` | `PaymentTerms` | `String(4)` |  | Payment Terms |  |  | S/4 only entity (no ECC CDC mapping) |
| `CashDiscount1Days` | `CashDiscount1Days` | `Decimal(3,0)` |  | Days 1 |  |  | S/4 only entity (no ECC CDC mapping) |
| `CashDiscount2Days` | `CashDiscount2Days` | `Decimal(3,0)` |  | Days 2 |  |  | S/4 only entity (no ECC CDC mapping) |
| `NetPaymentDays` | `NetPaymentDays` | `Decimal(3,0)` |  | Days Net |  |  | S/4 only entity (no ECC CDC mapping) |
| `CashDiscount1Percent` | `CashDiscount1Percent` | `Decimal(5,3)` |  | CD Percentage 1 |  |  | S/4 only entity (no ECC CDC mapping) |
| `CashDiscount2Percent` | `CashDiscount2Percent` | `Decimal(5,3)` |  | CD Percentage 2 |  |  | S/4 only entity (no ECC CDC mapping) |
| `DownPaymentType` | `DownPaymentType` | `String(4)` |  | Down Payment |  |  | S/4 only entity (no ECC CDC mapping) |
| `DownPaymentPercentageOfTotAmt` | `DownPaymentPercentageOfTotAmt` | `Decimal(5,2)` |  | Down Payment % |  |  | S/4 only entity (no ECC CDC mapping) |
| `DownPaymentAmount` | `DownPaymentAmount` | `Decimal(34,4)` |  | Down Payment Amount | DocumentCurrency |  | S/4 only entity (no ECC CDC mapping) |
| `DownPaymentDueDate` | `DownPaymentDueDate` | `Date` |  | Due Date for DP |  |  | S/4 only entity (no ECC CDC mapping) |
| `IncotermsClassification` | `IncotermsClassification` | `String(3)` |  | Incoterms |  |  | S/4 only entity (no ECC CDC mapping) |
| `IncotermsTransferLocation` | `IncotermsTransferLocation` | `String(28)` |  | Incoterms (Part 2) |  |  | S/4 only entity (no ECC CDC mapping) |
| `IncotermsVersion` | `IncotermsVersion` | `String(4)` |  | Incoterms Version |  |  | S/4 only entity (no ECC CDC mapping) |
| `IncotermsLocation1` | `IncotermsLocation1` | `String(70)` |  | Incoterms Location 1 |  |  | S/4 only entity (no ECC CDC mapping) |
| `IncotermsLocation2` | `IncotermsLocation2` | `String(70)` |  | Incoterms Location 2 |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsIntrastatReportingRelevant` | `IsIntrastatReportingRelevant` | `Boolean` |  | Intrastat Relevance |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsIntrastatReportingExcluded` | `IsIntrastatReportingExcluded` | `Boolean` |  | Intrastat Exclusion |  |  | S/4 only entity (no ECC CDC mapping) |
| `PricingDocument` | `PricingDocument` | `String(10)` |  | Doc. Condition No. |  |  | S/4 only entity (no ECC CDC mapping) |
| `PricingProcedure` | `PricingProcedure` | `String(6)` |  | Procedure |  |  | S/4 only entity (no ECC CDC mapping) |
| `DocumentCurrency` | `DocumentCurrency` | `String(5)` |  | Currency |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityStartDate` | `ValidityStartDate` | `Date` |  | Validity Per. Start |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityEndDate` | `ValidityEndDate` | `Date` |  | Validity Period End |  |  | S/4 only entity (no ECC CDC mapping) |
| `ExchangeRate` | `ExchangeRate` | `Decimal(9,5)` |  | Exchange Rate |  |  | S/4 only entity (no ECC CDC mapping) |
| `ExchangeRateIsFixed` | `ExchangeRateIsFixed` | `Boolean` |  | Fixed Exchange Rate |  |  | S/4 only entity (no ECC CDC mapping) |
| `LastChangeDateTime` | `LastChangeDateTime` | `Timestamp` |  | Last Changed |  |  | S/4 only entity (no ECC CDC mapping) |
| `TaxReturnCountry` | `TaxReturnCountry` | `String(3)` |  | Reporting C/R |  |  | S/4 only entity (no ECC CDC mapping) |
| `VATRegistrationCountry` | `VATRegistrationCountry` | `String(3)` |  | Ctry/Rgn Sls Tax No. |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurgReasonForDocCancellation` | `PurgReasonForDocCancellation` | `String(2)` |  | Reason for Canc. |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurgReleaseTimeTotalAmount` | `PurgReleaseTimeTotalAmount` | `Decimal(34,4)` |  | Tot. val. rel. | DocumentCurrency |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `PurchaseOrderAccountAssignment`

- **ABAP Name:** `C_PurOrdAccountAssignmentDEX`
- **Label:** Data Extraction for Purchase Order Account Assignments
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `PurchaseOrder` | `PurchaseOrder` | `String(10)` | Y | Purchasing Document |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchaseOrderItem` | `PurchaseOrderItem` | `String(5)` | Y | Item |  |  | S/4 only entity (no ECC CDC mapping) |
| `AccountAssignmentNumber` | `AccountAssignmentNumber` | `String(2)` | Y | Account Assgmt No. |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCenter` | `CostCenter` | `String(10)` |  | Cost Center |  |  | S/4 only entity (no ECC CDC mapping) |
| `MasterFixedAsset` | `MasterFixedAsset` | `String(12)` |  | Asset |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProjectNetwork` | `ProjectNetwork` | `String(12)` |  | Network |  |  | S/4 only entity (no ECC CDC mapping) |
| `Quantity` | `Quantity` | `Decimal(13,3)` |  | Quantity | PurchaseOrderQuantityUnit |  | S/4 only entity (no ECC CDC mapping) |
| `PurchaseOrderQuantityUnit` | `PurchaseOrderQuantityUnit` | `String(3)` |  | Order Unit |  |  | S/4 only entity (no ECC CDC mapping) |
| `MultipleAcctAssgmtDistrPercent` | `MultipleAcctAssgmtDistrPercent` | `Decimal(3,1)` |  | Distribution (%) |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurgDocNetAmount` | `PurgDocNetAmount` | `Decimal(34,4)` |  | Net Order Value | DocumentCurrency |  | S/4 only entity (no ECC CDC mapping) |
| `DocumentCurrency` | `DocumentCurrency` | `String(5)` |  | Currency |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsDeleted` | `IsDeleted` | `Boolean` |  | Deletion Indicator |  |  | S/4 only entity (no ECC CDC mapping) |
| `GLAccount` | `GLAccount` | `String(10)` |  | G/L Account |  |  | S/4 only entity (no ECC CDC mapping) |
| `BusinessArea` | `BusinessArea` | `String(4)` |  | Business Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `SalesOrder` | `SalesOrder` | `String(10)` |  | SD Document |  |  | S/4 only entity (no ECC CDC mapping) |
| `SalesOrderItem` | `SalesOrderItem` | `String(6)` |  | Item |  |  | S/4 only entity (no ECC CDC mapping) |
| `SalesOrderScheduleLine` | `SalesOrderScheduleLine` | `String(4)` |  | Schedule Line Number |  |  | S/4 only entity (no ECC CDC mapping) |
| `FixedAsset` | `FixedAsset` | `String(4)` |  | Subnumber |  |  | S/4 only entity (no ECC CDC mapping) |
| `OrderID` | `OrderID` | `String(12)` |  | Order |  |  | S/4 only entity (no ECC CDC mapping) |
| `UnloadingPointName` | `UnloadingPointName` | `String(25)` |  | Unloading Point |  |  | S/4 only entity (no ECC CDC mapping) |
| `ControllingArea` | `ControllingArea` | `String(4)` |  | Controlling Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostObject` | `CostObject` | `String(12)` |  | Cost Object |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProfitabilitySegment` | `ProfitabilitySegment` | `String(10)` |  | Profitability Segment (Deprecated) |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProfitabilitySegment_2` | `ProfitabilitySegment_2` | `String(10)` |  | Profitability Segment |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProfitCenter` | `ProfitCenter` | `String(10)` |  | Profit Center |  |  | S/4 only entity (no ECC CDC mapping) |
| `WBSElementInternalID` | `WBSElementInternalID` | `String(8)` |  | WBS Internal ID |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProjectNetworkInternalID` | `ProjectNetworkInternalID` | `String(10)` |  | Opertn Task List No. |  |  | S/4 only entity (no ECC CDC mapping) |
| `CommitmentItem` | `CommitmentItem` | `String(24)` |  |  |  |  | S/4 only entity (no ECC CDC mapping) |
| `FundsCenter` | `FundsCenter` | `String(16)` |  | Funds Center |  |  | S/4 only entity (no ECC CDC mapping) |
| `Fund` | `Fund` | `String(10)` |  | Fund |  |  | S/4 only entity (no ECC CDC mapping) |
| `FunctionalArea` | `FunctionalArea` | `String(16)` |  | Functional Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `GoodsRecipientName` | `GoodsRecipientName` | `String(12)` |  | Goods Recipient |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsFinallyInvoiced` | `IsFinallyInvoiced` | `Boolean` |  | Final Invoice |  |  | S/4 only entity (no ECC CDC mapping) |
| `RealEstateObject` | `RealEstateObject` | `String(8)` |  | Real Estate Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `NetworkActivityInternalID` | `NetworkActivityInternalID` | `String(8)` |  | Counter |  |  | S/4 only entity (no ECC CDC mapping) |
| `PartnerAccountNumber` | `PartnerAccountNumber` | `String(10)` |  | Partner |  |  | S/4 only entity (no ECC CDC mapping) |
| `JointVentureRecoveryCode` | `JointVentureRecoveryCode` | `String(2)` |  | Recovery Indicator |  |  | S/4 only entity (no ECC CDC mapping) |
| `SettlementReferenceDate` | `SettlementReferenceDate` | `Date` |  | Reference Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `OrderInternalID` | `OrderInternalID` | `String(10)` |  | Opertn Task List No. |  |  | S/4 only entity (no ECC CDC mapping) |
| `OrderIntBillOfOperationsItem` | `OrderIntBillOfOperationsItem` | `String(8)` |  | Counter |  |  | S/4 only entity (no ECC CDC mapping) |
| `TaxCode` | `TaxCode` | `String(2)` |  | Tax Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `TaxJurisdiction` | `TaxJurisdiction` | `String(15)` |  | Tax Jurisdiction |  |  | S/4 only entity (no ECC CDC mapping) |
| `NonDeductibleInputTaxAmount` | `NonDeductibleInputTaxAmount` | `Decimal(34,4)` |  | Non-deductible | DocumentCurrency |  | S/4 only entity (no ECC CDC mapping) |
| `CostCtrActivityType` | `CostCtrActivityType` | `String(6)` |  | Activity Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `BusinessProcess` | `BusinessProcess` | `String(12)` |  | Business Process |  |  | S/4 only entity (no ECC CDC mapping) |
| `GrantID` | `GrantID` | `String(20)` |  | Grant |  |  | S/4 only entity (no ECC CDC mapping) |
| `BudgetPeriod` | `BudgetPeriod` | `String(10)` |  | Budget Period |  |  | S/4 only entity (no ECC CDC mapping) |
| `EarmarkedFundsDocument` | `EarmarkedFundsDocument` | `String(10)` |  | Earmarked Funds |  |  | S/4 only entity (no ECC CDC mapping) |
| `EarmarkedFundsDocumentItem` | `EarmarkedFundsDocumentItem` | `String(3)` |  | Document Item |  |  | S/4 only entity (no ECC CDC mapping) |
| `ServiceDocumentType` | `ServiceDocumentType` | `String(4)` |  | Service Doc. Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `ServiceDocument` | `ServiceDocument` | `String(10)` |  | Service Document |  |  | S/4 only entity (no ECC CDC mapping) |
| `ServiceDocumentItem` | `ServiceDocumentItem` | `String(6)` |  | Service Doc. Item |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchaseOrderType` | `PurchaseOrderType` | `String(4)` |  | Purchasing Doc. Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchasingOrganization` | `PurchasingOrganization` | `String(4)` |  | Purch. Organization |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchasingGroup` | `PurchasingGroup` | `String(3)` |  | Purchasing Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `CreationDate` | `CreationDate` | `Date` |  | Created On |  |  | S/4 only entity (no ECC CDC mapping) |
| `LastChangeDateTime` | `LastChangeDateTime` | `Timestamp` |  | Last Changed |  |  | S/4 only entity (no ECC CDC mapping) |
| `Plant` | `Plant` | `String(4)` |  | Plant |  |  | S/4 only entity (no ECC CDC mapping) |
| `AccountAssignmentCategory` | `AccountAssignmentCategory` | `String(1)` |  | Acct Assignment Cat. |  |  | S/4 only entity (no ECC CDC mapping) |
| `CompanyCode` | `CompanyCode` | `String(4)` |  | Company Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsReturnsItem` | `IsReturnsItem` | `Boolean` |  | Returns Item |  |  | S/4 only entity (no ECC CDC mapping) |
| `SupplyingPlant` | `SupplyingPlant` | `String(4)` |  | Supplying Plant |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchaseOrderItemCategory` | `PurchaseOrderItemCategory` | `String(1)` |  | Item Category |  |  | S/4 only entity (no ECC CDC mapping) |
| `Material` | `Material` | `String(40)` |  | Material |  |  | S/4 only entity (no ECC CDC mapping) |
| `MaterialGroup` | `MaterialGroup` | `String(9)` |  | Material Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchaseOrderDate` | `PurchaseOrderDate` | `Date` |  | Purchase Order Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `StorageLocation` | `StorageLocation` | `String(4)` |  | Storage Location |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsCompletelyDelivered` | `IsCompletelyDelivered` | `Boolean` |  | Delivery Completed |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchasingInfoRecord` | `PurchasingInfoRecord` | `String(10)` |  | Purchasing Info Rec. |  |  | S/4 only entity (no ECC CDC mapping) |
| `RequirementTracking` | `RequirementTracking` | `String(10)` |  | Req. Tracking Number |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchaseOrderItemText` | `PurchaseOrderItemText` | `String(40)` |  | Short Text |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurgDocumentItemDeletionCode` | `PurgDocumentItemDeletionCode` | `String(1)` |  | Deletion Indicator |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchasingDocumentDeletionCode` | `PurchasingDocumentDeletionCode` | `String(1)` |  | Deletion Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `InvoiceIsExpected` | `InvoiceIsExpected` | `Boolean` |  | Invoice Receipt |  |  | S/4 only entity (no ECC CDC mapping) |
| `GoodsReceiptIsExpected` | `GoodsReceiptIsExpected` | `Boolean` |  | Goods Receipt |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductTypeCode` | `ProductTypeCode` | `String(2)` |  | Product Type Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsStatisticalItem` | `IsStatisticalItem` | `Boolean` |  | Statistical |  |  | S/4 only entity (no ECC CDC mapping) |
| `ReleaseIsNotCompleted` | `ReleaseIsNotCompleted` | `Boolean` |  | Subject to Release |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchasingCompletenessStatus` | `PurchasingCompletenessStatus` | `Boolean` |  | Incomplete |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchaseContract` | `PurchaseContract` | `String(10)` |  | Outline agreement |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchaseContractItem` | `PurchaseContractItem` | `String(5)` |  | Agreement Item |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `PurchaseOrderItem`

- **ABAP Name:** `C_PurchaseOrderItemDEX`
- **Label:** Data Extraction View for PO Item
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `PurchaseOrder` | `PurchaseOrder` | `String(10)` | Y | Purchase Order |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchaseOrderItem` | `PurchaseOrderItem` | `String(5)` | Y | Purchase Order Item |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchaseOrderType` | `PurchaseOrderType` | `String(4)` |  | Purchasing Doc. Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchasingGroup` | `PurchasingGroup` | `String(3)` |  | Purchasing Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchasingOrganization` | `PurchasingOrganization` | `String(4)` |  | Purch. Organization |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchasingDocumentOrigin` | `PurchasingDocumentOrigin` | `String(1)` |  | Status |  |  | S/4 only entity (no ECC CDC mapping) |
| `Supplier` | `Supplier` | `String(10)` |  | Supplier |  |  | S/4 only entity (no ECC CDC mapping) |
| `SupplyingSupplier` | `SupplyingSupplier` | `String(10)` |  | Goods Supplier |  |  | S/4 only entity (no ECC CDC mapping) |
| `SupplyingPlant` | `SupplyingPlant` | `String(4)` |  | Supplying Plant |  |  | S/4 only entity (no ECC CDC mapping) |
| `DocumentCurrency` | `DocumentCurrency` | `String(5)` |  | Currency |  |  | S/4 only entity (no ECC CDC mapping) |
| `ExchangeRate` | `ExchangeRate` | `Decimal(9,5)` |  | Exchange Rate |  |  | S/4 only entity (no ECC CDC mapping) |
| `InvoicingParty` | `InvoicingParty` | `String(10)` |  | Invoicing Party |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchaseOrderDate` | `PurchaseOrderDate` | `Date` |  | Purchase Order Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityStartDate` | `ValidityStartDate` | `Date` |  | Validity Per. Start |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityEndDate` | `ValidityEndDate` | `Date` |  | Validity Period End |  |  | S/4 only entity (no ECC CDC mapping) |
| `CreationDate` | `CreationDate` | `Date` |  | Created On |  |  | S/4 only entity (no ECC CDC mapping) |
| `LastChangeDateTime` | `LastChangeDateTime` | `Timestamp` |  | Last Changed |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurgDocumentItemDeletionCode` | `PurgDocumentItemDeletionCode` | `String(1)` |  | Deletion Indicator |  |  | S/4 only entity (no ECC CDC mapping) |
| `MaterialGroup` | `MaterialGroup` | `String(9)` |  | Material Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `Material` | `Material` | `String(40)` |  | Material |  |  | S/4 only entity (no ECC CDC mapping) |
| `ManufacturerMaterial` | `ManufacturerMaterial` | `String(40)` |  | Material |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchaseOrderCategory` | `PurchaseOrderCategory` | `String(1)` |  | Purch. Doc. Category |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchasingOrderReason` | `PurchasingOrderReason` | `String(3)` |  | Reason for Ordering |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchaseOrderItemText` | `PurchaseOrderItemText` | `String(40)` |  | Short Text |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchaseOrderItemCategory` | `PurchaseOrderItemCategory` | `String(1)` |  | Item Category |  |  | S/4 only entity (no ECC CDC mapping) |
| `CompanyCode` | `CompanyCode` | `String(4)` |  | Company Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `Plant` | `Plant` | `String(4)` |  | Plant |  |  | S/4 only entity (no ECC CDC mapping) |
| `StorageLocation` | `StorageLocation` | `String(4)` |  | Storage Location |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchaseContract` | `PurchaseContract` | `String(10)` |  | Outline agreement |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchaseContractItem` | `PurchaseContractItem` | `String(5)` |  | Agreement Item |  |  | S/4 only entity (no ECC CDC mapping) |
| `BaseUnit` | `BaseUnit` | `String(3)` |  | Base Unit of Measure |  |  | S/4 only entity (no ECC CDC mapping) |
| `OrderQuantity` | `OrderQuantity` | `Decimal(13,3)` |  | Order Quantity | PurchaseOrderQuantityUnit |  | S/4 only entity (no ECC CDC mapping) |
| `PurchaseOrderQuantityUnit` | `PurchaseOrderQuantityUnit` | `String(3)` |  | Order Unit |  |  | S/4 only entity (no ECC CDC mapping) |
| `NetPriceAmount` | `NetPriceAmount` | `Decimal(34,4)` |  | Net Order Price | DocumentCurrency |  | S/4 only entity (no ECC CDC mapping) |
| `NetAmount` | `NetAmount` | `Decimal(34,4)` |  | Net Order Value | DocumentCurrency |  | S/4 only entity (no ECC CDC mapping) |
| `LocalCurrency` | `LocalCurrency` | `String(5)` |  | Currency |  |  | S/4 only entity (no ECC CDC mapping) |
| `NetPriceQuantity` | `NetPriceQuantity` | `Decimal(5,0)` |  | Price Unit | OrderPriceUnit |  | S/4 only entity (no ECC CDC mapping) |
| `OrderPriceUnit` | `OrderPriceUnit` | `String(3)` |  | Order Price Unit |  |  | S/4 only entity (no ECC CDC mapping) |
| `RequisitionerName` | `RequisitionerName` | `String(12)` |  | Requisitioner |  |  | S/4 only entity (no ECC CDC mapping) |
| `RetailPromotion` | `RetailPromotion` | `String(10)` |  | Retail Promotion |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsCompletelyDelivered` | `IsCompletelyDelivered` | `Boolean` |  | Delivery Completed |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsReturnsItem` | `IsReturnsItem` | `Boolean` |  | Returns Item |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsFinallyInvoiced` | `IsFinallyInvoiced` | `Boolean` |  | Final Invoice |  |  | S/4 only entity (no ECC CDC mapping) |
| `InvoiceIsExpected` | `InvoiceIsExpected` | `Boolean` |  | Invoice Receipt |  |  | S/4 only entity (no ECC CDC mapping) |
| `OrderItemQtyToBaseQtyDnmntr` | `OrderItemQtyToBaseQtyDnmntr` | `Decimal(5,0)` |  | Denominator |  |  | S/4 only entity (no ECC CDC mapping) |
| `OrderItemQtyToBaseQtyNmrtr` | `OrderItemQtyToBaseQtyNmrtr` | `Decimal(5,0)` |  | Numerator |  |  | S/4 only entity (no ECC CDC mapping) |
| `InvoiceIsGoodsReceiptBased` | `InvoiceIsGoodsReceiptBased` | `Boolean` |  | GR-Based Inv. Verif. |  |  | S/4 only entity (no ECC CDC mapping) |
| `GoodsReceiptIsExpected` | `GoodsReceiptIsExpected` | `Boolean` |  | Goods Receipt |  |  | S/4 only entity (no ECC CDC mapping) |
| `EvaldRcptSettlmtIsAllowed` | `EvaldRcptSettlmtIsAllowed` | `Boolean` |  | Eval. Receipt Sett. |  |  | S/4 only entity (no ECC CDC mapping) |
| `AccountAssignmentCategory` | `AccountAssignmentCategory` | `String(1)` |  | Acct Assignment Cat. |  |  | S/4 only entity (no ECC CDC mapping) |
| `GoodsReceiptIsNonValuated` | `GoodsReceiptIsNonValuated` | `Boolean` |  | GR Non-Valuated |  |  | S/4 only entity (no ECC CDC mapping) |
| `MaterialType` | `MaterialType` | `String(4)` |  | Material Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `OverdelivTolrtdLmtRatioInPct` | `OverdelivTolrtdLmtRatioInPct` | `Decimal(3,1)` |  | Overdeliv. Tolerance |  |  | S/4 only entity (no ECC CDC mapping) |
| `ServicePerformer` | `ServicePerformer` | `String(10)` |  | Service Performer |  |  | S/4 only entity (no ECC CDC mapping) |
| `TaxCode` | `TaxCode` | `String(2)` |  | Tax Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `UnderdelivTolrtdLmtRatioInPct` | `UnderdelivTolrtdLmtRatioInPct` | `Decimal(3,1)` |  | Underdel. Tolerance |  |  | S/4 only entity (no ECC CDC mapping) |
| `UnlimitedOverdeliveryIsAllowed` | `UnlimitedOverdeliveryIsAllowed` | `Boolean` |  | Unltd Overdelivery |  |  | S/4 only entity (no ECC CDC mapping) |
| `SupplierMaterialNumber` | `SupplierMaterialNumber` | `String(35)` |  | Supplier Mat. No. |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductTypeCode` | `ProductTypeCode` | `String(2)` |  | Product Type Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `CreatedByUser` | `CreatedByUser` | `String(12)` |  | Created By |  |  | S/4 only entity (no ECC CDC mapping) |
| `ExpectedOverallLimitAmount` | `ExpectedOverallLimitAmount` | `Decimal(34,4)` |  | Expected Value | DocumentCurrency |  | S/4 only entity (no ECC CDC mapping) |
| `OverallLimitAmount` | `OverallLimitAmount` | `Decimal(34,4)` |  | Overall Limit | DocumentCurrency |  | S/4 only entity (no ECC CDC mapping) |
| `RequirementSegment` | `RequirementSegment` | `String(40)` |  | Requirement Segment |  |  | S/4 only entity (no ECC CDC mapping) |
| `ReleaseIsNotCompleted` | `ReleaseIsNotCompleted` | `Boolean` |  | Subject to Release |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchasingCompletenessStatus` | `PurchasingCompletenessStatus` | `Boolean` |  | Incomplete |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsStatisticalItem` | `IsStatisticalItem` | `Boolean` |  | Statistical |  |  | S/4 only entity (no ECC CDC mapping) |
| `MultipleAcctAssgmtDistribution` | `MultipleAcctAssgmtDistribution` | `String(1)` |  | Distribut. Indicator |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchaseRequisition` | `PurchaseRequisition` | `String(10)` |  | Purchase Requisition |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchaseRequisitionItem` | `PurchaseRequisitionItem` | `String(5)` |  | Item of requisition |  |  | S/4 only entity (no ECC CDC mapping) |
| `SupplierConfirmationControlKey` | `SupplierConfirmationControlKey` | `String(4)` |  | Confirmation Control |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchasingDocumentDeletionCode` | `PurchasingDocumentDeletionCode` | `String(1)` |  | Deletion Code |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `PurchaseOrderScheduleLine`

- **ABAP Name:** `C_PurOrdScheduleLineDEX`
- **Label:** Data Extraction for Purchase Order Schedule Lines
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `PurchaseOrder` | `PurchaseOrder` | `String(10)` | Y | Purchasing Document |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchaseOrderItem` | `PurchaseOrderItem` | `String(5)` | Y | Item |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchaseOrderScheduleLine` | `PurchaseOrderScheduleLine` | `String(4)` | Y | Schedule Line |  |  | S/4 only entity (no ECC CDC mapping) |
| `ScheduleLineDeliveryDate` | `ScheduleLineDeliveryDate` | `Date` |  | Delivery Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `SchedLineStscDeliveryDate` | `SchedLineStscDeliveryDate` | `Date` |  | Stat.-Rel. Del. Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `ScheduleLineDeliveryTime` | `ScheduleLineDeliveryTime` | `String(6)` |  | Time |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchaseRequisition` | `PurchaseRequisition` | `String(10)` |  | Purchase Requisition |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchaseRequisitionItem` | `PurchaseRequisitionItem` | `String(5)` |  | Item of requisition |  |  | S/4 only entity (no ECC CDC mapping) |
| `Batch` | `Batch` | `String(10)` |  | Batch |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchasingSchdLnNrOfReminders` | `PurchasingSchdLnNrOfReminders` | `Decimal(3,0)` |  | No. Rem./Expediters |  |  | S/4 only entity (no ECC CDC mapping) |
| `RequisitionerName` | `RequisitionerName` | `String(12)` |  | Requisitioner |  |  | S/4 only entity (no ECC CDC mapping) |
| `RetailPromotion` | `RetailPromotion` | `String(10)` |  | Retail Promotion |  |  | S/4 only entity (no ECC CDC mapping) |
| `ArticleCategory` | `ArticleCategory` | `String(2)` |  | Material Category |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchasingOrderReason` | `PurchasingOrderReason` | `String(3)` |  | Reason for Ordering |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsCompletelyDelivered` | `IsCompletelyDelivered` | `Boolean` |  | Delivery Completed |  |  | S/4 only entity (no ECC CDC mapping) |
| `ManufacturerMaterial` | `ManufacturerMaterial` | `String(40)` |  | Material |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsFinallyInvoiced` | `IsFinallyInvoiced` | `Boolean` |  | Final Invoice |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchaseContract` | `PurchaseContract` | `String(10)` |  | Outline agreement |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchaseContractItem` | `PurchaseContractItem` | `String(5)` |  | Agreement Item |  |  | S/4 only entity (no ECC CDC mapping) |
| `StorageLocation` | `StorageLocation` | `String(4)` |  | Storage Location |  |  | S/4 only entity (no ECC CDC mapping) |
| `BaseUnit` | `BaseUnit` | `String(3)` |  | Base Unit of Measure |  |  | S/4 only entity (no ECC CDC mapping) |
| `MaterialGroup` | `MaterialGroup` | `String(9)` |  | Material Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `Material` | `Material` | `String(40)` |  | Material |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchaseOrderQuantityUnit` | `PurchaseOrderQuantityUnit` | `String(3)` |  | Order Unit |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchaseOrderItemCategory` | `PurchaseOrderItemCategory` | `String(1)` |  | Item Category |  |  | S/4 only entity (no ECC CDC mapping) |
| `IssuingStorageLocation` | `IssuingStorageLocation` | `String(4)` |  | Issuing Storage Loc. |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchaseOrderItemText` | `PurchaseOrderItemText` | `String(40)` |  | Short Text |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchasingParentItem` | `PurchasingParentItem` | `String(5)` |  | Higher-Level Item |  |  | S/4 only entity (no ECC CDC mapping) |
| `OrderItemQtyToBaseQtyDnmntr` | `OrderItemQtyToBaseQtyDnmntr` | `Decimal(5,0)` |  | Denominator |  |  | S/4 only entity (no ECC CDC mapping) |
| `OrderItemQtyToBaseQtyNmrtr` | `OrderItemQtyToBaseQtyNmrtr` | `Decimal(5,0)` |  | Numerator |  |  | S/4 only entity (no ECC CDC mapping) |
| `InvoiceIsGoodsReceiptBased` | `InvoiceIsGoodsReceiptBased` | `Boolean` |  | GR-Based Inv. Verif. |  |  | S/4 only entity (no ECC CDC mapping) |
| `GoodsReceiptIsExpected` | `GoodsReceiptIsExpected` | `Boolean` |  | Goods Receipt |  |  | S/4 only entity (no ECC CDC mapping) |
| `Plant` | `Plant` | `String(4)` |  | Plant |  |  | S/4 only entity (no ECC CDC mapping) |
| `EvaldRcptSettlmtIsAllowed` | `EvaldRcptSettlmtIsAllowed` | `Boolean` |  | Eval. Receipt Sett. |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchaseOrderDate` | `PurchaseOrderDate` | `Date` |  | Purchase Order Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchaseOrderType` | `PurchaseOrderType` | `String(4)` |  | Purchasing Doc. Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchasingGroup` | `PurchasingGroup` | `String(3)` |  | Purchasing Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchasingOrganization` | `PurchasingOrganization` | `String(4)` |  | Purch. Organization |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityStartDate` | `ValidityStartDate` | `Date` |  | Validity Per. Start |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityEndDate` | `ValidityEndDate` | `Date` |  | Validity Period End |  |  | S/4 only entity (no ECC CDC mapping) |
| `Supplier` | `Supplier` | `String(10)` |  | Supplier |  |  | S/4 only entity (no ECC CDC mapping) |
| `InvoicingParty` | `InvoicingParty` | `String(10)` |  | Invoicing Party |  |  | S/4 only entity (no ECC CDC mapping) |
| `SupplyingSupplier` | `SupplyingSupplier` | `String(10)` |  | Goods Supplier |  |  | S/4 only entity (no ECC CDC mapping) |
| `SupplyingPlant` | `SupplyingPlant` | `String(4)` |  | Supplying Plant |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchasingDocumentOrigin` | `PurchasingDocumentOrigin` | `String(1)` |  | Status |  |  | S/4 only entity (no ECC CDC mapping) |
| `DocumentCurrency` | `DocumentCurrency` | `String(5)` |  | Currency |  |  | S/4 only entity (no ECC CDC mapping) |
| `ExchangeRate` | `ExchangeRate` | `Decimal(9,5)` |  | Exchange Rate |  |  | S/4 only entity (no ECC CDC mapping) |
| `DelivDateCategory` | `DelivDateCategory` | `String(1)` |  | Deliv. date category |  |  | S/4 only entity (no ECC CDC mapping) |
| `ScheduleLineOrderQuantity` | `ScheduleLineOrderQuantity` | `Decimal(13,3)` |  | Scheduled Quantity | PurchaseOrderQuantityUnit |  | S/4 only entity (no ECC CDC mapping) |
| `PrevDelivQtyOfScheduleLine` | `PrevDelivQtyOfScheduleLine` | `Decimal(13,3)` |  | Previous Quantity | PurchaseOrderQuantityUnit |  | S/4 only entity (no ECC CDC mapping) |
| `RoughGoodsReceiptQty` | `RoughGoodsReceiptQty` | `Decimal(13,3)` |  | Quantity Delivered | PurchaseOrderQuantityUnit |  | S/4 only entity (no ECC CDC mapping) |
| `ScheduleLineIssuedQuantity` | `ScheduleLineIssuedQuantity` | `Decimal(13,3)` |  | Issued Quantity | PurchaseOrderQuantityUnit |  | S/4 only entity (no ECC CDC mapping) |
| `SourceOfCreation` | `SourceOfCreation` | `String(1)` |  | Creation indicator |  |  | S/4 only entity (no ECC CDC mapping) |
| `Reservation` | `Reservation` | `String(10)` |  | Reservation |  |  | S/4 only entity (no ECC CDC mapping) |
| `ScheduleLineIsFixed` | `ScheduleLineIsFixed` | `Boolean` |  | Fixing Indicator |  |  | S/4 only entity (no ECC CDC mapping) |
| `StockTransferDeliveredQuantity` | `StockTransferDeliveredQuantity` | `Decimal(13,3)` |  | Qty Delivered | PurchaseOrderQuantityUnit |  | S/4 only entity (no ECC CDC mapping) |
| `ScheduleLineCommittedQuantity` | `ScheduleLineCommittedQuantity` | `Decimal(13,3)` |  | Committed Quantity | PurchaseOrderQuantityUnit |  | S/4 only entity (no ECC CDC mapping) |
| `ProductAvailabilityDate` | `ProductAvailabilityDate` | `Date` |  | Material Avail. Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductAvailabilityTime` | `ProductAvailabilityTime` | `String(6)` |  | Matl Staging Time |  |  | S/4 only entity (no ECC CDC mapping) |
| `LoadingDate` | `LoadingDate` | `Date` |  | Loading Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `LoadingTime` | `LoadingTime` | `String(6)` |  | Loading Time |  |  | S/4 only entity (no ECC CDC mapping) |
| `TransportationPlanningDate` | `TransportationPlanningDate` | `Date` |  | Transptn Plang Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `TransportationPlanningTime` | `TransportationPlanningTime` | `String(6)` |  | Transp. Plan. Time |  |  | S/4 only entity (no ECC CDC mapping) |
| `GoodsIssueDate` | `GoodsIssueDate` | `Date` |  | Goods Issue Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `GoodsIssueTime` | `GoodsIssueTime` | `String(6)` |  | Goods Issue Time |  |  | S/4 only entity (no ECC CDC mapping) |
| `STOLatestPossibleGRDate` | `STOLatestPossibleGRDate` | `Date` |  | GR End Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `STOLatestPossibleGRTime` | `STOLatestPossibleGRTime` | `String(6)` |  | GR End Time |  |  | S/4 only entity (no ECC CDC mapping) |
| `OpenPurchaseOrderNetAmount` | `OpenPurchaseOrderNetAmount` | `Decimal(34,4)` |  |  | DocumentCurrency |  | S/4 only entity (no ECC CDC mapping) |
| `IsReturnsItem` | `IsReturnsItem` | `Boolean` |  | Returns Item |  |  | S/4 only entity (no ECC CDC mapping) |
| `CompanyCode` | `CompanyCode` | `String(4)` |  | Company Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductTypeCode` | `ProductTypeCode` | `String(2)` |  | Product Type Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchasingDocumentDeletionCode` | `PurchasingDocumentDeletionCode` | `String(1)` |  | Deletion Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurgDocumentItemDeletionCode` | `PurgDocumentItemDeletionCode` | `String(1)` |  | Deletion Indicator |  |  | S/4 only entity (no ECC CDC mapping) |
| `ReleaseIsNotCompleted` | `ReleaseIsNotCompleted` | `Boolean` |  | Subject to Release |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchasingCompletenessStatus` | `PurchasingCompletenessStatus` | `Boolean` |  | Incomplete |  |  | S/4 only entity (no ECC CDC mapping) |
| `SupplierConfirmationControlKey` | `SupplierConfirmationControlKey` | `String(4)` |  | Confirmation Control |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsStatisticalItem` | `IsStatisticalItem` | `Boolean` |  | Statistical |  |  | S/4 only entity (no ECC CDC mapping) |
| `ScheduleLineOpenQuantity` | `ScheduleLineOpenQuantity` | `Decimal(14,3)` |  |  | PurchaseOrderQuantityUnit |  | S/4 only entity (no ECC CDC mapping) |
