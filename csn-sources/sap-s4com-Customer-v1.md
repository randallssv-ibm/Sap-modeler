# Customer

> Source file: `sap-s4com-Customer-v1.json`

**Technical Name:** `` | **Data Category:** `DIMENSION` | **VDM Type:** `BASIC` | **Size:** `XL`


## Entity: `Customer`

- **ABAP Name:** `I_Customer`
- **Label:** Customer
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** ADRC, KNA1

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Customer` | `KUNNR` | `KUNNR` | `KNA1` | `String(10)` | Y | Customer |  |  |  |
| `CustomerName` | `MD_CUSTOMER_NAME` | `MD_CUSTOMER_NAME` | `KNA1` | `String(80)` |  | Name of Customer |  |  |  |
| `CustomerFullName` | `MD_CUSTOMER_FULL_NAME` | `MD_CUSTOMER_FULL_NAME` | `KNA1` | `String(220)` |  | Customer Name |  |  |  |
| `BPCustomerName` | `CUSTOMERNAME_2` | `CUSTOMERNAME_2` | `KNA1` | `String(81)` |  | Business Partner - Customer Name |  |  |  |
| `BPCustomerFullName` | `MD_CUSTOMER_FULL_NAME` | `MD_CUSTOMER_FULL_NAME` | `KNA1` | `String(220)` |  | Business Partner - Customer Full Name |  |  |  |
| `CreatedByUser` | `ERNAM_RF` | `ERNAM_RF` | `KNA1` | `String(12)` |  | Created by |  |  |  |
| `CreationDate` | `ERDAT_RF` | `ERDAT_RF` | `KNA1` | `Date` |  | Created On |  |  |  |
| `AddressID` | `ADRNR` | `ADDRNUMBER` | `ADRC` | `String(10)` |  | Address |  |  |  |
| `CustomerClassification` | `KUKLA` | `KUKLA` | `KNA1` | `String(2)` |  | Customer Classific. |  | _CustomerClassification |  |
| `VATRegistration` | `STCEG` | `STCEG` | `KNA1` | `String(20)` |  | VAT Registration No. |  |  |  |
| `CustomerAccountGroup` | `KTOKD` | `KTOKD` | `KNA1` | `String(4)` |  | Account Group |  |  |  |
| `AuthorizationGroup` | `BRGRU` | `BRGRU` | `KNA1` | `String(4)` |  | Authorization |  |  |  |
| `DeliveryIsBlocked` | `LIFSD_X` | `LIFSD_X` | `KNA1` | `String(2)` |  | Delivery block |  |  |  |
| `PostingIsBlocked` | `SPERB_X` | `SPERB_X` | `KNA1` | `Boolean` |  | Posting Block |  |  |  |
| `BillingIsBlockedForCustomer` | `FAKSD_X` | `FAKSD_X` | `KNA1` | `String(2)` |  | Billing Block |  |  |  |
| `OrderIsBlockedForCustomer` | `AUFSD_X` | `AUFSD_X` | `KNA1` | `String(2)` |  | Order Block |  |  |  |
| `InternationalLocationNumber1` | `BBBNR` | `BBBNR` | `KNA1` | `String(7)` |  | Int. location no. 1 |  |  |  |
| `IsOneTimeAccount` | `XCPDK` | `XCPDK` | `KNA1` | `Boolean` |  | One-Time Account |  |  |  |
| `TaxJurisdiction` | `TXJCD` | `TXJCD` | `KNA1` | `String(15)` |  | Tax Jurisdiction |  |  |  |
| `Industry` | `BRSCH` | `BRSCH` | `KNA1` | `String(4)` |  | Industry |  |  |  |
| `TaxNumberType` | `J_1ATOID` | `J_1ATOID` | `KNA1` | `String(2)` |  | Tax Number Type |  |  |  |
| `TaxNumber1` | `STCD1` | `STCD1` | `KNA1` | `String(16)` |  | Tax Number 1 |  |  |  |
| `TaxNumber2` | `STCD2` | `STCD2` | `KNA1` | `String(11)` |  | Tax Number 2 |  |  |  |
| `TaxNumber3` | `STCD3` | `STCD3` | `KNA1` | `String(18)` |  | Tax Number 3 |  |  |  |
| `TaxNumber4` | `STCD4` | `STCD4` | `KNA1` | `String(18)` |  | Tax Number 4 |  |  |  |
| `TaxNumber5` | `STCD5` | `STCD5` | `KNA1` | `String(60)` |  | Tax Number 5 |  |  |  |
| `TaxNumber6` | `STCD6` | `STCD6` | `KNA1` | `String(20)` |  | Tax Number 6 |  |  |  |
| `CustomerCorporateGroup` | `KONZS` | `KONZS` | `KNA1` | `String(10)` |  | Group Key |  |  |  |
| `Supplier` | `LIFNR` | `LIFNR` | `KNA1` | `String(10)` |  | Supplier |  |  |  |
| `NielsenRegion` | `NIELS` | `NIELS` | `KNA1` | `String(2)` |  | Nielsen Indicator |  |  |  |
| `IndustryCode1` | `BRAN1_D` | `BRAN1` | `KNA1` | `String(10)` |  | Industry Code 1 |  |  |  |
| `IndustryCode2` | `BRAN2` | `BRAN2` | `KNA1` | `String(10)` |  | Industry Code 2 |  |  |  |
| `IndustryCode3` | `BRAN3` | `BRAN3` | `KNA1` | `String(10)` |  | Industry Code 3 |  |  |  |
| `IndustryCode4` | `BRAN4` | `BRAN4` | `KNA1` | `String(10)` |  | Industry Code 4 |  |  |  |
| `IndustryCode5` | `BRAN5` | `BRAN5` | `KNA1` | `String(10)` |  | Industry Code 5 |  |  |  |
| `Country` | `LAND1_GP` | `LAND1_GP` | `KNA1` | `String(3)` |  | Country/Region Key |  |  |  |
| `OrganizationBPName1` | `NAME1_GP` | `NAME1_GP` | `KNA1` | `String(35)` |  | Name |  |  |  |
| `OrganizationBPName2` | `NAME2_GP` | `NAME2_GP` | `KNA1` | `String(35)` |  | Name 2 |  |  |  |
| `CityName` | `ORT01_GP` | `ORT01_GP` | `KNA1` | `String(35)` |  | City |  |  |  |
| `PostalCode` | `PSTLZ` | `PSTLZ` | `KNA1` | `String(10)` |  | Postal Code |  |  |  |
| `StreetName` | `STRAS_GP` | `STRAS_GP` | `KNA1` | `String(35)` |  | Street |  |  |  |
| `SortField` | `SORTL` | `SORTL` | `KNA1` | `String(10)` |  | Search Term |  |  |  |
| `FaxNumber` | `TELFX` | `TELFX` | `KNA1` | `String(31)` |  | Fax Number |  |  |  |
| `BR_SUFRAMACode` | `J_1BSUFRAMA` | `J_1BSUFRAMA` | `KNA1` | `String(9)` |  | Suframa Code |  |  |  |
| `Region` | `REGIO` | `REGIO` | `KNA1` | `String(3)` |  | Region |  |  |  |
| `TelephoneNumber1` | `TELF1` | `TELF1` | `KNA1` | `String(16)` |  | Telephone 1 |  |  |  |
| `TelephoneNumber2` | `TELF2` | `TELF2` | `KNA1` | `String(16)` |  | Telephone 2 |  |  |  |
| `AlternativePayerAccount` | `KNRZA` | `KNRZA` | `KNA1` | `String(10)` |  | Alternative Payer |  |  |  |
| `DataMediumExchangeIndicator` | `DTAMS` | `DTAMS` | `KNA1` | `String(1)` |  | DME Recipient Code |  |  |  |
| `VATLiability` | `STKZU` | `STKZU` | `KNA1` | `Boolean` |  | Liable for VAT |  |  |  |
| `IsBusinessPurposeCompleted` |  |  |  | `Boolean` |  | Purpose Completed |  |  |  |
| `ResponsibleType` | `J_1AFITP_D` | `J_1AFITP` | `KNA1` | `String(2)` |  | Tax Type |  |  |  |
| `FiscalAddress` | `FISKN_D` | `FISKN` | `KNA1` | `String(10)` |  | Fiscal address |  |  |  |
| `NFPartnerIsNaturalPerson` |  |  |  | `Boolean` |  | Natural Person |  |  |  |
| `DeletionIndicator` | `LOEVM_X` | `LOEVM_X` | `KNA1` | `Boolean` |  | Deletion Flag |  |  |  |
| `Language` | `SPRAS` | `SPRAS` | `KNA1` | `String(2)` |  | Language Key |  |  |  |
| `TradingPartner` | `RASSC` | `RASSC` | `KNA1` | `String(6)` |  | Trading Partner No. |  | _GlobalCompany |  |
| `DeliveryDateTypeRule` | `SD_DELIVERY_DATE_TYPE_RULE` | `SD_DELIVERY_DATE_TYPE_RULE` | `KNA1` | `String(1)` |  | Deliv Date Rule |  |  |  |
| `ExpressTrainStationName` | `BAHNE` | `BAHNE` | `KNA1` | `String(25)` |  | Express station |  |  |  |
| `TrainStationName` | `BAHNS` | `BAHNS` | `KNA1` | `String(25)` |  | Train station |  |  |  |
| `InternationalLocationNumber2` | `BBSNR` | `BBSNR` | `KNA1` | `String(5)` |  | Int. location no. 2 |  |  |  |
| `InternationalLocationNumber3` | `BUBKZ` | `BUBKZ` | `KNA1` | `String(1)` |  | Check digit |  |  |  |
| `CityCode` | `CITYC` | `CITYC` | `KNA1` | `String(4)` |  | City Code |  |  |  |
| `County` | `COUNC` | `COUNC` | `KNA1` | `String(3)` |  | County Code |  |  |  |
| `CustomerHasUnloadingPoint` | `EXABL` | `EXABL` | `KNA1` | `Boolean` |  | Unloading points |  |  |  |
| `CustomerWorkingTimeCalendar` | `KNAZK` | `KNAZK` | `KNA1` | `String(2)` |  | Working times |  |  |  |
| `IsCompetitor` | `DEAR1` | `DEAR1` | `KNA1` | `Boolean` |  | Competitors |  |  |  |
| `TaxInvoiceRepresentativeName` | `REPRES` | `REPRES` | `KNA1` | `String(10)` |  | Rep's Name |  |  |  |
| `BusinessType` | `GESTYP` | `GESTYP` | `KNA1` | `String(30)` |  | Type of Business |  |  |  |
| `IndustryType` | `INDTYP` | `INDTYP` | `KNA1` | `String(30)` |  | Type of Industry |  |  |  |
| `TW_CollvBillingIsSupported` |  |  |  | `Boolean` |  | Consolidated Invoic. |  |  |  |
| `AlternativePayeeIsAllowed` | `XREGU` | `XREGU` | `KNA1` | `Boolean` |  | Alt.payer in doc? |  |  |  |
| `FreeDefinedAttribute01` | `KATR1` | `KATR1` | `KNA1` | `String(2)` |  | Attribute 1 |  |  |  |
| `FreeDefinedAttribute02` | `KATR2` | `KATR2` | `KNA1` | `String(2)` |  | Attribute 2 |  |  |  |
| `FreeDefinedAttribute03` | `KATR3` | `KATR3` | `KNA1` | `String(2)` |  | Attribute 3 |  |  |  |
| `FreeDefinedAttribute04` | `KATR4` | `KATR4` | `KNA1` | `String(2)` |  | Attribute 4 |  |  |  |
| `FreeDefinedAttribute05` | `KATR5` | `KATR5` | `KNA1` | `String(2)` |  | Attribute 5 |  |  |  |
| `FreeDefinedAttribute06` | `KATR6` | `KATR6` | `KNA1` | `String(3)` |  | Attribute 6 |  |  |  |
| `FreeDefinedAttribute07` | `KATR7` | `KATR7` | `KNA1` | `String(3)` |  | Attribute 7 |  |  |  |
| `FreeDefinedAttribute08` | `KATR8` | `KATR8` | `KNA1` | `String(3)` |  | Attribute 8 |  |  |  |
| `FreeDefinedAttribute09` | `KATR9` | `KATR9` | `KNA1` | `String(3)` |  | Attribute 9 |  |  |  |
| `FreeDefinedAttribute10` | `KATR10` | `KATR10` | `KNA1` | `String(3)` |  | Attribute 10 |  |  |  |
| `PaymentReason` | `FARP_PAYT_RSN` | `PAYT_RSN` | `KNA1` | `String(4)` |  | Payment Reason |  |  |  |
| `CustomerConditionGroup1` | `KDKG1` | `KDKG1` | `KNA1` | `String(2)` |  | Condition Group 1 |  |  |  |
| `CustomerConditionGroup2` | `KDKG2` | `KDKG2` | `KNA1` | `String(2)` |  | Condition Group 2 |  |  |  |
| `CustomerConditionGroup3` | `KDKG3` | `KDKG3` | `KNA1` | `String(2)` |  | Condition Group 3 |  |  |  |
| `CustomerConditionGroup4` | `KDKG4` | `KDKG4` | `KNA1` | `String(2)` |  | Condition Group 4 |  |  |  |
| `CustomerConditionGroup5` | `KDKG5` | `KDKG5` | `KNA1` | `String(2)` |  | Condition Group 5 |  |  |  |
| `IsSalesProspect` |  |  |  | `Boolean` |  | Prospect |  |  |  |
| `PaymentIsBlockedForCustomer` | `SPERZ` | `SPERZ` | `KNA1` | `Boolean` |  | Payment block |  |  |  |
| `IsConsumer` | `DEAR6` | `DEAR6` | `KNA1` | `Boolean` |  | Consumer |  |  |  |
| `DataControllerSet` | `BU_XDCSET` | `BU_XDCSET` | `KNA1` | `String(1)` |  | Data Ctrlr. Set |  |  |  |
| `DataController1` | `BU_DATA_CONTROLLER` | `BU_DATA_CONTROLLER` | `KNA1` | `String(30)` |  | Data Controller |  |  |  |
| `DataController2` | `BU_DATA_CONTROLLER` | `BU_DATA_CONTROLLER` | `KNA1` | `String(30)` |  | Data Controller |  |  |  |
| `DataController3` | `BU_DATA_CONTROLLER` | `BU_DATA_CONTROLLER` | `KNA1` | `String(30)` |  | Data Controller |  |  |  |
| `DataController4` | `BU_DATA_CONTROLLER` | `BU_DATA_CONTROLLER` | `KNA1` | `String(30)` |  | Data Controller |  |  |  |
| `DataController5` | `BU_DATA_CONTROLLER` | `BU_DATA_CONTROLLER` | `KNA1` | `String(30)` |  | Data Controller |  |  |  |
| `DataController6` | `BU_DATA_CONTROLLER` | `BU_DATA_CONTROLLER` | `KNA1` | `String(30)` |  | Data Controller |  |  |  |
| `DataController7` | `BU_DATA_CONTROLLER` | `BU_DATA_CONTROLLER` | `KNA1` | `String(30)` |  | Data Controller |  |  |  |
| `DataController8` | `BU_DATA_CONTROLLER` | `BU_DATA_CONTROLLER` | `KNA1` | `String(30)` |  | Data Controller |  |  |  |
| `DataController9` | `BU_DATA_CONTROLLER` | `BU_DATA_CONTROLLER` | `KNA1` | `String(30)` |  | Data Controller |  |  |  |
| `DataController10` | `BU_DATA_CONTROLLER` | `BU_DATA_CONTROLLER` | `KNA1` | `String(30)` |  | Data Controller |  |  |  |
| `BusinessPartnerName1` | `AD_NAME1` | `AD_NAME1` | `KNA1` | `String(40)` |  | Business Partner Organization  - Name 1 |  |  |  |
| `BusinessPartnerName2` | `AD_NAME2` | `AD_NAME2` | `KNA1` | `String(40)` |  | Business Partner Organization  - Name 2 |  |  |  |
| `BusinessPartnerName3` | `AD_NAME3` | `AD_NAME3` | `KNA1` | `String(40)` |  | Business Partner Organization  - Name 3 |  |  |  |
| `BusinessPartnerName4` | `AD_NAME4` | `AD_NAME4` | `KNA1` | `String(40)` |  | Business Partner Organization  - Name 4 |  |  |  |
| `BPAddrCityName` | `AD_CITY1` | `AD_CITY1` | `KNA1` | `String(40)` |  | Business Partner Address – City |  |  |  |
| `BPAddrStreetName` | `AD_STREET` | `AD_STREET` | `KNA1` | `String(60)` |  | Business Partner Address – Street |  |  |  |
| `AddressSearchTerm1` | `AD_SORT1` | `AD_SORT1` | `KNA1` | `String(20)` |  | Business Partner Address - Search Term 1 |  |  |  |
| `AddressSearchTerm2` | `AD_SORT2` | `AD_SORT2` | `KNA1` | `String(20)` |  | Business Partner Address - Search Term 2 |  |  |  |
| `DistrictName` | `AD_CITY2` | `AD_CITY2` | `KNA1` | `String(40)` |  | Business Partner Address – District |  |  |  |
| `POBoxDeviatingCityName` | `AD_POBXLOC` | `AD_POBXLOC` | `KNA1` | `String(40)` |  | Business Partner Address - PO Box Deviating City |  |  |  |
| `BusinessPartnerFormOfAddress` | `AD_TITLE` | `AD_TITLE` | `KNA1` | `String(4)` |  | Business Partner - Form of Address |  |  |  |
| `BR_ICMSTaxPayerType` | `J_1BICMSTAXPAY` | `J_1BICMSTAXPAY` | `KNA1` | `String(2)` |  | ICMS Taxpayer |  |  |  |


## Entity: `CustomerCompanyCode`

- **ABAP Name:** `I_CustomerCompany`
- **Label:** Customer Company
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** KNB1, KNB5

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Customer` | `KUNNR` | `KUNNR` | `KNB5` | `String(10)` | Y | Customer |  | _Customer |  |
| `CompanyCode` | `BUKRS` | `BUKRS` | `KNB5` | `String(4)` | Y | Company Code |  |  |  |
| `AccountingClerk` | `BUSAB` | `BUSAB` | `KNB1` | `String(2)` |  | Clerk Abbrev. |  |  |  |
| `ReconciliationAccount` | `AKONT` | `AKONT` | `KNB1` | `String(10)` |  | Reconciliation Acct |  |  |  |
| `AuthorizationGroup` | `BRGRU` | `BRGRU` | `KNB1` | `String(4)` |  | Authorization |  |  |  |
| `CustomerHeadOffice` | `KNRZE` | `KNRZE` | `KNB1` | `String(10)` |  | Head Office |  |  |  |
| `AlternativePayerAccount` | `KNRZB` | `KNRZB` | `KNB1` | `String(10)` |  | Alternative payer |  |  |  |
| `PaymentBlockingReason` | `DZAHLS` | `DZAHLS` | `KNB1` | `String(1)` |  | Payment Block |  | _PaymentBlockValueHelp |  |
| `InterestCalculationCode` | `VZSKZ` | `VZSKZ` | `KNB1` | `String(2)` |  | Interest Indicator |  |  |  |
| `InterestCalculationDate` | `DZINDT` | `DZINDT` | `KNB1` | `Date` |  | Last Key Date |  |  |  |
| `IntrstCalcFrequencyInMonths` | `DZINRT` | `DZINRT` | `KNB1` | `String(2)` |  | Int.Calc.Freq. |  |  |  |
| `CustomerAccountNote` | `KVERM` | `KVERM` | `KNB1` | `String(30)` |  | Account Memo |  |  |  |
| `APARToleranceGroup` | `TOGRU` | `TOGRU` | `KNB1` | `String(4)` |  | Tolerance Group |  |  |  |
| `HouseBank` | `HBKID` | `HBKID` | `KNB1` | `String(5)` |  | House Bank |  |  |  |
| `ItemIsToBePaidSeparately` | `XPORE` | `XPORE` | `KNB1` | `Boolean` |  | Individual Payment |  |  |  |
| `PaytAdviceIsSentbyEDI` | `XEDIP` | `XEDIP` | `KNB1` | `Boolean` |  | Pmnt advice by EDI |  |  |  |
| `PhysicalInventoryBlockInd` | `SPERB_B` | `SPERB_B` | `KNB1` | `Boolean` |  | Co.code post.block |  |  |  |
| `UserAtCustomer` | `DZSABE_D` | `DZSABE` | `KNB1` | `String(15)` |  | User at customer |  |  |  |
| `AccountingClerkPhoneNumber` | `TLFNS` | `TLFNS` | `KNB1` | `String(30)` |  | Acct.clerks tel.no. |  |  |  |
| `AccountingClerkFaxNumber` | `TLFXS` | `TLFXS` | `KNB1` | `String(31)` |  | Acctg clerk's fax |  |  |  |
| `AccountingClerkInternetAddress` | `INTAD` | `INTAD` | `KNB1` | `String(130)` |  | Clrk's internet add. |  |  |  |
| `AccountByCustomer` | `EIKTO_D` | `EIKTO` | `KNB1` | `String(12)` |  | Account at Customer |  |  |  |
| `IsToBeLocallyProcessed` | `XDEZV` | `XDEZV` | `KNB1` | `Boolean` |  | Local Processing |  |  |  |
| `CollectiveInvoiceVariant` | `PERKZ_KNB1` | `PERKZ_KNB1` | `KNB1` | `String(1)` |  | Coll.Invoice Variant |  |  |  |
| `LayoutSortingRule` | `DZUAWA` | `DZUAWA` | `KNB1` | `String(3)` |  | Sort key |  |  |  |
| `PaymentTerms` | `DZTERM` | `DZTERM` | `KNB1` | `String(4)` |  | Terms of Payment |  |  |  |
| `CustomerSupplierClearingIsUsed` | `XVERR_KNB1` | `XVERR_KNB1` | `KNB1` | `Boolean` |  | Clearing with vendor |  |  |  |
| `RecordPaymentHistoryIndicator` | `XZVER` | `XZVER` | `KNB1` | `Boolean` |  | Record Pmnt History |  |  |  |
| `PaymentMethodsList` | `DZWELS` | `DZWELS` | `KNB1` | `String(10)` |  | Payment Methods |  |  |  |
| `DeletionIndicator` | `LOEVM_B` | `LOEVM_B` | `KNB1` | `Boolean` |  | Co.Cde Deletion Flag |  |  |  |
| `CreditMemoPaymentTerms` | `GUZTE` | `GUZTE` | `KNB1` | `String(4)` |  | Credit Memo Pyt Term |  |  |  |
| `DunningNoticeGroup` | `MGRUP` | `MGRUP` | `KNB1` | `String(2)` |  | Grouping Key |  |  |  |
| `LastInterestCalcRunDate` | `DATLZ` | `DATLZ` | `KNB1` | `Date` |  | Last Int. Calc. |  |  |  |
| `CustPreviousMasterRecordNumber` | `ALTKN` | `ALTKN` | `KNB1` | `String(10)` |  | Previous Account No. |  |  |  |
| `ValueAdjustmentKey` | `WBRSL` | `WBRSL` | `KNB1` | `String(2)` |  | Value Adjustment |  |  |  |
| `CashPlanningGroup` | `FDGRV` | `FDGRV` | `KNB1` | `String(10)` |  | Planning Group |  | _CashPlanningGroup |  |
| `SupplierReleaseGroup` | `FRGRP` | `FRGRP` | `KNB1` | `String(4)` |  | Release Group |  |  |  |
| `PersonnelNumber` | `PERNR_D` | `PERNR` | `KNB1` | `String(8)` |  | Personnel Number |  |  |  |
| `BuyingGroupAccountNumber` | `EKVBD` | `EKVBD` | `KNB1` | `String(10)` |  | Buying Group |  |  |  |
| `BillExchChargePaymentTerms` | `WAKON` | `WAKON` | `KNB1` | `String(4)` |  | B/Ex. Charges Terms |  |  |  |
| `CheckPaidDurationInDays` | `KULTG` | `KULTG` | `KNB1` | `Decimal(3,0)` |  | Check Cashing Time |  |  |  |
| `CustomerPaymentBlockingReason` | `DZAHLS` | `DZAHLS` | `KNB1` | `String(1)` |  | Payment Block |  |  |  |
| `PaymentMethodSupplement` | `UZAWE` | `UZAWE` | `KNB1` | `String(2)` |  | Pmt Meth. Supplement |  |  |  |
| `AcctsReceivablePledgingCode` | `CESSION_KZ` | `CESSION_KZ` | `KNB1` | `String(2)` |  | AR Pledging Ind. |  |  |  |
| `LockboxInternalID` | `LOCKB` | `LOCKB` | `KNB1` | `String(7)` |  | Lockbox |  |  |  |
| `IsBusinessPurposeCompleted` |  |  |  | `Boolean` |  | Purpose Completed |  |  |  |
| `WithholdingTaxCountry` | `QLAND` | `QLAND` | `KNB1` | `String(3)` |  | WTax C/R Key |  |  |  |
| `KnownOrNegotiatedLeave` | `URLID` | `URLID` | `KNB1` | `String(4)` |  | Known/Negotiat.Leave |  |  |  |
| `DeletionIsBlocked` | `NODEL_B` | `NODEL_B` | `KNB1` | `Boolean` |  | CoCd Deletion Block |  |  |  |
| `PaymentClearingGroup` | `FAR_PAYMENT_CLEARING_GROUP` | `FAR_PAYMENT_CLEARING_GROUP` | `KNB1` | `String(8)` |  | Payment Clrg Grp ID |  |  |  |
| `PaymentReason` | `FARP_PAYT_RSN` | `PAYT_RSN` | `KNB1` | `String(4)` |  | Payment Reason |  |  |  |
| `BPPeriodicAccountStatement` | `XAUSZ` | `XAUSZ` | `KNB1` | `String(1)` |  | Account Statement |  |  |  |
| `US_FrgnAcctTaxRcpntCntry` | `LAND1` | `LAND1` | `KNB1` | `String(3)` |  | Country/Region Key |  |  |  |
| `US_GlobIntermediaryIdnNumber` | `FIWTUS_RECIPIENT_GIIN` | `FIWTUS_RECIPIENT_GIIN` | `KNB1` | `String(19)` |  | US Recipient GIIN |  |  |  |
| `US_RecipientForeignTaxID` | `FIWTUS_RECIPIENT_FTID` | `FIWTUS_RECIPIENT_FTID` | `KNB1` | `String(22)` |  | US Recipient FTID |  |  |  |
| `US_LobTreatyCode` | `FIWTUS_LOB_CODE` | `FIWTUS_LOB_CODE` | `KNB1` | `String(2)` |  | LOB Treaty Code |  |  |  |
| `US_FW8BENReceiveDate` | `FIWTUS_W8_RECV_DATE` | `FIWTUS_W8_RECV_DATE` | `KNB1` | `Date` |  | W8 Form Rec Date |  |  |  |
| `US_FW9ReceiveDate` | `FIWTUS_W9_RECV_DATE` | `FIWTUS_W9_RECV_DATE` | `KNB1` | `Date` |  | W9 Form Rec Date |  |  |  |
| `US_SecondTINNoticeIsIssued` | `FIWTUS_SECOND_TIN_NOTICE` | `FIWTUS_SECOND_TIN_NOTICE` | `KNB1` | `String(1)` |  | Second TIN Notice |  |  |  |
| `US_FrgnRecipientHasPartnership` | `FIWTUS_PARTNERSHIP_IND` | `FIWTUS_PARTNERSHIP_IND` | `KNB1` | `String(1)` |  | Partnership Int Ind |  |  |  |
| `US_FrgnAcctTaxFilingIsRequired` | `FIWTUS_FATCA_IND` | `FIWTUS_FATCA_IND` | `KNB1` | `String(1)` |  | FATCA Ind |  |  |  |
| `US_Chapter4StatusCode` | `FIWTUS_CHAP4_STATUS_CODE` | `FIWTUS_CHAP4_STATUS_CODE` | `KNB1` | `String(2)` |  | Chaptr 4 Status Code |  |  |  |
| `LastDunnedOn` | `MADAT` | `MADAT` | `KNB1` | `Date` |  | Last Dunned |  |  |  |
| `DunningProcedure` | `MAHNA` | `MAHNA` | `KNB1` | `String(4)` |  | Dunning Procedure |  |  |  |
| `DunningLevel` | `MAHNS_D` | `MAHNS` | `KNB1` | `String(1)` |  | Dunning Level |  |  |  |
| `DunningBlock` | `MANSP` | `MANSP` | `KNB1` | `String(1)` |  | Dunning Block |  |  |  |
| `DunningRecipient` | `KNRMA` | `KNRMA` | `KNB1` | `String(10)` |  | Dunning Recipient |  |  |  |
| `LegDunningProcedureOn` | `GMVDT` | `GMVDT` | `KNB1` | `Date` |  | Legal Dunn.Proc.From |  |  |  |
| `IsActiveEntity` | `SDRAFT_IS_ACTIVE` | `SDRAFT_IS_ACTIVE` | `KNB1` | `Boolean` |  | Is active |  |  |  |


