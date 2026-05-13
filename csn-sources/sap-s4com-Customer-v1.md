# Customer

> Source file: `sap-s4com-Customer-v1.json`

**Technical Name:** `` | **Data Category:** `DIMENSION` | **VDM Type:** `BASIC` | **Size:** `XL`


## Entity: `Customer`

- **ABAP CDS Name:** `I_Customer`
- **Label:** Customer
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** ADRC, KNA1

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Customer` | `KUNNR` | `KNA1` | `KUNNR` |  |  | `String(10)` | Y | Customer |  |  |
| `CustomerName` | `MD_CUSTOMER_NAME` |  |  |  |  | `String(80)` |  | Name of Customer |  |  |
| `CustomerFullName` | `MD_CUSTOMER_FULL_NAME` | `KNA1` | `NAME1` |  |  | `String(220)` |  | Customer Name |  |  |
| `BPCustomerName` | `CUSTOMERNAME_2` |  |  |  |  | `String(81)` |  | Business Partner - Customer Name |  |  |
| `BPCustomerFullName` | `MD_CUSTOMER_FULL_NAME` |  |  |  |  | `String(220)` |  | Business Partner - Customer Full Name |  |  |
| `CreatedByUser` | `ERNAM_RF` |  |  |  |  | `String(12)` |  | Created by |  |  |
| `CreationDate` | `ERDAT_RF` |  |  |  |  | `Date` |  | Created On |  |  |
| `AddressID` | `ADRNR` | `ADRC` | `ADDRNUMBER` |  |  | `String(10)` |  | Address |  |  |
| `CustomerClassification` | `KUKLA` |  |  |  |  | `String(2)` |  | Customer Classific. |  |  |
| `VATRegistration` | `STCEG` |  |  |  |  | `String(20)` |  | VAT Registration No. |  |  |
| `CustomerAccountGroup` | `KTOKD` | `KNA1` | `KTOKD` |  |  | `String(4)` |  | Account Group |  |  |
| `AuthorizationGroup` | `BRGRU` |  |  |  |  | `String(4)` |  | Authorization |  |  |
| `DeliveryIsBlocked` | `LIFSD_X` |  |  |  |  | `String(2)` |  | Delivery block |  |  |
| `PostingIsBlocked` | `SPERB_X` |  |  |  |  | `Boolean` |  | Posting Block |  |  |
| `BillingIsBlockedForCustomer` | `FAKSD_X` |  |  |  |  | `String(2)` |  | Billing Block |  |  |
| `OrderIsBlockedForCustomer` | `AUFSD_X` |  |  |  |  | `String(2)` |  | Order Block |  |  |
| `InternationalLocationNumber1` | `BBBNR` |  |  |  |  | `String(7)` |  | Int. location no. 1 |  |  |
| `IsOneTimeAccount` | `XCPDK` |  |  |  |  | `Boolean` |  | One-Time Account |  |  |
| `TaxJurisdiction` | `TXJCD` |  |  |  |  | `String(15)` |  | Tax Jurisdiction |  |  |
| `Industry` | `BRSCH` |  |  |  |  | `String(4)` |  | Industry |  |  |
| `TaxNumberType` | `J_1ATOID` |  |  |  |  | `String(2)` |  | Tax Number Type |  |  |
| `TaxNumber1` | `STCD1` | `KNA1` | `STCD1` |  |  | `String(16)` |  | Tax Number 1 |  |  |
| `TaxNumber2` | `STCD2` | `KNA1` | `STCD2` |  |  | `String(11)` |  | Tax Number 2 |  |  |
| `TaxNumber3` | `STCD3` |  |  |  |  | `String(18)` |  | Tax Number 3 |  |  |
| `TaxNumber4` | `STCD4` |  |  |  |  | `String(18)` |  | Tax Number 4 |  |  |
| `TaxNumber5` | `STCD5` |  |  |  |  | `String(60)` |  | Tax Number 5 |  |  |
| `TaxNumber6` | `STCD6` |  |  |  |  | `String(20)` |  | Tax Number 6 |  |  |
| `CustomerCorporateGroup` | `KONZS` |  |  |  |  | `String(10)` |  | Group Key |  |  |
| `Supplier` | `LIFNR` |  |  |  |  | `String(10)` |  | Supplier |  |  |
| `NielsenRegion` | `NIELS` |  |  |  |  | `String(2)` |  | Nielsen Indicator |  |  |
| `IndustryCode1` | `BRAN1_D` | `KNA1` | `BRSCH` |  |  | `String(10)` |  | Industry Code 1 |  |  |
| `IndustryCode2` | `BRAN2` |  |  |  |  | `String(10)` |  | Industry Code 2 |  |  |
| `IndustryCode3` | `BRAN3` |  |  |  |  | `String(10)` |  | Industry Code 3 |  |  |
| `IndustryCode4` | `BRAN4` |  |  |  |  | `String(10)` |  | Industry Code 4 |  |  |
| `IndustryCode5` | `BRAN5` |  |  |  |  | `String(10)` |  | Industry Code 5 |  |  |
| `Country` | `LAND1_GP` | `KNA1` | `LAND1` |  |  | `String(3)` |  | Country/Region Key |  |  |
| `OrganizationBPName1` | `NAME1_GP` |  |  |  |  | `String(35)` |  | Name |  |  |
| `OrganizationBPName2` | `NAME2_GP` |  |  |  |  | `String(35)` |  | Name 2 |  |  |
| `CityName` | `ORT01_GP` | `KNA1` | `ORT01` |  |  | `String(35)` |  | City |  |  |
| `PostalCode` | `PSTLZ` | `KNA1` | `PSTLZ` |  |  | `String(10)` |  | Postal Code |  |  |
| `StreetName` | `STRAS_GP` | `KNA1` | `STRAS` |  |  | `String(35)` |  | Street |  |  |
| `SortField` | `SORTL` |  |  |  |  | `String(10)` |  | Search Term |  |  |
| `FaxNumber` | `TELFX` |  |  |  |  | `String(31)` |  | Fax Number |  |  |
| `BR_SUFRAMACode` | `J_1BSUFRAMA` |  |  |  |  | `String(9)` |  | Suframa Code |  |  |
| `Region` | `REGIO` | `KNA1` | `REGIO` |  |  | `String(3)` |  | Region |  |  |
| `TelephoneNumber1` | `TELF1` |  |  |  |  | `String(16)` |  | Telephone 1 |  |  |
| `TelephoneNumber2` | `TELF2` |  |  |  |  | `String(16)` |  | Telephone 2 |  |  |
| `AlternativePayerAccount` | `KNRZA` |  |  |  |  | `String(10)` |  | Alternative Payer |  |  |
| `DataMediumExchangeIndicator` | `DTAMS` |  |  |  |  | `String(1)` |  | DME Recipient Code |  |  |
| `VATLiability` | `STKZU` |  |  |  |  | `Boolean` |  | Liable for VAT |  |  |
| `IsBusinessPurposeCompleted` |  |  |  |  |  | `Boolean` |  | Purpose Completed |  |  |
| `ResponsibleType` | `J_1AFITP_D` |  |  |  |  | `String(2)` |  | Tax Type |  |  |
| `FiscalAddress` | `FISKN_D` |  |  |  |  | `String(10)` |  | Fiscal address |  |  |
| `NFPartnerIsNaturalPerson` |  |  |  |  |  | `Boolean` |  | Natural Person |  |  |
| `DeletionIndicator` | `LOEVM_X` |  |  |  |  | `Boolean` |  | Deletion Flag |  |  |
| `Language` | `SPRAS` | `KNA1` | `SPRAS` |  |  | `String(2)` |  | Language Key |  |  |
| `TradingPartner` | `RASSC` |  |  |  |  | `String(6)` |  | Trading Partner No. |  |  |
| `DeliveryDateTypeRule` | `SD_DELIVERY_DATE_TYPE_RULE` |  |  |  |  | `String(1)` |  | Deliv Date Rule |  |  |
| `ExpressTrainStationName` | `BAHNE` |  |  |  |  | `String(25)` |  | Express station |  |  |
| `TrainStationName` | `BAHNS` |  |  |  |  | `String(25)` |  | Train station |  |  |
| `InternationalLocationNumber2` | `BBSNR` |  |  |  |  | `String(5)` |  | Int. location no. 2 |  |  |
| `InternationalLocationNumber3` | `BUBKZ` |  |  |  |  | `String(1)` |  | Check digit |  |  |
| `CityCode` | `CITYC` |  |  |  |  | `String(4)` |  | City Code |  |  |
| `County` | `COUNC` |  |  |  |  | `String(3)` |  | County Code |  |  |
| `CustomerHasUnloadingPoint` | `EXABL` |  |  |  |  | `Boolean` |  | Unloading points |  |  |
| `CustomerWorkingTimeCalendar` | `KNAZK` |  |  |  |  | `String(2)` |  | Working times |  |  |
| `IsCompetitor` | `DEAR1` |  |  |  |  | `Boolean` |  | Competitors |  |  |
| `TaxInvoiceRepresentativeName` | `REPRES` |  |  |  |  | `String(10)` |  | Rep's Name |  |  |
| `BusinessType` | `GESTYP` |  |  |  |  | `String(30)` |  | Type of Business |  |  |
| `IndustryType` | `INDTYP` |  |  |  |  | `String(30)` |  | Type of Industry |  |  |
| `TW_CollvBillingIsSupported` |  |  |  |  |  | `Boolean` |  | Consolidated Invoic. |  |  |
| `AlternativePayeeIsAllowed` | `XREGU` |  |  |  |  | `Boolean` |  | Alt.payer in doc? |  |  |
| `FreeDefinedAttribute01` | `KATR1` |  |  |  |  | `String(2)` |  | Attribute 1 |  |  |
| `FreeDefinedAttribute02` | `KATR2` |  |  |  |  | `String(2)` |  | Attribute 2 |  |  |
| `FreeDefinedAttribute03` | `KATR3` |  |  |  |  | `String(2)` |  | Attribute 3 |  |  |
| `FreeDefinedAttribute04` | `KATR4` |  |  |  |  | `String(2)` |  | Attribute 4 |  |  |
| `FreeDefinedAttribute05` | `KATR5` |  |  |  |  | `String(2)` |  | Attribute 5 |  |  |
| `FreeDefinedAttribute06` | `KATR6` |  |  |  |  | `String(3)` |  | Attribute 6 |  |  |
| `FreeDefinedAttribute07` | `KATR7` |  |  |  |  | `String(3)` |  | Attribute 7 |  |  |
| `FreeDefinedAttribute08` | `KATR8` |  |  |  |  | `String(3)` |  | Attribute 8 |  |  |
| `FreeDefinedAttribute09` | `KATR9` |  |  |  |  | `String(3)` |  | Attribute 9 |  |  |
| `FreeDefinedAttribute10` | `KATR10` |  |  |  |  | `String(3)` |  | Attribute 10 |  |  |
| `PaymentReason` | `FARP_PAYT_RSN` |  |  |  |  | `String(4)` |  | Payment Reason |  |  |
| `CustomerConditionGroup1` | `KDKG1` |  |  |  |  | `String(2)` |  | Condition Group 1 |  |  |
| `CustomerConditionGroup2` | `KDKG2` |  |  |  |  | `String(2)` |  | Condition Group 2 |  |  |
| `CustomerConditionGroup3` | `KDKG3` |  |  |  |  | `String(2)` |  | Condition Group 3 |  |  |
| `CustomerConditionGroup4` | `KDKG4` |  |  |  |  | `String(2)` |  | Condition Group 4 |  |  |
| `CustomerConditionGroup5` | `KDKG5` |  |  |  |  | `String(2)` |  | Condition Group 5 |  |  |
| `IsSalesProspect` |  |  |  |  |  | `Boolean` |  | Prospect |  |  |
| `PaymentIsBlockedForCustomer` | `SPERZ` |  |  |  |  | `Boolean` |  | Payment block |  |  |
| `IsConsumer` | `DEAR6` |  |  |  |  | `Boolean` |  | Consumer |  |  |
| `DataControllerSet` | `BU_XDCSET` |  |  |  |  | `String(1)` |  | Data Ctrlr. Set |  |  |
| `DataController1` | `BU_DATA_CONTROLLER` |  |  |  |  | `String(30)` |  | Data Controller |  |  |
| `DataController2` | `BU_DATA_CONTROLLER` |  |  |  |  | `String(30)` |  | Data Controller |  |  |
| `DataController3` | `BU_DATA_CONTROLLER` |  |  |  |  | `String(30)` |  | Data Controller |  |  |
| `DataController4` | `BU_DATA_CONTROLLER` |  |  |  |  | `String(30)` |  | Data Controller |  |  |
| `DataController5` | `BU_DATA_CONTROLLER` |  |  |  |  | `String(30)` |  | Data Controller |  |  |
| `DataController6` | `BU_DATA_CONTROLLER` |  |  |  |  | `String(30)` |  | Data Controller |  |  |
| `DataController7` | `BU_DATA_CONTROLLER` |  |  |  |  | `String(30)` |  | Data Controller |  |  |
| `DataController8` | `BU_DATA_CONTROLLER` |  |  |  |  | `String(30)` |  | Data Controller |  |  |
| `DataController9` | `BU_DATA_CONTROLLER` |  |  |  |  | `String(30)` |  | Data Controller |  |  |
| `DataController10` | `BU_DATA_CONTROLLER` |  |  |  |  | `String(30)` |  | Data Controller |  |  |
| `BusinessPartnerName1` | `AD_NAME1` |  |  |  |  | `String(40)` |  | Business Partner Organization  - Name 1 |  |  |
| `BusinessPartnerName2` | `AD_NAME2` |  |  |  |  | `String(40)` |  | Business Partner Organization  - Name 2 |  |  |
| `BusinessPartnerName3` | `AD_NAME3` |  |  |  |  | `String(40)` |  | Business Partner Organization  - Name 3 |  |  |
| `BusinessPartnerName4` | `AD_NAME4` |  |  |  |  | `String(40)` |  | Business Partner Organization  - Name 4 |  |  |
| `BPAddrCityName` | `AD_CITY1` |  |  |  |  | `String(40)` |  | Business Partner Address – City |  |  |
| `BPAddrStreetName` | `AD_STREET` |  |  |  |  | `String(60)` |  | Business Partner Address – Street |  |  |
| `AddressSearchTerm1` | `AD_SORT1` |  |  |  |  | `String(20)` |  | Business Partner Address - Search Term 1 |  |  |
| `AddressSearchTerm2` | `AD_SORT2` |  |  |  |  | `String(20)` |  | Business Partner Address - Search Term 2 |  |  |
| `DistrictName` | `AD_CITY2` |  |  |  |  | `String(40)` |  | Business Partner Address – District |  |  |
| `POBoxDeviatingCityName` | `AD_POBXLOC` |  |  |  |  | `String(40)` |  | Business Partner Address - PO Box Deviating City |  |  |
| `BusinessPartnerFormOfAddress` | `AD_TITLE` |  |  |  |  | `String(4)` |  | Business Partner - Form of Address |  |  |
| `BR_ICMSTaxPayerType` | `J_1BICMSTAXPAY` |  |  |  |  | `String(2)` |  | ICMS Taxpayer |  |  |


## Entity: `CustomerCompanyCode`

- **ABAP CDS Name:** `I_CustomerCompany`
- **Label:** Customer Company
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** KNB1, KNB5

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Customer` | `KUNNR` | `KNB5` | `KUNNR` |  |  | `String(10)` | Y | Customer |  |  |
| `CompanyCode` | `BUKRS` | `KNB5` | `BUKRS` |  |  | `String(4)` | Y | Company Code |  |  |
| `AccountingClerk` | `BUSAB` |  |  |  |  | `String(2)` |  | Clerk Abbrev. |  |  |
| `ReconciliationAccount` | `AKONT` | `KNB1` | `AKONT` |  |  | `String(10)` |  | Reconciliation Acct |  |  |
| `AuthorizationGroup` | `BRGRU` |  |  |  |  | `String(4)` |  | Authorization |  |  |
| `CustomerHeadOffice` | `KNRZE` |  |  |  |  | `String(10)` |  | Head Office |  |  |
| `AlternativePayerAccount` | `KNRZB` |  |  |  |  | `String(10)` |  | Alternative payer |  |  |
| `PaymentBlockingReason` | `DZAHLS` | `KNB1` | `ZAHLS` |  |  | `String(1)` |  | Payment Block |  |  |
| `InterestCalculationCode` | `VZSKZ` |  |  |  |  | `String(2)` |  | Interest Indicator |  |  |
| `InterestCalculationDate` | `DZINDT` |  |  |  |  | `Date` |  | Last Key Date |  |  |
| `IntrstCalcFrequencyInMonths` | `DZINRT` |  |  |  |  | `String(2)` |  | Int.Calc.Freq. |  |  |
| `CustomerAccountNote` | `KVERM` |  |  |  |  | `String(30)` |  | Account Memo |  |  |
| `APARToleranceGroup` | `TOGRU` |  |  |  |  | `String(4)` |  | Tolerance Group |  |  |
| `HouseBank` | `HBKID` |  |  |  |  | `String(5)` |  | House Bank |  |  |
| `ItemIsToBePaidSeparately` | `XPORE` |  |  |  |  | `Boolean` |  | Individual Payment |  |  |
| `PaytAdviceIsSentbyEDI` | `XEDIP` |  |  |  |  | `Boolean` |  | Pmnt advice by EDI |  |  |
| `PhysicalInventoryBlockInd` | `SPERB_B` |  |  |  |  | `Boolean` |  | Co.code post.block |  |  |
| `UserAtCustomer` | `DZSABE_D` |  |  |  |  | `String(15)` |  | User at customer |  |  |
| `AccountingClerkPhoneNumber` | `TLFNS` |  |  |  |  | `String(30)` |  | Acct.clerks tel.no. |  |  |
| `AccountingClerkFaxNumber` | `TLFXS` |  |  |  |  | `String(31)` |  | Acctg clerk's fax |  |  |
| `AccountingClerkInternetAddress` | `INTAD` |  |  |  |  | `String(130)` |  | Clrk's internet add. |  |  |
| `AccountByCustomer` | `EIKTO_D` |  |  |  |  | `String(12)` |  | Account at Customer |  |  |
| `IsToBeLocallyProcessed` | `XDEZV` |  |  |  |  | `Boolean` |  | Local Processing |  |  |
| `CollectiveInvoiceVariant` | `PERKZ_KNB1` |  |  |  |  | `String(1)` |  | Coll.Invoice Variant |  |  |
| `LayoutSortingRule` | `DZUAWA` |  |  |  |  | `String(3)` |  | Sort key |  |  |
| `PaymentTerms` | `DZTERM` | `KNB1` | `ZTERM` |  |  | `String(4)` |  | Terms of Payment |  |  |
| `CustomerSupplierClearingIsUsed` | `XVERR_KNB1` |  |  |  |  | `Boolean` |  | Clearing with vendor |  |  |
| `RecordPaymentHistoryIndicator` | `XZVER` |  |  |  |  | `Boolean` |  | Record Pmnt History |  |  |
| `PaymentMethodsList` | `DZWELS` |  |  |  |  | `String(10)` |  | Payment Methods |  |  |
| `DeletionIndicator` | `LOEVM_B` |  |  |  |  | `Boolean` |  | Co.Cde Deletion Flag |  |  |
| `CreditMemoPaymentTerms` | `GUZTE` |  |  |  |  | `String(4)` |  | Credit Memo Pyt Term |  |  |
| `DunningNoticeGroup` | `MGRUP` |  |  |  |  | `String(2)` |  | Grouping Key |  |  |
| `LastInterestCalcRunDate` | `DATLZ` |  |  |  |  | `Date` |  | Last Int. Calc. |  |  |
| `CustPreviousMasterRecordNumber` | `ALTKN` |  |  |  |  | `String(10)` |  | Previous Account No. |  |  |
| `ValueAdjustmentKey` | `WBRSL` |  |  |  |  | `String(2)` |  | Value Adjustment |  |  |
| `CashPlanningGroup` | `FDGRV` |  |  |  |  | `String(10)` |  | Planning Group |  |  |
| `SupplierReleaseGroup` | `FRGRP` |  |  |  |  | `String(4)` |  | Release Group |  |  |
| `PersonnelNumber` | `PERNR_D` |  |  |  |  | `String(8)` |  | Personnel Number |  |  |
| `BuyingGroupAccountNumber` | `EKVBD` |  |  |  |  | `String(10)` |  | Buying Group |  |  |
| `BillExchChargePaymentTerms` | `WAKON` |  |  |  |  | `String(4)` |  | B/Ex. Charges Terms |  |  |
| `CheckPaidDurationInDays` | `KULTG` |  |  |  |  | `Decimal(3,0)` |  | Check Cashing Time |  |  |
| `CustomerPaymentBlockingReason` | `DZAHLS` |  |  |  |  | `String(1)` |  | Payment Block |  |  |
| `PaymentMethodSupplement` | `UZAWE` |  |  |  |  | `String(2)` |  | Pmt Meth. Supplement |  |  |
| `AcctsReceivablePledgingCode` | `CESSION_KZ` |  |  |  |  | `String(2)` |  | AR Pledging Ind. |  |  |
| `LockboxInternalID` | `LOCKB` |  |  |  |  | `String(7)` |  | Lockbox |  |  |
| `IsBusinessPurposeCompleted` |  |  |  |  |  | `Boolean` |  | Purpose Completed |  |  |
| `WithholdingTaxCountry` | `QLAND` |  |  |  |  | `String(3)` |  | WTax C/R Key |  |  |
| `KnownOrNegotiatedLeave` | `URLID` |  |  |  |  | `String(4)` |  | Known/Negotiat.Leave |  |  |
| `DeletionIsBlocked` | `NODEL_B` |  |  |  |  | `Boolean` |  | CoCd Deletion Block |  |  |
| `PaymentClearingGroup` | `FAR_PAYMENT_CLEARING_GROUP` |  |  |  |  | `String(8)` |  | Payment Clrg Grp ID |  |  |
| `PaymentReason` | `FARP_PAYT_RSN` |  |  |  |  | `String(4)` |  | Payment Reason |  |  |
| `BPPeriodicAccountStatement` | `XAUSZ` |  |  |  |  | `String(1)` |  | Account Statement |  |  |
| `US_FrgnAcctTaxRcpntCntry` | `LAND1` |  |  |  |  | `String(3)` |  | Country/Region Key |  |  |
| `US_GlobIntermediaryIdnNumber` | `FIWTUS_RECIPIENT_GIIN` |  |  |  |  | `String(19)` |  | US Recipient GIIN |  |  |
| `US_RecipientForeignTaxID` | `FIWTUS_RECIPIENT_FTID` |  |  |  |  | `String(22)` |  | US Recipient FTID |  |  |
| `US_LobTreatyCode` | `FIWTUS_LOB_CODE` |  |  |  |  | `String(2)` |  | LOB Treaty Code |  |  |
| `US_FW8BENReceiveDate` | `FIWTUS_W8_RECV_DATE` |  |  |  |  | `Date` |  | W8 Form Rec Date |  |  |
| `US_FW9ReceiveDate` | `FIWTUS_W9_RECV_DATE` |  |  |  |  | `Date` |  | W9 Form Rec Date |  |  |
| `US_SecondTINNoticeIsIssued` | `FIWTUS_SECOND_TIN_NOTICE` |  |  |  |  | `String(1)` |  | Second TIN Notice |  |  |
| `US_FrgnRecipientHasPartnership` | `FIWTUS_PARTNERSHIP_IND` |  |  |  |  | `String(1)` |  | Partnership Int Ind |  |  |
| `US_FrgnAcctTaxFilingIsRequired` | `FIWTUS_FATCA_IND` |  |  |  |  | `String(1)` |  | FATCA Ind |  |  |
| `US_Chapter4StatusCode` | `FIWTUS_CHAP4_STATUS_CODE` |  |  |  |  | `String(2)` |  | Chaptr 4 Status Code |  |  |
| `LastDunnedOn` | `MADAT` |  |  |  |  | `Date` |  | Last Dunned |  |  |
| `DunningProcedure` | `MAHNA` |  |  |  |  | `String(4)` |  | Dunning Procedure |  |  |
| `DunningLevel` | `MAHNS_D` |  |  |  |  | `String(1)` |  | Dunning Level |  |  |
| `DunningBlock` | `MANSP` |  |  |  |  | `String(1)` |  | Dunning Block |  |  |
| `DunningRecipient` | `KNRMA` |  |  |  |  | `String(10)` |  | Dunning Recipient |  |  |
| `LegDunningProcedureOn` | `GMVDT` |  |  |  |  | `Date` |  | Legal Dunn.Proc.From |  |  |
| `IsActiveEntity` | `SDRAFT_IS_ACTIVE` |  |  |  |  | `Boolean` |  | Is active |  |  |


