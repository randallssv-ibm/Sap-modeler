# Customer

> Source file: `sap-s4com-Customer-v1.json`

**Technical Name:** `` | **Data Category:** `DIMENSION` | **VDM Type:** `BASIC` | **Size:** `XL`


## Entity: `Customer`

- **ABAP CDS Name:** `I_Customer`
- **Label:** Customer
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** KNA1, ADRC

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
| `IndustryCode1` | `BRAN1_D` |  |  |  |  | `String(10)` |  | Industry Code 1 |  |  |
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
- **ECC Source Tables:** KNB1

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Customer` | `KUNNR` | `KNB5` | `KUNNR` |  |  | `String(10)` | Y | Customer |  |  |
| `CompanyCode` | `BUKRS` | `KNB5` | `BUKRS` |  |  | `String(4)` | Y | Company Code |  |  |
| `AccountingClerk` | `BUSAB` |  |  |  |  | `String(2)` |  | Clerk Abbrev. |  |  |
| `ReconciliationAccount` | `AKONT` | `KNB1` | `AKONT` |  |  | `String(10)` |  | Reconciliation Acct |  |  |
| `AuthorizationGroup` | `BRGRU` |  |  |  |  | `String(4)` |  | Authorization |  |  |
| `CustomerHeadOffice` | `KNRZE` |  |  |  |  | `String(10)` |  | Head Office |  |  |
| `AlternativePayerAccount` | `KNRZB` |  |  |  |  | `String(10)` |  | Alternative payer |  |  |
| `PaymentBlockingReason` | `DZAHLS` |  |  |  |  | `String(1)` |  | Payment Block |  |  |
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
- **ECC Source Tables:** KNB5

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `CompanyCode` | `BUKRS` |  |  |  |  | `String(4)` | Y | Company Code |  |  |
| `Customer` | `KUNNR` |  |  |  |  | `String(10)` | Y | Customer |  |  |
| `DunningArea` | `MABER` |  |  |  |  | `String(2)` | Y | Dunning Area |  |  |
| `LastDunnedOn` | `MADAT` |  |  |  |  | `Date` |  | Last Dunned |  |  |
| `DunningProcedure` | `MAHNA` |  |  |  |  | `String(4)` |  | Dunning Procedure |  |  |
| `DunningLevel` | `MAHNS_D` |  |  |  |  | `String(1)` |  | Dunning Level |  |  |
| `DunningBlock` | `MANSP` |  |  |  |  | `String(1)` |  | Dunning Block |  |  |
| `DunningRecipient` | `KNRMA` |  |  |  |  | `String(10)` |  | Dunning Recipient |  |  |
| `LegDunningProcedureOn` | `GMVDT` |  |  |  |  | `Date` |  | Legal Dunn.Proc.From |  |  |
| `DunningClerk` | `BUSAB_MA` |  |  |  |  | `String(2)` |  | Dunning Clerk |  |  |


## Entity: `CustomerSalesArea`

- **ABAP CDS Name:** `I_CustomerSalesArea`
- **Label:** Customer Sales Area
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** KNVV

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Customer` | `KUNNR` |  |  |  |  | `String(10)` | Y | Customer |  |  |
| `SalesOrganization` | `VKORG` |  |  |  |  | `String(4)` | Y | Sales Organization |  |  |
| `DistributionChannel` | `VTWEG` |  |  |  |  | `String(2)` | Y | Distribution Channel |  |  |
| `Division` | `SPART` |  |  |  |  | `String(2)` | Y | Division |  |  |
| `CustomerABCClassification` | `KLABC` |  |  |  |  | `String(2)` |  | ABC Classification |  |  |
| `SalesOffice` | `VKBUR` |  |  |  |  | `String(4)` |  | Sales Office |  |  |
| `SalesGroup` | `VKGRP` |  |  |  |  | `String(3)` |  | Sales Group |  |  |
| `OrderIsBlockedForCustomer` | `AUFSD_V` |  |  |  |  | `String(2)` |  | Ord.blk:sls ar. |  |  |
| `Currency` | `WAERS_V02D` |  |  |  |  | `String(5)` |  | Currency |  |  |
| `CustomerPriceGroup` | `KONDA` |  |  |  |  | `String(2)` |  | Customer Price Group |  |  |
| `PriceListType` | `PLTYP` |  |  |  |  | `String(2)` |  | Price List Type |  |  |
| `DeliveryPriority` | `LPRIO` |  |  |  |  | `String(2)` |  | Delivery Priority |  |  |
| `ShippingCondition` | `VSBED` |  |  |  |  | `String(2)` |  | Shipping Conditions |  |  |
| `IncotermsClassification` | `INCO1` |  |  |  |  | `String(3)` |  | Incoterms |  |  |
| `SupplyingPlant` | `DWERK_EXT` |  |  |  |  | `String(4)` |  | Delivering Plant |  |  |
| `CompleteDeliveryIsDefined` | `AUTLF` |  |  |  |  | `Boolean` |  | Complete Delivery |  |  |
| `DeliveryIsBlockedForCustomer` | `LIFSD_V` |  |  |  |  | `String(2)` |  | DelBlckSalesAr. |  |  |
| `BillingIsBlockedForCustomer` | `FAKSD_V` |  |  |  |  | `String(2)` |  | BBlock for SlsA |  |  |
| `CustomerPaymentTerms` | `DZTERM` |  |  |  |  | `String(4)` |  | Terms of Payment |  |  |
| `CustomerAccountAssignmentGroup` | `KTGRD` |  |  |  |  | `String(2)` |  | Acct Assmt Grp Cust. |  |  |
| `AccountByCustomer` | `EIKTO` |  |  |  |  | `String(12)` |  | Account at Customer |  |  |
| `CustomerGroup` | `KDGRP` |  |  |  |  | `String(2)` |  | Customer Group |  |  |
| `CustomerPricingProcedure` | `KALKS` |  |  |  |  | `String(2)` |  | Cust.Pric.Procedure |  |  |
| `OrderCombinationIsAllowed` | `KZAZU_D` |  |  |  |  | `Boolean` |  | Order Combination |  |  |
| `PartialDeliveryIsAllowed` | `KZTLF` |  |  |  |  | `String(1)` |  | Partial Deliv./Item |  |  |
| `InvoiceDate` | `PERFK` |  |  |  |  | `String(2)` |  | Invoicing Dates |  |  |
| `PaymentTerms` | `DZTERM` |  |  |  |  | `String(4)` |  | Terms of Payment |  |  |
| `IncotermsTransferLocation` | `INCO2` |  |  |  |  | `String(28)` |  | Incoterms (Part 2) |  |  |
| `ItemOrderProbabilityInPercent` | `AWAHR` |  |  |  |  | `String(3)` |  | Order Probability |  |  |
| `IncotermsLocation2` | `INCO3_L` |  |  |  |  | `String(70)` |  | Incoterms Location 2 |  |  |
| `RecordCreatedDate` | `ERDAT` |  |  |  |  | `Date` |  | Created On |  |  |
| `AuthorizationGroup` | `BEGRU` |  |  |  |  | `String(4)` |  | Authorization Group |  |  |
| `SalesDistrict` | `BZIRK` |  |  |  |  | `String(6)` |  | Sales District |  |  |
| `IncotermsVersion` | `INCOV` |  |  |  |  | `String(4)` |  | Incoterms Version |  |  |
| `IncotermsLocation1` | `INCO2_L` |  |  |  |  | `String(70)` |  | Incoterms Location 1 |  |  |
| `DeletionIndicator` | `LOEVM_V` |  |  |  |  | `Boolean` |  | Del.ID SlsArea |  |  |
| `IsBusinessPurposeCompleted` |  |  |  |  |  | `Boolean` |  | Purpose Completed |  |  |
| `SalesItemProposal` | `VSORT` |  |  |  |  | `String(10)` |  | Item proposal |  |  |
| `CustProdProposalProcedure` | `PVKSM` |  |  |  |  | `String(2)` |  | PP customer proced. |  |  |
| `ProofOfDeliveryTime` |  |  |  |  |  | `String(6)` |  |  |  |  |
| `ProofOfDeliveryTimeValue` | `CUST_POD` |  |  |  |  | `Decimal(6,2)` |  | POD timeframe |  |  |
| `MaxNmbrOfPartialDelivery` | `ANTLF` |  |  |  |  | `Decimal(1,0)` |  | Max.Part.Deliveries |  |  |
| `UnderdelivTolrtdLmtRatioInPct` | `UNTTO` |  |  |  |  | `Decimal(3,1)` |  | Underdel. Tolerance |  |  |
| `OverdelivTolrtdLmtRatioInPct` | `UEBTO` |  |  |  |  | `Decimal(3,1)` |  | Overdeliv. Tolerance |  |  |
| `IsActiveEntity` | `SDRAFT_IS_ACTIVE` |  |  |  |  | `Boolean` |  | Is active |  |  |
| `AdditionalCustomerGroup1` | `KVGR1` |  |  |  |  | `String(3)` |  | Customer Group 1 |  |  |
| `AdditionalCustomerGroup2` | `KVGR2` |  |  |  |  | `String(3)` |  | Customer Group 2 |  |  |
| `AdditionalCustomerGroup3` | `KVGR3` |  |  |  |  | `String(3)` |  | Customer Group 3 |  |  |
| `AdditionalCustomerGroup4` | `KVGR4` |  |  |  |  | `String(3)` |  | Customer Group 4 |  |  |
| `AdditionalCustomerGroup5` | `KVGR5` |  |  |  |  | `String(3)` |  | Customer Group 5 |  |  |
| `InvoiceListSchedule` | `PERRL` |  |  |  |  | `String(2)` |  | Invoice List Sched. |  |  |
| `ExchangeRateType` | `KURST` |  |  |  |  | `String(4)` |  | Exchange Rate Type |  |  |
| `PaymentGuaranteeProcedure` | `KABSSCH_CM` |  |  |  |  | `String(4)` |  | Paymt guarant. proc. |  |  |
| `SuplrIsRlvtForSettlmtMgmt` | `AGREL` |  |  |  |  | `Boolean` |  | Settlement Mgmt. |  |  |
| `CustIsRlvtForSettlmtMgmt` | `AGREL` |  |  |  |  | `Boolean` |  | Settlement Mgmt. |  |  |
| `ProductUnitGroup` | `MEGRU` |  |  |  |  | `String(4)` |  | Unit of Measure Grp |  |  |
| `SlsDocIsRlvtForProofOfDeliv` | `PODKZ` |  |  |  |  | `Boolean` |  | Relevant for POD |  |  |
| `SlsUnlmtdOvrdelivIsAllwd` | `UEBTK_V` |  |  |  |  | `Boolean` |  | Unlimited Tolerance |  |  |
| `CreditControlArea` | `KKBER` |  |  |  |  | `String(4)` |  | Credit Control Area |  |  |
| `CustomerIsRebateRelevant` | `BOKRE` |  |  |  |  | `Boolean` |  | Rebate |  |  |
| `InspSbstHasNoTimeOrQuantity` | `PRFRE` |  |  |  |  | `Boolean` |  | Price determination |  |  |
| `ManualInvoiceMaintIsRelevant` | `MRNKZ` |  |  |  |  | `Boolean` |  | Man. Invoice Maint. |  |  |
| `IncotermsSupChnLoc1AddlUUID` |  |  |  |  |  | `UUID` |  | Location UUID |  |  |
| `IncotermsSupChnLoc2AddlUUID` |  |  |  |  |  | `UUID` |  | Location UUID |  |  |
| `IncotermsSupChnDvtgLocAddlUUID` |  |  |  |  |  | `UUID` |  | Location UUID |  |  |
| `SalesBlockForCustomer` | `CASSD_V` |  |  |  |  | `String(2)` |  | Sales Block |  |  |
| `CustomerStatisticsGroup` | `STGKU` |  |  |  |  | `String(1)` |  | Customer Stats.Group |  |  |
| `RetailAdditionalCustomerGrp6` | `FSH_KVGR6` |  |  |  |  | `String(3)` |  | Customer Group 6 |  |  |
| `RetailAdditionalCustomerGrp7` | `FSH_KVGR7` |  |  |  |  | `String(3)` |  | Customer Group 7 |  |  |
| `RetailAdditionalCustomerGrp8` | `FSH_KVGR8` |  |  |  |  | `String(3)` |  | Customer Group 8 |  |  |
| `RetailAdditionalCustomerGrp9` | `FSH_KVGR9` |  |  |  |  | `String(3)` |  | Customer Group 9 |  |  |
| `RetailAdditionalCustomerGrp10` | `FSH_KVGR10` |  |  |  |  | `String(3)` |  | Customer Group 10 |  |  |


