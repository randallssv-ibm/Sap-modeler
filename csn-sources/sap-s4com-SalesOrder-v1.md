# SalesOrder

> Source file: `sap-s4com-SalesOrder-v1.json`

**Technical Name:** `` | **Data Category:** `DIMENSION` | **VDM Type:** `BASIC` | **Size:** `L`


## Entity: `SalesOrder`

- **ABAP CDS Name:** `I_SalesOrder`
- **Label:** Sales Order
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** VBAK, VBKD, VEDA

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `SalesOrder` | `VDM_SALES_ORDER` | `VEDA` | `VBELN` |  |  | `String(10)` | Y | Sales Order |  |  |
| `SalesOrderType` | `SALES_ORDER_TYPE` | `VBAK` | `AUART` |  |  | `String(4)` |  | Sales Order Type |  |  |
| `SalesOrderProcessingType` | `VBKLT` |  |  |  |  | `String(1)` |  | Processing Type |  |  |
| `CreatedByUser` | `ERNAM` |  |  |  |  | `String(12)` |  | Created By |  |  |
| `LastChangedByUser` | `LAST_CHANGED_BY_USER` |  |  |  |  | `String(12)` |  | Last Changed By |  |  |
| `CreationDate` | `ERDAT` | `VBAK` | `ERDAT` |  |  | `Date` |  | Created On |  |  |
| `CreationTime` | `CREATION_TIME` |  |  |  |  | `String(6)` |  | Created At |  |  |
| `LastChangeDate` | `AEDAT` |  |  |  |  | `Date` |  | Changed On |  |  |
| `LastChangeDateTime` | `TIMESTAMPL` |  |  |  |  | `Timestamp` |  | Time Stamp |  |  |
| `SenderBusinessSystemName` | `SD_EXT_BUS_SYST_ID` |  |  |  |  | `String(60)` |  | Ext. Bus. Syst. ID |  |  |
| `ExternalDocumentID` | `SD_EXT_REF_DOC_ID` |  |  |  |  | `String(40)` |  | External Document ID |  |  |
| `ExternalDocLastChangeDateTime` | `EXT_REV_TMSTMP` |  |  |  |  | `Timestamp` |  | External Revision |  |  |
| `SalesOrganization` | `VKORG` | `VBAK` | `VKORG` |  |  | `String(4)` |  | Sales Organization |  |  |
| `DistributionChannel` | `VTWEG` | `VBAK` | `VTWEG` |  |  | `String(2)` |  | Distribution Channel |  |  |
| `OrganizationDivision` | `SPART` |  |  |  |  | `String(2)` |  | Division |  |  |
| `SalesGroup` | `VKGRP` |  |  |  |  | `String(3)` |  | Sales Group |  |  |
| `SalesOffice` | `VKBUR` |  |  |  |  | `String(4)` |  | Sales Office |  |  |
| `SoldToParty` | `KUNAG` | `VBAK` | `KUNNR` |  |  | `String(10)` |  | Sold-to Party |  |  |
| `CustomerGroup` | `KDGRP` |  |  |  |  | `String(2)` |  | Customer Group |  |  |
| `AdditionalCustomerGroup1` | `KVGR1` |  |  |  |  | `String(3)` |  | Customer Group 1 |  |  |
| `AdditionalCustomerGroup2` | `KVGR2` |  |  |  |  | `String(3)` |  | Customer Group 2 |  |  |
| `AdditionalCustomerGroup3` | `KVGR3` |  |  |  |  | `String(3)` |  | Customer Group 3 |  |  |
| `AdditionalCustomerGroup4` | `KVGR4` |  |  |  |  | `String(3)` |  | Customer Group 4 |  |  |
| `AdditionalCustomerGroup5` | `KVGR5` |  |  |  |  | `String(3)` |  | Customer Group 5 |  |  |
| `SlsDocIsRlvtForProofOfDeliv` | `VDM_SD_PROOF_OF_DELIVERY_RLVT` |  |  |  |  | `Boolean` |  | Relevant for Proof of Delivery |  |  |
| `CreditControlArea` | `KKBER` |  |  |  |  | `String(4)` |  | Credit Control Area |  |  |
| `CustomerRebateAgreement` | `KNUMA` |  |  |  |  | `String(10)` |  | Agreement |  |  |
| `SalesOrderDate` | `AUDAT` | `VBAK` | `AUDAT` |  |  | `Date` |  | Document Date |  |  |
| `ServicesRenderedDate` | `VDM_SD_SERVICES_RENDERED_DATE` |  |  |  |  | `Date` |  | Date of Services Rendered |  |  |
| `SDDocumentReason` | `AUGRU` |  |  |  |  | `String(3)` |  | Order Reason |  |  |
| `PurchaseOrderByCustomer` | `BSTKD` | `VBAK` | `BSTNK` |  |  | `String(35)` |  | Customer Reference |  |  |
| `PurchaseOrderByShipToParty` | `SD_PURCHASE_ORDER_BY_SHIPTO` |  |  |  |  | `String(35)` |  | Customer Reference (Ship-to Party) |  |  |
| `SDDocumentCollectiveNumber` | `SUBMI_SD` |  |  |  |  | `String(10)` |  | Collective Number |  |  |
| `CustomerPurchaseOrderType` | `BSARK` |  |  |  |  | `String(4)` |  | Purchase Order Type |  |  |
| `CustomerPurchaseOrderDate` | `VDM_SD_CUSTOMER_REFERENCE_DATE` |  |  |  |  | `Date` |  | Customer Reference Date |  |  |
| `CustomerPurchaseOrderSuplmnt` | `BSTZD` |  |  |  |  | `String(4)` |  | Supplement |  |  |
| `SalesDistrict` | `BZIRK` |  |  |  |  | `String(6)` |  | Sales District |  |  |
| `StatisticsCurrency` | `STWAE` |  |  |  |  | `String(5)` |  | Statistics Currency |  |  |
| `ProductCatalog` | `WMINR` |  |  |  |  | `String(10)` |  | Catalog |  |  |
| `NextCreditCheckDate` | `CMNUP` |  |  |  |  | `Date` |  | Next Credit Check |  |  |
| `LastCustomerContactDate` | `MAHDT` |  |  |  |  | `Date` |  | Last Contact Date |  |  |
| `TotalNetAmount` | `NETWR_AK` |  |  |  |  | `Decimal(34,4)` |  | Net Value | TransactionCurrency |  |
| `TransactionCurrency` | `WAERK` | `VBAK` | `WAERK` |  |  | `String(5)` |  | Document Currency |  |  |
| `PricingDate` | `PRSDT` |  |  |  |  | `Date` |  | Pricing Date |  |  |
| `PriceDetnExchangeRate` | `KURSK_NOT_CONVERTED` |  |  |  |  | `Decimal(9,5)` |  | Exchange Rate |  |  |
| `RetailPromotion` | `WAKTION` |  |  |  |  | `String(10)` |  | Retail Promotion |  |  |
| `SalesOrderCondition` | `KNUMV` |  |  |  |  | `String(10)` |  | Doc. Condition No. |  |  |
| `SDPricingProcedure` | `KALSMASD` |  |  |  |  | `String(6)` |  | Pricing Procedure |  |  |
| `CustomerPriceGroup` | `KONDA` |  |  |  |  | `String(2)` |  | Customer Price Group |  |  |
| `PriceListType` | `PLTYP` |  |  |  |  | `String(2)` |  | Price List Type |  |  |
| `BillingPlan` | `FPLNR` |  |  |  |  | `String(10)` |  | Bill. Plan No. |  |  |
| `CustomerTaxClassification1` | `TAXK1_AK` |  |  |  |  | `String(1)` |  | Alt.Tax Classific. |  |  |
| `CustomerTaxClassification2` | `TAXK2` |  |  |  |  | `String(1)` |  | Tax Class.2 Customer |  |  |
| `CustomerTaxClassification3` | `TAXK3` |  |  |  |  | `String(1)` |  | Tax Class.3 Customer |  |  |
| `CustomerTaxClassification4` | `TAXK4` |  |  |  |  | `String(1)` |  | Tax Class.4 Customer |  |  |
| `CustomerTaxClassification5` | `TAXK5` |  |  |  |  | `String(1)` |  | Tax Class.5 Customer |  |  |
| `CustomerTaxClassification6` | `TAXK6` |  |  |  |  | `String(1)` |  | Tax Class.6 Customer |  |  |
| `CustomerTaxClassification7` | `TAXK7` |  |  |  |  | `String(1)` |  | Tax Class.7 Customer |  |  |
| `CustomerTaxClassification8` | `TAXK8` |  |  |  |  | `String(1)` |  | Tax Class.8 Customer |  |  |
| `CustomerTaxClassification9` | `TAXK9` |  |  |  |  | `String(1)` |  | Tax Class.9 Customer |  |  |
| `TaxDepartureCountry` | `VDM_SD_TAX_DEPARTURE_COUNTRY` |  |  |  |  | `String(3)` |  | Tax Departure Country/Region |  |  |
| `VATRegistrationCountry` | `VDM_SD_VAT_REGISTRATION_CNTRY` |  |  |  |  | `String(3)` |  | Tax Destination Country/Region |  |  |
| `RequestedDeliveryDate` | `REQD_DELIVERY_DATE` |  |  |  |  | `Date` |  | Requested Delivery Date |  |  |
| `DeliveryDateTypeRule` | `VDM_SD_DELIVERY_DATE_TYPE_RULE` |  |  |  |  | `String(1)` |  | Delivery Date Rule |  |  |
| `ShippingType` | `VSARTTR` |  |  |  |  | `String(2)` |  | Shipping Type |  |  |
| `ShippingCondition` | `VSBED` |  |  |  |  | `String(2)` |  | Shipping Conditions |  |  |
| `ReceivingPoint` | `EMPST` |  |  |  |  | `String(25)` |  | Receiving Point |  |  |
| `IncotermsClassification` | `INCO1` |  |  |  |  | `String(3)` |  | Incoterms |  |  |
| `IncotermsTransferLocation` | `INCO2` |  |  |  |  | `String(28)` |  | Incoterms (Part 2) |  |  |
| `IncotermsLocation1` | `INCO2_L` |  |  |  |  | `String(70)` |  | Incoterms Location 1 |  |  |
| `IncotermsLocation2` | `INCO3_L` |  |  |  |  | `String(70)` |  | Incoterms Location 2 |  |  |
| `IncotermsVersion` | `INCOV` |  |  |  |  | `String(4)` |  | Incoterms Version |  |  |
| `CompleteDeliveryIsDefined` | `AUTLF` |  |  |  |  | `Boolean` |  | Complete Delivery |  |  |
| `OrderCombinationIsAllowed` | `VDM_SD_ORDER_COMBINATION_IND` |  |  |  |  | `Boolean` |  | Order Combination |  |  |
| `DeliveryBlockReason` | `LIFSK` |  |  |  |  | `String(2)` |  | Delivery Block |  |  |
| `FashionCancelDate` | `FSH_CANDATE` |  |  |  |  | `Date` |  | Cancellation Date |  |  |
| `SalesOrderApprovalReason` | `SD_APM_APPROVAL_REASON_VDM` |  |  |  |  | `String(4)` |  | Approval Request Reason |  |  |
| `BillingDocumentDate` | `FKDAT` |  |  |  |  | `Date` |  | Billing Date |  |  |
| `BillingCompanyCode` | `BUKRS_VF` |  |  |  |  | `String(4)` |  | CCode to Be Billed |  |  |
| `HeaderBillingBlockReason` | `FAKSK` |  |  |  |  | `String(2)` |  | Billing Block |  |  |
| `CustomerPaymentTerms` | `DZTERM` |  |  |  |  | `String(4)` |  | Terms of Payment |  |  |
| `PaymentMethod` | `SCHZW_BSEG` |  |  |  |  | `String(1)` |  | Payment Method |  |  |
| `FixedValueDate` | `VALDT` |  |  |  |  | `Date` |  | Fixed Value Date |  |  |
| `FiscalYear` | `GJAHR` |  |  |  |  | `String(4)` |  | Fiscal Year |  |  |
| `FiscalPeriod` | `POPER` |  |  |  |  | `String(3)` |  | Posting Period |  | ECC MONAT unpadded '3'; S/4 ACDOCA.POPER zero-padded '003' |
| `ExchangeRateDate` | `WWERT_D` |  |  |  |  | `Date` |  | Translation Date |  |  |
| `ExchangeRateType` | `KURST` |  |  |  |  | `String(4)` |  | Exchange Rate Type |  |  |
| `AccountingExchangeRate` | `KURRF` |  |  |  |  | `Decimal(9,5)` |  | Exchng. Rate Accntg. |  |  |
| `BusinessArea` | `GSBER` |  |  |  |  | `String(4)` |  | Business Area |  |  |
| `CustomerAccountAssignmentGroup` | `SD_ACCOUNT_ASSGMT_GROUP_CUST` |  |  |  |  | `String(2)` |  | Account Assignment Group for Customer |  |  |
| `CostCenterBusinessArea` | `GSKST` |  |  |  |  | `String(4)` |  | Business Area |  |  |
| `CostCenter` | `KOSTL` |  |  |  |  | `String(10)` |  | Cost Center |  |  |
| `ControllingArea` | `KOKRS` |  |  |  |  | `String(4)` |  | Controlling Area |  |  |
| `OrderID` | `AUFNR` |  |  |  |  | `String(12)` |  | Order |  |  |
| `ControllingObject` | `OBJKO` |  |  |  |  | `String(22)` |  | Object No. Header |  |  |
| `AssignmentReference` | `ORDNR_V` |  |  |  |  | `String(18)` |  | Assignment |  |  |
| `PaymentPlan` | `RPLNR` |  |  |  |  | `String(10)` |  | Paym. Card Plan No. |  |  |
| `ContractAccount` | `CORR_VKONT_KK` |  |  |  |  | `String(12)` |  | Contract Account |  |  |
| `AdditionalValueDays` | `VALTG` |  |  |  |  | `String(2)` |  | Addit. Value Days |  |  |
| `CustomerCreditAccount` | `KNKLI` |  |  |  |  | `String(10)` |  | Credit Account |  |  |
| `ReferenceSDDocument` | `VGBEL` |  |  |  |  | `String(10)` |  | Reference Document |  |  |
| `ReferenceSDDocumentCategory` | `REFERENCE_SD_DOCUMENT_CATEGORY` |  |  |  |  | `String(4)` |  | Reference Document Category |  |  |
| `CorrespncExternalReference` | `IHREZ` |  |  |  |  | `String(12)` |  | Your Reference |  |  |
| `CorrespncExtRefByShipToParty` | `IHREZ_E` |  |  |  |  | `String(12)` |  | Your Reference |  |  |
| `AccountingDocExternalReference` | `XBLNR_V1` |  |  |  |  | `String(16)` |  | Reference |  |  |
| `BusinessSolutionOrder` | `CRMS4_SOLO_OBJECT_ID` |  |  |  |  | `String(10)` |  | Solution Order |  |  |
| `OverallSDProcessStatus` | `GBSTK` |  |  |  |  | `String(1)` |  | Overall Status |  |  |
| `OverallPurchaseConfStatus` | `COSTA_D` |  |  |  |  | `String(1)` |  | Purchasing Conf. Sts |  |  |
| `OverallSDDocumentRejectionSts` | `ABSTK` |  |  |  |  | `String(1)` |  | Rejection Status |  |  |
| `TotalBlockStatus` | `SPSTG` |  |  |  |  | `String(1)` |  | Overall Block Status |  |  |
| `OverallDelivConfStatus` | `BESTK` |  |  |  |  | `String(1)` |  | Delivery Conf. Sts |  |  |
| `OverallTotalDeliveryStatus` | `LKGSK` |  |  |  |  | `String(1)` |  | Ovrl Delivery Status |  |  |
| `OverallDeliveryStatus` | `LFSTK` |  |  |  |  | `String(1)` |  | Delivery Status |  |  |
| `OverallDeliveryBlockStatus` | `DELIVERY_BLOCK_STATUS` |  |  |  |  | `String(1)` |  | Delivery Block Status |  |  |
| `OverallOrdReltdBillgStatus` | `SDMD_ORDER_RELATED_BILLING_STS` |  |  |  |  | `String(1)` |  | Order-Related Billing Status |  |  |
| `OverallBillingBlockStatus` | `BILLING_BLOCK_STATUS` |  |  |  |  | `String(1)` |  | Billing Block Status |  |  |
| `OverallTotalSDDocRefStatus` | `RFGSK` |  |  |  |  | `String(1)` |  | Ovrl Reference Sts |  |  |
| `OverallSDDocReferenceStatus` | `RFSTK` |  |  |  |  | `String(1)` |  | Reference Status |  |  |
| `TotalCreditCheckStatus` | `CMGST` |  |  |  |  | `String(1)` |  | Credit Status |  |  |
| `MaxDocValueCreditCheckStatus` | `CMPSC` |  |  |  |  | `String(1)` |  | Maximum Value |  |  |
| `PaymentTermCreditCheckStatus` | `CMPSD` |  |  |  |  | `String(1)` |  | Terms of Payment |  |  |
| `FinDocCreditCheckStatus` | `CMPSI` |  |  |  |  | `String(1)` |  | Financial Document |  |  |
| `ExprtInsurCreditCheckStatus` | `CMPSJ` |  |  |  |  | `String(1)` |  | Expt Cred. Insurance |  |  |
| `PaytAuthsnCreditCheckSts` | `CMPSK` |  |  |  |  | `String(1)` |  | Payment Card Status |  |  |
| `CentralCreditCheckStatus` | `CMPS_CM` |  |  |  |  | `String(1)` |  | SAP Cred. Mgmt |  |  |
| `CentralCreditChkTechErrSts` | `CMPS_TE` |  |  |  |  | `String(1)` |  | CrMa TE Status |  |  |
| `HdrGeneralIncompletionStatus` | `UVALL_UK` |  |  |  |  | `String(1)` |  | Overall Header |  |  |
| `OverallPricingIncompletionSts` | `UVPRS_UK` |  |  |  |  | `String(1)` |  | Pricing – All Items |  |  |
| `HeaderDelivIncompletionStatus` | `UVVLK_UK` |  |  |  |  | `String(1)` |  | Delivery – Header |  |  |
| `HeaderBillgIncompletionStatus` | `UVFAK_UK` |  |  |  |  | `String(1)` |  | Billing – Header |  |  |
| `OvrlItmGeneralIncompletionSts` | `UVALL_SU` |  |  |  |  | `String(1)` |  | All Items |  |  |
| `OvrlItmBillingIncompletionSts` | `UVFAK_SU` |  |  |  |  | `String(1)` |  | Billing – All Items |  |  |
| `OvrlItmDelivIncompletionSts` | `UVVLS_SU` |  |  |  |  | `String(1)` |  | Delivery – All Items |  |  |
| `OverallChmlCmplncStatus` | `MON_TDD_TOTAL_PCSTA` |  |  |  |  | `String(1)` |  | Product Marketability Status |  |  |
| `OverallDangerousGoodsStatus` | `MON_TDD_TOTAL_DGSTA` |  |  |  |  | `String(1)` |  | Dangerous Goods Status |  |  |
| `OverallSafetyDataSheetStatus` | `MON_TDD_TOTAL_SDSSTA` |  |  |  |  | `String(1)` |  | Safety Data Sheet Status |  |  |
| `SalesDocApprovalStatus` | `SD_APM_APPROVAL_STATUS` |  |  |  |  | `String(1)` |  | Approval Status |  |  |
| `OverallTrdCmplncEmbargoSts` | `TDD_TOTAL_EMCST` |  |  |  |  | `String(1)` |  | Embargo Status |  |  |
| `OvrlTrdCmplncSnctndListChkSts` | `TDD_TOTAL_SLCST` |  |  |  |  | `String(1)` |  | Screening Status |  |  |
| `OvrlTrdCmplncLegalCtrlChkSts` | `VDM_SD_OVRL_LEGAL_CTRL_STATUS` |  |  |  |  | `String(1)` |  | Legal Control Status |  |  |
| `SalesOrderDownPaymentStatus` | `DP_CLEAR_STA` |  |  |  |  | `String(1)` |  | Down Payment Status |  |  |
| `OmniChnlSalesPromotionStatus` | `TDD_BOB_STATUS` |  |  |  |  | `String(1)` |  | OmniChnl Sls Pro Sts |  |  |
| `AlternativePricingDate` | `CROSSITEM_PRC_DATE` |  |  |  |  | `Date` |  | CrossItemPricingDate |  |  |
| `IsEUTriangularDeal` | `XEGDR` |  |  |  |  | `Boolean` |  | EU Triangular Deal |  |  |
| `RetailAdditionalCustomerGrp6` | `FSH_KVGR6` |  |  |  |  | `String(3)` |  | Customer Group 6 |  |  |
| `RetailAdditionalCustomerGrp7` | `FSH_KVGR7` |  |  |  |  | `String(3)` |  | Customer Group 7 |  |  |
| `RetailAdditionalCustomerGrp8` | `FSH_KVGR8` |  |  |  |  | `String(3)` |  | Customer Group 8 |  |  |
| `RetailAdditionalCustomerGrp9` | `FSH_KVGR9` |  |  |  |  | `String(3)` |  | Customer Group 9 |  |  |
| `RetailAdditionalCustomerGrp10` | `FSH_KVGR10` |  |  |  |  | `String(3)` |  | Customer Group 10 |  |  |
| `Store` | `WERKS_D` |  |  |  |  | `String(4)` |  | Plant |  |  |
| `CustomerConditionGroup1` | `KDKG1` |  |  |  |  | `String(2)` |  | Condition Group 1 |  |  |
| `CustomerConditionGroup2` | `KDKG2` |  |  |  |  | `String(2)` |  | Condition Group 2 |  |  |
| `CustomerConditionGroup3` | `KDKG3` |  |  |  |  | `String(2)` |  | Condition Group 3 |  |  |
| `CustomerConditionGroup4` | `KDKG4` |  |  |  |  | `String(2)` |  | Condition Group 4 |  |  |
| `CustomerConditionGroup5` | `KDKG5` |  |  |  |  | `String(2)` |  | Condition Group 5 |  |  |
| `SlsDocSo2PLastContactPersnName` | `SLS_DOC_SO2P_LSTCNTCTPERSN_NM` |  |  |  |  | `String(35)` |  | Name of Last Contact |  |  |
| `SlsDocSo2PLstCntctPersnTelNmbr` | `SLS_DOC_SO2P_LSTCNTCTPERSN_TEL` |  |  |  |  | `String(16)` |  | Tel. No. Last Cntct |  |  |
| `POCorrespncExternalReference` | `SLS_PURG_DOC_EXT_REF` |  |  |  |  | `String(12)` |  | Pur. Order Ext. Ref. |  |  |