## Entity: `CustomerDunning`

- **ABAP CDS Name:** `I_CustomerDunning`
- **Label:** Customer Company Code Dunning Fields
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `CompanyCode` | `BUKRS` |  |  |  |  | `String(4)` | Y | Company Code |  | S/4 only entity |
| `Customer` | `KUNNR` |  |  |  |  | `String(10)` | Y | Customer |  | S/4 only entity |
| `DunningArea` | `MABER` |  |  |  |  | `String(2)` | Y | Dunning Area |  | S/4 only entity |
| `LastDunnedOn` | `MADAT` |  |  |  |  | `Date` |  | Last Dunned |  | S/4 only entity |
| `DunningProcedure` | `MAHNA` |  |  |  |  | `String(4)` |  | Dunning Procedure |  | S/4 only entity |
| `DunningLevel` | `MAHNS_D` |  |  |  |  | `String(1)` |  | Dunning Level |  | S/4 only entity |
| `DunningBlock` | `MANSP` |  |  |  |  | `String(1)` |  | Dunning Block |  | S/4 only entity |
| `DunningRecipient` | `KNRMA` |  |  |  |  | `String(10)` |  | Dunning Recipient |  | S/4 only entity |
| `LegDunningProcedureOn` | `GMVDT` |  |  |  |  | `Date` |  | Legal Dunn.Proc.From |  | S/4 only entity |
| `DunningClerk` | `BUSAB_MA` |  |  |  |  | `String(2)` |  | Dunning Clerk |  | S/4 only entity |