## Entity: `CustomerSalesAreaTax`

- **ABAP CDS Name:** `I_CustSalesAreaTax`
- **Label:** Customer Sales Area Tax
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** KNVI

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Customer` | `KUNNR` |  |  |  |  | `String(10)` | Y | Customer |  |  |
| `SalesOrganization` | `VKORG` |  |  |  |  | `String(4)` | Y | Sales Organization |  |  |
| `DistributionChannel` | `VTWKU` |  |  |  |  | `String(2)` | Y | RefDistCh-Cust/Mat. |  |  |
| `Division` | `SPART` |  |  |  |  | `String(2)` | Y | Division |  |  |
| `DepartureCountry` | `ALAND` |  |  |  |  | `String(3)` | Y | Departure Ctry/Reg. |  |  |
| `CustomerTaxCategory` | `TATYP` |  |  |  |  | `String(4)` | Y | Tax Condition Type |  |  |
| `CustomerTaxClassification` | `TAKLD` |  |  |  |  | `String(1)` |  | Tax Classification |  |  |
| `AuthorizationGroup` | `BRGRU` |  |  |  |  | `String(4)` |  | Authorization |  |  |
| `IsBusinessPurposeCompleted` |  |  |  |  |  | `Boolean` |  | Purpose Completed |  |  |


## Entity: `CustomerUnloadingPoint`

- **ABAP CDS Name:** `I_CustomerUnloadingPoint`
- **Label:** Customer Unloading Point
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** KNVA

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Customer` | `KUNNR` |  |  |  |  | `String(10)` | Y | Customer |  |  |
| `UnloadingPointName` | `ABLAD` |  |  |  |  | `String(25)` | Y | Unloading Point |  |  |
| `CustomerFactoryCalenderCode` | `KNKAL` |  |  |  |  | `String(2)` |  | Cust.fact.calendar |  |  |
| `BPGoodsReceivingHoursCode` | `WANID` |  |  |  |  | `String(3)` |  | Goods receiving hrs |  |  |
| `IsDfltBPUnloadingPoint` | `DEFAB` |  |  |  |  | `Boolean` |  | Default unloading pt |  |  |
| `MondayMorningOpeningTime` | `WAMOAB1` |  |  |  |  | `String(6)` |  | Monday |  |  |
| `MondayMorningClosingTime` | `WAMOBI1` |  |  |  |  | `String(6)` |  | Monday |  |  |
| `MondayAfternoonOpeningTime` | `WAMOAB2` |  |  |  |  | `String(6)` |  | Monday |  |  |
| `MondayAfternoonClosingTime` | `WAMOBI2` |  |  |  |  | `String(6)` |  | Monday |  |  |
| `TuesdayMorningOpeningTime` | `WADIAB1` |  |  |  |  | `String(6)` |  | Tuesday |  |  |
| `TuesdayMorningClosingTime` | `WADIBI1` |  |  |  |  | `String(6)` |  | Tuesday |  |  |
| `TuesdayAfternoonOpeningTime` | `WADIAB2` |  |  |  |  | `String(6)` |  | Tuesday |  |  |
| `TuesdayAfternoonClosingTime` | `WADIBI2` |  |  |  |  | `String(6)` |  | Tuesday |  |  |
| `WednesdayMorningOpeningTime` | `WAMIAB1` |  |  |  |  | `String(6)` |  | Wednesday |  |  |
| `WednesdayMorningClosingTime` | `WAMIBI1` |  |  |  |  | `String(6)` |  | Wednesday |  |  |
| `WednesdayAfternoonOpeningTime` | `WAMIAB2` |  |  |  |  | `String(6)` |  | Wednesday |  |  |
| `WednesdayAfternoonClosingTime` | `WAMIBI2` |  |  |  |  | `String(6)` |  | Wednesday |  |  |
| `ThursdayMorningOpeningTime` | `WADOAB1` |  |  |  |  | `String(6)` |  | Thursday |  |  |
| `ThursdayMorningClosingTime` | `WADOBI1` |  |  |  |  | `String(6)` |  | Thursday |  |  |
| `ThursdayAfternoonOpeningTime` | `WADOAB2` |  |  |  |  | `String(6)` |  | Thursday |  |  |
| `ThursdayAfternoonClosingTime` | `WADOBI2` |  |  |  |  | `String(6)` |  | Thursday |  |  |
| `FridayMorningOpeningTime` | `WAFRAB1` |  |  |  |  | `String(6)` |  | Friday |  |  |
| `FridayMorningClosingTime` | `WAFRBI1` |  |  |  |  | `String(6)` |  | Friday |  |  |
| `FridayAfternoonOpeningTime` | `WAFRAB2` |  |  |  |  | `String(6)` |  | Friday |  |  |
| `FridayAfternoonClosingTime` | `WAFRBI2` |  |  |  |  | `String(6)` |  | Friday |  |  |
| `SaturdayMorningOpeningTime` | `WASAAB1` |  |  |  |  | `String(6)` |  | Saturday |  |  |
| `SaturdayMorningClosingTime` | `WASABI1` |  |  |  |  | `String(6)` |  | Saturday |  |  |
| `SaturdayAfternoonOpeningTime` | `WASAAB2` |  |  |  |  | `String(6)` |  | Saturday |  |  |
| `SaturdayAfternoonClosingTime` | `WASABI2` |  |  |  |  | `String(6)` |  | Saturday |  |  |
| `SundayMorningOpeningTime` | `WASOAB1` |  |  |  |  | `String(6)` |  | Sunday |  |  |
| `SundayMorningClosingTime` | `WASOBI1` |  |  |  |  | `String(6)` |  | Sunday |  |  |
| `SundayAfternoonOpeningTime` | `WASOAB2` |  |  |  |  | `String(6)` |  | Sunday |  |  |
| `SundayAfternoonClosingTime` | `WASOBI2` |  |  |  |  | `String(6)` |  | Sunday |  |  |