## Entity: `SalesOrderItem`

- **ABAP CDS Name:** `I_SalesOrderItem`
- **Label:** Sales Order Item
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** VBAK, VBAP, VBKD, VEDA

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `SalesOrder` | `VDM_SALES_ORDER` | `VEDA` | `VBELN` |  |  | `String(10)` | Y | Sales Order |  |  |
| `SalesOrderItem` | `SALES_ORDER_ITEM` | `VEDA` | `VPOSN` |  |  | `String(6)` | Y | Item |  |  |
| `SalesOrderItemUUID` |  |  |  |  |  | `UUID` |  | GUID 16 |  |  |
| `SalesOrderItemCategory` | `PSTYV` |  |  |  |  | `String(4)` |  | Item Category |  |  |
| `SalesOrderItemType` | `POSAR` |  |  |  |  | `String(1)` |  | Item Type |  |  |
| `IsReturnsItem` | `SHKZG_VA` |  |  |  |  | `Boolean` |  | Returns |  |  |
| `CreatedByUser` | `ERNAM` |  |  |  |  | `String(12)` |  | Created By |  |  |
| `CreationDate` | `ERDAT` | `VBAK` | `ERDAT` |  |  | `Date` |  | Created On |  |  |
| `CreationTime` | `CREATION_TIME` |  |  |  |  | `String(6)` |  | Created At |  |  |
| `LastChangeDate` | `AEDAT` |  |  |  |  | `Date` |  | Changed On |  |  |
| `Division` | `SPART` | `VBAK` | `SPART` |  |  | `String(2)` |  | Division |  |  |
| `Material` | `MATNR` | `VBAP` | `MATNR` |  |  | `String(40)` |  | Material |  |  |
| `Product` | `PRODUCTNUMBER` |  |  |  |  | `String(40)` |  | Product |  |  |
| `OriginallyRequestedMaterial` | `MATWA` |  |  |  |  | `String(40)` |  | Material Entered |  |  |
| `MaterialByCustomer` | `MATNR_KU` |  |  |  |  | `String(35)` |  | Customer Material |  |  |
| `InternationalArticleNumber` | `EAN11` |  |  |  |  | `String(18)` |  | EAN/UPC |  |  |
| `Batch` | `CHARG_D` |  |  |  |  | `String(10)` |  | Batch |  |  |
| `ProductHierarchyNode` | `PRODH_D` |  |  |  |  | `String(18)` |  | Product Hierarchy |  |  |
| `ProductCatalog` | `WMINR` |  |  |  |  | `String(10)` |  | Catalog |  |  |
| `MaterialSubstitutionReason` | `SUGRD` |  |  |  |  | `String(4)` |  | Substitution Reason |  |  |
| `MaterialGroup` | `MATKL` |  |  |  |  | `String(9)` |  | Material Group |  |  |
| `ProductGroup` | `PRODUCTGROUP` |  |  |  |  | `String(9)` |  | Product Group |  |  |
| `MaterialPricingGroup` | `PRODUCTPRICINGGROUP` |  |  |  |  | `String(2)` |  | Product Price Group |  |  |
| `AdditionalMaterialGroup1` | `MVGR1` |  |  |  |  | `String(3)` |  | Material Group 1 |  |  |
| `AdditionalMaterialGroup2` | `MVGR2` |  |  |  |  | `String(3)` |  | Material Group 2 |  |  |
| `AdditionalMaterialGroup3` | `MVGR3` |  |  |  |  | `String(3)` |  | Material Group 3 |  |  |
| `AdditionalMaterialGroup4` | `MVGR4` |  |  |  |  | `String(3)` |  | Material Group 4 |  |  |
| `AdditionalMaterialGroup5` | `MVGR5` |  |  |  |  | `String(3)` |  | Material Group 5 |  |  |
| `Plant` | `WERKS_EXT` | `VBAP` | `WERKS` |  |  | `String(4)` |  | Plant |  |  |
| `OriginalPlant` | `ORIGINAL_PLANT` |  |  |  |  | `String(4)` |  | Original Plant |  |  |
| `StorageLocation` | `LGORT_D` | `VBAP` | `LGORT` |  |  | `String(4)` |  | Storage Location |  |  |
| `DeliveryGroup` | `GRKOR` |  |  |  |  | `String(3)` |  | Delivery Group |  |  |
| `ProductConfiguration` | `CUOBJ_VA` |  |  |  |  | `String(18)` |  | Configuration |  |  |
| `BOMExplosionDate` | `STDAT` |  |  |  |  | `Date` |  | BOM Key Date |  |  |
| `SalesOrderItemText` | `ARKTX` |  |  |  |  | `String(40)` |  | Item Description |  |  |
| `PurchaseOrderByCustomer` | `BSTKD` | `VBAK` | `BSTNK` |  |  | `String(35)` |  | Customer Reference |  |  |
| `PurchaseOrderByShipToParty` | `SD_PURCHASE_ORDER_BY_SHIPTO` |  |  |  |  | `String(35)` |  | Customer Reference (Ship-to Party) |  |  |
| `CustomerPurchaseOrderDate` | `BSTDK` |  |  |  |  | `Date` |  | Customer Ref. Date |  |  |
| `UnderlyingPurchaseOrderItem` | `POSEX` |  |  |  |  | `String(6)` |  | Purchase Order Item |  |  |
| `UndrlgPurOrdItmByShipToParty` | `POSEX_E` |  |  |  |  | `String(6)` |  | Purchase Order Item |  |  |
| `CorrespncExternalReference` | `IHREZ` |  |  |  |  | `String(12)` |  | Your Reference |  |  |
| `CorrespncExtRefByShipToParty` | `IHREZ_E` |  |  |  |  | `String(12)` |  | Your Reference |  |  |
| `ExternalItemID` | `SD_EXT_REF_ITEM_ID` |  |  |  |  | `String(40)` |  | External Item ID |  |  |
| `OrderQuantity` | `KWMENG` |  |  |  |  | `Decimal(15,3)` |  | Order Quantity | OrderQuantityUnit |  |
| `OrderQuantityUnit` | `VRKME` |  |  |  |  | `String(3)` |  | Sales Unit |  |  |
| `OrderToBaseQuantityDnmntr` | `UMVKN` |  |  |  |  | `Decimal(5,0)` |  | Denominator |  |  |
| `OrderToBaseQuantityNmrtr` | `UMVKZ` |  |  |  |  | `Decimal(5,0)` |  | Numerator |  |  |
| `TargetQuantity` | `DZMENG` |  |  |  |  | `Decimal(13,3)` |  | Target Quantity | TargetQuantityUnit |  |
| `TargetQuantityUnit` | `DZIEME` |  |  |  |  | `String(3)` |  | Target Quantity UoM |  |  |
| `TargetToBaseQuantityDnmntr` | `UMZIN` |  |  |  |  | `Decimal(5,0)` |  | Conversion Factor |  |  |
| `TargetToBaseQuantityNmrtr` | `UMZIZ` |  |  |  |  | `Decimal(5,0)` |  | Conversion Factor |  |  |
| `ConfdDelivQtyInOrderQtyUnit` | `CONFIRMED_QUANTITY` |  |  |  |  | `Decimal(15,3)` |  | Confirmed Quantity | OrderQuantityUnit |  |
| `TargetDelivQtyInOrderQtyUnit` | `LSMENG` |  |  |  |  | `Decimal(15,3)` |  | Required Deliv. Qty | OrderQuantityUnit |  |
| `ConfdDeliveryQtyInBaseUnit` | `KLMENG` |  |  |  |  | `Decimal(15,3)` |  | Cumltv Confd Qty(BU) | BaseUnit |  |
| `BaseUnit` | `MEINS` |  |  |  |  | `String(3)` |  | Base Unit of Measure |  |  |
| `CommittedDelivQtyInOrdQtyUnit` | `COMMITTEDDELIVQTYINORDQTYUNIT` |  |  |  |  | `Decimal(15,3)` |  | Committed Delivery Quantity | OrderQuantityUnit |  |
| `CommittedDelivCreationDate` | `COMMITTEDDELIVCREATIONDATE` |  |  |  |  | `Date` |  | Committed Delivery Creation Date |  |  |
| `CommittedDeliveryDate` | `COMMITTEDDELIVERYDATE` |  |  |  |  | `Date` |  | Committed Delivery Date |  |  |
| `RequestedQuantity` | `REQD_QTY` | `VBAP` | `KWMENG` |  |  | `Decimal(15,3)` |  | Requested Quantity | RequestedQuantityUnit |  |
| `RequestedQuantityUnit` | `REQD_QTY_UNIT` |  |  |  |  | `String(3)` |  | Requested Qty Unit |  |  |
| `RequestedQuantityInBaseUnit` | `TDD_REQQTY_BU` |  |  |  |  | `Decimal(15,3)` |  | Requ.SalesOrder Qty. | BaseUnit |  |
| `ItemGrossWeight` | `BRGEW_AP` |  |  |  |  | `Decimal(15,3)` |  | Gross Weight | ItemWeightUnit |  |
| `ItemNetWeight` | `NTGEW_AP` |  |  |  |  | `Decimal(15,3)` |  | Net Weight | ItemWeightUnit |  |
| `ItemWeightUnit` | `GEWEI` |  |  |  |  | `String(3)` |  | Unit of Weight |  |  |
| `ItemVolume` | `VOLUM_AP` |  |  |  |  | `Decimal(15,3)` |  | Volume | ItemVolumeUnit |  |
| `ItemVolumeUnit` | `VOLEH` |  |  |  |  | `String(3)` |  | Volume Unit |  |  |
| `ServicesRenderedDate` | `VDM_SD_SERVICES_RENDERED_DATE` |  |  |  |  | `Date` |  | Date of Services Rendered |  |  |
| `SalesDistrict` | `BZIRK` |  |  |  |  | `String(6)` |  | Sales District |  |  |
| `SalesDeal` | `KNUMA_AG` |  |  |  |  | `String(10)` |  | Sales Deal |  |  |
| `SalesPromotion` | `KNUMA_PI` |  |  |  |  | `String(10)` |  | Promotion |  |  |
| `RetailPromotion` | `WAKTION` |  |  |  |  | `String(10)` |  | Retail Promotion |  |  |
| `CustomerGroup` | `KDGRP` |  |  |  |  | `String(2)` |  | Customer Group |  |  |
| `SalesDocumentRjcnReason` | `ABGRU_VA` |  |  |  |  | `String(2)` |  | Reason for Rejection |  |  |
| `RequirementSegment` | `SGT_RCAT` |  |  |  |  | `String(40)` |  | Requirement Segment |  |  |
| `SlsDocIsRlvtForProofOfDeliv` | `PODKZ` |  |  |  |  | `Boolean` |  | Relevant for POD |  |  |
| `NetAmount` | `NETWR_AP` |  |  |  |  | `Decimal(34,4)` |  | Net Value | TransactionCurrency |  |
| `TransactionCurrency` | `WAERK` | `VBAK` | `WAERK` |  |  | `String(5)` |  | Document Currency |  |  |
| `PricingDate` | `PRSDT` |  |  |  |  | `Date` |  | Pricing Date |  |  |
| `PricingReferenceMaterial` | `PMATN` |  |  |  |  | `String(40)` |  | Pricing Ref. Matl |  |  |
| `ExchangeRateDate` | `WWERT_D` |  |  |  |  | `Date` |  | Translation Date |  |  |
| `PriceDetnExchangeRate` | `KURSK_NOT_CONVERTED` |  |  |  |  | `Decimal(9,5)` |  | Exchange Rate |  |  |
| `NetPriceAmount` | `NETPR` |  |  |  |  | `Decimal(34,4)` |  | Net Price | TransactionCurrency |  |
| `NetPriceQuantity` | `KPEIN` |  |  |  |  | `Decimal(5,0)` |  | Pricing Unit | NetPriceQuantityUnit |  |
| `NetPriceQuantityUnit` | `KMEIN` |  |  |  |  | `String(3)` |  | Unit of Measure |  |  |
| `StatisticalValueControl` | `KOWRR` |  |  |  |  | `String(1)` |  | Statistical Value |  |  |
| `SalesDocumentItemProcgCode` | `TDD_ITEM_PROCESS_CODE` |  |  |  |  | `String(1)` |  | Processing Code |  |  |
| `DownPaymentProcessingVariant` | `SDBIL_DWN_PAYT_PROCG_VAR` |  |  |  |  | `String(1)` |  | Down Payment Variant |  |  |
| `TaxAmount` | `MWSBP` |  |  |  |  | `Decimal(34,4)` |  | Tax Amount | TransactionCurrency |  |
| `ProductTaxClassification1` | `TAXMT` |  |  |  |  | `String(1)` |  | Tax Classifc. Mat. |  |  |
| `ProductTaxClassification2` | `TAXMT` |  |  |  |  | `String(1)` |  | Tax Classifc. Mat. |  |  |
| `ProductTaxClassification3` | `TAXMT` |  |  |  |  | `String(1)` |  | Tax Classifc. Mat. |  |  |
| `ProductTaxClassification4` | `TAXMT` |  |  |  |  | `String(1)` |  | Tax Classifc. Mat. |  |  |
| `ProductTaxClassification5` | `TAXMT` |  |  |  |  | `String(1)` |  | Tax Classifc. Mat. |  |  |
| `ProductTaxClassification6` | `TAXMT` |  |  |  |  | `String(1)` |  | Tax Classifc. Mat. |  |  |
| `ProductTaxClassification7` | `TAXMT` |  |  |  |  | `String(1)` |  | Tax Classifc. Mat. |  |  |
| `ProductTaxClassification8` | `TAXMT` |  |  |  |  | `String(1)` |  | Tax Classifc. Mat. |  |  |
| `ProductTaxClassification9` | `TAXMT` |  |  |  |  | `String(1)` |  | Tax Classifc. Mat. |  |  |
| `MatlAccountAssignmentGroup` | `KTGRM` |  |  |  |  | `String(2)` |  | Acct Assmt Grp Mat. |  |  |
| `CostAmount` | `WAVWR` |  |  |  |  | `Decimal(34,4)` |  | Cost | TransactionCurrency |  |
| `Subtotal1Amount` | `KZWI1` |  |  |  |  | `Decimal(34,4)` |  | Subtotal 1 | TransactionCurrency |  |
| `Subtotal2Amount` | `KZWI2` |  |  |  |  | `Decimal(34,4)` |  | Subtotal 2 | TransactionCurrency |  |
| `Subtotal3Amount` | `KZWI3` |  |  |  |  | `Decimal(34,4)` |  | Subtotal 3 | TransactionCurrency |  |
| `Subtotal4Amount` | `KZWI4` |  |  |  |  | `Decimal(34,4)` |  | Subtotal 4 | TransactionCurrency |  |
| `Subtotal5Amount` | `KZWI5` |  |  |  |  | `Decimal(34,4)` |  | Subtotal 5 | TransactionCurrency |  |
| `Subtotal6Amount` | `KZWI6` |  |  |  |  | `Decimal(34,4)` |  | Subtotal 6 | TransactionCurrency |  |
| `SalesOrderCondition` | `KNUMV` |  |  |  |  | `String(10)` |  | Doc. Condition No. |  |  |
| `CustomerPriceGroup` | `KONDA` |  |  |  |  | `String(2)` |  | Customer Price Group |  |  |
| `ShippingPoint` | `VSTEL` |  |  |  |  | `String(4)` |  | Shipping Point |  |  |
| `ShippingType` | `VSARTTR` |  |  |  |  | `String(2)` |  | Shipping Type |  |  |
| `InventorySpecialStockType` | `SOBKZ` |  |  |  |  | `String(1)` |  | Special Stock |  |  |
| `DeliveryPriority` | `LPRIO` |  |  |  |  | `String(2)` |  | Delivery Priority |  |  |
| `Route` | `ROUTE` |  |  |  |  | `String(6)` |  | Route |  |  |
| `DeliveryDateQuantityIsFixed` | `FIXMG` |  |  |  |  | `Boolean` |  | Fixed Date and Qty |  |  |
| `DeliveryDateTypeRule` | `SD_DELIVERY_DATE_TYPE_RULE` |  |  |  |  | `String(1)` |  | Deliv Date Rule |  |  |
| `PartialDeliveryIsAllowed` | `PARTIAL_DELIVERY_ALLOWED` |  |  |  |  | `String(1)` |  | Partial Delivery for Item |  |  |
| `MaxNmbrOfPartialDelivery` | `NMBRPARTIALDELIV` |  |  |  |  | `Decimal(1,0)` |  | Number of Partial Deliveries |  |  |
| `UnlimitedOverdeliveryIsAllowed` | `UEBTK_V` |  |  |  |  | `Boolean` |  | Unlimited Tolerance |  |  |
| `OverdelivTolrtdLmtRatioInPct` | `UEBTO` |  |  |  |  | `Decimal(3,1)` |  | Overdeliv. Tolerance |  |  |
| `UnderdelivTolrtdLmtRatioInPct` | `UNTTO` |  |  |  |  | `Decimal(3,1)` |  | Underdel. Tolerance |  |  |
| `MinDeliveryQtyInBaseUnit` | `MINLF` |  |  |  |  | `Decimal(13,3)` |  | Minimum Delivery Qty | BaseUnit |  |
| `OpenDeliveryLeadingUnitCode` | `KZFME` |  |  |  |  | `String(1)` |  | Leading UoM |  |  |
| `ItemIsDeliveryRelevant` | `LFREL_AP` |  |  |  |  | `Boolean` |  | Itm Relev.for Deliv. |  |  |
| `ReceivingPoint` | `EMPST` |  |  |  |  | `String(25)` |  | Receiving Point |  |  |
| `IncotermsVersion` | `INCOV` |  |  |  |  | `String(4)` |  | Incoterms Version |  |  |
| `IncotermsClassification` | `INCO1` |  |  |  |  | `String(3)` |  | Incoterms |  |  |
| `IncotermsTransferLocation` | `INCO2` |  |  |  |  | `String(28)` |  | Incoterms (Part 2) |  |  |
| `IncotermsLocation1` | `INCO2_L` |  |  |  |  | `String(70)` |  | Incoterms Location 1 |  |  |
| `IncotermsLocation2` | `INCO3_L` |  |  |  |  | `String(70)` |  | Incoterms Location 2 |  |  |
| `OrderCombinationIsAllowed` | `VDM_SD_ORDER_COMBINATION_IND` |  |  |  |  | `Boolean` |  | Order Combination |  |  |
| `CustomerPaymentTerms` | `DZTERM` |  |  |  |  | `String(4)` |  | Terms of Payment |  |  |
| `PaymentMethod` | `SCHZW_BSEG` |  |  |  |  | `String(1)` |  | Payment Method |  |  |
| `FixedValueDate` | `VALDT` |  |  |  |  | `Date` |  | Fixed Value Date |  |  |
| `AdditionalValueDays` | `VALTG` |  |  |  |  | `String(2)` |  | Addit. Value Days |  |  |
| `ProductSeasonYear` | `FSH_SAISJ` |  |  |  |  | `String(4)` |  | Season Year |  |  |
| `ProductSeason` | `FSH_SAISO` |  |  |  |  | `String(10)` |  | Season |  |  |
| `ProductCollection` | `FSH_COLLECTION` |  |  |  |  | `String(10)` |  | Collection |  |  |
| `ProductTheme` | `FSH_THEME` |  |  |  |  | `String(10)` |  | Theme |  |  |
| `FashionCancelDate` | `FSH_CANDATE` |  |  |  |  | `Date` |  | Cancellation Date |  |  |
| `ProductCharacteristic1` | `WRF_CHARSTC1` |  |  |  |  | `String(18)` |  | Characteristic 1 |  |  |
| `ProductCharacteristic2` | `WRF_CHARSTC2` |  |  |  |  | `String(18)` |  | Characteristic 2 |  |  |
| `ProductCharacteristic3` | `WRF_CHARSTC3` |  |  |  |  | `String(18)` |  | Characteristic 3 |  |  |
| `ShippingGroupNumber` | `RFM_PSST_GROUP_ID` |  |  |  |  | `String(10)` |  | PSST Group |  |  |
| `ShippingGroupRule` | `RFM_PSST_RULE` |  |  |  |  | `String(4)` |  | PSST Grouping Rule |  |  |
| `BillingDocumentDate` | `FKDAT` |  |  |  |  | `Date` |  | Billing Date |  |  |
| `ItemIsBillingRelevant` | `FKREL` |  |  |  |  | `String(1)` |  | Relevant for Billing |  |  |
| `ItemBillingBlockReason` | `FAKSP_AP` |  |  |  |  | `String(2)` |  | Billing Block |  |  |
| `BillingPlan` | `FPLNR` |  |  |  |  | `String(10)` |  | Bill. Plan No. |  |  |
| `FiscalYear` | `GJAHR` |  |  |  |  | `String(4)` |  | Fiscal Year |  |  |
| `FiscalPeriod` | `POPER` |  |  |  |  | `String(3)` |  | Posting Period |  | ECC MONAT unpadded '3'; S/4 ACDOCA.POPER zero-padded '003' |
| `CustomerAccountAssignmentGroup` | `KTGRD` |  |  |  |  | `String(2)` |  | Acct Assmt Grp Cust. |  |  |
| `BusinessArea` | `GSBER` |  |  |  |  | `String(4)` |  | Business Area |  |  |
| `ControllingArea` | `KOKRS` |  |  |  |  | `String(4)` |  | Controlling Area |  |  |
| `ProfitCenter` | `PRCTR` | `VBAP` | `PRCTR` |  |  | `String(10)` |  | Profit Center |  |  |
| `WBSElement` | `PS_PSP_PNR` | `VBAP` | `PS_PSP_PNR` |  |  | `String(8)` |  | WBS Element |  |  |
| `WBSElementInternalID` | `PS_S4_PSPNR` |  |  |  |  | `String(8)` |  | WBS Internal ID |  |  |
| `OrderID` | `AUFNR` |  |  |  |  | `String(12)` |  | Order |  |  |
| `ControllingObject` | `OBJPO` |  |  |  |  | `String(22)` |  | Object No.Item |  |  |
| `ProfitabilitySegment` | `RKEOBJNR_NUMC` |  |  |  |  | `String(10)` |  | Profitability Segment (Deprecated) |  |  |
| `ProfitabilitySegment_2` | `RKEOBJNR_CHAR` |  |  |  |  | `String(10)` |  | Profitability Segment |  |  |
| `OriginSDDocument` | `VBELV` |  |  |  |  | `String(10)` |  | Originating Document |  |  |
| `OriginSDDocumentItem` | `POSNV` |  |  |  |  | `String(6)` |  | Originating Item |  |  |
| `AccountingExchangeRate` | `KURRF` |  |  |  |  | `Decimal(9,5)` |  | Exchng. Rate Accntg. |  |  |
| `ContractAccount` | `CORR_VKONT_KK` |  |  |  |  | `String(12)` |  | Contract Account |  |  |
| `ReferenceSDDocument` | `VGBEL` |  |  |  |  | `String(10)` |  | Reference Document |  |  |
| `ReferenceSDDocumentItem` | `VGPOS` |  |  |  |  | `String(6)` |  | Reference Item |  |  |
| `ReferenceSDDocumentCategory` | `REFERENCE_SD_DOCUMENT_CATEGORY` |  |  |  |  | `String(4)` |  | Reference Document Category |  |  |
| `HigherLevelItem` | `UEPOS` |  |  |  |  | `String(6)` |  | Higher-Level Item |  |  |
| `HigherLevelItemUsage` | `UEPVW` |  |  |  |  | `String(1)` |  | Usage of HL Item |  |  |
| `BusinessSolutionOrder` | `CRMS4_SOLO_OBJECT_ID` |  |  |  |  | `String(10)` |  | Solution Order |  |  |
| `BusinessSolutionOrderItem` | `CRMS4_SOLO_NUMBER_INT` |  |  |  |  | `String(6)` |  | Solution Order Item |  |  |
| `BusSolnOrdItemBundleItem` | `CRMS4_BUNDLE_ITEM_NUMBER` |  |  |  |  | `String(6)` |  | Bundle Item No. |  |  |
| `SDProcessStatus` | `GBSTA` |  |  |  |  | `String(1)` |  | Overall Status |  |  |
| `DeliveryConfirmationStatus` | `BESTA` |  |  |  |  | `String(1)` |  | Delivery Conf. Sts |  |  |
| `PurchaseConfirmationStatus` | `COSTA_D` |  |  |  |  | `String(1)` |  | Purchasing Conf. Sts |  |  |
| `TotalDeliveryStatus` | `LFGSA` |  |  |  |  | `String(1)` |  | Ovrl Delivery Status |  |  |
| `DeliveryStatus` | `LFSTA` |  |  |  |  | `String(1)` |  | Delivery Status |  |  |
| `DeliveryBlockStatus` | `DELIVERY_BLOCK_STATUS` |  |  |  |  | `String(1)` |  | Delivery Block Status |  |  |
| `OrderRelatedBillingStatus` | `SLS_DOC_ORDER_REL_BILLING_STS` |  |  |  |  | `String(1)` |  | Order-Related Billing Status |  |  |
| `BillingBlockStatus` | `FSSTA` |  |  |  |  | `String(1)` |  | Billing Block Status |  |  |
| `ItemGeneralIncompletionStatus` | `ITEM_GENERAL_INCOMPLETION_STS` |  |  |  |  | `String(1)` |  | Incompletion Status |  |  |
| `ItemBillingIncompletionStatus` | `UVFAK_UP` |  |  |  |  | `String(1)` |  | Billing – Item |  |  |
| `PricingIncompletionStatus` | `UVPRS_UP` |  |  |  |  | `String(1)` |  | Pricing – Item |  |  |
| `ItemDeliveryIncompletionStatus` | `UVVLK_UP` |  |  |  |  | `String(1)` |  | Delivery – Item |  |  |
| `SDDocReferenceStatus` | `RFSTA` |  |  |  |  | `String(1)` |  | Reference Status |  |  |
| `SDDocumentRejectionStatus` | `ABSTA_VB` |  |  |  |  | `String(1)` |  | Rejection Status |  |  |
| `TotalSDDocReferenceStatus` | `RFGSA` |  |  |  |  | `String(1)` |  | Ovrl Reference Sts |  |  |
| `ChmlCmplncStatus` | `MON_TDD_PCSTA` |  |  |  |  | `String(1)` |  | Product Marketability Status |  |  |
| `DangerousGoodsStatus` | `MON_TDD_DGSTA` |  |  |  |  | `String(1)` |  | Dangerous Goods Status |  |  |
| `SafetyDataSheetStatus` | `MON_TDD_SDSSTA` |  |  |  |  | `String(1)` |  | Safety Data Sheet Status |  |  |
| `SlsOrderItemDownPaymentStatus` | `DP_CLEAR_STA` |  |  |  |  | `String(1)` |  | Down Payment Status |  |  |
| `TrdCmplncEmbargoSts` | `EMBARGOCHKSTS` |  |  |  |  | `String(1)` |  | Embargo Status |  |  |
| `TrdCmplncSnctndListChkSts` | `WATCHLISTSCRNGCHKSTS` |  |  |  |  | `String(1)` |  | Screening Status |  |  |
| `OvrlTrdCmplncLegalCtrlChkSts` | `LGLCTRLCHKSTS` |  |  |  |  | `String(1)` |  | Legal Control Status |  |  |
| `AltvBsdConfSubstitutionStatus` | `ATP_ABC_SUBSTITUTION_STATUS` |  |  |  |  | `String(1)` |  | Substitution Status |  |  |
| `OmniChannelSalesPromotion` | `TDD_BOB_PROMOTION_ID` |  |  |  |  | `Integer64` |  | OmniChnl PromoID |  |  |
| `OmniChannelSalesPromotionRule` | `TDD_BOB_FG_ID` |  |  |  |  | `Integer64` |  | FGID OmniChnl |  |  |
| `ConsumptionPosting` | `KZVBR` |  |  |  |  | `String(1)` |  | Consumption |  |  |
| `CappedNetAmount` | `CAPPED_NET_AMOUNT` |  |  |  |  | `Decimal(34,4)` |  | Net Amount Cap | TransactionCurrency |  |
| `CappedNetAmtAlertThldInPct` | `CAPPED_NET_AMOUNT_ALERT_THLD` |  |  |  |  | `String(3)` |  | Cap Notif. Threshold |  |  |
| `TotalStandAloneSellingPrice` | `IFRS15_TOTAL_SSP` |  |  |  |  | `Decimal(34,4)` |  | SSP | TransactionCurrency |  |
| `SalesOrderType` | `SALES_ORDER_TYPE` | `VBAK` | `AUART` |  |  | `String(4)` |  | Sales Order Type |  |  |
| `SalesOrganization` | `VKORG` | `VBAK` | `VKORG` |  |  | `String(4)` |  | Sales Organization |  |  |
| `DistributionChannel` | `VTWEG` | `VBAK` | `VTWEG` |  |  | `String(2)` |  | Distribution Channel |  |  |
| `OrganizationDivision` | `SPART` |  |  |  |  | `String(2)` |  | Division |  |  |
| `SalesOffice` | `VKBUR` |  |  |  |  | `String(4)` |  | Sales Office |  |  |
| `SalesGroup` | `VKGRP` |  |  |  |  | `String(3)` |  | Sales Group |  |  |
| `SoldToParty` | `KUNAG` | `VBAK` | `KUNNR` |  |  | `String(10)` |  | Sold-to Party |  |  |
| `AdditionalCustomerGroup1` | `KVGR1` |  |  |  |  | `String(3)` |  | Customer Group 1 |  |  |
| `AdditionalCustomerGroup2` | `KVGR2` |  |  |  |  | `String(3)` |  | Customer Group 2 |  |  |
| `AdditionalCustomerGroup3` | `KVGR3` |  |  |  |  | `String(3)` |  | Customer Group 3 |  |  |
| `AdditionalCustomerGroup4` | `KVGR4` |  |  |  |  | `String(3)` |  | Customer Group 4 |  |  |
| `AdditionalCustomerGroup5` | `KVGR5` |  |  |  |  | `String(3)` |  | Customer Group 5 |  |  |
| `SalesOrderDate` | `AUDAT` | `VBAK` | `AUDAT` |  |  | `Date` |  | Document Date |  |  |
| `SDDocumentReason` | `AUGRU` |  |  |  |  | `String(3)` |  | Order Reason |  |  |
| `RequestedDeliveryDate` | `REQD_DELIVERY_DATE` |  |  |  |  | `Date` |  | Requested Delivery Date |  |  |
| `ShippingCondition` | `VSBED` |  |  |  |  | `String(2)` |  | Shipping Conditions |  |  |
| `ShipToParty` | `KUNWE` |  |  |  |  | `String(10)` |  | Ship-to Party |  |  |
| `PayerParty` | `KUNRG` |  |  |  |  | `String(10)` |  | Payer |  |  |
| `BillToParty` | `KUNRE` |  |  |  |  | `String(10)` |  | Bill-to Party |  |  |
| `SalesEmployee` | `SALES_EMPL` |  |  |  |  | `String(8)` |  | Sales Employee |  |  |
| `ResponsibleEmployee` | `RESP_EMPL` |  |  |  |  | `String(8)` |  | Employee Responsible |  |  |
| `SalesEmployeeWorkAgreement` | `SALES_EMPL` |  |  |  |  | `String(8)` |  | Sales Employee |  |  |
| `ResponsibleEmployeeWorkAgrmt` | `RESP_EMPL` |  |  |  |  | `String(8)` |  | Employee Responsible |  |  |
| `SeasonCompletenessStatus` | `RFM_SCC_INDICATOR` |  |  |  |  | `String(1)` |  | Season Comp.Ind |  |  |
| `CustomerConditionGroup1` | `KDKG1` |  |  |  |  | `String(2)` |  | Condition Group 1 |  |  |
| `CustomerConditionGroup2` | `KDKG2` |  |  |  |  | `String(2)` |  | Condition Group 2 |  |  |
| `CustomerConditionGroup3` | `KDKG3` |  |  |  |  | `String(2)` |  | Condition Group 3 |  |  |
| `CustomerConditionGroup4` | `KDKG4` |  |  |  |  | `String(2)` |  | Condition Group 4 |  |  |
| `CustomerConditionGroup5` | `KDKG5` |  |  |  |  | `String(2)` |  | Condition Group 5 |  |  |
| `POCorrespncExternalReference` | `SLS_PURG_DOC_EXT_REF` |  |  |  |  | `String(12)` |  | Pur. Order Ext. Ref. |  |  |