## Entity: `CustomerDunning`

- **ABAP Name:** `I_CustomerDunning`
- **Label:** Customer Company Code Dunning Fields
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `CompanyCode` | `BUKRS` | `BUKRS` |  | `String(4)` | Y | Company Code |  | _CustomerCompany | S/4 only entity — no ECC CDC mapping |
| `Customer` | `KUNNR` | `KUNNR` |  | `String(10)` | Y | Customer |  | _Customer | S/4 only entity — no ECC CDC mapping |
| `DunningArea` | `MABER` | `MABER` |  | `String(2)` | Y | Dunning Area |  |  | S/4 only entity — no ECC CDC mapping |
| `LastDunnedOn` | `MADAT` | `MADAT` |  | `Date` |  | Last Dunned |  |  | S/4 only entity — no ECC CDC mapping |
| `DunningProcedure` | `MAHNA` | `MAHNA` |  | `String(4)` |  | Dunning Procedure |  | _DunningProcedure | S/4 only entity — no ECC CDC mapping |
| `DunningLevel` | `MAHNS_D` | `MAHNS` |  | `String(1)` |  | Dunning Level |  |  | S/4 only entity — no ECC CDC mapping |
| `DunningBlock` | `MANSP` | `MANSP` |  | `String(1)` |  | Dunning Block |  | _DunningBlock | S/4 only entity — no ECC CDC mapping |
| `DunningRecipient` | `KNRMA` | `KNRMA` |  | `String(10)` |  | Dunning Recipient |  | _DunningRecipient | S/4 only entity — no ECC CDC mapping |
| `LegDunningProcedureOn` | `GMVDT` | `GMVDT` |  | `Date` |  | Legal Dunn.Proc.From |  |  | S/4 only entity — no ECC CDC mapping |
| `DunningClerk` | `BUSAB_MA` | `BUSAB_MA` |  | `String(2)` |  | Dunning Clerk |  | _DunningClerk | S/4 only entity — no ECC CDC mapping |


