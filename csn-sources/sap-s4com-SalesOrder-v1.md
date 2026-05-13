# SalesOrder

> Source file: `sap-s4com-SalesOrder-v1.json`

**Technical Name:** `` | **Data Category:** `DIMENSION` | **VDM Type:** `BASIC` | **Size:** `L`


## Entity: `SalesOrder`

- **ABAP Name:** `I_SalesOrder`
- **Label:** Sales Order
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** vbkd, veda, vbak

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `SalesOrder` | `VBAK` | `VBELN` | `String(10)` | Y | Sales Order |  |  |  |
| `SalesOrderType` | `VBAK` | `AUART` | `String(4)` |  | Sales Order Type |  |  |  |
| `SalesOrderProcessingType` |  |  | `String(1)` |  | Processing Type |  |  |  |
| `CreatedByUser` |  |  | `String(12)` |  | Created By |  |  |  |
| `LastChangedByUser` |  |  | `String(12)` |  | Last Changed By |  |  |  |
| `CreationDate` | `VBAK` | `ERDAT` | `Date` |  | Created On |  |  |  |
| `CreationTime` |  |  | `String(6)` |  | Created At |  |  |  |
| `LastChangeDate` |  |  | `Date` |  | Changed On |  |  |  |
| `LastChangeDateTime` |  |  | `Timestamp` |  | Time Stamp |  |  |  |
| `SenderBusinessSystemName` |  |  | `String(60)` |  | Ext. Bus. Syst. ID |  |  |  |
| `ExternalDocumentID` |  |  | `String(40)` |  | External Document ID |  |  |  |
| `ExternalDocLastChangeDateTime` |  |  | `Timestamp` |  | External Revision |  |  |  |
| `SalesOrganization` | `VBAK` | `VKORG` | `String(4)` |  | Sales Organization |  |  |  |
| `DistributionChannel` | `VBAK` | `VTWEG` | `String(2)` |  | Distribution Channel |  |  |  |
| `OrganizationDivision` |  |  | `String(2)` |  | Division |  |  |  |
| `SalesGroup` |  |  | `String(3)` |  | Sales Group |  |  |  |
| `SalesOffice` |  |  | `String(4)` |  | Sales Office |  |  |  |
| `SoldToParty` | `VBAK` | `KUNNR` | `String(10)` |  | Sold-to Party |  |  |  |
| `CustomerGroup` |  |  | `String(2)` |  | Customer Group |  |  |  |
| `AdditionalCustomerGroup1` |  |  | `String(3)` |  | Customer Group 1 |  |  |  |
| `AdditionalCustomerGroup2` |  |  | `String(3)` |  | Customer Group 2 |  |  |  |
| `AdditionalCustomerGroup3` |  |  | `String(3)` |  | Customer Group 3 |  |  |  |
| `AdditionalCustomerGroup4` |  |  | `String(3)` |  | Customer Group 4 |  |  |  |
| `AdditionalCustomerGroup5` |  |  | `String(3)` |  | Customer Group 5 |  |  |  |
| `SlsDocIsRlvtForProofOfDeliv` |  |  | `Boolean` |  | Relevant for Proof of Delivery |  |  |  |
| `CreditControlArea` |  |  | `String(4)` |  | Credit Control Area |  |  |  |
| `CustomerRebateAgreement` |  |  | `String(10)` |  | Agreement |  |  |  |
| `SalesOrderDate` | `VBAK` | `AUDAT` | `Date` |  | Document Date |  |  |  |
| `ServicesRenderedDate` |  |  | `Date` |  | Date of Services Rendered |  |  |  |
| `SDDocumentReason` |  |  | `String(3)` |  | Order Reason |  |  |  |
| `PurchaseOrderByCustomer` | `VBAK` | `BSTNK` | `String(35)` |  | Customer Reference |  |  |  |
| `PurchaseOrderByShipToParty` |  |  | `String(35)` |  | Customer Reference (Ship-to Party) |  |  |  |
| `SDDocumentCollectiveNumber` |  |  | `String(10)` |  | Collective Number |  |  |  |
| `CustomerPurchaseOrderType` |  |  | `String(4)` |  | Purchase Order Type |  |  |  |
| `CustomerPurchaseOrderDate` |  |  | `Date` |  | Customer Reference Date |  |  |  |
| `CustomerPurchaseOrderSuplmnt` |  |  | `String(4)` |  | Supplement |  |  |  |
| `SalesDistrict` |  |  | `String(6)` |  | Sales District |  |  |  |
| `StatisticsCurrency` |  |  | `String(5)` |  | Statistics Currency |  |  |  |
| `ProductCatalog` |  |  | `String(10)` |  | Catalog |  |  |  |
| `NextCreditCheckDate` |  |  | `Date` |  | Next Credit Check |  |  |  |
| `LastCustomerContactDate` |  |  | `Date` |  | Last Contact Date |  |  |  |
| `TotalNetAmount` |  |  | `Decimal(34,4)` |  | Net Value | TransactionCurrency |  |  |
| `TransactionCurrency` | `VBAK` | `WAERK` | `String(5)` |  | Document Currency |  |  |  |
| `PricingDate` |  |  | `Date` |  | Pricing Date |  |  |  |
| `PriceDetnExchangeRate` |  |  | `Decimal(9,5)` |  | Exchange Rate |  |  |  |
| `RetailPromotion` |  |  | `String(10)` |  | Retail Promotion |  |  |  |
| `SalesOrderCondition` |  |  | `String(10)` |  | Doc. Condition No. |  |  |  |
| `SDPricingProcedure` |  |  | `String(6)` |  | Pricing Procedure |  |  |  |
| `CustomerPriceGroup` |  |  | `String(2)` |  | Customer Price Group |  |  |  |
| `PriceListType` |  |  | `String(2)` |  | Price List Type |  |  |  |
| `BillingPlan` |  |  | `String(10)` |  | Bill. Plan No. |  |  |  |
| `CustomerTaxClassification1` |  |  | `String(1)` |  | Alt.Tax Classific. |  |  |  |
| `CustomerTaxClassification2` |  |  | `String(1)` |  | Tax Class.2 Customer |  |  |  |
| `CustomerTaxClassification3` |  |  | `String(1)` |  | Tax Class.3 Customer |  |  |  |
| `CustomerTaxClassification4` |  |  | `String(1)` |  | Tax Class.4 Customer |  |  |  |
| `CustomerTaxClassification5` |  |  | `String(1)` |  | Tax Class.5 Customer |  |  |  |
| `CustomerTaxClassification6` |  |  | `String(1)` |  | Tax Class.6 Customer |  |  |  |
| `CustomerTaxClassification7` |  |  | `String(1)` |  | Tax Class.7 Customer |  |  |  |
| `CustomerTaxClassification8` |  |  | `String(1)` |  | Tax Class.8 Customer |  |  |  |
| `CustomerTaxClassification9` |  |  | `String(1)` |  | Tax Class.9 Customer |  |  |  |
| `TaxDepartureCountry` |  |  | `String(3)` |  | Tax Departure Country/Region |  |  |  |
| `VATRegistrationCountry` |  |  | `String(3)` |  | Tax Destination Country/Region |  |  |  |
| `RequestedDeliveryDate` |  |  | `Date` |  | Requested Delivery Date |  |  |  |
| `DeliveryDateTypeRule` |  |  | `String(1)` |  | Delivery Date Rule |  |  |  |
| `ShippingType` |  |  | `String(2)` |  | Shipping Type |  |  |  |
| `ShippingCondition` |  |  | `String(2)` |  | Shipping Conditions |  |  |  |
| `ReceivingPoint` |  |  | `String(25)` |  | Receiving Point |  |  |  |
| `IncotermsClassification` |  |  | `String(3)` |  | Incoterms |  |  |  |
| `IncotermsTransferLocation` |  |  | `String(28)` |  | Incoterms (Part 2) |  |  |  |
| `IncotermsLocation1` |  |  | `String(70)` |  | Incoterms Location 1 |  |  |  |
| `IncotermsLocation2` |  |  | `String(70)` |  | Incoterms Location 2 |  |  |  |
| `IncotermsVersion` |  |  | `String(4)` |  | Incoterms Version |  |  |  |
| `CompleteDeliveryIsDefined` |  |  | `Boolean` |  | Complete Delivery |  |  |  |
| `OrderCombinationIsAllowed` |  |  | `Boolean` |  | Order Combination |  |  |  |
| `DeliveryBlockReason` |  |  | `String(2)` |  | Delivery Block |  |  |  |
| `FashionCancelDate` |  |  | `Date` |  | Cancellation Date |  |  |  |
| `SalesOrderApprovalReason` |  |  | `String(4)` |  | Approval Request Reason |  |  |  |
| `BillingDocumentDate` |  |  | `Date` |  | Billing Date |  |  |  |
| `BillingCompanyCode` |  |  | `String(4)` |  | CCode to Be Billed |  |  |  |
| `HeaderBillingBlockReason` |  |  | `String(2)` |  | Billing Block |  |  |  |
| `CustomerPaymentTerms` |  |  | `String(4)` |  | Terms of Payment |  |  |  |
| `PaymentMethod` |  |  | `String(1)` |  | Payment Method |  |  |  |
| `FixedValueDate` |  |  | `Date` |  | Fixed Value Date |  |  |  |
| `FiscalYear` |  |  | `String(4)` |  | Fiscal Year |  |  |  |
| `FiscalPeriod` |  |  | `String(3)` |  | Posting Period |  |  | ECC BKPF.MONAT unpadded ('3'); S/4 zero-padded ('003') |
| `ExchangeRateDate` |  |  | `Date` |  | Translation Date |  |  |  |
| `ExchangeRateType` |  |  | `String(4)` |  | Exchange Rate Type |  |  |  |
| `AccountingExchangeRate` |  |  | `Decimal(9,5)` |  | Exchng. Rate Accntg. |  |  |  |
| `BusinessArea` |  |  | `String(4)` |  | Business Area |  |  |  |
| `CustomerAccountAssignmentGroup` |  |  | `String(2)` |  | Account Assignment Group for Customer |  |  |  |
| `CostCenterBusinessArea` |  |  | `String(4)` |  | Business Area |  |  |  |
| `CostCenter` |  |  | `String(10)` |  | Cost Center |  |  |  |
| `ControllingArea` | `TKA01` | `KOKRS` | `String(4)` |  | Controlling Area |  |  |  |
| `OrderID` |  |  | `String(12)` |  | Order |  |  |  |
| `ControllingObject` |  |  | `String(22)` |  | Object No. Header |  |  |  |
| `AssignmentReference` |  |  | `String(18)` |  | Assignment |  |  |  |
| `PaymentPlan` |  |  | `String(10)` |  | Paym. Card Plan No. |  |  |  |
| `ContractAccount` |  |  | `String(12)` |  | Contract Account |  |  |  |
| `AdditionalValueDays` |  |  | `String(2)` |  | Addit. Value Days |  |  |  |
| `CustomerCreditAccount` |  |  | `String(10)` |  | Credit Account |  |  |  |
| `ReferenceSDDocument` |  |  | `String(10)` |  | Reference Document |  |  |  |
| `ReferenceSDDocumentCategory` |  |  | `String(4)` |  | Reference Document Category |  |  |  |
| `CorrespncExternalReference` |  |  | `String(12)` |  | Your Reference |  |  |  |
| `CorrespncExtRefByShipToParty` |  |  | `String(12)` |  | Your Reference |  |  |  |
| `AccountingDocExternalReference` |  |  | `String(16)` |  | Reference |  |  |  |
| `BusinessSolutionOrder` |  |  | `String(10)` |  | Solution Order |  |  |  |
| `OverallSDProcessStatus` |  |  | `String(1)` |  | Overall Status |  |  |  |
| `OverallPurchaseConfStatus` |  |  | `String(1)` |  | Purchasing Conf. Sts |  |  |  |
| `OverallSDDocumentRejectionSts` |  |  | `String(1)` |  | Rejection Status |  |  |  |
| `TotalBlockStatus` |  |  | `String(1)` |  | Overall Block Status |  |  |  |
| `OverallDelivConfStatus` |  |  | `String(1)` |  | Delivery Conf. Sts |  |  |  |
| `OverallTotalDeliveryStatus` |  |  | `String(1)` |  | Ovrl Delivery Status |  |  |  |
| `OverallDeliveryStatus` |  |  | `String(1)` |  | Delivery Status |  |  |  |
| `OverallDeliveryBlockStatus` |  |  | `String(1)` |  | Delivery Block Status |  |  |  |
| `OverallOrdReltdBillgStatus` |  |  | `String(1)` |  | Order-Related Billing Status |  |  |  |
| `OverallBillingBlockStatus` |  |  | `String(1)` |  | Billing Block Status |  |  |  |
| `OverallTotalSDDocRefStatus` |  |  | `String(1)` |  | Ovrl Reference Sts |  |  |  |
| `OverallSDDocReferenceStatus` |  |  | `String(1)` |  | Reference Status |  |  |  |
| `TotalCreditCheckStatus` |  |  | `String(1)` |  | Credit Status |  |  |  |
| `MaxDocValueCreditCheckStatus` |  |  | `String(1)` |  | Maximum Value |  |  |  |
| `PaymentTermCreditCheckStatus` |  |  | `String(1)` |  | Terms of Payment |  |  |  |
| `FinDocCreditCheckStatus` |  |  | `String(1)` |  | Financial Document |  |  |  |
| `ExprtInsurCreditCheckStatus` |  |  | `String(1)` |  | Expt Cred. Insurance |  |  |  |
| `PaytAuthsnCreditCheckSts` |  |  | `String(1)` |  | Payment Card Status |  |  |  |
| `CentralCreditCheckStatus` |  |  | `String(1)` |  | SAP Cred. Mgmt |  |  |  |
| `CentralCreditChkTechErrSts` |  |  | `String(1)` |  | CrMa TE Status |  |  |  |
| `HdrGeneralIncompletionStatus` |  |  | `String(1)` |  | Overall Header |  |  |  |
| `OverallPricingIncompletionSts` |  |  | `String(1)` |  | Pricing – All Items |  |  |  |
| `HeaderDelivIncompletionStatus` |  |  | `String(1)` |  | Delivery – Header |  |  |  |
| `HeaderBillgIncompletionStatus` |  |  | `String(1)` |  | Billing – Header |  |  |  |
| `OvrlItmGeneralIncompletionSts` |  |  | `String(1)` |  | All Items |  |  |  |
| `OvrlItmBillingIncompletionSts` |  |  | `String(1)` |  | Billing – All Items |  |  |  |
| `OvrlItmDelivIncompletionSts` |  |  | `String(1)` |  | Delivery – All Items |  |  |  |
| `OverallChmlCmplncStatus` |  |  | `String(1)` |  | Product Marketability Status |  |  |  |
| `OverallDangerousGoodsStatus` |  |  | `String(1)` |  | Dangerous Goods Status |  |  |  |
| `OverallSafetyDataSheetStatus` |  |  | `String(1)` |  | Safety Data Sheet Status |  |  |  |
| `SalesDocApprovalStatus` |  |  | `String(1)` |  | Approval Status |  |  |  |
| `OverallTrdCmplncEmbargoSts` |  |  | `String(1)` |  | Embargo Status |  |  |  |
| `OvrlTrdCmplncSnctndListChkSts` |  |  | `String(1)` |  | Screening Status |  |  |  |
| `OvrlTrdCmplncLegalCtrlChkSts` |  |  | `String(1)` |  | Legal Control Status |  |  |  |
| `SalesOrderDownPaymentStatus` |  |  | `String(1)` |  | Down Payment Status |  |  |  |
| `OmniChnlSalesPromotionStatus` |  |  | `String(1)` |  | OmniChnl Sls Pro Sts |  |  |  |
| `AlternativePricingDate` |  |  | `Date` |  | CrossItemPricingDate |  |  |  |
| `IsEUTriangularDeal` |  |  | `Boolean` |  | EU Triangular Deal |  |  |  |
| `RetailAdditionalCustomerGrp6` |  |  | `String(3)` |  | Customer Group 6 |  |  |  |
| `RetailAdditionalCustomerGrp7` |  |  | `String(3)` |  | Customer Group 7 |  |  |  |
| `RetailAdditionalCustomerGrp8` |  |  | `String(3)` |  | Customer Group 8 |  |  |  |
| `RetailAdditionalCustomerGrp9` |  |  | `String(3)` |  | Customer Group 9 |  |  |  |
| `RetailAdditionalCustomerGrp10` |  |  | `String(3)` |  | Customer Group 10 |  |  |  |
| `Store` |  |  | `String(4)` |  | Plant |  |  |  |
| `CustomerConditionGroup1` |  |  | `String(2)` |  | Condition Group 1 |  |  |  |
| `CustomerConditionGroup2` |  |  | `String(2)` |  | Condition Group 2 |  |  |  |
| `CustomerConditionGroup3` |  |  | `String(2)` |  | Condition Group 3 |  |  |  |
| `CustomerConditionGroup4` |  |  | `String(2)` |  | Condition Group 4 |  |  |  |
| `CustomerConditionGroup5` |  |  | `String(2)` |  | Condition Group 5 |  |  |  |
| `SlsDocSo2PLastContactPersnName` |  |  | `String(35)` |  | Name of Last Contact |  |  |  |
| `SlsDocSo2PLstCntctPersnTelNmbr` |  |  | `String(16)` |  | Tel. No. Last Cntct |  |  |  |
| `POCorrespncExternalReference` |  |  | `String(12)` |  | Pur. Order Ext. Ref. |  |  |  |