## Entity: `CustomerSalesArea`

- **ABAP CDS Name:** `I_CustomerSalesArea`
- **Label:** Customer Sales Area
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Customer` | `KUNNR` |  |  |  |  | `String(10)` | Y | Customer |  | S/4 only entity |
| `SalesOrganization` | `VKORG` |  |  |  |  | `String(4)` | Y | Sales Organization |  | S/4 only entity |
| `DistributionChannel` | `VTWEG` |  |  |  |  | `String(2)` | Y | Distribution Channel |  | S/4 only entity |
| `Division` | `SPART` |  |  |  |  | `String(2)` | Y | Division |  | S/4 only entity |
| `CustomerABCClassification` | `KLABC` |  |  |  |  | `String(2)` |  | ABC Classification |  | S/4 only entity |
| `SalesOffice` | `VKBUR` |  |  |  |  | `String(4)` |  | Sales Office |  | S/4 only entity |
| `SalesGroup` | `VKGRP` |  |  |  |  | `String(3)` |  | Sales Group |  | S/4 only entity |
| `OrderIsBlockedForCustomer` | `AUFSD_V` |  |  |  |  | `String(2)` |  | Ord.blk:sls ar. |  | S/4 only entity |
| `Currency` | `WAERS_V02D` |  |  |  |  | `String(5)` |  | Currency |  | S/4 only entity |
| `CustomerPriceGroup` | `KONDA` |  |  |  |  | `String(2)` |  | Customer Price Group |  | S/4 only entity |
| `PriceListType` | `PLTYP` |  |  |  |  | `String(2)` |  | Price List Type |  | S/4 only entity |
| `DeliveryPriority` | `LPRIO` |  |  |  |  | `String(2)` |  | Delivery Priority |  | S/4 only entity |
| `ShippingCondition` | `VSBED` |  |  |  |  | `String(2)` |  | Shipping Conditions |  | S/4 only entity |
| `IncotermsClassification` | `INCO1` |  |  |  |  | `String(3)` |  | Incoterms |  | S/4 only entity |
| `SupplyingPlant` | `DWERK_EXT` |  |  |  |  | `String(4)` |  | Delivering Plant |  | S/4 only entity |
| `CompleteDeliveryIsDefined` | `AUTLF` |  |  |  |  | `Boolean` |  | Complete Delivery |  | S/4 only entity |
| `DeliveryIsBlockedForCustomer` | `LIFSD_V` |  |  |  |  | `String(2)` |  | DelBlckSalesAr. |  | S/4 only entity |
| `BillingIsBlockedForCustomer` | `FAKSD_V` |  |  |  |  | `String(2)` |  | BBlock for SlsA |  | S/4 only entity |
| `CustomerPaymentTerms` | `DZTERM` |  |  |  |  | `String(4)` |  | Terms of Payment |  | S/4 only entity |
| `CustomerAccountAssignmentGroup` | `KTGRD` |  |  |  |  | `String(2)` |  | Acct Assmt Grp Cust. |  | S/4 only entity |
| `AccountByCustomer` | `EIKTO` |  |  |  |  | `String(12)` |  | Account at Customer |  | S/4 only entity |
| `CustomerGroup` | `KDGRP` |  |  |  |  | `String(2)` |  | Customer Group |  | S/4 only entity |
| `CustomerPricingProcedure` | `KALKS` |  |  |  |  | `String(2)` |  | Cust.Pric.Procedure |  | S/4 only entity |
| `OrderCombinationIsAllowed` | `KZAZU_D` |  |  |  |  | `Boolean` |  | Order Combination |  | S/4 only entity |
| `PartialDeliveryIsAllowed` | `KZTLF` |  |  |  |  | `String(1)` |  | Partial Deliv./Item |  | S/4 only entity |
| `InvoiceDate` | `PERFK` |  |  |  |  | `String(2)` |  | Invoicing Dates |  | S/4 only entity |
| `PaymentTerms` | `DZTERM` |  |  |  |  | `String(4)` |  | Terms of Payment |  | S/4 only entity |
| `IncotermsTransferLocation` | `INCO2` |  |  |  |  | `String(28)` |  | Incoterms (Part 2) |  | S/4 only entity |
| `ItemOrderProbabilityInPercent` | `AWAHR` |  |  |  |  | `String(3)` |  | Order Probability |  | S/4 only entity |
| `IncotermsLocation2` | `INCO3_L` |  |  |  |  | `String(70)` |  | Incoterms Location 2 |  | S/4 only entity |
| `RecordCreatedDate` | `ERDAT` |  |  |  |  | `Date` |  | Created On |  | S/4 only entity |
| `AuthorizationGroup` | `BEGRU` |  |  |  |  | `String(4)` |  | Authorization Group |  | S/4 only entity |
| `SalesDistrict` | `BZIRK` |  |  |  |  | `String(6)` |  | Sales District |  | S/4 only entity |
| `IncotermsVersion` | `INCOV` |  |  |  |  | `String(4)` |  | Incoterms Version |  | S/4 only entity |
| `IncotermsLocation1` | `INCO2_L` |  |  |  |  | `String(70)` |  | Incoterms Location 1 |  | S/4 only entity |
| `DeletionIndicator` | `LOEVM_V` |  |  |  |  | `Boolean` |  | Del.ID SlsArea |  | S/4 only entity |
| `IsBusinessPurposeCompleted` |  |  |  |  |  | `Boolean` |  | Purpose Completed |  | S/4 only entity |
| `SalesItemProposal` | `VSORT` |  |  |  |  | `String(10)` |  | Item proposal |  | S/4 only entity |
| `CustProdProposalProcedure` | `PVKSM` |  |  |  |  | `String(2)` |  | PP customer proced. |  | S/4 only entity |
| `ProofOfDeliveryTime` |  |  |  |  |  | `String(6)` |  |  |  | S/4 only entity |
| `ProofOfDeliveryTimeValue` | `CUST_POD` |  |  |  |  | `Decimal(6,2)` |  | POD timeframe |  | S/4 only entity |
| `MaxNmbrOfPartialDelivery` | `ANTLF` |  |  |  |  | `Decimal(1,0)` |  | Max.Part.Deliveries |  | S/4 only entity |
| `UnderdelivTolrtdLmtRatioInPct` | `UNTTO` |  |  |  |  | `Decimal(3,1)` |  | Underdel. Tolerance |  | S/4 only entity |
| `OverdelivTolrtdLmtRatioInPct` | `UEBTO` |  |  |  |  | `Decimal(3,1)` |  | Overdeliv. Tolerance |  | S/4 only entity |
| `IsActiveEntity` | `SDRAFT_IS_ACTIVE` |  |  |  |  | `Boolean` |  | Is active |  | S/4 only entity |
| `AdditionalCustomerGroup1` | `KVGR1` |  |  |  |  | `String(3)` |  | Customer Group 1 |  | S/4 only entity |
| `AdditionalCustomerGroup2` | `KVGR2` |  |  |  |  | `String(3)` |  | Customer Group 2 |  | S/4 only entity |
| `AdditionalCustomerGroup3` | `KVGR3` |  |  |  |  | `String(3)` |  | Customer Group 3 |  | S/4 only entity |
| `AdditionalCustomerGroup4` | `KVGR4` |  |  |  |  | `String(3)` |  | Customer Group 4 |  | S/4 only entity |
| `AdditionalCustomerGroup5` | `KVGR5` |  |  |  |  | `String(3)` |  | Customer Group 5 |  | S/4 only entity |
| `InvoiceListSchedule` | `PERRL` |  |  |  |  | `String(2)` |  | Invoice List Sched. |  | S/4 only entity |
| `ExchangeRateType` | `KURST` |  |  |  |  | `String(4)` |  | Exchange Rate Type |  | S/4 only entity |
| `PaymentGuaranteeProcedure` | `KABSSCH_CM` |  |  |  |  | `String(4)` |  | Paymt guarant. proc. |  | S/4 only entity |
| `SuplrIsRlvtForSettlmtMgmt` | `AGREL` |  |  |  |  | `Boolean` |  | Settlement Mgmt. |  | S/4 only entity |
| `CustIsRlvtForSettlmtMgmt` | `AGREL` |  |  |  |  | `Boolean` |  | Settlement Mgmt. |  | S/4 only entity |
| `ProductUnitGroup` | `MEGRU` |  |  |  |  | `String(4)` |  | Unit of Measure Grp |  | S/4 only entity |
| `SlsDocIsRlvtForProofOfDeliv` | `PODKZ` |  |  |  |  | `Boolean` |  | Relevant for POD |  | S/4 only entity |
| `SlsUnlmtdOvrdelivIsAllwd` | `UEBTK_V` |  |  |  |  | `Boolean` |  | Unlimited Tolerance |  | S/4 only entity |
| `CreditControlArea` | `KKBER` |  |  |  |  | `String(4)` |  | Credit Control Area |  | S/4 only entity |
| `CustomerIsRebateRelevant` | `BOKRE` |  |  |  |  | `Boolean` |  | Rebate |  | S/4 only entity |
| `InspSbstHasNoTimeOrQuantity` | `PRFRE` |  |  |  |  | `Boolean` |  | Price determination |  | S/4 only entity |
| `ManualInvoiceMaintIsRelevant` | `MRNKZ` |  |  |  |  | `Boolean` |  | Man. Invoice Maint. |  | S/4 only entity |
| `IncotermsSupChnLoc1AddlUUID` |  |  |  |  |  | `UUID` |  | Location UUID |  | S/4 only entity |
| `IncotermsSupChnLoc2AddlUUID` |  |  |  |  |  | `UUID` |  | Location UUID |  | S/4 only entity |
| `IncotermsSupChnDvtgLocAddlUUID` |  |  |  |  |  | `UUID` |  | Location UUID |  | S/4 only entity |
| `SalesBlockForCustomer` | `CASSD_V` |  |  |  |  | `String(2)` |  | Sales Block |  | S/4 only entity |
| `CustomerStatisticsGroup` | `STGKU` |  |  |  |  | `String(1)` |  | Customer Stats.Group |  | S/4 only entity |
| `RetailAdditionalCustomerGrp6` | `FSH_KVGR6` |  |  |  |  | `String(3)` |  | Customer Group 6 |  | S/4 only entity |
| `RetailAdditionalCustomerGrp7` | `FSH_KVGR7` |  |  |  |  | `String(3)` |  | Customer Group 7 |  | S/4 only entity |
| `RetailAdditionalCustomerGrp8` | `FSH_KVGR8` |  |  |  |  | `String(3)` |  | Customer Group 8 |  | S/4 only entity |
| `RetailAdditionalCustomerGrp9` | `FSH_KVGR9` |  |  |  |  | `String(3)` |  | Customer Group 9 |  | S/4 only entity |
| `RetailAdditionalCustomerGrp10` | `FSH_KVGR10` |  |  |  |  | `String(3)` |  | Customer Group 10 |  | S/4 only entity |


## Entity: `CustomerSalesAreaTax`

- **ABAP CDS Name:** `I_CustSalesAreaTax`
- **Label:** Customer Sales Area Tax
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Customer` | `KUNNR` |  |  |  |  | `String(10)` | Y | Customer |  | S/4 only entity |
| `SalesOrganization` | `VKORG` |  |  |  |  | `String(4)` | Y | Sales Organization |  | S/4 only entity |
| `DistributionChannel` | `VTWKU` |  |  |  |  | `String(2)` | Y | RefDistCh-Cust/Mat. |  | S/4 only entity |
| `Division` | `SPART` |  |  |  |  | `String(2)` | Y | Division |  | S/4 only entity |
| `DepartureCountry` | `ALAND` |  |  |  |  | `String(3)` | Y | Departure Ctry/Reg. |  | S/4 only entity |
| `CustomerTaxCategory` | `TATYP` |  |  |  |  | `String(4)` | Y | Tax Condition Type |  | S/4 only entity |
| `CustomerTaxClassification` | `TAKLD` |  |  |  |  | `String(1)` |  | Tax Classification |  | S/4 only entity |
| `AuthorizationGroup` | `BRGRU` |  |  |  |  | `String(4)` |  | Authorization |  | S/4 only entity |
| `IsBusinessPurposeCompleted` |  |  |  |  |  | `Boolean` |  | Purpose Completed |  | S/4 only entity |