## Entity: `CustomerSalesArea`

- **ABAP Name:** `I_CustomerSalesArea`
- **Label:** Customer Sales Area
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Customer` | `KUNNR` | `KUNNR` |  | `String(10)` | Y | Customer |  | _Customer | S/4 only entity — no ECC CDC mapping |
| `SalesOrganization` | `VKORG` | `VKORG` |  | `String(4)` | Y | Sales Organization |  | _SalesOrganization | S/4 only entity — no ECC CDC mapping |
| `DistributionChannel` | `VTWEG` | `VTWEG` |  | `String(2)` | Y | Distribution Channel |  | _DistributionChannel | S/4 only entity — no ECC CDC mapping |
| `Division` | `SPART` | `SPART` |  | `String(2)` | Y | Division |  | _Division | S/4 only entity — no ECC CDC mapping |
| `CustomerABCClassification` | `KLABC` | `KLABC` |  | `String(2)` |  | ABC Classification |  |  | S/4 only entity — no ECC CDC mapping |
| `SalesOffice` | `VKBUR` | `VKBUR` |  | `String(4)` |  | Sales Office |  | _SalesOffice | S/4 only entity — no ECC CDC mapping |
| `SalesGroup` | `VKGRP` | `VKGRP` |  | `String(3)` |  | Sales Group |  | _SalesGroup | S/4 only entity — no ECC CDC mapping |
| `OrderIsBlockedForCustomer` | `AUFSD_V` | `AUFSD_V` |  | `String(2)` |  | Ord.blk:sls ar. |  |  | S/4 only entity — no ECC CDC mapping |
| `Currency` | `WAERS_V02D` | `WAERS_V02D` |  | `String(5)` |  | Currency |  | _Currency | S/4 only entity — no ECC CDC mapping |
| `CustomerPriceGroup` | `KONDA` | `KONDA` |  | `String(2)` |  | Customer Price Group |  |  | S/4 only entity — no ECC CDC mapping |
| `PriceListType` | `PLTYP` | `PLTYP` |  | `String(2)` |  | Price List Type |  |  | S/4 only entity — no ECC CDC mapping |
| `DeliveryPriority` | `LPRIO` | `LPRIO` |  | `String(2)` |  | Delivery Priority |  | _DeliveryPriority | S/4 only entity — no ECC CDC mapping |
| `ShippingCondition` | `VSBED` | `VSBED` |  | `String(2)` |  | Shipping Conditions |  | _ShippingCondition | S/4 only entity — no ECC CDC mapping |
| `IncotermsClassification` | `INCO1` | `INCO1` |  | `String(3)` |  | Incoterms |  | _IncotermsClassification | S/4 only entity — no ECC CDC mapping |
| `SupplyingPlant` | `DWERK_EXT` | `DWERK_EXT` |  | `String(4)` |  | Delivering Plant |  | _SupplyingPlant | S/4 only entity — no ECC CDC mapping |
| `CompleteDeliveryIsDefined` | `AUTLF` | `AUTLF` |  | `Boolean` |  | Complete Delivery |  |  | S/4 only entity — no ECC CDC mapping |
| `DeliveryIsBlockedForCustomer` | `LIFSD_V` | `LIFSD_V` |  | `String(2)` |  | DelBlckSalesAr. |  | _DeliveryIsBlockedForCustomer | S/4 only entity — no ECC CDC mapping |
| `BillingIsBlockedForCustomer` | `FAKSD_V` | `FAKSD_V` |  | `String(2)` |  | BBlock for SlsA |  | _BillingIsBlockedForCustomer | S/4 only entity — no ECC CDC mapping |
| `CustomerPaymentTerms` | `DZTERM` | `DZTERM` |  | `String(4)` |  | Terms of Payment |  | _CustomerPaymentTerms | S/4 only entity — no ECC CDC mapping |
| `CustomerAccountAssignmentGroup` | `KTGRD` | `KTGRD` |  | `String(2)` |  | Acct Assmt Grp Cust. |  |  | S/4 only entity — no ECC CDC mapping |
| `AccountByCustomer` | `EIKTO` | `EIKTO` |  | `String(12)` |  | Account at Customer |  |  | S/4 only entity — no ECC CDC mapping |
| `CustomerGroup` | `KDGRP` | `KDGRP` |  | `String(2)` |  | Customer Group |  |  | S/4 only entity — no ECC CDC mapping |
| `CustomerPricingProcedure` | `KALKS` | `KALKS` |  | `String(2)` |  | Cust.Pric.Procedure |  |  | S/4 only entity — no ECC CDC mapping |
| `OrderCombinationIsAllowed` | `KZAZU_D` | `KZAZU` |  | `Boolean` |  | Order Combination |  |  | S/4 only entity — no ECC CDC mapping |
| `PartialDeliveryIsAllowed` | `KZTLF` | `KZTLF` |  | `String(1)` |  | Partial Deliv./Item |  |  | S/4 only entity — no ECC CDC mapping |
| `InvoiceDate` | `PERFK` | `PERFK` |  | `String(2)` |  | Invoicing Dates |  |  | S/4 only entity — no ECC CDC mapping |
| `PaymentTerms` | `DZTERM` | `DZTERM` |  | `String(4)` |  | Terms of Payment |  |  | S/4 only entity — no ECC CDC mapping |
| `IncotermsTransferLocation` | `INCO2` | `INCO2` |  | `String(28)` |  | Incoterms (Part 2) |  |  | S/4 only entity — no ECC CDC mapping |
| `ItemOrderProbabilityInPercent` | `AWAHR` | `AWAHR` |  | `String(3)` |  | Order Probability |  |  | S/4 only entity — no ECC CDC mapping |
| `IncotermsLocation2` | `INCO3_L` | `INCO3_L` |  | `String(70)` |  | Incoterms Location 2 |  |  | S/4 only entity — no ECC CDC mapping |
| `RecordCreatedDate` | `ERDAT` | `ERDAT` |  | `Date` |  | Created On |  |  | S/4 only entity — no ECC CDC mapping |
| `AuthorizationGroup` | `BEGRU` | `BEGRU` |  | `String(4)` |  | Authorization Group |  |  | S/4 only entity — no ECC CDC mapping |
| `SalesDistrict` | `BZIRK` | `BZIRK` |  | `String(6)` |  | Sales District |  |  | S/4 only entity — no ECC CDC mapping |
| `IncotermsVersion` | `INCOV` | `INCOV` |  | `String(4)` |  | Incoterms Version |  |  | S/4 only entity — no ECC CDC mapping |
| `IncotermsLocation1` | `INCO2_L` | `INCO2_L` |  | `String(70)` |  | Incoterms Location 1 |  |  | S/4 only entity — no ECC CDC mapping |
| `DeletionIndicator` | `LOEVM_V` | `LOEVM_V` |  | `Boolean` |  | Del.ID SlsArea |  |  | S/4 only entity — no ECC CDC mapping |
| `IsBusinessPurposeCompleted` |  |  |  | `Boolean` |  | Purpose Completed |  |  | S/4 only entity — no ECC CDC mapping |
| `SalesItemProposal` | `VSORT` | `VSORT` |  | `String(10)` |  | Item proposal |  |  | S/4 only entity — no ECC CDC mapping |
| `CustProdProposalProcedure` | `PVKSM` | `PVKSM` |  | `String(2)` |  | PP customer proced. |  | _CustProdProposalProcedure | S/4 only entity — no ECC CDC mapping |
| `ProofOfDeliveryTime` |  |  |  | `String(6)` |  |  |  |  | S/4 only entity — no ECC CDC mapping |
| `ProofOfDeliveryTimeValue` | `CUST_POD` | `CUST_POD` |  | `Decimal(6,2)` |  | POD timeframe |  |  | S/4 only entity — no ECC CDC mapping |
| `MaxNmbrOfPartialDelivery` | `ANTLF` | `ANTLF` |  | `Decimal(1,0)` |  | Max.Part.Deliveries |  |  | S/4 only entity — no ECC CDC mapping |
| `UnderdelivTolrtdLmtRatioInPct` | `UNTTO` | `UNTTO` |  | `Decimal(3,1)` |  | Underdel. Tolerance |  |  | S/4 only entity — no ECC CDC mapping |
| `OverdelivTolrtdLmtRatioInPct` | `UEBTO` | `UEBTO` |  | `Decimal(3,1)` |  | Overdeliv. Tolerance |  |  | S/4 only entity — no ECC CDC mapping |
| `IsActiveEntity` | `SDRAFT_IS_ACTIVE` | `SDRAFT_IS_ACTIVE` |  | `Boolean` |  | Is active |  |  | S/4 only entity — no ECC CDC mapping |
| `AdditionalCustomerGroup1` | `KVGR1` | `KVGR1` |  | `String(3)` |  | Customer Group 1 |  |  | S/4 only entity — no ECC CDC mapping |
| `AdditionalCustomerGroup2` | `KVGR2` | `KVGR2` |  | `String(3)` |  | Customer Group 2 |  |  | S/4 only entity — no ECC CDC mapping |
| `AdditionalCustomerGroup3` | `KVGR3` | `KVGR3` |  | `String(3)` |  | Customer Group 3 |  |  | S/4 only entity — no ECC CDC mapping |
| `AdditionalCustomerGroup4` | `KVGR4` | `KVGR4` |  | `String(3)` |  | Customer Group 4 |  |  | S/4 only entity — no ECC CDC mapping |
| `AdditionalCustomerGroup5` | `KVGR5` | `KVGR5` |  | `String(3)` |  | Customer Group 5 |  |  | S/4 only entity — no ECC CDC mapping |
| `InvoiceListSchedule` | `PERRL` | `PERRL` |  | `String(2)` |  | Invoice List Sched. |  | _FactoryCalendar | S/4 only entity — no ECC CDC mapping |
| `ExchangeRateType` | `KURST` | `KURST` |  | `String(4)` |  | Exchange Rate Type |  | _ExchangeRateType | S/4 only entity — no ECC CDC mapping |
| `PaymentGuaranteeProcedure` | `KABSSCH_CM` | `KABSSCH_CM` |  | `String(4)` |  | Paymt guarant. proc. |  | _PaytGuarProcedVH | S/4 only entity — no ECC CDC mapping |
| `SuplrIsRlvtForSettlmtMgmt` | `AGREL` | `AGREL` |  | `Boolean` |  | Settlement Mgmt. |  |  | S/4 only entity — no ECC CDC mapping |
| `CustIsRlvtForSettlmtMgmt` | `AGREL` | `AGREL` |  | `Boolean` |  | Settlement Mgmt. |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductUnitGroup` | `MEGRU` | `MEGRU` |  | `String(4)` |  | Unit of Measure Grp |  |  | S/4 only entity — no ECC CDC mapping |
| `SlsDocIsRlvtForProofOfDeliv` | `PODKZ` | `PODKZ` |  | `Boolean` |  | Relevant for POD |  |  | S/4 only entity — no ECC CDC mapping |
| `SlsUnlmtdOvrdelivIsAllwd` | `UEBTK_V` | `UEBTK_V` |  | `Boolean` |  | Unlimited Tolerance |  |  | S/4 only entity — no ECC CDC mapping |
| `CreditControlArea` | `KKBER` | `KKBER` |  | `String(4)` |  | Credit Control Area |  |  | S/4 only entity — no ECC CDC mapping |
| `CustomerIsRebateRelevant` | `BOKRE` | `BOKRE` |  | `Boolean` |  | Rebate |  |  | S/4 only entity — no ECC CDC mapping |
| `InspSbstHasNoTimeOrQuantity` | `PRFRE` | `PRFRE` |  | `Boolean` |  | Price determination |  |  | S/4 only entity — no ECC CDC mapping |
| `ManualInvoiceMaintIsRelevant` | `MRNKZ` | `MRNKZ` |  | `Boolean` |  | Man. Invoice Maint. |  |  | S/4 only entity — no ECC CDC mapping |
| `IncotermsSupChnLoc1AddlUUID` |  |  |  | `UUID` |  | Location UUID |  |  | S/4 only entity — no ECC CDC mapping |
| `IncotermsSupChnLoc2AddlUUID` |  |  |  | `UUID` |  | Location UUID |  |  | S/4 only entity — no ECC CDC mapping |
| `IncotermsSupChnDvtgLocAddlUUID` |  |  |  | `UUID` |  | Location UUID |  |  | S/4 only entity — no ECC CDC mapping |
| `SalesBlockForCustomer` | `CASSD_V` | `CASSD_V` |  | `String(2)` |  | Sales Block |  |  | S/4 only entity — no ECC CDC mapping |
| `CustomerStatisticsGroup` | `STGKU` | `STGKU` |  | `String(1)` |  | Customer Stats.Group |  |  | S/4 only entity — no ECC CDC mapping |
| `RetailAdditionalCustomerGrp6` | `FSH_KVGR6` | `FSH_KVGR6` |  | `String(3)` |  | Customer Group 6 |  |  | S/4 only entity — no ECC CDC mapping |
| `RetailAdditionalCustomerGrp7` | `FSH_KVGR7` | `FSH_KVGR7` |  | `String(3)` |  | Customer Group 7 |  |  | S/4 only entity — no ECC CDC mapping |
| `RetailAdditionalCustomerGrp8` | `FSH_KVGR8` | `FSH_KVGR8` |  | `String(3)` |  | Customer Group 8 |  |  | S/4 only entity — no ECC CDC mapping |
| `RetailAdditionalCustomerGrp9` | `FSH_KVGR9` | `FSH_KVGR9` |  | `String(3)` |  | Customer Group 9 |  |  | S/4 only entity — no ECC CDC mapping |
| `RetailAdditionalCustomerGrp10` | `FSH_KVGR10` | `FSH_KVGR10` |  | `String(3)` |  | Customer Group 10 |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `CustomerSalesAreaTax`

