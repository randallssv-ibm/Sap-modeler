# SalesOrder

> Source file: `sap-s4com-SalesOrder-v1.json`

**Technical Name:** `` | **Data Category:** `DIMENSION` | **VDM Type:** `BASIC` | **Size:** `L`


## Entity: `SalesOrder`

- **ABAP Name:** `I_SalesOrder`
- **Label:** Sales Order
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** VBAK, VBKD, VEDA

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `SalesOrder` | `VDM_SALES_ORDER` | `VBELN` | `VEDA` | `String(10)` | Y | Sales Order |  |  |  |
| `SalesOrderType` | `SALES_ORDER_TYPE` | `SALES_ORDER_TYPE` | `VBAK` | `String(4)` |  | Sales Order Type |  |  |  |
| `SalesOrderProcessingType` | `VBKLT` | `VBKLT` | `VBAK` | `String(1)` |  | Processing Type |  |  |  |
| `CreatedByUser` | `ERNAM` | `ERNAM` | `VBAK` | `String(12)` |  | Created By |  |  |  |
| `LastChangedByUser` | `LAST_CHANGED_BY_USER` | `LAST_CHANGED_BY_USER` | `VBAK` | `String(12)` |  | Last Changed By |  |  |  |
| `CreationDate` | `ERDAT` | `ERDAT` | `VBAK` | `Date` |  | Created On |  |  |  |
| `CreationTime` | `CREATION_TIME` | `CREATION_TIME` | `VBAK` | `String(6)` |  | Created At |  |  |  |
| `LastChangeDate` | `AEDAT` | `AEDAT` | `VBAK` | `Date` |  | Changed On |  |  |  |
| `LastChangeDateTime` | `TIMESTAMPL` | `TIMESTAMPL` | `VBAK` | `Timestamp` |  | Time Stamp |  |  |  |
| `SenderBusinessSystemName` | `SD_EXT_BUS_SYST_ID` | `SD_EXT_BUS_SYST_ID` | `VBAK` | `String(60)` |  | Ext. Bus. Syst. ID |  |  |  |
| `ExternalDocumentID` | `SD_EXT_REF_DOC_ID` | `SD_EXT_REF_DOC_ID` | `VBAK` | `String(40)` |  | External Document ID |  |  |  |
| `ExternalDocLastChangeDateTime` | `EXT_REV_TMSTMP` | `EXT_REV_TMSTMP` | `VBAK` | `Timestamp` |  | External Revision |  |  |  |
| `SalesOrganization` | `VKORG` | `VKORG` | `VBAK` | `String(4)` |  | Sales Organization |  |  |  |
| `DistributionChannel` | `VTWEG` | `VTWEG` | `VBAK` | `String(2)` |  | Distribution Channel |  |  |  |
| `OrganizationDivision` | `SPART` | `SPART` | `VBAK` | `String(2)` |  | Division |  |  |  |
| `SalesGroup` | `VKGRP` | `VKGRP` | `VBAK` | `String(3)` |  | Sales Group |  |  |  |
| `SalesOffice` | `VKBUR` | `VKBUR` | `VBAK` | `String(4)` |  | Sales Office |  |  |  |
| `SoldToParty` | `KUNAG` | `KUNAG` | `VBAK` | `String(10)` |  | Sold-to Party |  |  |  |
| `CustomerGroup` | `KDGRP` | `KDGRP` | `VBAK` | `String(2)` |  | Customer Group |  |  |  |
| `AdditionalCustomerGroup1` | `KVGR1` | `KVGR1` | `VBAK` | `String(3)` |  | Customer Group 1 |  |  |  |
| `AdditionalCustomerGroup2` | `KVGR2` | `KVGR2` | `VBAK` | `String(3)` |  | Customer Group 2 |  |  |  |
| `AdditionalCustomerGroup3` | `KVGR3` | `KVGR3` | `VBAK` | `String(3)` |  | Customer Group 3 |  |  |  |
| `AdditionalCustomerGroup4` | `KVGR4` | `KVGR4` | `VBAK` | `String(3)` |  | Customer Group 4 |  |  |  |
| `AdditionalCustomerGroup5` | `KVGR5` | `KVGR5` | `VBAK` | `String(3)` |  | Customer Group 5 |  |  |  |
| `SlsDocIsRlvtForProofOfDeliv` | `VDM_SD_PROOF_OF_DELIVERY_RLVT` | `VDM_SD_PROOF_OF_DELIVERY_RLVT` | `VBAK` | `Boolean` |  | Relevant for Proof of Delivery |  |  |  |
| `CreditControlArea` | `KKBER` | `KKBER` | `VBAK` | `String(4)` |  | Credit Control Area |  |  |  |
| `CustomerRebateAgreement` | `KNUMA` | `KNUMA` | `VBAK` | `String(10)` |  | Agreement |  |  |  |
| `SalesOrderDate` | `AUDAT` | `AUDAT` | `VBAK` | `Date` |  | Document Date |  |  |  |
| `ServicesRenderedDate` | `VDM_SD_SERVICES_RENDERED_DATE` | `VDM_SD_SERVICES_RENDERED_DATE` | `VBAK` | `Date` |  | Date of Services Rendered |  |  |  |
| `SDDocumentReason` | `AUGRU` | `AUGRU` | `VBAK` | `String(3)` |  | Order Reason |  |  |  |
| `PurchaseOrderByCustomer` | `BSTKD` | `BSTKD` | `VBAK` | `String(35)` |  | Customer Reference |  |  |  |
| `PurchaseOrderByShipToParty` | `SD_PURCHASE_ORDER_BY_SHIPTO` | `SD_PURCHASE_ORDER_BY_SHIPTO` | `VBAK` | `String(35)` |  | Customer Reference (Ship-to Party) |  |  |  |
| `SDDocumentCollectiveNumber` | `SUBMI_SD` | `SUBMI_SD` | `VBAK` | `String(10)` |  | Collective Number |  |  |  |
| `CustomerPurchaseOrderType` | `BSARK` | `BSARK` | `VBAK` | `String(4)` |  | Purchase Order Type |  |  |  |
| `CustomerPurchaseOrderDate` | `VDM_SD_CUSTOMER_REFERENCE_DATE` | `VDM_SD_CUSTOMER_REFERENCE_DATE` | `VBAK` | `Date` |  | Customer Reference Date |  |  |  |
| `CustomerPurchaseOrderSuplmnt` | `BSTZD` | `BSTZD` | `VBAK` | `String(4)` |  | Supplement |  |  |  |
| `SalesDistrict` | `BZIRK` | `BZIRK` | `VBAK` | `String(6)` |  | Sales District |  |  |  |
| `StatisticsCurrency` | `STWAE` | `STWAE` | `VBAK` | `String(5)` |  | Statistics Currency |  |  |  |
| `ProductCatalog` | `WMINR` | `WMINR` | `VBAK` | `String(10)` |  | Catalog |  |  |  |
| `NextCreditCheckDate` | `CMNUP` | `CMNUP` | `VBAK` | `Date` |  | Next Credit Check |  |  |  |
| `LastCustomerContactDate` | `MAHDT` | `MAHDT` | `VBAK` | `Date` |  | Last Contact Date |  |  |  |
| `TotalNetAmount` | `NETWR_AK` | `NETWR_AK` | `VBAK` | `Decimal(34,4)` |  | Net Value | TransactionCurrency |  |  |
| `TransactionCurrency` | `WAERK` | `WAERK` | `VBAK` | `String(5)` |  | Document Currency |  |  |  |
| `PricingDate` | `PRSDT` | `PRSDT` | `VBAK` | `Date` |  | Pricing Date |  |  |  |
| `PriceDetnExchangeRate` | `KURSK_NOT_CONVERTED` | `KURSK_NOT_CONVERTED` | `VBAK` | `Decimal(9,5)` |  | Exchange Rate |  |  |  |
| `RetailPromotion` | `WAKTION` | `WAKTION` | `VBAK` | `String(10)` |  | Retail Promotion |  |  |  |
| `SalesOrderCondition` | `KNUMV` | `KNUMV` | `VBAK` | `String(10)` |  | Doc. Condition No. |  |  |  |
| `SDPricingProcedure` | `KALSMASD` | `KALSMASD` | `VBAK` | `String(6)` |  | Pricing Procedure |  |  |  |
| `CustomerPriceGroup` | `KONDA` | `KONDA` | `VBAK` | `String(2)` |  | Customer Price Group |  |  |  |
| `PriceListType` | `PLTYP` | `PLTYP` | `VBAK` | `String(2)` |  | Price List Type |  |  |  |
| `BillingPlan` | `FPLNR` | `FPLNR` | `VBAK` | `String(10)` |  | Bill. Plan No. |  |  |  |
| `CustomerTaxClassification1` | `TAXK1_AK` | `TAXK1_AK` | `VBAK` | `String(1)` |  | Alt.Tax Classific. |  |  |  |
| `CustomerTaxClassification2` | `TAXK2` | `TAXK2` | `VBAK` | `String(1)` |  | Tax Class.2 Customer |  |  |  |
| `CustomerTaxClassification3` | `TAXK3` | `TAXK3` | `VBAK` | `String(1)` |  | Tax Class.3 Customer |  |  |  |
| `CustomerTaxClassification4` | `TAXK4` | `TAXK4` | `VBAK` | `String(1)` |  | Tax Class.4 Customer |  |  |  |
| `CustomerTaxClassification5` | `TAXK5` | `TAXK5` | `VBAK` | `String(1)` |  | Tax Class.5 Customer |  |  |  |
| `CustomerTaxClassification6` | `TAXK6` | `TAXK6` | `VBAK` | `String(1)` |  | Tax Class.6 Customer |  |  |  |
| `CustomerTaxClassification7` | `TAXK7` | `TAXK7` | `VBAK` | `String(1)` |  | Tax Class.7 Customer |  |  |  |
| `CustomerTaxClassification8` | `TAXK8` | `TAXK8` | `VBAK` | `String(1)` |  | Tax Class.8 Customer |  |  |  |
| `CustomerTaxClassification9` | `TAXK9` | `TAXK9` | `VBAK` | `String(1)` |  | Tax Class.9 Customer |  |  |  |
| `TaxDepartureCountry` | `VDM_SD_TAX_DEPARTURE_COUNTRY` | `VDM_SD_TAX_DEPARTURE_COUNTRY` | `VBAK` | `String(3)` |  | Tax Departure Country/Region |  |  |  |
| `VATRegistrationCountry` | `VDM_SD_VAT_REGISTRATION_CNTRY` | `VDM_SD_VAT_REGISTRATION_CNTRY` | `VBAK` | `String(3)` |  | Tax Destination Country/Region |  |  |  |
| `RequestedDeliveryDate` | `REQD_DELIVERY_DATE` | `REQD_DELIVERY_DATE` | `VBAK` | `Date` |  | Requested Delivery Date |  |  |  |
| `DeliveryDateTypeRule` | `VDM_SD_DELIVERY_DATE_TYPE_RULE` | `VDM_SD_DELIVERY_DATE_TYPE_RULE` | `VBAK` | `String(1)` |  | Delivery Date Rule |  |  |  |
| `ShippingType` | `VSARTTR` | `VSARTTR` | `VBAK` | `String(2)` |  | Shipping Type |  |  |  |
| `ShippingCondition` | `VSBED` | `VSBED` | `VBAK` | `String(2)` |  | Shipping Conditions |  |  |  |
| `ReceivingPoint` | `EMPST` | `EMPST` | `VBAK` | `String(25)` |  | Receiving Point |  |  |  |
| `IncotermsClassification` | `INCO1` | `INCO1` | `VBAK` | `String(3)` |  | Incoterms |  |  |  |
| `IncotermsTransferLocation` | `INCO2` | `INCO2` | `VBAK` | `String(28)` |  | Incoterms (Part 2) |  |  |  |
| `IncotermsLocation1` | `INCO2_L` | `INCO2_L` | `VBAK` | `String(70)` |  | Incoterms Location 1 |  |  |  |
| `IncotermsLocation2` | `INCO3_L` | `INCO3_L` | `VBAK` | `String(70)` |  | Incoterms Location 2 |  |  |  |
| `IncotermsVersion` | `INCOV` | `INCOV` | `VBAK` | `String(4)` |  | Incoterms Version |  |  |  |
| `CompleteDeliveryIsDefined` | `AUTLF` | `AUTLF` | `VBAK` | `Boolean` |  | Complete Delivery |  |  |  |
| `OrderCombinationIsAllowed` | `VDM_SD_ORDER_COMBINATION_IND` | `VDM_SD_ORDER_COMBINATION_IND` | `VBAK` | `Boolean` |  | Order Combination |  |  |  |
| `DeliveryBlockReason` | `LIFSK` | `LIFSK` | `VBAK` | `String(2)` |  | Delivery Block |  |  |  |
| `FashionCancelDate` | `FSH_CANDATE` | `FSH_CANDATE` | `VBAK` | `Date` |  | Cancellation Date |  |  |  |
| `SalesOrderApprovalReason` | `SD_APM_APPROVAL_REASON_VDM` | `SD_APM_APPROVAL_REASON_VDM` | `VBAK` | `String(4)` |  | Approval Request Reason |  |  |  |
| `BillingDocumentDate` | `FKDAT` | `FKDAT` | `VBAK` | `Date` |  | Billing Date |  |  |  |
| `BillingCompanyCode` | `BUKRS_VF` | `BUKRS_VF` | `VBAK` | `String(4)` |  | CCode to Be Billed |  |  |  |
| `HeaderBillingBlockReason` | `FAKSK` | `FAKSK` | `VBAK` | `String(2)` |  | Billing Block |  |  |  |
| `CustomerPaymentTerms` | `DZTERM` | `DZTERM` | `VBAK` | `String(4)` |  | Terms of Payment |  |  |  |
| `PaymentMethod` | `SCHZW_BSEG` | `SCHZW_BSEG` | `VBAK` | `String(1)` |  | Payment Method |  |  |  |
| `FixedValueDate` | `VALDT` | `VALDT` | `VBAK` | `Date` |  | Fixed Value Date |  |  |  |
| `FiscalYear` | `GJAHR` | `GJAHR` | `VBAK` | `String(4)` |  | Fiscal Year |  |  |  |
| `FiscalPeriod` | `POPER` | `POPER` | `VBAK` | `String(3)` |  | Posting Period |  |  | ECC: unpadded '3' (MONAT); S/4: zero-padded '003' |
| `ExchangeRateDate` | `WWERT_D` | `WWERT` | `VBAK` | `Date` |  | Translation Date |  |  |  |
| `ExchangeRateType` | `KURST` | `KURST` | `VBAK` | `String(4)` |  | Exchange Rate Type |  |  |  |
| `AccountingExchangeRate` | `KURRF` | `KURRF` | `VBAK` | `Decimal(9,5)` |  | Exchng. Rate Accntg. |  |  |  |
| `BusinessArea` | `GSBER` | `GSBER` | `VBAK` | `String(4)` |  | Business Area |  |  |  |
| `CustomerAccountAssignmentGroup` | `SD_ACCOUNT_ASSGMT_GROUP_CUST` | `SD_ACCOUNT_ASSGMT_GROUP_CUST` | `VBAK` | `String(2)` |  | Account Assignment Group for Customer |  |  |  |
| `CostCenterBusinessArea` | `GSKST` | `GSKST` | `VBAK` | `String(4)` |  | Business Area |  |  |  |
| `CostCenter` | `KOSTL` | `KOSTL` | `VBAK` | `String(10)` |  | Cost Center |  |  |  |
| `ControllingArea` | `KOKRS` | `KOKRS` | `VBAK` | `String(4)` |  | Controlling Area |  |  |  |
| `OrderID` | `AUFNR` | `AUFNR` | `VBAK` | `String(12)` |  | Order |  |  |  |
| `ControllingObject` | `OBJKO` | `OBJKO` | `VBAK` | `String(22)` |  | Object No. Header |  |  |  |
| `AssignmentReference` | `ORDNR_V` | `ORDNR_V` | `VBAK` | `String(18)` |  | Assignment |  |  |  |
| `PaymentPlan` | `RPLNR` | `RPLNR` | `VBAK` | `String(10)` |  | Paym. Card Plan No. |  |  |  |
| `ContractAccount` | `CORR_VKONT_KK` | `CORR_VKONT_KK` | `VBAK` | `String(12)` |  | Contract Account |  |  |  |
| `AdditionalValueDays` | `VALTG` | `VALTG` | `VBAK` | `String(2)` |  | Addit. Value Days |  |  |  |
| `CustomerCreditAccount` | `KNKLI` | `KNKLI` | `VBAK` | `String(10)` |  | Credit Account |  |  |  |
| `ReferenceSDDocument` | `VGBEL` | `VGBEL` | `VBAK` | `String(10)` |  | Reference Document |  |  |  |
| `ReferenceSDDocumentCategory` | `REFERENCE_SD_DOCUMENT_CATEGORY` | `REFERENCE_SD_DOCUMENT_CATEGORY` | `VBAK` | `String(4)` |  | Reference Document Category |  |  |  |
| `CorrespncExternalReference` | `IHREZ` | `IHREZ` | `VBAK` | `String(12)` |  | Your Reference |  |  |  |
| `CorrespncExtRefByShipToParty` | `IHREZ_E` | `IHREZ_E` | `VBAK` | `String(12)` |  | Your Reference |  |  |  |
| `AccountingDocExternalReference` | `XBLNR_V1` | `XBLNR_V1` | `VBAK` | `String(16)` |  | Reference |  |  |  |
| `BusinessSolutionOrder` | `CRMS4_SOLO_OBJECT_ID` | `CRMS4_SOLO_OBJECT_ID` | `VBAK` | `String(10)` |  | Solution Order |  |  |  |
| `OverallSDProcessStatus` | `GBSTK` | `GBSTK` | `VBAK` | `String(1)` |  | Overall Status |  |  |  |
| `OverallPurchaseConfStatus` | `COSTA_D` | `COSTA` | `VBAK` | `String(1)` |  | Purchasing Conf. Sts |  |  |  |
| `OverallSDDocumentRejectionSts` | `ABSTK` | `ABSTK` | `VBAK` | `String(1)` |  | Rejection Status |  |  |  |
| `TotalBlockStatus` | `SPSTG` | `SPSTG` | `VBAK` | `String(1)` |  | Overall Block Status |  |  |  |
| `OverallDelivConfStatus` | `BESTK` | `BESTK` | `VBAK` | `String(1)` |  | Delivery Conf. Sts |  |  |  |
| `OverallTotalDeliveryStatus` | `LKGSK` | `LKGSK` | `VBAK` | `String(1)` |  | Ovrl Delivery Status |  |  |  |
| `OverallDeliveryStatus` | `LFSTK` | `LFSTK` | `VBAK` | `String(1)` |  | Delivery Status |  |  |  |
| `OverallDeliveryBlockStatus` | `DELIVERY_BLOCK_STATUS` | `DELIVERY_BLOCK_STATUS` | `VBAK` | `String(1)` |  | Delivery Block Status |  |  |  |
| `OverallOrdReltdBillgStatus` | `SDMD_ORDER_RELATED_BILLING_STS` | `SDMD_ORDER_RELATED_BILLING_STS` | `VBAK` | `String(1)` |  | Order-Related Billing Status |  |  |  |
| `OverallBillingBlockStatus` | `BILLING_BLOCK_STATUS` | `BILLING_BLOCK_STATUS` | `VBAK` | `String(1)` |  | Billing Block Status |  |  |  |
| `OverallTotalSDDocRefStatus` | `RFGSK` | `RFGSK` | `VBAK` | `String(1)` |  | Ovrl Reference Sts |  |  |  |
| `OverallSDDocReferenceStatus` | `RFSTK` | `RFSTK` | `VBAK` | `String(1)` |  | Reference Status |  |  |  |
| `TotalCreditCheckStatus` | `CMGST` | `CMGST` | `VBAK` | `String(1)` |  | Credit Status |  |  |  |
| `MaxDocValueCreditCheckStatus` | `CMPSC` | `CMPSC` | `VBAK` | `String(1)` |  | Maximum Value |  |  |  |
| `PaymentTermCreditCheckStatus` | `CMPSD` | `CMPSD` | `VBAK` | `String(1)` |  | Terms of Payment |  |  |  |
| `FinDocCreditCheckStatus` | `CMPSI` | `CMPSI` | `VBAK` | `String(1)` |  | Financial Document |  |  |  |
| `ExprtInsurCreditCheckStatus` | `CMPSJ` | `CMPSJ` | `VBAK` | `String(1)` |  | Expt Cred. Insurance |  |  |  |
| `PaytAuthsnCreditCheckSts` | `CMPSK` | `CMPSK` | `VBAK` | `String(1)` |  | Payment Card Status |  |  |  |
| `CentralCreditCheckStatus` | `CMPS_CM` | `CMPS_CM` | `VBAK` | `String(1)` |  | SAP Cred. Mgmt |  |  |  |
| `CentralCreditChkTechErrSts` | `CMPS_TE` | `CMPS_TE` | `VBAK` | `String(1)` |  | CrMa TE Status |  |  |  |
| `HdrGeneralIncompletionStatus` | `UVALL_UK` | `UVALL_UK` | `VBAK` | `String(1)` |  | Overall Header |  |  |  |
| `OverallPricingIncompletionSts` | `UVPRS_UK` | `UVPRS_UK` | `VBAK` | `String(1)` |  | Pricing – All Items |  |  |  |
| `HeaderDelivIncompletionStatus` | `UVVLK_UK` | `UVVLK_UK` | `VBAK` | `String(1)` |  | Delivery – Header |  |  |  |
| `HeaderBillgIncompletionStatus` | `UVFAK_UK` | `UVFAK_UK` | `VBAK` | `String(1)` |  | Billing – Header |  |  |  |
| `OvrlItmGeneralIncompletionSts` | `UVALL_SU` | `UVALL_SU` | `VBAK` | `String(1)` |  | All Items |  |  |  |
| `OvrlItmBillingIncompletionSts` | `UVFAK_SU` | `UVFAK_SU` | `VBAK` | `String(1)` |  | Billing – All Items |  |  |  |
| `OvrlItmDelivIncompletionSts` | `UVVLS_SU` | `UVVLS_SU` | `VBAK` | `String(1)` |  | Delivery – All Items |  |  |  |
| `OverallChmlCmplncStatus` | `MON_TDD_TOTAL_PCSTA` | `MON_TDD_TOTAL_PCSTA` | `VBAK` | `String(1)` |  | Product Marketability Status |  |  |  |
| `OverallDangerousGoodsStatus` | `MON_TDD_TOTAL_DGSTA` | `MON_TDD_TOTAL_DGSTA` | `VBAK` | `String(1)` |  | Dangerous Goods Status |  |  |  |
| `OverallSafetyDataSheetStatus` | `MON_TDD_TOTAL_SDSSTA` | `MON_TDD_TOTAL_SDSSTA` | `VBAK` | `String(1)` |  | Safety Data Sheet Status |  |  |  |
| `SalesDocApprovalStatus` | `SD_APM_APPROVAL_STATUS` | `SD_APM_APPROVAL_STATUS` | `VBAK` | `String(1)` |  | Approval Status |  |  |  |
| `OverallTrdCmplncEmbargoSts` | `TDD_TOTAL_EMCST` | `TDD_TOTAL_EMCST` | `VBAK` | `String(1)` |  | Embargo Status |  |  |  |
| `OvrlTrdCmplncSnctndListChkSts` | `TDD_TOTAL_SLCST` | `TDD_TOTAL_SLCST` | `VBAK` | `String(1)` |  | Screening Status |  |  |  |
| `OvrlTrdCmplncLegalCtrlChkSts` | `VDM_SD_OVRL_LEGAL_CTRL_STATUS` | `VDM_SD_OVRL_LEGAL_CTRL_STATUS` | `VBAK` | `String(1)` |  | Legal Control Status |  |  |  |
| `SalesOrderDownPaymentStatus` | `DP_CLEAR_STA` | `DP_CLEAR_STA` | `VBAK` | `String(1)` |  | Down Payment Status |  |  |  |
| `OmniChnlSalesPromotionStatus` | `TDD_BOB_STATUS` | `TDD_BOB_STATUS` | `VBAK` | `String(1)` |  | OmniChnl Sls Pro Sts |  |  |  |
| `AlternativePricingDate` | `CROSSITEM_PRC_DATE` | `CROSSITEM_PRC_DATE` | `VBAK` | `Date` |  | CrossItemPricingDate |  |  |  |
| `IsEUTriangularDeal` | `XEGDR` | `XEGDR` | `VBAK` | `Boolean` |  | EU Triangular Deal |  |  |  |
| `RetailAdditionalCustomerGrp6` | `FSH_KVGR6` | `FSH_KVGR6` | `VBAK` | `String(3)` |  | Customer Group 6 |  |  |  |
| `RetailAdditionalCustomerGrp7` | `FSH_KVGR7` | `FSH_KVGR7` | `VBAK` | `String(3)` |  | Customer Group 7 |  |  |  |
| `RetailAdditionalCustomerGrp8` | `FSH_KVGR8` | `FSH_KVGR8` | `VBAK` | `String(3)` |  | Customer Group 8 |  |  |  |
| `RetailAdditionalCustomerGrp9` | `FSH_KVGR9` | `FSH_KVGR9` | `VBAK` | `String(3)` |  | Customer Group 9 |  |  |  |
| `RetailAdditionalCustomerGrp10` | `FSH_KVGR10` | `FSH_KVGR10` | `VBAK` | `String(3)` |  | Customer Group 10 |  |  |  |
| `Store` | `WERKS_D` | `WERKS` | `VBAK` | `String(4)` |  | Plant |  |  |  |
| `CustomerConditionGroup1` | `KDKG1` | `KDKG1` | `VBAK` | `String(2)` |  | Condition Group 1 |  |  |  |
| `CustomerConditionGroup2` | `KDKG2` | `KDKG2` | `VBAK` | `String(2)` |  | Condition Group 2 |  |  |  |
| `CustomerConditionGroup3` | `KDKG3` | `KDKG3` | `VBAK` | `String(2)` |  | Condition Group 3 |  |  |  |
| `CustomerConditionGroup4` | `KDKG4` | `KDKG4` | `VBAK` | `String(2)` |  | Condition Group 4 |  |  |  |
| `CustomerConditionGroup5` | `KDKG5` | `KDKG5` | `VBAK` | `String(2)` |  | Condition Group 5 |  |  |  |
| `SlsDocSo2PLastContactPersnName` | `SLS_DOC_SO2P_LSTCNTCTPERSN_NM` | `SLS_DOC_SO2P_LSTCNTCTPERSN_NM` | `VBAK` | `String(35)` |  | Name of Last Contact |  |  |  |
| `SlsDocSo2PLstCntctPersnTelNmbr` | `SLS_DOC_SO2P_LSTCNTCTPERSN_TEL` | `SLS_DOC_SO2P_LSTCNTCTPERSN_TEL` | `VBAK` | `String(16)` |  | Tel. No. Last Cntct |  |  |  |
| `POCorrespncExternalReference` | `SLS_PURG_DOC_EXT_REF` | `SLS_PURG_DOC_EXT_REF` | `VBAK` | `String(12)` |  | Pur. Order Ext. Ref. |  |  |  |