## Entity: `SalesOrderItem`

- **ABAP Name:** `I_SalesOrderItem`
- **Label:** Sales Order Item
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** vbap, vbkd, veda, vbak

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `SalesOrder` | `VBAK` | `VBELN` | `String(10)` | Y | Sales Order |  | _SalesOrder |  |
| `SalesOrderItem` | `VBAP` | `POSNR` | `String(6)` | Y | Item |  |  |  |
| `SalesOrderItemUUID` |  |  | `UUID` |  | GUID 16 |  |  |  |
| `SalesOrderItemCategory` |  |  | `String(4)` |  | Item Category |  |  |  |
| `SalesOrderItemType` |  |  | `String(1)` |  | Item Type |  |  |  |
| `IsReturnsItem` |  |  | `Boolean` |  | Returns |  |  |  |
| `CreatedByUser` |  |  | `String(12)` |  | Created By |  |  |  |
| `CreationDate` | `VBAK` | `ERDAT` | `Date` |  | Created On |  |  |  |
| `CreationTime` |  |  | `String(6)` |  | Created At |  |  |  |
| `LastChangeDate` |  |  | `Date` |  | Changed On |  |  |  |
| `Division` | `VBAK` | `SPART` | `String(2)` |  | Division |  |  |  |
| `Material` | `VBAP` | `MATNR` | `String(40)` |  | Material |  |  |  |
| `Product` |  |  | `String(40)` |  | Product |  |  |  |
| `OriginallyRequestedMaterial` |  |  | `String(40)` |  | Material Entered |  |  |  |
| `MaterialByCustomer` |  |  | `String(35)` |  | Customer Material |  |  |  |
| `InternationalArticleNumber` |  |  | `String(18)` |  | EAN/UPC |  |  |  |
| `Batch` |  |  | `String(10)` |  | Batch |  |  |  |
| `ProductHierarchyNode` |  |  | `String(18)` |  | Product Hierarchy |  |  |  |
| `ProductCatalog` |  |  | `String(10)` |  | Catalog |  |  |  |
| `MaterialSubstitutionReason` |  |  | `String(4)` |  | Substitution Reason |  |  |  |
| `MaterialGroup` |  |  | `String(9)` |  | Material Group |  |  |  |
| `ProductGroup` |  |  | `String(9)` |  | Product Group |  |  |  |
| `MaterialPricingGroup` |  |  | `String(2)` |  | Product Price Group |  |  |  |
| `AdditionalMaterialGroup1` |  |  | `String(3)` |  | Material Group 1 |  |  |  |
| `AdditionalMaterialGroup2` |  |  | `String(3)` |  | Material Group 2 |  |  |  |
| `AdditionalMaterialGroup3` |  |  | `String(3)` |  | Material Group 3 |  |  |  |
| `AdditionalMaterialGroup4` |  |  | `String(3)` |  | Material Group 4 |  |  |  |
| `AdditionalMaterialGroup5` |  |  | `String(3)` |  | Material Group 5 |  |  |  |
| `Plant` | `VBAP` | `WERKS` | `String(4)` |  | Plant |  |  |  |
| `OriginalPlant` |  |  | `String(4)` |  | Original Plant |  |  |  |
| `StorageLocation` | `VBAP` | `LGORT` | `String(4)` |  | Storage Location |  |  |  |
| `DeliveryGroup` |  |  | `String(3)` |  | Delivery Group |  |  |  |
| `ProductConfiguration` |  |  | `String(18)` |  | Configuration |  |  |  |
| `BOMExplosionDate` |  |  | `Date` |  | BOM Key Date |  |  |  |
| `SalesOrderItemText` |  |  | `String(40)` |  | Item Description |  |  |  |
| `PurchaseOrderByCustomer` | `VBAK` | `BSTNK` | `String(35)` |  | Customer Reference |  |  |  |
| `PurchaseOrderByShipToParty` |  |  | `String(35)` |  | Customer Reference (Ship-to Party) |  |  |  |
| `CustomerPurchaseOrderDate` |  |  | `Date` |  | Customer Ref. Date |  |  |  |
| `UnderlyingPurchaseOrderItem` |  |  | `String(6)` |  | Purchase Order Item |  |  |  |
| `UndrlgPurOrdItmByShipToParty` |  |  | `String(6)` |  | Purchase Order Item |  |  |  |
| `CorrespncExternalReference` |  |  | `String(12)` |  | Your Reference |  |  |  |
| `CorrespncExtRefByShipToParty` |  |  | `String(12)` |  | Your Reference |  |  |  |
| `ExternalItemID` |  |  | `String(40)` |  | External Item ID |  |  |  |
| `OrderQuantity` |  |  | `Decimal(15,3)` |  | Order Quantity | OrderQuantityUnit |  |  |
| `OrderQuantityUnit` |  |  | `String(3)` |  | Sales Unit |  |  |  |
| `OrderToBaseQuantityDnmntr` |  |  | `Decimal(5,0)` |  | Denominator |  |  |  |
| `OrderToBaseQuantityNmrtr` |  |  | `Decimal(5,0)` |  | Numerator |  |  |  |
| `TargetQuantity` |  |  | `Decimal(13,3)` |  | Target Quantity | TargetQuantityUnit |  |  |
| `TargetQuantityUnit` |  |  | `String(3)` |  | Target Quantity UoM |  |  |  |
| `TargetToBaseQuantityDnmntr` |  |  | `Decimal(5,0)` |  | Conversion Factor |  |  |  |
| `TargetToBaseQuantityNmrtr` |  |  | `Decimal(5,0)` |  | Conversion Factor |  |  |  |
| `ConfdDelivQtyInOrderQtyUnit` |  |  | `Decimal(15,3)` |  | Confirmed Quantity | OrderQuantityUnit |  |  |
| `TargetDelivQtyInOrderQtyUnit` |  |  | `Decimal(15,3)` |  | Required Deliv. Qty | OrderQuantityUnit |  |  |
| `ConfdDeliveryQtyInBaseUnit` |  |  | `Decimal(15,3)` |  | Cumltv Confd Qty(BU) | BaseUnit |  |  |
| `BaseUnit` |  |  | `String(3)` |  | Base Unit of Measure |  |  |  |
| `CommittedDelivQtyInOrdQtyUnit` |  |  | `Decimal(15,3)` |  | Committed Delivery Quantity | OrderQuantityUnit |  |  |
| `CommittedDelivCreationDate` |  |  | `Date` |  | Committed Delivery Creation Date |  |  |  |
| `CommittedDeliveryDate` |  |  | `Date` |  | Committed Delivery Date |  |  |  |
| `RequestedQuantity` | `VBAP` | `KWMENG` | `Decimal(15,3)` |  | Requested Quantity | RequestedQuantityUnit |  |  |
| `RequestedQuantityUnit` |  |  | `String(3)` |  | Requested Qty Unit |  |  |  |
| `RequestedQuantityInBaseUnit` |  |  | `Decimal(15,3)` |  | Requ.SalesOrder Qty. | BaseUnit |  |  |
| `ItemGrossWeight` |  |  | `Decimal(15,3)` |  | Gross Weight | ItemWeightUnit |  |  |
| `ItemNetWeight` |  |  | `Decimal(15,3)` |  | Net Weight | ItemWeightUnit |  |  |
| `ItemWeightUnit` |  |  | `String(3)` |  | Unit of Weight |  |  |  |
| `ItemVolume` |  |  | `Decimal(15,3)` |  | Volume | ItemVolumeUnit |  |  |
| `ItemVolumeUnit` |  |  | `String(3)` |  | Volume Unit |  |  |  |
| `ServicesRenderedDate` |  |  | `Date` |  | Date of Services Rendered |  |  |  |
| `SalesDistrict` |  |  | `String(6)` |  | Sales District |  |  |  |
| `SalesDeal` |  |  | `String(10)` |  | Sales Deal |  |  |  |
| `SalesPromotion` |  |  | `String(10)` |  | Promotion |  |  |  |
| `RetailPromotion` |  |  | `String(10)` |  | Retail Promotion |  |  |  |
| `CustomerGroup` |  |  | `String(2)` |  | Customer Group |  |  |  |
| `SalesDocumentRjcnReason` |  |  | `String(2)` |  | Reason for Rejection |  |  |  |
| `RequirementSegment` |  |  | `String(40)` |  | Requirement Segment |  |  |  |
| `SlsDocIsRlvtForProofOfDeliv` |  |  | `Boolean` |  | Relevant for POD |  |  |  |
| `NetAmount` | `VBAP` | `NETWR` | `Decimal(34,4)` |  | Net Value | TransactionCurrency |  |  |
| `TransactionCurrency` | `VBAK` | `WAERK` | `String(5)` |  | Document Currency |  |  |  |
| `PricingDate` |  |  | `Date` |  | Pricing Date |  |  |  |
| `PricingReferenceMaterial` |  |  | `String(40)` |  | Pricing Ref. Matl |  |  |  |
| `ExchangeRateDate` |  |  | `Date` |  | Translation Date |  |  |  |
| `PriceDetnExchangeRate` |  |  | `Decimal(9,5)` |  | Exchange Rate |  |  |  |
| `NetPriceAmount` |  |  | `Decimal(34,4)` |  | Net Price | TransactionCurrency |  |  |
| `NetPriceQuantity` |  |  | `Decimal(5,0)` |  | Pricing Unit | NetPriceQuantityUnit |  |  |
| `NetPriceQuantityUnit` |  |  | `String(3)` |  | Unit of Measure |  |  |  |
| `StatisticalValueControl` |  |  | `String(1)` |  | Statistical Value |  |  |  |
| `SalesDocumentItemProcgCode` |  |  | `String(1)` |  | Processing Code |  |  |  |
| `DownPaymentProcessingVariant` |  |  | `String(1)` |  | Down Payment Variant |  |  |  |
| `TaxAmount` |  |  | `Decimal(34,4)` |  | Tax Amount | TransactionCurrency |  |  |
| `ProductTaxClassification1` |  |  | `String(1)` |  | Tax Classifc. Mat. |  |  |  |
| `ProductTaxClassification2` |  |  | `String(1)` |  | Tax Classifc. Mat. |  |  |  |
| `ProductTaxClassification3` |  |  | `String(1)` |  | Tax Classifc. Mat. |  |  |  |
| `ProductTaxClassification4` |  |  | `String(1)` |  | Tax Classifc. Mat. |  |  |  |
| `ProductTaxClassification5` |  |  | `String(1)` |  | Tax Classifc. Mat. |  |  |  |
| `ProductTaxClassification6` |  |  | `String(1)` |  | Tax Classifc. Mat. |  |  |  |
| `ProductTaxClassification7` |  |  | `String(1)` |  | Tax Classifc. Mat. |  |  |  |
| `ProductTaxClassification8` |  |  | `String(1)` |  | Tax Classifc. Mat. |  |  |  |
| `ProductTaxClassification9` |  |  | `String(1)` |  | Tax Classifc. Mat. |  |  |  |
| `MatlAccountAssignmentGroup` |  |  | `String(2)` |  | Acct Assmt Grp Mat. |  |  |  |
| `CostAmount` |  |  | `Decimal(34,4)` |  | Cost | TransactionCurrency |  |  |
| `Subtotal1Amount` |  |  | `Decimal(34,4)` |  | Subtotal 1 | TransactionCurrency |  |  |
| `Subtotal2Amount` |  |  | `Decimal(34,4)` |  | Subtotal 2 | TransactionCurrency |  |  |
| `Subtotal3Amount` |  |  | `Decimal(34,4)` |  | Subtotal 3 | TransactionCurrency |  |  |
| `Subtotal4Amount` |  |  | `Decimal(34,4)` |  | Subtotal 4 | TransactionCurrency |  |  |
| `Subtotal5Amount` |  |  | `Decimal(34,4)` |  | Subtotal 5 | TransactionCurrency |  |  |
| `Subtotal6Amount` |  |  | `Decimal(34,4)` |  | Subtotal 6 | TransactionCurrency |  |  |
| `SalesOrderCondition` |  |  | `String(10)` |  | Doc. Condition No. |  |  |  |
| `CustomerPriceGroup` |  |  | `String(2)` |  | Customer Price Group |  |  |  |
| `ShippingPoint` |  |  | `String(4)` |  | Shipping Point |  |  |  |
| `ShippingType` |  |  | `String(2)` |  | Shipping Type |  |  |  |
| `InventorySpecialStockType` |  |  | `String(1)` |  | Special Stock |  |  |  |
| `DeliveryPriority` |  |  | `String(2)` |  | Delivery Priority |  |  |  |
| `Route` |  |  | `String(6)` |  | Route |  |  |  |
| `DeliveryDateQuantityIsFixed` |  |  | `Boolean` |  | Fixed Date and Qty |  |  |  |
| `DeliveryDateTypeRule` |  |  | `String(1)` |  | Deliv Date Rule |  |  |  |
| `PartialDeliveryIsAllowed` |  |  | `String(1)` |  | Partial Delivery for Item |  |  |  |
| `MaxNmbrOfPartialDelivery` |  |  | `Decimal(1,0)` |  | Number of Partial Deliveries |  |  |  |
| `UnlimitedOverdeliveryIsAllowed` |  |  | `Boolean` |  | Unlimited Tolerance |  |  |  |
| `OverdelivTolrtdLmtRatioInPct` |  |  | `Decimal(3,1)` |  | Overdeliv. Tolerance |  |  |  |
| `UnderdelivTolrtdLmtRatioInPct` |  |  | `Decimal(3,1)` |  | Underdel. Tolerance |  |  |  |
| `MinDeliveryQtyInBaseUnit` |  |  | `Decimal(13,3)` |  | Minimum Delivery Qty | BaseUnit |  |  |
| `OpenDeliveryLeadingUnitCode` |  |  | `String(1)` |  | Leading UoM |  |  |  |
| `ItemIsDeliveryRelevant` |  |  | `Boolean` |  | Itm Relev.for Deliv. |  |  |  |
| `ReceivingPoint` |  |  | `String(25)` |  | Receiving Point |  |  |  |
| `IncotermsVersion` |  |  | `String(4)` |  | Incoterms Version |  |  |  |
| `IncotermsClassification` |  |  | `String(3)` |  | Incoterms |  |  |  |
| `IncotermsTransferLocation` |  |  | `String(28)` |  | Incoterms (Part 2) |  |  |  |
| `IncotermsLocation1` |  |  | `String(70)` |  | Incoterms Location 1 |  |  |  |
| `IncotermsLocation2` |  |  | `String(70)` |  | Incoterms Location 2 |  |  |  |
| `OrderCombinationIsAllowed` |  |  | `Boolean` |  | Order Combination |  |  |  |
| `CustomerPaymentTerms` |  |  | `String(4)` |  | Terms of Payment |  |  |  |
| `PaymentMethod` |  |  | `String(1)` |  | Payment Method |  |  |  |
| `FixedValueDate` |  |  | `Date` |  | Fixed Value Date |  |  |  |
| `AdditionalValueDays` |  |  | `String(2)` |  | Addit. Value Days |  |  |  |
| `ProductSeasonYear` |  |  | `String(4)` |  | Season Year |  |  |  |
| `ProductSeason` |  |  | `String(10)` |  | Season |  |  |  |
| `ProductCollection` |  |  | `String(10)` |  | Collection |  |  |  |
| `ProductTheme` |  |  | `String(10)` |  | Theme |  |  |  |
| `FashionCancelDate` |  |  | `Date` |  | Cancellation Date |  |  |  |
| `ProductCharacteristic1` |  |  | `String(18)` |  | Characteristic 1 |  |  |  |
| `ProductCharacteristic2` |  |  | `String(18)` |  | Characteristic 2 |  |  |  |
| `ProductCharacteristic3` |  |  | `String(18)` |  | Characteristic 3 |  |  |  |
| `ShippingGroupNumber` |  |  | `String(10)` |  | PSST Group |  |  |  |
| `ShippingGroupRule` |  |  | `String(4)` |  | PSST Grouping Rule |  |  |  |
| `BillingDocumentDate` |  |  | `Date` |  | Billing Date |  |  |  |
| `ItemIsBillingRelevant` |  |  | `String(1)` |  | Relevant for Billing |  |  |  |
| `ItemBillingBlockReason` |  |  | `String(2)` |  | Billing Block |  |  |  |
| `BillingPlan` |  |  | `String(10)` |  | Bill. Plan No. |  |  |  |
| `FiscalYear` |  |  | `String(4)` |  | Fiscal Year |  |  |  |
| `FiscalPeriod` |  |  | `String(3)` |  | Posting Period |  |  | ECC BKPF.MONAT unpadded ('3'); S/4 zero-padded ('003') |
| `CustomerAccountAssignmentGroup` |  |  | `String(2)` |  | Acct Assmt Grp Cust. |  |  |  |
| `BusinessArea` |  |  | `String(4)` |  | Business Area |  |  |  |
| `ControllingArea` | `TKA01` | `KOKRS` | `String(4)` |  | Controlling Area |  |  |  |
| `ProfitCenter` | `VBAP` | `PRCTR` | `String(10)` |  | Profit Center |  |  |  |
| `WBSElement` | `VBAP` | `PS_PSP_PNR` | `String(8)` |  | WBS Element |  |  |  |
| `WBSElementInternalID` |  |  | `String(8)` |  | WBS Internal ID |  |  |  |
| `OrderID` |  |  | `String(12)` |  | Order |  |  |  |
| `ControllingObject` |  |  | `String(22)` |  | Object No.Item |  |  |  |
| `ProfitabilitySegment` |  |  | `String(10)` |  | Profitability Segment (Deprecated) |  |  |  |
| `ProfitabilitySegment_2` |  |  | `String(10)` |  | Profitability Segment |  |  |  |
| `OriginSDDocument` |  |  | `String(10)` |  | Originating Document |  |  |  |
| `OriginSDDocumentItem` |  |  | `String(6)` |  | Originating Item |  |  |  |
| `AccountingExchangeRate` |  |  | `Decimal(9,5)` |  | Exchng. Rate Accntg. |  |  |  |
| `ContractAccount` |  |  | `String(12)` |  | Contract Account |  |  |  |
| `ReferenceSDDocument` |  |  | `String(10)` |  | Reference Document |  |  |  |
| `ReferenceSDDocumentItem` |  |  | `String(6)` |  | Reference Item |  |  |  |
| `ReferenceSDDocumentCategory` |  |  | `String(4)` |  | Reference Document Category |  |  |  |
| `HigherLevelItem` |  |  | `String(6)` |  | Higher-Level Item |  |  |  |
| `HigherLevelItemUsage` |  |  | `String(1)` |  | Usage of HL Item |  |  |  |
| `BusinessSolutionOrder` |  |  | `String(10)` |  | Solution Order |  |  |  |
| `BusinessSolutionOrderItem` |  |  | `String(6)` |  | Solution Order Item |  |  |  |
| `BusSolnOrdItemBundleItem` |  |  | `String(6)` |  | Bundle Item No. |  |  |  |
| `SDProcessStatus` |  |  | `String(1)` |  | Overall Status |  |  |  |
| `DeliveryConfirmationStatus` |  |  | `String(1)` |  | Delivery Conf. Sts |  |  |  |
| `PurchaseConfirmationStatus` |  |  | `String(1)` |  | Purchasing Conf. Sts |  |  |  |
| `TotalDeliveryStatus` |  |  | `String(1)` |  | Ovrl Delivery Status |  |  |  |
| `DeliveryStatus` |  |  | `String(1)` |  | Delivery Status |  |  |  |
| `DeliveryBlockStatus` |  |  | `String(1)` |  | Delivery Block Status |  |  |  |
| `OrderRelatedBillingStatus` |  |  | `String(1)` |  | Order-Related Billing Status |  |  |  |
| `BillingBlockStatus` |  |  | `String(1)` |  | Billing Block Status |  |  |  |
| `ItemGeneralIncompletionStatus` |  |  | `String(1)` |  | Incompletion Status |  |  |  |
| `ItemBillingIncompletionStatus` |  |  | `String(1)` |  | Billing – Item |  |  |  |
| `PricingIncompletionStatus` |  |  | `String(1)` |  | Pricing – Item |  |  |  |
| `ItemDeliveryIncompletionStatus` |  |  | `String(1)` |  | Delivery – Item |  |  |  |
| `SDDocReferenceStatus` |  |  | `String(1)` |  | Reference Status |  |  |  |
| `SDDocumentRejectionStatus` |  |  | `String(1)` |  | Rejection Status |  |  |  |
| `TotalSDDocReferenceStatus` |  |  | `String(1)` |  | Ovrl Reference Sts |  |  |  |
| `ChmlCmplncStatus` |  |  | `String(1)` |  | Product Marketability Status |  |  |  |
| `DangerousGoodsStatus` |  |  | `String(1)` |  | Dangerous Goods Status |  |  |  |
| `SafetyDataSheetStatus` |  |  | `String(1)` |  | Safety Data Sheet Status |  |  |  |
| `SlsOrderItemDownPaymentStatus` |  |  | `String(1)` |  | Down Payment Status |  |  |  |
| `TrdCmplncEmbargoSts` |  |  | `String(1)` |  | Embargo Status |  |  |  |
| `TrdCmplncSnctndListChkSts` |  |  | `String(1)` |  | Screening Status |  |  |  |
| `OvrlTrdCmplncLegalCtrlChkSts` |  |  | `String(1)` |  | Legal Control Status |  |  |  |
| `AltvBsdConfSubstitutionStatus` |  |  | `String(1)` |  | Substitution Status |  |  |  |
| `OmniChannelSalesPromotion` |  |  | `Integer64` |  | OmniChnl PromoID |  |  |  |
| `OmniChannelSalesPromotionRule` |  |  | `Integer64` |  | FGID OmniChnl |  |  |  |
| `ConsumptionPosting` |  |  | `String(1)` |  | Consumption |  |  |  |
| `CappedNetAmount` |  |  | `Decimal(34,4)` |  | Net Amount Cap | TransactionCurrency |  |  |
| `CappedNetAmtAlertThldInPct` |  |  | `String(3)` |  | Cap Notif. Threshold |  |  |  |
| `TotalStandAloneSellingPrice` |  |  | `Decimal(34,4)` |  | SSP | TransactionCurrency |  |  |
| `SalesOrderType` | `VBAK` | `AUART` | `String(4)` |  | Sales Order Type |  |  |  |
| `SalesOrganization` | `VBAK` | `VKORG` | `String(4)` |  | Sales Organization |  |  |  |
| `DistributionChannel` | `VBAK` | `VTWEG` | `String(2)` |  | Distribution Channel |  |  |  |
| `OrganizationDivision` |  |  | `String(2)` |  | Division |  |  |  |
| `SalesOffice` |  |  | `String(4)` |  | Sales Office |  |  |  |
| `SalesGroup` |  |  | `String(3)` |  | Sales Group |  |  |  |
| `SoldToParty` | `VBAK` | `KUNNR` | `String(10)` |  | Sold-to Party |  |  |  |
| `AdditionalCustomerGroup1` |  |  | `String(3)` |  | Customer Group 1 |  |  |  |
| `AdditionalCustomerGroup2` |  |  | `String(3)` |  | Customer Group 2 |  |  |  |
| `AdditionalCustomerGroup3` |  |  | `String(3)` |  | Customer Group 3 |  |  |  |
| `AdditionalCustomerGroup4` |  |  | `String(3)` |  | Customer Group 4 |  |  |  |
| `AdditionalCustomerGroup5` |  |  | `String(3)` |  | Customer Group 5 |  |  |  |
| `SalesOrderDate` | `VBAK` | `AUDAT` | `Date` |  | Document Date |  |  |  |
| `SDDocumentReason` |  |  | `String(3)` |  | Order Reason |  |  |  |
| `RequestedDeliveryDate` |  |  | `Date` |  | Requested Delivery Date |  |  |  |
| `ShippingCondition` |  |  | `String(2)` |  | Shipping Conditions |  |  |  |
| `ShipToParty` |  |  | `String(10)` |  | Ship-to Party |  |  |  |
| `PayerParty` |  |  | `String(10)` |  | Payer |  |  |  |
| `BillToParty` |  |  | `String(10)` |  | Bill-to Party |  |  |  |
| `SalesEmployee` |  |  | `String(8)` |  | Sales Employee |  |  |  |
| `ResponsibleEmployee` |  |  | `String(8)` |  | Employee Responsible |  |  |  |
| `SalesEmployeeWorkAgreement` |  |  | `String(8)` |  | Sales Employee |  |  |  |
| `ResponsibleEmployeeWorkAgrmt` |  |  | `String(8)` |  | Employee Responsible |  |  |  |
| `SeasonCompletenessStatus` |  |  | `String(1)` |  | Season Comp.Ind |  |  |  |
| `CustomerConditionGroup1` |  |  | `String(2)` |  | Condition Group 1 |  |  |  |
| `CustomerConditionGroup2` |  |  | `String(2)` |  | Condition Group 2 |  |  |  |
| `CustomerConditionGroup3` |  |  | `String(2)` |  | Condition Group 3 |  |  |  |
| `CustomerConditionGroup4` |  |  | `String(2)` |  | Condition Group 4 |  |  |  |
| `CustomerConditionGroup5` |  |  | `String(2)` |  | Condition Group 5 |  |  |  |
| `POCorrespncExternalReference` |  |  | `String(12)` |  | Pur. Order Ext. Ref. |  |  |  |