## Entity: `CustomerUnloadingPoint`

- **ABAP CDS Name:** `I_CustomerUnloadingPoint`
- **Label:** Customer Unloading Point
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Customer` | `KUNNR` |  |  |  |  | `String(10)` | Y | Customer |  | S/4 only entity |
| `UnloadingPointName` | `ABLAD` |  |  |  |  | `String(25)` | Y | Unloading Point |  | S/4 only entity |
| `CustomerFactoryCalenderCode` | `KNKAL` |  |  |  |  | `String(2)` |  | Cust.fact.calendar |  | S/4 only entity |
| `BPGoodsReceivingHoursCode` | `WANID` |  |  |  |  | `String(3)` |  | Goods receiving hrs |  | S/4 only entity |
| `IsDfltBPUnloadingPoint` | `DEFAB` |  |  |  |  | `Boolean` |  | Default unloading pt |  | S/4 only entity |
| `MondayMorningOpeningTime` | `WAMOAB1` |  |  |  |  | `String(6)` |  | Monday |  | S/4 only entity |
| `MondayMorningClosingTime` | `WAMOBI1` |  |  |  |  | `String(6)` |  | Monday |  | S/4 only entity |
| `MondayAfternoonOpeningTime` | `WAMOAB2` |  |  |  |  | `String(6)` |  | Monday |  | S/4 only entity |
| `MondayAfternoonClosingTime` | `WAMOBI2` |  |  |  |  | `String(6)` |  | Monday |  | S/4 only entity |
| `TuesdayMorningOpeningTime` | `WADIAB1` |  |  |  |  | `String(6)` |  | Tuesday |  | S/4 only entity |
| `TuesdayMorningClosingTime` | `WADIBI1` |  |  |  |  | `String(6)` |  | Tuesday |  | S/4 only entity |
| `TuesdayAfternoonOpeningTime` | `WADIAB2` |  |  |  |  | `String(6)` |  | Tuesday |  | S/4 only entity |
| `TuesdayAfternoonClosingTime` | `WADIBI2` |  |  |  |  | `String(6)` |  | Tuesday |  | S/4 only entity |
| `WednesdayMorningOpeningTime` | `WAMIAB1` |  |  |  |  | `String(6)` |  | Wednesday |  | S/4 only entity |
| `WednesdayMorningClosingTime` | `WAMIBI1` |  |  |  |  | `String(6)` |  | Wednesday |  | S/4 only entity |
| `WednesdayAfternoonOpeningTime` | `WAMIAB2` |  |  |  |  | `String(6)` |  | Wednesday |  | S/4 only entity |
| `WednesdayAfternoonClosingTime` | `WAMIBI2` |  |  |  |  | `String(6)` |  | Wednesday |  | S/4 only entity |
| `ThursdayMorningOpeningTime` | `WADOAB1` |  |  |  |  | `String(6)` |  | Thursday |  | S/4 only entity |
| `ThursdayMorningClosingTime` | `WADOBI1` |  |  |  |  | `String(6)` |  | Thursday |  | S/4 only entity |
| `ThursdayAfternoonOpeningTime` | `WADOAB2` |  |  |  |  | `String(6)` |  | Thursday |  | S/4 only entity |
| `ThursdayAfternoonClosingTime` | `WADOBI2` |  |  |  |  | `String(6)` |  | Thursday |  | S/4 only entity |
| `FridayMorningOpeningTime` | `WAFRAB1` |  |  |  |  | `String(6)` |  | Friday |  | S/4 only entity |
| `FridayMorningClosingTime` | `WAFRBI1` |  |  |  |  | `String(6)` |  | Friday |  | S/4 only entity |
| `FridayAfternoonOpeningTime` | `WAFRAB2` |  |  |  |  | `String(6)` |  | Friday |  | S/4 only entity |
| `FridayAfternoonClosingTime` | `WAFRBI2` |  |  |  |  | `String(6)` |  | Friday |  | S/4 only entity |
| `SaturdayMorningOpeningTime` | `WASAAB1` |  |  |  |  | `String(6)` |  | Saturday |  | S/4 only entity |
| `SaturdayMorningClosingTime` | `WASABI1` |  |  |  |  | `String(6)` |  | Saturday |  | S/4 only entity |
| `SaturdayAfternoonOpeningTime` | `WASAAB2` |  |  |  |  | `String(6)` |  | Saturday |  | S/4 only entity |
| `SaturdayAfternoonClosingTime` | `WASABI2` |  |  |  |  | `String(6)` |  | Saturday |  | S/4 only entity |
| `SundayMorningOpeningTime` | `WASOAB1` |  |  |  |  | `String(6)` |  | Sunday |  | S/4 only entity |
| `SundayMorningClosingTime` | `WASOBI1` |  |  |  |  | `String(6)` |  | Sunday |  | S/4 only entity |
| `SundayAfternoonOpeningTime` | `WASOAB2` |  |  |  |  | `String(6)` |  | Sunday |  | S/4 only entity |
| `SundayAfternoonClosingTime` | `WASOBI2` |  |  |  |  | `String(6)` |  | Sunday |  | S/4 only entity |


## Entity: `CustomerWithHoldingTax`

- **ABAP CDS Name:** `I_CustomerWithTax`
- **Label:** Customer WithHolding Tax
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Customer` | `KUNNR` |  |  |  |  | `String(10)` | Y | Customer |  | S/4 only entity |
| `CompanyCode` | `BUKRS` |  |  |  |  | `String(4)` | Y | Company Code |  | S/4 only entity |
| `WithholdingTaxType` | `WITHT` |  |  |  |  | `String(2)` | Y | Withholding Tax Type |  | S/4 only entity |
| `WithholdingTaxCode` | `WT_WITHCD` |  |  |  |  | `String(2)` |  | W/Tax Code |  | S/4 only entity |
| `WithholdingTaxAgent` | `WT_WTAGT` |  |  |  |  | `Boolean` |  | WTax Agent |  | S/4 only entity |
| `ObligationDateBegin` | `WT_AGTDF` |  |  |  |  | `Date` |  | W/Tax Obligated Frm |  | S/4 only entity |
| `ObligationDateEnd` | `WT_AGTDT` |  |  |  |  | `Date` |  | Oblig.to W/Tax Until |  | S/4 only entity |
| `WithholdingTaxNumber` | `WT_WTSTCD` |  |  |  |  | `String(16)` |  | W/tax number |  | S/4 only entity |
| `WithholdingTaxCertificate` | `WT_EXNR` |  |  |  |  | `String(25)` |  | Exemption Number |  | S/4 only entity |
| `WithholdingTaxExmptPercent` | `WT_EXRT` |  |  |  |  | `Decimal(5,2)` |  | Exemption Rate |  | S/4 only entity |
| `ExemptionDateBegin` | `WT_EXDF` |  |  |  |  | `Date` |  | Exemption Start Date |  | S/4 only entity |
| `ExemptionDateEnd` | `WT_EXDT` |  |  |  |  | `Date` |  | Exemption End Date |  | S/4 only entity |
| `ExemptionReason` | `WT_WTEXRS` |  |  |  |  | `String(2)` |  | Exemption Reason |  | S/4 only entity |