- **ABAP Name:** `I_CustSalesAreaTax`
- **Label:** Customer Sales Area Tax
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Customer` | `KUNNR` | `KUNNR` |  | `String(10)` | Y | Customer |  | _Customer | S/4 only entity — no ECC CDC mapping |
| `SalesOrganization` | `VKORG` | `VKORG` |  | `String(4)` | Y | Sales Organization |  | _SalesOrganization | S/4 only entity — no ECC CDC mapping |
| `DistributionChannel` | `VTWKU` | `VTWKU` |  | `String(2)` | Y | RefDistCh-Cust/Mat. |  | _DistributionChannel | S/4 only entity — no ECC CDC mapping |
| `Division` | `SPART` | `SPART` |  | `String(2)` | Y | Division |  | _Division | S/4 only entity — no ECC CDC mapping |
| `DepartureCountry` | `ALAND` | `ALAND` |  | `String(3)` | Y | Departure Ctry/Reg. |  | _Country | S/4 only entity — no ECC CDC mapping |
| `CustomerTaxCategory` | `TATYP` | `TATYP` |  | `String(4)` | Y | Tax Condition Type |  |  | S/4 only entity — no ECC CDC mapping |
| `CustomerTaxClassification` | `TAKLD` | `TAKLD` |  | `String(1)` |  | Tax Classification |  |  | S/4 only entity — no ECC CDC mapping |
| `AuthorizationGroup` | `BRGRU` | `BRGRU` |  | `String(4)` |  | Authorization |  |  | S/4 only entity — no ECC CDC mapping |
| `IsBusinessPurposeCompleted` |  |  |  | `Boolean` |  | Purpose Completed |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `CustomerUnloadingPoint`

- **ABAP Name:** `I_CustomerUnloadingPoint`
- **Label:** Customer Unloading Point
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Customer` | `KUNNR` | `KUNNR` |  | `String(10)` | Y | Customer |  | _Customer | S/4 only entity — no ECC CDC mapping |
| `UnloadingPointName` | `ABLAD` | `ABLAD` |  | `String(25)` | Y | Unloading Point |  |  | S/4 only entity — no ECC CDC mapping |
| `CustomerFactoryCalenderCode` | `KNKAL` | `KNKAL` |  | `String(2)` |  | Cust.fact.calendar |  |  | S/4 only entity — no ECC CDC mapping |
| `BPGoodsReceivingHoursCode` | `WANID` | `WANID` |  | `String(3)` |  | Goods receiving hrs |  |  | S/4 only entity — no ECC CDC mapping |
| `IsDfltBPUnloadingPoint` | `DEFAB` | `DEFAB` |  | `Boolean` |  | Default unloading pt |  |  | S/4 only entity — no ECC CDC mapping |
| `MondayMorningOpeningTime` | `WAMOAB1` | `WAMOAB1` |  | `String(6)` |  | Monday |  |  | S/4 only entity — no ECC CDC mapping |
| `MondayMorningClosingTime` | `WAMOBI1` | `WAMOBI1` |  | `String(6)` |  | Monday |  |  | S/4 only entity — no ECC CDC mapping |
| `MondayAfternoonOpeningTime` | `WAMOAB2` | `WAMOAB2` |  | `String(6)` |  | Monday |  |  | S/4 only entity — no ECC CDC mapping |
| `MondayAfternoonClosingTime` | `WAMOBI2` | `WAMOBI2` |  | `String(6)` |  | Monday |  |  | S/4 only entity — no ECC CDC mapping |
| `TuesdayMorningOpeningTime` | `WADIAB1` | `WADIAB1` |  | `String(6)` |  | Tuesday |  |  | S/4 only entity — no ECC CDC mapping |
| `TuesdayMorningClosingTime` | `WADIBI1` | `WADIBI1` |  | `String(6)` |  | Tuesday |  |  | S/4 only entity — no ECC CDC mapping |
| `TuesdayAfternoonOpeningTime` | `WADIAB2` | `WADIAB2` |  | `String(6)` |  | Tuesday |  |  | S/4 only entity — no ECC CDC mapping |
| `TuesdayAfternoonClosingTime` | `WADIBI2` | `WADIBI2` |  | `String(6)` |  | Tuesday |  |  | S/4 only entity — no ECC CDC mapping |
| `WednesdayMorningOpeningTime` | `WAMIAB1` | `WAMIAB1` |  | `String(6)` |  | Wednesday |  |  | S/4 only entity — no ECC CDC mapping |
| `WednesdayMorningClosingTime` | `WAMIBI1` | `WAMIBI1` |  | `String(6)` |  | Wednesday |  |  | S/4 only entity — no ECC CDC mapping |
| `WednesdayAfternoonOpeningTime` | `WAMIAB2` | `WAMIAB2` |  | `String(6)` |  | Wednesday |  |  | S/4 only entity — no ECC CDC mapping |
| `WednesdayAfternoonClosingTime` | `WAMIBI2` | `WAMIBI2` |  | `String(6)` |  | Wednesday |  |  | S/4 only entity — no ECC CDC mapping |
| `ThursdayMorningOpeningTime` | `WADOAB1` | `WADOAB1` |  | `String(6)` |  | Thursday |  |  | S/4 only entity — no ECC CDC mapping |
| `ThursdayMorningClosingTime` | `WADOBI1` | `WADOBI1` |  | `String(6)` |  | Thursday |  |  | S/4 only entity — no ECC CDC mapping |
| `ThursdayAfternoonOpeningTime` | `WADOAB2` | `WADOAB2` |  | `String(6)` |  | Thursday |  |  | S/4 only entity — no ECC CDC mapping |
| `ThursdayAfternoonClosingTime` | `WADOBI2` | `WADOBI2` |  | `String(6)` |  | Thursday |  |  | S/4 only entity — no ECC CDC mapping |
| `FridayMorningOpeningTime` | `WAFRAB1` | `WAFRAB1` |  | `String(6)` |  | Friday |  |  | S/4 only entity — no ECC CDC mapping |
| `FridayMorningClosingTime` | `WAFRBI1` | `WAFRBI1` |  | `String(6)` |  | Friday |  |  | S/4 only entity — no ECC CDC mapping |
| `FridayAfternoonOpeningTime` | `WAFRAB2` | `WAFRAB2` |  | `String(6)` |  | Friday |  |  | S/4 only entity — no ECC CDC mapping |
| `FridayAfternoonClosingTime` | `WAFRBI2` | `WAFRBI2` |  | `String(6)` |  | Friday |  |  | S/4 only entity — no ECC CDC mapping |
| `SaturdayMorningOpeningTime` | `WASAAB1` | `WASAAB1` |  | `String(6)` |  | Saturday |  |  | S/4 only entity — no ECC CDC mapping |
| `SaturdayMorningClosingTime` | `WASABI1` | `WASABI1` |  | `String(6)` |  | Saturday |  |  | S/4 only entity — no ECC CDC mapping |
| `SaturdayAfternoonOpeningTime` | `WASAAB2` | `WASAAB2` |  | `String(6)` |  | Saturday |  |  | S/4 only entity — no ECC CDC mapping |
| `SaturdayAfternoonClosingTime` | `WASABI2` | `WASABI2` |  | `String(6)` |  | Saturday |  |  | S/4 only entity — no ECC CDC mapping |
| `SundayMorningOpeningTime` | `WASOAB1` | `WASOAB1` |  | `String(6)` |  | Sunday |  |  | S/4 only entity — no ECC CDC mapping |
| `SundayMorningClosingTime` | `WASOBI1` | `WASOBI1` |  | `String(6)` |  | Sunday |  |  | S/4 only entity — no ECC CDC mapping |
| `SundayAfternoonOpeningTime` | `WASOAB2` | `WASOAB2` |  | `String(6)` |  | Sunday |  |  | S/4 only entity — no ECC CDC mapping |
| `SundayAfternoonClosingTime` | `WASOBI2` | `WASOBI2` |  | `String(6)` |  | Sunday |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `CustomerWithHoldingTax`