## Entity: `CustomerWithHoldingTax`

- **ABAP CDS Name:** `I_CustomerWithTax`
- **Label:** Customer WithHolding Tax
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** KNBW

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Customer` | `KUNNR` |  |  |  |  | `String(10)` | Y | Customer |  |  |
| `CompanyCode` | `BUKRS` |  |  |  |  | `String(4)` | Y | Company Code |  |  |
| `WithholdingTaxType` | `WITHT` |  |  |  |  | `String(2)` | Y | Withholding Tax Type |  |  |
| `WithholdingTaxCode` | `WT_WITHCD` |  |  |  |  | `String(2)` |  | W/Tax Code |  |  |
| `WithholdingTaxAgent` | `WT_WTAGT` |  |  |  |  | `Boolean` |  | WTax Agent |  |  |
| `ObligationDateBegin` | `WT_AGTDF` |  |  |  |  | `Date` |  | W/Tax Obligated Frm |  |  |
| `ObligationDateEnd` | `WT_AGTDT` |  |  |  |  | `Date` |  | Oblig.to W/Tax Until |  |  |
| `WithholdingTaxNumber` | `WT_WTSTCD` |  |  |  |  | `String(16)` |  | W/tax number |  |  |
| `WithholdingTaxCertificate` | `WT_EXNR` |  |  |  |  | `String(25)` |  | Exemption Number |  |  |
| `WithholdingTaxExmptPercent` | `WT_EXRT` |  |  |  |  | `Decimal(5,2)` |  | Exemption Rate |  |  |
| `ExemptionDateBegin` | `WT_EXDF` |  |  |  |  | `Date` |  | Exemption Start Date |  |  |
| `ExemptionDateEnd` | `WT_EXDT` |  |  |  |  | `Date` |  | Exemption End Date |  |  |
| `ExemptionReason` | `WT_WTEXRS` |  |  |  |  | `String(2)` |  | Exemption Reason |  |  |