## Entity: `SalesOrderItem`

- **ABAP Name:** `I_SalesOrderItem`
- **Label:** Sales Order Item
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** VBAK, VBAP, VBKD, VEDA

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `SalesOrder` | `VDM_SALES_ORDER` | `VBELN` | `VEDA` | `String(10)` | Y | Sales Order |  | _SalesOrder |  |
| `SalesOrderItem` | `SALES_ORDER_ITEM` | `VPOSN` | `VEDA` | `String(6)` | Y | Item |  |  |  |
| `SalesOrderItemUUID` |  |  |  | `UUID` |  | GUID 16 |  |  |  |
| `SalesOrderItemCategory` | `PSTYV` | `PSTYV` | `VBAP` | `String(4)` |  | Item Category |  |  |  |
| `SalesOrderItemType` | `POSAR` | `POSAR` | `VBAP` | `String(1)` |  | Item Type |  |  |  |
| `IsReturnsItem` | `SHKZG_VA` | `SHKZG_VA` | `VBAP` | `Boolean` |  | Returns |  |  |  |
| `CreatedByUser` | `ERNAM` | `ERNAM` | `VBAP` | `String(12)` |  | Created By |  |  |  |
| `CreationDate` | `ERDAT` | `ERDAT` | `VBAP` | `Date` |  | Created On |  |  |  |
| `CreationTime` | `CREATION_TIME` | `CREATION_TIME` | `VBAP` | `String(6)` |  | Created At |  |  |  |
| `LastChangeDate` | `AEDAT` | `AEDAT` | `VBAP` | `Date` |  | Changed On |  |  |  |
| `Division` | `SPART` | `SPART` | `VBAP` | `String(2)` |  | Division |  |  |  |
| `Material` | `MATNR` | `MATNR` | `VBAP` | `String(40)` |  | Material |  |  |  |
| `Product` | `PRODUCTNUMBER` | `PRODUCTNUMBER` | `VBAP` | `String(40)` |  | Product |  |  |  |
| `OriginallyRequestedMaterial` | `MATWA` | `MATWA` | `VBAP` | `String(40)` |  | Material Entered |  |  |  |
| `MaterialByCustomer` | `MATNR_KU` | `MATNR_KU` | `VBAP` | `String(35)` |  | Customer Material |  |  |  |
| `InternationalArticleNumber` | `EAN11` | `EAN11` | `VBAP` | `String(18)` |  | EAN/UPC |  |  |  |
| `Batch` | `CHARG_D` | `CHARG` | `VBAP` | `String(10)` |  | Batch |  |  |  |
| `ProductHierarchyNode` | `PRODH_D` | `PRODH` | `VBAP` | `String(18)` |  | Product Hierarchy |  |  |  |
| `ProductCatalog` | `WMINR` | `WMINR` | `VBAP` | `String(10)` |  | Catalog |  |  |  |
| `MaterialSubstitutionReason` | `SUGRD` | `SUGRD` | `VBAP` | `String(4)` |  | Substitution Reason |  |  |  |
| `MaterialGroup` | `MATKL` | `MATKL` | `VBAP` | `String(9)` |  | Material Group |  |  |  |
| `ProductGroup` | `PRODUCTGROUP` | `PRODUCTGROUP` | `VBAP` | `String(9)` |  | Product Group |  |  |  |
| `MaterialPricingGroup` | `PRODUCTPRICINGGROUP` | `PRODUCTPRICINGGROUP` | `VBAP` | `String(2)` |  | Product Price Group |  |  |  |
| `AdditionalMaterialGroup1` | `MVGR1` | `MVGR1` | `VBAP` | `String(3)` |  | Material Group 1 |  |  |  |
| `AdditionalMaterialGroup2` | `MVGR2` | `MVGR2` | `VBAP` | `String(3)` |  | Material Group 2 |  |  |  |
| `AdditionalMaterialGroup3` | `MVGR3` | `MVGR3` | `VBAP` | `String(3)` |  | Material Group 3 |  |  |  |
| `AdditionalMaterialGroup4` | `MVGR4` | `MVGR4` | `VBAP` | `String(3)` |  | Material Group 4 |  |  |  |
| `AdditionalMaterialGroup5` | `MVGR5` | `MVGR5` | `VBAP` | `String(3)` |  | Material Group 5 |  |  |  |
| `Plant` | `WERKS_EXT` | `WERKS_EXT` | `VBAP` | `String(4)` |  | Plant |  |  |  |
| `OriginalPlant` | `ORIGINAL_PLANT` | `ORIGINAL_PLANT` | `VBAP` | `String(4)` |  | Original Plant |  |  |  |
| `StorageLocation` | `LGORT_D` | `LGORT` | `VBAP` | `String(4)` |  | Storage Location |  |  |  |
| `DeliveryGroup` | `GRKOR` | `GRKOR` | `VBAP` | `String(3)` |  | Delivery Group |  |  |  |
| `ProductConfiguration` | `CUOBJ_VA` | `CUOBJ_VA` | `VBAP` | `String(18)` |  | Configuration |  |  |  |
| `BOMExplosionDate` | `STDAT` | `STDAT` | `VBAP` | `Date` |  | BOM Key Date |  |  |  |
| `SalesOrderItemText` | `ARKTX` | `ARKTX` | `VBAP` | `String(40)` |  | Item Description |  |  |  |
| `PurchaseOrderByCustomer` | `BSTKD` | `BSTKD` | `VBAP` | `String(35)` |  | Customer Reference |  |  |  |
| `PurchaseOrderByShipToParty` | `SD_PURCHASE_ORDER_BY_SHIPTO` | `SD_PURCHASE_ORDER_BY_SHIPTO` | `VBAP` | `String(35)` |  | Customer Reference (Ship-to Party) |  |  |  |
| `CustomerPurchaseOrderDate` | `BSTDK` | `BSTDK` | `VBAP` | `Date` |  | Customer Ref. Date |  |  |  |
| `UnderlyingPurchaseOrderItem` | `POSEX` | `POSEX` | `VBAP` | `String(6)` |  | Purchase Order Item |  |  |  |
| `UndrlgPurOrdItmByShipToParty` | `POSEX_E` | `POSEX_E` | `VBAP` | `String(6)` |  | Purchase Order Item |  |  |  |
| `CorrespncExternalReference` | `IHREZ` | `IHREZ` | `VBAP` | `String(12)` |  | Your Reference |  |  |  |
| `CorrespncExtRefByShipToParty` | `IHREZ_E` | `IHREZ_E` | `VBAP` | `String(12)` |  | Your Reference |  |  |  |
| `ExternalItemID` | `SD_EXT_REF_ITEM_ID` | `SD_EXT_REF_ITEM_ID` | `VBAP` | `String(40)` |  | External Item ID |  |  |  |
| `OrderQuantity` | `KWMENG` | `KWMENG` | `VBAP` | `Decimal(15,3)` |  | Order Quantity | OrderQuantityUnit |  |  |
| `OrderQuantityUnit` | `VRKME` | `VRKME` | `VBAP` | `String(3)` |  | Sales Unit |  |  |  |
| `OrderToBaseQuantityDnmntr` | `UMVKN` | `UMVKN` | `VBAP` | `Decimal(5,0)` |  | Denominator |  |  |  |
| `OrderToBaseQuantityNmrtr` | `UMVKZ` | `UMVKZ` | `VBAP` | `Decimal(5,0)` |  | Numerator |  |  |  |
| `TargetQuantity` | `DZMENG` | `DZMENG` | `VBAP` | `Decimal(13,3)` |  | Target Quantity | TargetQuantityUnit |  |  |
| `TargetQuantityUnit` | `DZIEME` | `DZIEME` | `VBAP` | `String(3)` |  | Target Quantity UoM |  |  |  |
| `TargetToBaseQuantityDnmntr` | `UMZIN` | `UMZIN` | `VBAP` | `Decimal(5,0)` |  | Conversion Factor |  |  |  |
| `TargetToBaseQuantityNmrtr` | `UMZIZ` | `UMZIZ` | `VBAP` | `Decimal(5,0)` |  | Conversion Factor |  |  |  |
| `ConfdDelivQtyInOrderQtyUnit` | `CONFIRMED_QUANTITY` | `CONFIRMED_QUANTITY` | `VBAP` | `Decimal(15,3)` |  | Confirmed Quantity | OrderQuantityUnit |  |  |
| `TargetDelivQtyInOrderQtyUnit` | `LSMENG` | `LSMENG` | `VBAP` | `Decimal(15,3)` |  | Required Deliv. Qty | OrderQuantityUnit |  |  |
| `ConfdDeliveryQtyInBaseUnit` | `KLMENG` | `KLMENG` | `VBAP` | `Decimal(15,3)` |  | Cumltv Confd Qty(BU) | BaseUnit |  |  |
| `BaseUnit` | `MEINS` | `MEINS` | `VBAP` | `String(3)` |  | Base Unit of Measure |  |  |  |
| `CommittedDelivQtyInOrdQtyUnit` | `COMMITTEDDELIVQTYINORDQTYUNIT` | `COMMITTEDDELIVQTYINORDQTYUNIT` | `VBAP` | `Decimal(15,3)` |  | Committed Delivery Quantity | OrderQuantityUnit |  |  |
| `CommittedDelivCreationDate` | `COMMITTEDDELIVCREATIONDATE` | `COMMITTEDDELIVCREATIONDATE` | `VBAP` | `Date` |  | Committed Delivery Creation Date |  |  |  |
| `CommittedDeliveryDate` | `COMMITTEDDELIVERYDATE` | `COMMITTEDDELIVERYDATE` | `VBAP` | `Date` |  | Committed Delivery Date |  |  |  |
| `RequestedQuantity` | `REQD_QTY` | `REQD_QTY` | `VBAP` | `Decimal(15,3)` |  | Requested Quantity | RequestedQuantityUnit |  |  |
| `RequestedQuantityUnit` | `REQD_QTY_UNIT` | `REQD_QTY_UNIT` | `VBAP` | `String(3)` |  | Requested Qty Unit |  |  |  |
| `RequestedQuantityInBaseUnit` | `TDD_REQQTY_BU` | `TDD_REQQTY_BU` | `VBAP` | `Decimal(15,3)` |  | Requ.SalesOrder Qty. | BaseUnit |  |  |
| `ItemGrossWeight` | `BRGEW_AP` | `BRGEW_AP` | `VBAP` | `Decimal(15,3)` |  | Gross Weight | ItemWeightUnit |  |  |
| `ItemNetWeight` | `NTGEW_AP` | `NTGEW_AP` | `VBAP` | `Decimal(15,3)` |  | Net Weight | ItemWeightUnit |  |  |
| `ItemWeightUnit` | `GEWEI` | `GEWEI` | `VBAP` | `String(3)` |  | Unit of Weight |  |  |  |
| `ItemVolume` | `VOLUM_AP` | `VOLUM_AP` | `VBAP` | `Decimal(15,3)` |  | Volume | ItemVolumeUnit |  |  |
| `ItemVolumeUnit` | `VOLEH` | `VOLEH` | `VBAP` | `String(3)` |  | Volume Unit |  |  |  |
| `ServicesRenderedDate` | `VDM_SD_SERVICES_RENDERED_DATE` | `VDM_SD_SERVICES_RENDERED_DATE` | `VBAP` | `Date` |  | Date of Services Rendered |  |  |  |
| `SalesDistrict` | `BZIRK` | `BZIRK` | `VBAP` | `String(6)` |  | Sales District |  |  |  |
| `SalesDeal` | `KNUMA_AG` | `KNUMA_AG` | `VBAP` | `String(10)` |  | Sales Deal |  |  |  |
| `SalesPromotion` | `KNUMA_PI` | `KNUMA_PI` | `VBAP` | `String(10)` |  | Promotion |  |  |  |
| `RetailPromotion` | `WAKTION` | `WAKTION` | `VBAP` | `String(10)` |  | Retail Promotion |  |  |  |
| `CustomerGroup` | `KDGRP` | `KDGRP` | `VBAP` | `String(2)` |  | Customer Group |  |  |  |
| `SalesDocumentRjcnReason` | `ABGRU_VA` | `ABGRU_VA` | `VBAP` | `String(2)` |  | Reason for Rejection |  |  |  |
| `RequirementSegment` | `SGT_RCAT` | `SGT_RCAT` | `VBAP` | `String(40)` |  | Requirement Segment |  |  |  |
| `SlsDocIsRlvtForProofOfDeliv` | `PODKZ` | `PODKZ` | `VBAP` | `Boolean` |  | Relevant for POD |  |  |  |
| `NetAmount` | `NETWR_AP` | `NETWR_AP` | `VBAP` | `Decimal(34,4)` |  | Net Value | TransactionCurrency |  |  |
| `TransactionCurrency` | `WAERK` | `WAERK` | `VBAP` | `String(5)` |  | Document Currency |  |  |  |
| `PricingDate` | `PRSDT` | `PRSDT` | `VBAP` | `Date` |  | Pricing Date |  |  |  |
| `PricingReferenceMaterial` | `PMATN` | `PMATN` | `VBAP` | `String(40)` |  | Pricing Ref. Matl |  |  |  |
| `ExchangeRateDate` | `WWERT_D` | `WWERT` | `VBAP` | `Date` |  | Translation Date |  |  |  |
| `PriceDetnExchangeRate` | `KURSK_NOT_CONVERTED` | `KURSK_NOT_CONVERTED` | `VBAP` | `Decimal(9,5)` |  | Exchange Rate |  |  |  |
| `NetPriceAmount` | `NETPR` | `NETPR` | `VBAP` | `Decimal(34,4)` |  | Net Price | TransactionCurrency |  |  |
| `NetPriceQuantity` | `KPEIN` | `KPEIN` | `VBAP` | `Decimal(5,0)` |  | Pricing Unit | NetPriceQuantityUnit |  |  |
| `NetPriceQuantityUnit` | `KMEIN` | `KMEIN` | `VBAP` | `String(3)` |  | Unit of Measure |  |  |  |
| `StatisticalValueControl` | `KOWRR` | `KOWRR` | `VBAP` | `String(1)` |  | Statistical Value |  |  |  |
| `SalesDocumentItemProcgCode` | `TDD_ITEM_PROCESS_CODE` | `TDD_ITEM_PROCESS_CODE` | `VBAP` | `String(1)` |  | Processing Code |  |  |  |
| `DownPaymentProcessingVariant` | `SDBIL_DWN_PAYT_PROCG_VAR` | `SDBIL_DWN_PAYT_PROCG_VAR` | `VBAP` | `String(1)` |  | Down Payment Variant |  |  |  |
| `TaxAmount` | `MWSBP` | `MWSBP` | `VBAP` | `Decimal(34,4)` |  | Tax Amount | TransactionCurrency |  |  |
| `ProductTaxClassification1` | `TAXMT` | `TAXMT` | `VBAP` | `String(1)` |  | Tax Classifc. Mat. |  |  |  |
| `ProductTaxClassification2` | `TAXMT` | `TAXMT` | `VBAP` | `String(1)` |  | Tax Classifc. Mat. |  |  |  |
| `ProductTaxClassification3` | `TAXMT` | `TAXMT` | `VBAP` | `String(1)` |  | Tax Classifc. Mat. |  |  |  |
| `ProductTaxClassification4` | `TAXMT` | `TAXMT` | `VBAP` | `String(1)` |  | Tax Classifc. Mat. |  |  |  |
| `ProductTaxClassification5` | `TAXMT` | `TAXMT` | `VBAP` | `String(1)` |  | Tax Classifc. Mat. |  |  |  |
| `ProductTaxClassification6` | `TAXMT` | `TAXMT` | `VBAP` | `String(1)` |  | Tax Classifc. Mat. |  |  |  |
| `ProductTaxClassification7` | `TAXMT` | `TAXMT` | `VBAP` | `String(1)` |  | Tax Classifc. Mat. |  |  |  |
| `ProductTaxClassification8` | `TAXMT` | `TAXMT` | `VBAP` | `String(1)` |  | Tax Classifc. Mat. |  |  |  |
| `ProductTaxClassification9` | `TAXMT` | `TAXMT` | `VBAP` | `String(1)` |  | Tax Classifc. Mat. |  |  |  |
| `MatlAccountAssignmentGroup` | `KTGRM` | `KTGRM` | `VBAP` | `String(2)` |  | Acct Assmt Grp Mat. |  |  |  |
| `CostAmount` | `WAVWR` | `WAVWR` | `VBAP` | `Decimal(34,4)` |  | Cost | TransactionCurrency |  |  |
| `Subtotal1Amount` | `KZWI1` | `KZWI1` | `VBAP` | `Decimal(34,4)` |  | Subtotal 1 | TransactionCurrency |  |  |
| `Subtotal2Amount` | `KZWI2` | `KZWI2` | `VBAP` | `Decimal(34,4)` |  | Subtotal 2 | TransactionCurrency |  |  |
| `Subtotal3Amount` | `KZWI3` | `KZWI3` | `VBAP` | `Decimal(34,4)` |  | Subtotal 3 | TransactionCurrency |  |  |
| `Subtotal4Amount` | `KZWI4` | `KZWI4` | `VBAP` | `Decimal(34,4)` |  | Subtotal 4 | TransactionCurrency |  |  |
| `Subtotal5Amount` | `KZWI5` | `KZWI5` | `VBAP` | `Decimal(34,4)` |  | Subtotal 5 | TransactionCurrency |  |  |
| `Subtotal6Amount` | `KZWI6` | `KZWI6` | `VBAP` | `Decimal(34,4)` |  | Subtotal 6 | TransactionCurrency |  |  |
| `SalesOrderCondition` | `KNUMV` | `KNUMV` | `VBAP` | `String(10)` |  | Doc. Condition No. |  |  |  |
| `CustomerPriceGroup` | `KONDA` | `KONDA` | `VBAP` | `String(2)` |  | Customer Price Group |  |  |  |
| `ShippingPoint` | `VSTEL` | `VSTEL` | `VBAP` | `String(4)` |  | Shipping Point |  |  |  |
| `ShippingType` | `VSARTTR` | `VSARTTR` | `VBAP` | `String(2)` |  | Shipping Type |  |  |  |
| `InventorySpecialStockType` | `SOBKZ` | `SOBKZ` | `VBAP` | `String(1)` |  | Special Stock |  |  |  |
| `DeliveryPriority` | `LPRIO` | `LPRIO` | `VBAP` | `String(2)` |  | Delivery Priority |  |  |  |
| `Route` | `ROUTE` | `ROUTE` | `VBAP` | `String(6)` |  | Route |  |  |  |
| `DeliveryDateQuantityIsFixed` | `FIXMG` | `FIXMG` | `VBAP` | `Boolean` |  | Fixed Date and Qty |  |  |  |
| `DeliveryDateTypeRule` | `SD_DELIVERY_DATE_TYPE_RULE` | `SD_DELIVERY_DATE_TYPE_RULE` | `VBAP` | `String(1)` |  | Deliv Date Rule |  |  |  |
| `PartialDeliveryIsAllowed` | `PARTIAL_DELIVERY_ALLOWED` | `PARTIAL_DELIVERY_ALLOWED` | `VBAP` | `String(1)` |  | Partial Delivery for Item |  |  |  |
| `MaxNmbrOfPartialDelivery` | `NMBRPARTIALDELIV` | `NMBRPARTIALDELIV` | `VBAP` | `Decimal(1,0)` |  | Number of Partial Deliveries |  |  |  |
| `UnlimitedOverdeliveryIsAllowed` | `UEBTK_V` | `UEBTK_V` | `VBAP` | `Boolean` |  | Unlimited Tolerance |  |  |  |
| `OverdelivTolrtdLmtRatioInPct` | `UEBTO` | `UEBTO` | `VBAP` | `Decimal(3,1)` |  | Overdeliv. Tolerance |  |  |  |
| `UnderdelivTolrtdLmtRatioInPct` | `UNTTO` | `UNTTO` | `VBAP` | `Decimal(3,1)` |  | Underdel. Tolerance |  |  |  |
| `MinDeliveryQtyInBaseUnit` | `MINLF` | `MINLF` | `VBAP` | `Decimal(13,3)` |  | Minimum Delivery Qty | BaseUnit |  |  |
| `OpenDeliveryLeadingUnitCode` | `KZFME` | `KZFME` | `VBAP` | `String(1)` |  | Leading UoM |  |  |  |
| `ItemIsDeliveryRelevant` | `LFREL_AP` | `LFREL_AP` | `VBAP` | `Boolean` |  | Itm Relev.for Deliv. |  |  |  |
| `ReceivingPoint` | `EMPST` | `EMPST` | `VBAP` | `String(25)` |  | Receiving Point |  |  |  |
| `IncotermsVersion` | `INCOV` | `INCOV` | `VBAP` | `String(4)` |  | Incoterms Version |  |  |  |
| `IncotermsClassification` | `INCO1` | `INCO1` | `VBAP` | `String(3)` |  | Incoterms |  |  |  |
| `IncotermsTransferLocation` | `INCO2` | `INCO2` | `VBAP` | `String(28)` |  | Incoterms (Part 2) |  |  |  |
| `IncotermsLocation1` | `INCO2_L` | `INCO2_L` | `VBAP` | `String(70)` |  | Incoterms Location 1 |  |  |  |
| `IncotermsLocation2` | `INCO3_L` | `INCO3_L` | `VBAP` | `String(70)` |  | Incoterms Location 2 |  |  |  |
| `OrderCombinationIsAllowed` | `VDM_SD_ORDER_COMBINATION_IND` | `VDM_SD_ORDER_COMBINATION_IND` | `VBAP` | `Boolean` |  | Order Combination |  |  |  |
| `CustomerPaymentTerms` | `DZTERM` | `DZTERM` | `VBAP` | `String(4)` |  | Terms of Payment |  |  |  |
| `PaymentMethod` | `SCHZW_BSEG` | `SCHZW_BSEG` | `VBAP` | `String(1)` |  | Payment Method |  |  |  |
| `FixedValueDate` | `VALDT` | `VALDT` | `VBAP` | `Date` |  | Fixed Value Date |  |  |  |
| `AdditionalValueDays` | `VALTG` | `VALTG` | `VBAP` | `String(2)` |  | Addit. Value Days |  |  |  |
| `ProductSeasonYear` | `FSH_SAISJ` | `FSH_SAISJ` | `VBAP` | `String(4)` |  | Season Year |  |  |  |
| `ProductSeason` | `FSH_SAISO` | `FSH_SAISO` | `VBAP` | `String(10)` |  | Season |  |  |  |
| `ProductCollection` | `FSH_COLLECTION` | `FSH_COLLECTION` | `VBAP` | `String(10)` |  | Collection |  |  |  |
| `ProductTheme` | `FSH_THEME` | `FSH_THEME` | `VBAP` | `String(10)` |  | Theme |  |  |  |
| `FashionCancelDate` | `FSH_CANDATE` | `FSH_CANDATE` | `VBAP` | `Date` |  | Cancellation Date |  |  |  |
| `ProductCharacteristic1` | `WRF_CHARSTC1` | `WRF_CHARSTC1` | `VBAP` | `String(18)` |  | Characteristic 1 |  |  |  |
| `ProductCharacteristic2` | `WRF_CHARSTC2` | `WRF_CHARSTC2` | `VBAP` | `String(18)` |  | Characteristic 2 |  |  |  |
| `ProductCharacteristic3` | `WRF_CHARSTC3` | `WRF_CHARSTC3` | `VBAP` | `String(18)` |  | Characteristic 3 |  |  |  |
| `ShippingGroupNumber` | `RFM_PSST_GROUP_ID` | `RFM_PSST_GROUP_ID` | `VBAP` | `String(10)` |  | PSST Group |  |  |  |
| `ShippingGroupRule` | `RFM_PSST_RULE` | `RFM_PSST_RULE` | `VBAP` | `String(4)` |  | PSST Grouping Rule |  |  |  |
| `BillingDocumentDate` | `FKDAT` | `FKDAT` | `VBAP` | `Date` |  | Billing Date |  |  |  |
| `ItemIsBillingRelevant` | `FKREL` | `FKREL` | `VBAP` | `String(1)` |  | Relevant for Billing |  |  |  |
| `ItemBillingBlockReason` | `FAKSP_AP` | `FAKSP_AP` | `VBAP` | `String(2)` |  | Billing Block |  |  |  |
| `BillingPlan` | `FPLNR` | `FPLNR` | `VBAP` | `String(10)` |  | Bill. Plan No. |  |  |  |
| `FiscalYear` | `GJAHR` | `GJAHR` | `VBAP` | `String(4)` |  | Fiscal Year |  |  |  |
| `FiscalPeriod` | `POPER` | `POPER` | `VBAP` | `String(3)` |  | Posting Period |  |  | ECC: unpadded '3' (MONAT); S/4: zero-padded '003' |
| `CustomerAccountAssignmentGroup` | `KTGRD` | `KTGRD` | `VBAP` | `String(2)` |  | Acct Assmt Grp Cust. |  |  |  |
| `BusinessArea` | `GSBER` | `GSBER` | `VBAP` | `String(4)` |  | Business Area |  |  |  |
| `ControllingArea` | `KOKRS` | `KOKRS` | `VBAP` | `String(4)` |  | Controlling Area |  |  |  |
| `ProfitCenter` | `PRCTR` | `PRCTR` | `VBAP` | `String(10)` |  | Profit Center |  |  |  |
| `WBSElement` | `PS_PSP_PNR` | `PS_PSP_PNR` | `VBAP` | `String(8)` |  | WBS Element |  |  |  |
| `WBSElementInternalID` | `PS_S4_PSPNR` | `PS_S4_PSPNR` | `VBAP` | `String(8)` |  | WBS Internal ID |  |  |  |
| `OrderID` | `AUFNR` | `AUFNR` | `VBAP` | `String(12)` |  | Order |  |  |  |
| `ControllingObject` | `OBJPO` | `OBJPO` | `VBAP` | `String(22)` |  | Object No.Item |  |  |  |
| `ProfitabilitySegment` | `RKEOBJNR_NUMC` | `RKEOBJNR_NUMC` | `VBAP` | `String(10)` |  | Profitability Segment (Deprecated) |  |  |  |
| `ProfitabilitySegment_2` | `RKEOBJNR_CHAR` | `RKEOBJNR_CHAR` | `VBAP` | `String(10)` |  | Profitability Segment |  |  |  |
| `OriginSDDocument` | `VBELV` | `VBELV` | `VBAP` | `String(10)` |  | Originating Document |  |  |  |
| `OriginSDDocumentItem` | `POSNV` | `POSNV` | `VBAP` | `String(6)` |  | Originating Item |  |  |  |
| `AccountingExchangeRate` | `KURRF` | `KURRF` | `VBAP` | `Decimal(9,5)` |  | Exchng. Rate Accntg. |  |  |  |
| `ContractAccount` | `CORR_VKONT_KK` | `CORR_VKONT_KK` | `VBAP` | `String(12)` |  | Contract Account |  |  |  |
| `ReferenceSDDocument` | `VGBEL` | `VGBEL` | `VBAP` | `String(10)` |  | Reference Document |  |  |  |
| `ReferenceSDDocumentItem` | `VGPOS` | `VGPOS` | `VBAP` | `String(6)` |  | Reference Item |  |  |  |
| `ReferenceSDDocumentCategory` | `REFERENCE_SD_DOCUMENT_CATEGORY` | `REFERENCE_SD_DOCUMENT_CATEGORY` | `VBAP` | `String(4)` |  | Reference Document Category |  |  |  |
| `HigherLevelItem` | `UEPOS` | `UEPOS` | `VBAP` | `String(6)` |  | Higher-Level Item |  |  |  |
| `HigherLevelItemUsage` | `UEPVW` | `UEPVW` | `VBAP` | `String(1)` |  | Usage of HL Item |  |  |  |
| `BusinessSolutionOrder` | `CRMS4_SOLO_OBJECT_ID` | `CRMS4_SOLO_OBJECT_ID` | `VBAP` | `String(10)` |  | Solution Order |  |  |  |
| `BusinessSolutionOrderItem` | `CRMS4_SOLO_NUMBER_INT` | `CRMS4_SOLO_NUMBER_INT` | `VBAP` | `String(6)` |  | Solution Order Item |  |  |  |
| `BusSolnOrdItemBundleItem` | `CRMS4_BUNDLE_ITEM_NUMBER` | `CRMS4_BUNDLE_ITEM_NUMBER` | `VBAP` | `String(6)` |  | Bundle Item No. |  |  |  |
| `SDProcessStatus` | `GBSTA` | `GBSTA` | `VBAP` | `String(1)` |  | Overall Status |  |  |  |
| `DeliveryConfirmationStatus` | `BESTA` | `BESTA` | `VBAP` | `String(1)` |  | Delivery Conf. Sts |  |  |  |
| `PurchaseConfirmationStatus` | `COSTA_D` | `COSTA` | `VBAP` | `String(1)` |  | Purchasing Conf. Sts |  |  |  |
| `TotalDeliveryStatus` | `LFGSA` | `LFGSA` | `VBAP` | `String(1)` |  | Ovrl Delivery Status |  |  |  |
| `DeliveryStatus` | `LFSTA` | `LFSTA` | `VBAP` | `String(1)` |  | Delivery Status |  |  |  |
| `DeliveryBlockStatus` | `DELIVERY_BLOCK_STATUS` | `DELIVERY_BLOCK_STATUS` | `VBAP` | `String(1)` |  | Delivery Block Status |  |  |  |
| `OrderRelatedBillingStatus` | `SLS_DOC_ORDER_REL_BILLING_STS` | `SLS_DOC_ORDER_REL_BILLING_STS` | `VBAP` | `String(1)` |  | Order-Related Billing Status |  |  |  |
| `BillingBlockStatus` | `FSSTA` | `FSSTA` | `VBAP` | `String(1)` |  | Billing Block Status |  |  |  |
| `ItemGeneralIncompletionStatus` | `ITEM_GENERAL_INCOMPLETION_STS` | `ITEM_GENERAL_INCOMPLETION_STS` | `VBAP` | `String(1)` |  | Incompletion Status |  |  |  |
| `ItemBillingIncompletionStatus` | `UVFAK_UP` | `UVFAK_UP` | `VBAP` | `String(1)` |  | Billing – Item |  |  |  |
| `PricingIncompletionStatus` | `UVPRS_UP` | `UVPRS_UP` | `VBAP` | `String(1)` |  | Pricing – Item |  |  |  |
| `ItemDeliveryIncompletionStatus` | `UVVLK_UP` | `UVVLK_UP` | `VBAP` | `String(1)` |  | Delivery – Item |  |  |  |
| `SDDocReferenceStatus` | `RFSTA` | `RFSTA` | `VBAP` | `String(1)` |  | Reference Status |  |  |  |
| `SDDocumentRejectionStatus` | `ABSTA_VB` | `ABSTA_VB` | `VBAP` | `String(1)` |  | Rejection Status |  |  |  |
| `TotalSDDocReferenceStatus` | `RFGSA` | `RFGSA` | `VBAP` | `String(1)` |  | Ovrl Reference Sts |  |  |  |
| `ChmlCmplncStatus` | `MON_TDD_PCSTA` | `MON_TDD_PCSTA` | `VBAP` | `String(1)` |  | Product Marketability Status |  |  |  |
| `DangerousGoodsStatus` | `MON_TDD_DGSTA` | `MON_TDD_DGSTA` | `VBAP` | `String(1)` |  | Dangerous Goods Status |  |  |  |
| `SafetyDataSheetStatus` | `MON_TDD_SDSSTA` | `MON_TDD_SDSSTA` | `VBAP` | `String(1)` |  | Safety Data Sheet Status |  |  |  |
| `SlsOrderItemDownPaymentStatus` | `DP_CLEAR_STA` | `DP_CLEAR_STA` | `VBAP` | `String(1)` |  | Down Payment Status |  |  |  |
| `TrdCmplncEmbargoSts` | `EMBARGOCHKSTS` | `EMBARGOCHKSTS` | `VBAP` | `String(1)` |  | Embargo Status |  |  |  |
| `TrdCmplncSnctndListChkSts` | `WATCHLISTSCRNGCHKSTS` | `WATCHLISTSCRNGCHKSTS` | `VBAP` | `String(1)` |  | Screening Status |  |  |  |
| `OvrlTrdCmplncLegalCtrlChkSts` | `LGLCTRLCHKSTS` | `LGLCTRLCHKSTS` | `VBAP` | `String(1)` |  | Legal Control Status |  |  |  |
| `AltvBsdConfSubstitutionStatus` | `ATP_ABC_SUBSTITUTION_STATUS` | `ATP_ABC_SUBSTITUTION_STATUS` | `VBAP` | `String(1)` |  | Substitution Status |  |  |  |
| `OmniChannelSalesPromotion` | `TDD_BOB_PROMOTION_ID` | `TDD_BOB_PROMOTION_ID` | `VBAP` | `Integer64` |  | OmniChnl PromoID |  |  |  |
| `OmniChannelSalesPromotionRule` | `TDD_BOB_FG_ID` | `TDD_BOB_FG_ID` | `VBAP` | `Integer64` |  | FGID OmniChnl |  |  |  |
| `ConsumptionPosting` | `KZVBR` | `KZVBR` | `VBAP` | `String(1)` |  | Consumption |  |  |  |
| `CappedNetAmount` | `CAPPED_NET_AMOUNT` | `CAPPED_NET_AMOUNT` | `VBAP` | `Decimal(34,4)` |  | Net Amount Cap | TransactionCurrency |  |  |
| `CappedNetAmtAlertThldInPct` | `CAPPED_NET_AMOUNT_ALERT_THLD` | `CAPPED_NET_AMOUNT_ALERT_THLD` | `VBAP` | `String(3)` |  | Cap Notif. Threshold |  |  |  |
| `TotalStandAloneSellingPrice` | `IFRS15_TOTAL_SSP` | `IFRS15_TOTAL_SSP` | `VBAP` | `Decimal(34,4)` |  | SSP | TransactionCurrency |  |  |
| `SalesOrderType` | `SALES_ORDER_TYPE` | `SALES_ORDER_TYPE` | `VBAP` | `String(4)` |  | Sales Order Type |  |  |  |
| `SalesOrganization` | `VKORG` | `VKORG` | `VBAP` | `String(4)` |  | Sales Organization |  |  |  |
| `DistributionChannel` | `VTWEG` | `VTWEG` | `VBAP` | `String(2)` |  | Distribution Channel |  |  |  |
| `OrganizationDivision` | `SPART` | `SPART` | `VBAP` | `String(2)` |  | Division |  |  |  |
| `SalesOffice` | `VKBUR` | `VKBUR` | `VBAP` | `String(4)` |  | Sales Office |  |  |  |
| `SalesGroup` | `VKGRP` | `VKGRP` | `VBAP` | `String(3)` |  | Sales Group |  |  |  |
| `SoldToParty` | `KUNAG` | `KUNAG` | `VBAP` | `String(10)` |  | Sold-to Party |  |  |  |
| `AdditionalCustomerGroup1` | `KVGR1` | `KVGR1` | `VBAP` | `String(3)` |  | Customer Group 1 |  |  |  |
| `AdditionalCustomerGroup2` | `KVGR2` | `KVGR2` | `VBAP` | `String(3)` |  | Customer Group 2 |  |  |  |
| `AdditionalCustomerGroup3` | `KVGR3` | `KVGR3` | `VBAP` | `String(3)` |  | Customer Group 3 |  |  |  |
| `AdditionalCustomerGroup4` | `KVGR4` | `KVGR4` | `VBAP` | `String(3)` |  | Customer Group 4 |  |  |  |
| `AdditionalCustomerGroup5` | `KVGR5` | `KVGR5` | `VBAP` | `String(3)` |  | Customer Group 5 |  |  |  |
| `SalesOrderDate` | `AUDAT` | `AUDAT` | `VBAP` | `Date` |  | Document Date |  |  |  |
| `SDDocumentReason` | `AUGRU` | `AUGRU` | `VBAP` | `String(3)` |  | Order Reason |  |  |  |
| `RequestedDeliveryDate` | `REQD_DELIVERY_DATE` | `REQD_DELIVERY_DATE` | `VBAP` | `Date` |  | Requested Delivery Date |  |  |  |
| `ShippingCondition` | `VSBED` | `VSBED` | `VBAP` | `String(2)` |  | Shipping Conditions |  |  |  |
| `ShipToParty` | `KUNWE` | `KUNWE` | `VBAP` | `String(10)` |  | Ship-to Party |  |  |  |
| `PayerParty` | `KUNRG` | `KUNRG` | `VBAP` | `String(10)` |  | Payer |  |  |  |
| `BillToParty` | `KUNRE` | `KUNRE` | `VBAP` | `String(10)` |  | Bill-to Party |  |  |  |
| `SalesEmployee` | `SALES_EMPL` | `SALES_EMPL` | `VBAP` | `String(8)` |  | Sales Employee |  |  |  |
| `ResponsibleEmployee` | `RESP_EMPL` | `RESP_EMPL` | `VBAP` | `String(8)` |  | Employee Responsible |  |  |  |
| `SalesEmployeeWorkAgreement` | `SALES_EMPL` | `SALES_EMPL` | `VBAP` | `String(8)` |  | Sales Employee |  |  |  |
| `ResponsibleEmployeeWorkAgrmt` | `RESP_EMPL` | `RESP_EMPL` | `VBAP` | `String(8)` |  | Employee Responsible |  |  |  |
| `SeasonCompletenessStatus` | `RFM_SCC_INDICATOR` | `RFM_SCC_INDICATOR` | `VBAP` | `String(1)` |  | Season Comp.Ind |  |  |  |
| `CustomerConditionGroup1` | `KDKG1` | `KDKG1` | `VBAP` | `String(2)` |  | Condition Group 1 |  |  |  |
| `CustomerConditionGroup2` | `KDKG2` | `KDKG2` | `VBAP` | `String(2)` |  | Condition Group 2 |  |  |  |
| `CustomerConditionGroup3` | `KDKG3` | `KDKG3` | `VBAP` | `String(2)` |  | Condition Group 3 |  |  |  |
| `CustomerConditionGroup4` | `KDKG4` | `KDKG4` | `VBAP` | `String(2)` |  | Condition Group 4 |  |  |  |
| `CustomerConditionGroup5` | `KDKG5` | `KDKG5` | `VBAP` | `String(2)` |  | Condition Group 5 |  |  |  |
| `POCorrespncExternalReference` | `SLS_PURG_DOC_EXT_REF` | `SLS_PURG_DOC_EXT_REF` | `VBAP` | `String(12)` |  | Pur. Order Ext. Ref. |  |  |  |