- **ABAP Name:** `I_CustomerWithTax`
- **Label:** Customer WithHolding Tax
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Customer` | `KUNNR` | `KUNNR` |  | `String(10)` | Y | Customer |  | _Customer | S/4 only entity — no ECC CDC mapping |
| `CompanyCode` | `BUKRS` | `BUKRS` |  | `String(4)` | Y | Company Code |  | _CompanyCode | S/4 only entity — no ECC CDC mapping |
| `WithholdingTaxType` | `WITHT` | `WITHT` |  | `String(2)` | Y | Withholding Tax Type |  |  | S/4 only entity — no ECC CDC mapping |
| `WithholdingTaxCode` | `WT_WITHCD` | `WT_WITHCD` |  | `String(2)` |  | W/Tax Code |  |  | S/4 only entity — no ECC CDC mapping |
| `WithholdingTaxAgent` | `WT_WTAGT` | `WT_WTAGT` |  | `Boolean` |  | WTax Agent |  |  | S/4 only entity — no ECC CDC mapping |
| `ObligationDateBegin` | `WT_AGTDF` | `WT_AGTDF` |  | `Date` |  | W/Tax Obligated Frm |  |  | S/4 only entity — no ECC CDC mapping |
| `ObligationDateEnd` | `WT_AGTDT` | `WT_AGTDT` |  | `Date` |  | Oblig.to W/Tax Until |  |  | S/4 only entity — no ECC CDC mapping |
| `WithholdingTaxNumber` | `WT_WTSTCD` | `WT_WTSTCD` |  | `String(16)` |  | W/tax number |  |  | S/4 only entity — no ECC CDC mapping |
| `WithholdingTaxCertificate` | `WT_EXNR` | `WT_EXNR` |  | `String(25)` |  | Exemption Number |  |  | S/4 only entity — no ECC CDC mapping |
| `WithholdingTaxExmptPercent` | `WT_EXRT` | `WT_EXRT` |  | `Decimal(5,2)` |  | Exemption Rate |  |  | S/4 only entity — no ECC CDC mapping |
| `ExemptionDateBegin` | `WT_EXDF` | `WT_EXDF` |  | `Date` |  | Exemption Start Date |  |  | S/4 only entity — no ECC CDC mapping |
| `ExemptionDateEnd` | `WT_EXDT` | `WT_EXDT` |  | `Date` |  | Exemption End Date |  |  | S/4 only entity — no ECC CDC mapping |
| `ExemptionReason` | `WT_WTEXRS` | `WT_WTEXRS` |  | `String(2)` |  | Exemption Reason |  |  | S/4 only entity — no ECC CDC mapping |
