# Customer

> Source file: `sap-s4com-Customer-v1.json`

**Technical Name:** `` | **Data Category:** `DIMENSION` | **VDM Type:** `BASIC` | **Size:** `XL`


## Entity: `Customer`

- **ABAP Name:** `I_Customer`
- **Label:** Customer
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** ADRC, KNA1

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `Customer` | `KNA1` | `KUNNR` | `String(10)` | Y | Customer |  |  |  |
| `CustomerName` |  |  | `String(80)` |  | Name of Customer |  |  |  |
| `CustomerFullName` | `KNA1` | `NAME1` | `String(220)` |  | Customer Name |  |  |  |
| `BPCustomerName` |  |  | `String(81)` |  | Business Partner - Customer Name |  |  |  |
| `BPCustomerFullName` |  |  | `String(220)` |  | Business Partner - Customer Full Name |  |  |  |
| `CreatedByUser` |  |  | `String(12)` |  | Created by |  |  |  |
| `CreationDate` |  |  | `Date` |  | Created On |  |  |  |
| `AddressID` |  |  | `String(10)` |  | Address |  |  |  |
| `CustomerClassification` |  |  | `String(2)` |  | Customer Classific. |  | _CustomerClassification |  |
| `VATRegistration` |  |  | `String(20)` |  | VAT Registration No. |  |  |  |
| `CustomerAccountGroup` | `KNA1` | `KTOKD` | `String(4)` |  | Account Group |  |  |  |
| `AuthorizationGroup` |  |  | `String(4)` |  | Authorization |  |  |  |
| `DeliveryIsBlocked` |  |  | `String(2)` |  | Delivery block |  |  |  |
| `PostingIsBlocked` |  |  | `Boolean` |  | Posting Block |  |  |  |
| `BillingIsBlockedForCustomer` |  |  | `String(2)` |  | Billing Block |  |  |  |
| `OrderIsBlockedForCustomer` |  |  | `String(2)` |  | Order Block |  |  |  |
| `InternationalLocationNumber1` |  |  | `String(7)` |  | Int. location no. 1 |  |  |  |
| `IsOneTimeAccount` |  |  | `Boolean` |  | One-Time Account |  |  |  |
| `TaxJurisdiction` |  |  | `String(15)` |  | Tax Jurisdiction |  |  |  |
| `Industry` |  |  | `String(4)` |  | Industry |  |  |  |
| `TaxNumberType` |  |  | `String(2)` |  | Tax Number Type |  |  |  |
| `TaxNumber1` |  |  | `String(16)` |  | Tax Number 1 |  |  |  |
| `TaxNumber2` |  |  | `String(11)` |  | Tax Number 2 |  |  |  |
| `TaxNumber3` |  |  | `String(18)` |  | Tax Number 3 |  |  |  |
| `TaxNumber4` |  |  | `String(18)` |  | Tax Number 4 |  |  |  |
| `TaxNumber5` |  |  | `String(60)` |  | Tax Number 5 |  |  |  |
| `TaxNumber6` |  |  | `String(20)` |  | Tax Number 6 |  |  |  |
| `CustomerCorporateGroup` |  |  | `String(10)` |  | Group Key |  |  |  |
| `Supplier` |  |  | `String(10)` |  | Supplier |  |  |  |
| `NielsenRegion` |  |  | `String(2)` |  | Nielsen Indicator |  |  |  |
| `IndustryCode1` |  |  | `String(10)` |  | Industry Code 1 |  |  |  |
| `IndustryCode2` |  |  | `String(10)` |  | Industry Code 2 |  |  |  |
| `IndustryCode3` |  |  | `String(10)` |  | Industry Code 3 |  |  |  |
| `IndustryCode4` |  |  | `String(10)` |  | Industry Code 4 |  |  |  |
| `IndustryCode5` |  |  | `String(10)` |  | Industry Code 5 |  |  |  |
| `Country` | `KNA1` | `LAND1` | `String(3)` |  | Country/Region Key |  |  |  |
| `OrganizationBPName1` |  |  | `String(35)` |  | Name |  |  |  |
| `OrganizationBPName2` |  |  | `String(35)` |  | Name 2 |  |  |  |
| `CityName` | `KNA1` | `ORT01` | `String(35)` |  | City |  |  |  |
| `PostalCode` | `KNA1` | `PSTLZ` | `String(10)` |  | Postal Code |  |  |  |
| `StreetName` | `KNA1` | `STRAS` | `String(35)` |  | Street |  |  |  |
| `SortField` |  |  | `String(10)` |  | Search Term |  |  |  |
| `FaxNumber` |  |  | `String(31)` |  | Fax Number |  |  |  |
| `BR_SUFRAMACode` |  |  | `String(9)` |  | Suframa Code |  |  |  |
| `Region` | `KNA1` | `REGIO` | `String(3)` |  | Region |  |  |  |
| `TelephoneNumber1` |  |  | `String(16)` |  | Telephone 1 |  |  |  |
| `TelephoneNumber2` |  |  | `String(16)` |  | Telephone 2 |  |  |  |
| `AlternativePayerAccount` |  |  | `String(10)` |  | Alternative Payer |  |  |  |
| `DataMediumExchangeIndicator` |  |  | `String(1)` |  | DME Recipient Code |  |  |  |
| `VATLiability` |  |  | `Boolean` |  | Liable for VAT |  |  |  |
| `IsBusinessPurposeCompleted` |  |  | `Boolean` |  | Purpose Completed |  |  |  |
| `ResponsibleType` |  |  | `String(2)` |  | Tax Type |  |  |  |
| `FiscalAddress` |  |  | `String(10)` |  | Fiscal address |  |  |  |
| `NFPartnerIsNaturalPerson` |  |  | `Boolean` |  | Natural Person |  |  |  |
| `DeletionIndicator` |  |  | `Boolean` |  | Deletion Flag |  |  |  |
| `Language` | `KNA1` | `SPRAS` | `String(2)` |  | Language Key |  |  |  |
| `TradingPartner` |  |  | `String(6)` |  | Trading Partner No. |  | _GlobalCompany |  |
| `DeliveryDateTypeRule` |  |  | `String(1)` |  | Deliv Date Rule |  |  |  |
| `ExpressTrainStationName` |  |  | `String(25)` |  | Express station |  |  |  |
| `TrainStationName` |  |  | `String(25)` |  | Train station |  |  |  |
| `InternationalLocationNumber2` |  |  | `String(5)` |  | Int. location no. 2 |  |  |  |
| `InternationalLocationNumber3` |  |  | `String(1)` |  | Check digit |  |  |  |
| `CityCode` |  |  | `String(4)` |  | City Code |  |  |  |
| `County` |  |  | `String(3)` |  | County Code |  |  |  |
| `CustomerHasUnloadingPoint` |  |  | `Boolean` |  | Unloading points |  |  |  |
| `CustomerWorkingTimeCalendar` |  |  | `String(2)` |  | Working times |  |  |  |
| `IsCompetitor` |  |  | `Boolean` |  | Competitors |  |  |  |
| `TaxInvoiceRepresentativeName` |  |  | `String(10)` |  | Rep's Name |  |  |  |
| `BusinessType` |  |  | `String(30)` |  | Type of Business |  |  |  |
| `IndustryType` |  |  | `String(30)` |  | Type of Industry |  |  |  |
| `TW_CollvBillingIsSupported` |  |  | `Boolean` |  | Consolidated Invoic. |  |  |  |
| `AlternativePayeeIsAllowed` |  |  | `Boolean` |  | Alt.payer in doc? |  |  |  |
| `FreeDefinedAttribute01` |  |  | `String(2)` |  | Attribute 1 |  |  |  |
| `FreeDefinedAttribute02` |  |  | `String(2)` |  | Attribute 2 |  |  |  |
| `FreeDefinedAttribute03` |  |  | `String(2)` |  | Attribute 3 |  |  |  |
| `FreeDefinedAttribute04` |  |  | `String(2)` |  | Attribute 4 |  |  |  |
| `FreeDefinedAttribute05` |  |  | `String(2)` |  | Attribute 5 |  |  |  |
| `FreeDefinedAttribute06` |  |  | `String(3)` |  | Attribute 6 |  |  |  |
| `FreeDefinedAttribute07` |  |  | `String(3)` |  | Attribute 7 |  |  |  |
| `FreeDefinedAttribute08` |  |  | `String(3)` |  | Attribute 8 |  |  |  |
| `FreeDefinedAttribute09` |  |  | `String(3)` |  | Attribute 9 |  |  |  |
| `FreeDefinedAttribute10` |  |  | `String(3)` |  | Attribute 10 |  |  |  |
| `PaymentReason` |  |  | `String(4)` |  | Payment Reason |  |  |  |
| `CustomerConditionGroup1` |  |  | `String(2)` |  | Condition Group 1 |  |  |  |
| `CustomerConditionGroup2` |  |  | `String(2)` |  | Condition Group 2 |  |  |  |
| `CustomerConditionGroup3` |  |  | `String(2)` |  | Condition Group 3 |  |  |  |
| `CustomerConditionGroup4` |  |  | `String(2)` |  | Condition Group 4 |  |  |  |
| `CustomerConditionGroup5` |  |  | `String(2)` |  | Condition Group 5 |  |  |  |
| `IsSalesProspect` |  |  | `Boolean` |  | Prospect |  |  |  |
| `PaymentIsBlockedForCustomer` |  |  | `Boolean` |  | Payment block |  |  |  |
| `IsConsumer` |  |  | `Boolean` |  | Consumer |  |  |  |
| `DataControllerSet` |  |  | `String(1)` |  | Data Ctrlr. Set |  |  |  |
| `DataController1` |  |  | `String(30)` |  | Data Controller |  |  |  |
| `DataController2` |  |  | `String(30)` |  | Data Controller |  |  |  |
| `DataController3` |  |  | `String(30)` |  | Data Controller |  |  |  |
| `DataController4` |  |  | `String(30)` |  | Data Controller |  |  |  |
| `DataController5` |  |  | `String(30)` |  | Data Controller |  |  |  |
| `DataController6` |  |  | `String(30)` |  | Data Controller |  |  |  |
| `DataController7` |  |  | `String(30)` |  | Data Controller |  |  |  |
| `DataController8` |  |  | `String(30)` |  | Data Controller |  |  |  |
| `DataController9` |  |  | `String(30)` |  | Data Controller |  |  |  |
| `DataController10` |  |  | `String(30)` |  | Data Controller |  |  |  |
| `BusinessPartnerName1` |  |  | `String(40)` |  | Business Partner Organization  - Name 1 |  |  |  |
| `BusinessPartnerName2` |  |  | `String(40)` |  | Business Partner Organization  - Name 2 |  |  |  |
| `BusinessPartnerName3` |  |  | `String(40)` |  | Business Partner Organization  - Name 3 |  |  |  |
| `BusinessPartnerName4` |  |  | `String(40)` |  | Business Partner Organization  - Name 4 |  |  |  |
| `BPAddrCityName` |  |  | `String(40)` |  | Business Partner Address – City |  |  |  |
| `BPAddrStreetName` |  |  | `String(60)` |  | Business Partner Address – Street |  |  |  |
| `AddressSearchTerm1` |  |  | `String(20)` |  | Business Partner Address - Search Term 1 |  |  |  |
| `AddressSearchTerm2` |  |  | `String(20)` |  | Business Partner Address - Search Term 2 |  |  |  |
| `DistrictName` |  |  | `String(40)` |  | Business Partner Address – District |  |  |  |
| `POBoxDeviatingCityName` |  |  | `String(40)` |  | Business Partner Address - PO Box Deviating City |  |  |  |
| `BusinessPartnerFormOfAddress` |  |  | `String(4)` |  | Business Partner - Form of Address |  |  |  |
| `BR_ICMSTaxPayerType` |  |  | `String(2)` |  | ICMS Taxpayer |  |  |  |


## Entity: `CustomerCompanyCode`

- **ABAP Name:** `I_CustomerCompany`
- **Label:** Customer Company
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** KNB5, KNB1

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `Customer` | `KNA1` | `KUNNR` | `String(10)` | Y | Customer |  | _Customer |  |
| `CompanyCode` | `KNB1` | `BUKRS` | `String(4)` | Y | Company Code |  |  |  |
| `AccountingClerk` |  |  | `String(2)` |  | Clerk Abbrev. |  |  |  |
| `ReconciliationAccount` | `KNB1` | `AKONT` | `String(10)` |  | Reconciliation Acct |  |  |  |
| `AuthorizationGroup` |  |  | `String(4)` |  | Authorization |  |  |  |
| `CustomerHeadOffice` |  |  | `String(10)` |  | Head Office |  |  |  |
| `AlternativePayerAccount` |  |  | `String(10)` |  | Alternative payer |  |  |  |
| `PaymentBlockingReason` | `KNB1` | `ZAHLS` | `String(1)` |  | Payment Block |  | _PaymentBlockValueHelp |  |
| `InterestCalculationCode` |  |  | `String(2)` |  | Interest Indicator |  |  |  |
| `InterestCalculationDate` |  |  | `Date` |  | Last Key Date |  |  |  |
| `IntrstCalcFrequencyInMonths` |  |  | `String(2)` |  | Int.Calc.Freq. |  |  |  |
| `CustomerAccountNote` |  |  | `String(30)` |  | Account Memo |  |  |  |
| `APARToleranceGroup` |  |  | `String(4)` |  | Tolerance Group |  |  |  |
| `HouseBank` |  |  | `String(5)` |  | House Bank |  |  |  |
| `ItemIsToBePaidSeparately` |  |  | `Boolean` |  | Individual Payment |  |  |  |
| `PaytAdviceIsSentbyEDI` |  |  | `Boolean` |  | Pmnt advice by EDI |  |  |  |
| `PhysicalInventoryBlockInd` |  |  | `Boolean` |  | Co.code post.block |  |  |  |
| `UserAtCustomer` |  |  | `String(15)` |  | User at customer |  |  |  |
| `AccountingClerkPhoneNumber` |  |  | `String(30)` |  | Acct.clerks tel.no. |  |  |  |
| `AccountingClerkFaxNumber` |  |  | `String(31)` |  | Acctg clerk's fax |  |  |  |
| `AccountingClerkInternetAddress` |  |  | `String(130)` |  | Clrk's internet add. |  |  |  |
| `AccountByCustomer` |  |  | `String(12)` |  | Account at Customer |  |  |  |
| `IsToBeLocallyProcessed` |  |  | `Boolean` |  | Local Processing |  |  |  |
| `CollectiveInvoiceVariant` |  |  | `String(1)` |  | Coll.Invoice Variant |  |  |  |
| `LayoutSortingRule` |  |  | `String(3)` |  | Sort key |  |  |  |
| `PaymentTerms` | `KNB1` | `ZTERM` | `String(4)` |  | Terms of Payment |  |  |  |
| `CustomerSupplierClearingIsUsed` |  |  | `Boolean` |  | Clearing with vendor |  |  |  |
| `RecordPaymentHistoryIndicator` |  |  | `Boolean` |  | Record Pmnt History |  |  |  |
| `PaymentMethodsList` |  |  | `String(10)` |  | Payment Methods |  |  |  |
| `DeletionIndicator` |  |  | `Boolean` |  | Co.Cde Deletion Flag |  |  |  |
| `CreditMemoPaymentTerms` |  |  | `String(4)` |  | Credit Memo Pyt Term |  |  |  |
| `DunningNoticeGroup` |  |  | `String(2)` |  | Grouping Key |  |  |  |
| `LastInterestCalcRunDate` |  |  | `Date` |  | Last Int. Calc. |  |  |  |
| `CustPreviousMasterRecordNumber` |  |  | `String(10)` |  | Previous Account No. |  |  |  |
| `ValueAdjustmentKey` |  |  | `String(2)` |  | Value Adjustment |  |  |  |
| `CashPlanningGroup` |  |  | `String(10)` |  | Planning Group |  | _CashPlanningGroup |  |
| `SupplierReleaseGroup` |  |  | `String(4)` |  | Release Group |  |  |  |
| `PersonnelNumber` |  |  | `String(8)` |  | Personnel Number |  |  |  |
| `BuyingGroupAccountNumber` |  |  | `String(10)` |  | Buying Group |  |  |  |
| `BillExchChargePaymentTerms` |  |  | `String(4)` |  | B/Ex. Charges Terms |  |  |  |
| `CheckPaidDurationInDays` |  |  | `Decimal(3,0)` |  | Check Cashing Time |  |  |  |
| `CustomerPaymentBlockingReason` |  |  | `String(1)` |  | Payment Block |  |  |  |
| `PaymentMethodSupplement` |  |  | `String(2)` |  | Pmt Meth. Supplement |  |  |  |
| `AcctsReceivablePledgingCode` |  |  | `String(2)` |  | AR Pledging Ind. |  |  |  |
| `LockboxInternalID` |  |  | `String(7)` |  | Lockbox |  |  |  |
| `IsBusinessPurposeCompleted` |  |  | `Boolean` |  | Purpose Completed |  |  |  |
| `WithholdingTaxCountry` |  |  | `String(3)` |  | WTax C/R Key |  |  |  |
| `KnownOrNegotiatedLeave` |  |  | `String(4)` |  | Known/Negotiat.Leave |  |  |  |
| `DeletionIsBlocked` |  |  | `Boolean` |  | CoCd Deletion Block |  |  |  |
| `PaymentClearingGroup` |  |  | `String(8)` |  | Payment Clrg Grp ID |  |  |  |
| `PaymentReason` |  |  | `String(4)` |  | Payment Reason |  |  |  |
| `BPPeriodicAccountStatement` |  |  | `String(1)` |  | Account Statement |  |  |  |
| `US_FrgnAcctTaxRcpntCntry` |  |  | `String(3)` |  | Country/Region Key |  |  |  |
| `US_GlobIntermediaryIdnNumber` |  |  | `String(19)` |  | US Recipient GIIN |  |  |  |
| `US_RecipientForeignTaxID` |  |  | `String(22)` |  | US Recipient FTID |  |  |  |
| `US_LobTreatyCode` |  |  | `String(2)` |  | LOB Treaty Code |  |  |  |
| `US_FW8BENReceiveDate` |  |  | `Date` |  | W8 Form Rec Date |  |  |  |
| `US_FW9ReceiveDate` |  |  | `Date` |  | W9 Form Rec Date |  |  |  |
| `US_SecondTINNoticeIsIssued` |  |  | `String(1)` |  | Second TIN Notice |  |  |  |
| `US_FrgnRecipientHasPartnership` |  |  | `String(1)` |  | Partnership Int Ind |  |  |  |
| `US_FrgnAcctTaxFilingIsRequired` |  |  | `String(1)` |  | FATCA Ind |  |  |  |
| `US_Chapter4StatusCode` |  |  | `String(2)` |  | Chaptr 4 Status Code |  |  |  |
| `LastDunnedOn` |  |  | `Date` |  | Last Dunned |  |  |  |
| `DunningProcedure` |  |  | `String(4)` |  | Dunning Procedure |  |  |  |
| `DunningLevel` |  |  | `String(1)` |  | Dunning Level |  |  |  |
| `DunningBlock` |  |  | `String(1)` |  | Dunning Block |  |  |  |
| `DunningRecipient` |  |  | `String(10)` |  | Dunning Recipient |  |  |  |
| `LegDunningProcedureOn` |  |  | `Date` |  | Legal Dunn.Proc.From |  |  |  |
| `IsActiveEntity` |  |  | `Boolean` |  | Is active |  |  |  |


## Entity: `CustomerDunning`

- **ABAP Name:** `I_CustomerDunning`
- **Label:** Customer Company Code Dunning Fields
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `CompanyCode` | `T001` | `BUKRS` | `String(4)` | Y | Company Code |  | _CustomerCompany |  |
| `Customer` |  |  | `String(10)` | Y | Customer |  | _Customer | S/4 only entity |
| `DunningArea` |  |  | `String(2)` | Y | Dunning Area |  |  | S/4 only entity |
| `LastDunnedOn` |  |  | `Date` |  | Last Dunned |  |  | S/4 only entity |
| `DunningProcedure` |  |  | `String(4)` |  | Dunning Procedure |  | _DunningProcedure | S/4 only entity |
| `DunningLevel` |  |  | `String(1)` |  | Dunning Level |  |  | S/4 only entity |
| `DunningBlock` |  |  | `String(1)` |  | Dunning Block |  | _DunningBlock | S/4 only entity |
| `DunningRecipient` |  |  | `String(10)` |  | Dunning Recipient |  | _DunningRecipient | S/4 only entity |
| `LegDunningProcedureOn` |  |  | `Date` |  | Legal Dunn.Proc.From |  |  | S/4 only entity |
| `DunningClerk` |  |  | `String(2)` |  | Dunning Clerk |  | _DunningClerk | S/4 only entity |


## Entity: `CustomerSalesArea`

- **ABAP Name:** `I_CustomerSalesArea`
- **Label:** Customer Sales Area
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `Customer` |  |  | `String(10)` | Y | Customer |  | _Customer | S/4 only entity |
| `SalesOrganization` |  |  | `String(4)` | Y | Sales Organization |  | _SalesOrganization | S/4 only entity |
| `DistributionChannel` |  |  | `String(2)` | Y | Distribution Channel |  | _DistributionChannel | S/4 only entity |
| `Division` |  |  | `String(2)` | Y | Division |  | _Division | S/4 only entity |
| `CustomerABCClassification` |  |  | `String(2)` |  | ABC Classification |  |  | S/4 only entity |
| `SalesOffice` |  |  | `String(4)` |  | Sales Office |  | _SalesOffice | S/4 only entity |
| `SalesGroup` |  |  | `String(3)` |  | Sales Group |  | _SalesGroup | S/4 only entity |
| `OrderIsBlockedForCustomer` |  |  | `String(2)` |  | Ord.blk:sls ar. |  |  | S/4 only entity |
| `Currency` |  |  | `String(5)` |  | Currency |  | _Currency | S/4 only entity |
| `CustomerPriceGroup` |  |  | `String(2)` |  | Customer Price Group |  |  | S/4 only entity |
| `PriceListType` |  |  | `String(2)` |  | Price List Type |  |  | S/4 only entity |
| `DeliveryPriority` |  |  | `String(2)` |  | Delivery Priority |  | _DeliveryPriority | S/4 only entity |
| `ShippingCondition` |  |  | `String(2)` |  | Shipping Conditions |  | _ShippingCondition | S/4 only entity |
| `IncotermsClassification` |  |  | `String(3)` |  | Incoterms |  | _IncotermsClassification | S/4 only entity |
| `SupplyingPlant` |  |  | `String(4)` |  | Delivering Plant |  | _SupplyingPlant | S/4 only entity |
| `CompleteDeliveryIsDefined` |  |  | `Boolean` |  | Complete Delivery |  |  | S/4 only entity |
| `DeliveryIsBlockedForCustomer` |  |  | `String(2)` |  | DelBlckSalesAr. |  | _DeliveryIsBlockedForCustomer | S/4 only entity |
| `BillingIsBlockedForCustomer` |  |  | `String(2)` |  | BBlock for SlsA |  | _BillingIsBlockedForCustomer | S/4 only entity |
| `CustomerPaymentTerms` |  |  | `String(4)` |  | Terms of Payment |  | _CustomerPaymentTerms | S/4 only entity |
| `CustomerAccountAssignmentGroup` |  |  | `String(2)` |  | Acct Assmt Grp Cust. |  |  | S/4 only entity |
| `AccountByCustomer` |  |  | `String(12)` |  | Account at Customer |  |  | S/4 only entity |
| `CustomerGroup` |  |  | `String(2)` |  | Customer Group |  |  | S/4 only entity |
| `CustomerPricingProcedure` |  |  | `String(2)` |  | Cust.Pric.Procedure |  |  | S/4 only entity |
| `OrderCombinationIsAllowed` |  |  | `Boolean` |  | Order Combination |  |  | S/4 only entity |
| `PartialDeliveryIsAllowed` |  |  | `String(1)` |  | Partial Deliv./Item |  |  | S/4 only entity |
| `InvoiceDate` |  |  | `String(2)` |  | Invoicing Dates |  |  | S/4 only entity |
| `PaymentTerms` |  |  | `String(4)` |  | Terms of Payment |  |  | S/4 only entity |
| `IncotermsTransferLocation` |  |  | `String(28)` |  | Incoterms (Part 2) |  |  | S/4 only entity |
| `ItemOrderProbabilityInPercent` |  |  | `String(3)` |  | Order Probability |  |  | S/4 only entity |
| `IncotermsLocation2` |  |  | `String(70)` |  | Incoterms Location 2 |  |  | S/4 only entity |
| `RecordCreatedDate` |  |  | `Date` |  | Created On |  |  | S/4 only entity |
| `AuthorizationGroup` |  |  | `String(4)` |  | Authorization Group |  |  | S/4 only entity |
| `SalesDistrict` |  |  | `String(6)` |  | Sales District |  |  | S/4 only entity |
| `IncotermsVersion` |  |  | `String(4)` |  | Incoterms Version |  |  | S/4 only entity |
| `IncotermsLocation1` |  |  | `String(70)` |  | Incoterms Location 1 |  |  | S/4 only entity |
| `DeletionIndicator` |  |  | `Boolean` |  | Del.ID SlsArea |  |  | S/4 only entity |
| `IsBusinessPurposeCompleted` |  |  | `Boolean` |  | Purpose Completed |  |  | S/4 only entity |
| `SalesItemProposal` |  |  | `String(10)` |  | Item proposal |  |  | S/4 only entity |
| `CustProdProposalProcedure` |  |  | `String(2)` |  | PP customer proced. |  | _CustProdProposalProcedure | S/4 only entity |
| `ProofOfDeliveryTime` |  |  | `String(6)` |  |  |  |  | S/4 only entity |
| `ProofOfDeliveryTimeValue` |  |  | `Decimal(6,2)` |  | POD timeframe |  |  | S/4 only entity |
| `MaxNmbrOfPartialDelivery` |  |  | `Decimal(1,0)` |  | Max.Part.Deliveries |  |  | S/4 only entity |
| `UnderdelivTolrtdLmtRatioInPct` |  |  | `Decimal(3,1)` |  | Underdel. Tolerance |  |  | S/4 only entity |
| `OverdelivTolrtdLmtRatioInPct` |  |  | `Decimal(3,1)` |  | Overdeliv. Tolerance |  |  | S/4 only entity |
| `IsActiveEntity` |  |  | `Boolean` |  | Is active |  |  | S/4 only entity |
| `AdditionalCustomerGroup1` |  |  | `String(3)` |  | Customer Group 1 |  |  | S/4 only entity |
| `AdditionalCustomerGroup2` |  |  | `String(3)` |  | Customer Group 2 |  |  | S/4 only entity |
| `AdditionalCustomerGroup3` |  |  | `String(3)` |  | Customer Group 3 |  |  | S/4 only entity |
| `AdditionalCustomerGroup4` |  |  | `String(3)` |  | Customer Group 4 |  |  | S/4 only entity |
| `AdditionalCustomerGroup5` |  |  | `String(3)` |  | Customer Group 5 |  |  | S/4 only entity |
| `InvoiceListSchedule` |  |  | `String(2)` |  | Invoice List Sched. |  | _FactoryCalendar | S/4 only entity |
| `ExchangeRateType` |  |  | `String(4)` |  | Exchange Rate Type |  | _ExchangeRateType | S/4 only entity |
| `PaymentGuaranteeProcedure` |  |  | `String(4)` |  | Paymt guarant. proc. |  | _PaytGuarProcedVH | S/4 only entity |
| `SuplrIsRlvtForSettlmtMgmt` |  |  | `Boolean` |  | Settlement Mgmt. |  |  | S/4 only entity |
| `CustIsRlvtForSettlmtMgmt` |  |  | `Boolean` |  | Settlement Mgmt. |  |  | S/4 only entity |
| `ProductUnitGroup` |  |  | `String(4)` |  | Unit of Measure Grp |  |  | S/4 only entity |
| `SlsDocIsRlvtForProofOfDeliv` |  |  | `Boolean` |  | Relevant for POD |  |  | S/4 only entity |
| `SlsUnlmtdOvrdelivIsAllwd` |  |  | `Boolean` |  | Unlimited Tolerance |  |  | S/4 only entity |
| `CreditControlArea` |  |  | `String(4)` |  | Credit Control Area |  |  | S/4 only entity |
| `CustomerIsRebateRelevant` |  |  | `Boolean` |  | Rebate |  |  | S/4 only entity |
| `InspSbstHasNoTimeOrQuantity` |  |  | `Boolean` |  | Price determination |  |  | S/4 only entity |
| `ManualInvoiceMaintIsRelevant` |  |  | `Boolean` |  | Man. Invoice Maint. |  |  | S/4 only entity |
| `IncotermsSupChnLoc1AddlUUID` |  |  | `UUID` |  | Location UUID |  |  | S/4 only entity |
| `IncotermsSupChnLoc2AddlUUID` |  |  | `UUID` |  | Location UUID |  |  | S/4 only entity |
| `IncotermsSupChnDvtgLocAddlUUID` |  |  | `UUID` |  | Location UUID |  |  | S/4 only entity |
| `SalesBlockForCustomer` |  |  | `String(2)` |  | Sales Block |  |  | S/4 only entity |
| `CustomerStatisticsGroup` |  |  | `String(1)` |  | Customer Stats.Group |  |  | S/4 only entity |
| `RetailAdditionalCustomerGrp6` |  |  | `String(3)` |  | Customer Group 6 |  |  | S/4 only entity |
| `RetailAdditionalCustomerGrp7` |  |  | `String(3)` |  | Customer Group 7 |  |  | S/4 only entity |
| `RetailAdditionalCustomerGrp8` |  |  | `String(3)` |  | Customer Group 8 |  |  | S/4 only entity |
| `RetailAdditionalCustomerGrp9` |  |  | `String(3)` |  | Customer Group 9 |  |  | S/4 only entity |
| `RetailAdditionalCustomerGrp10` |  |  | `String(3)` |  | Customer Group 10 |  |  | S/4 only entity |


## Entity: `CustomerSalesAreaTax`

- **ABAP Name:** `I_CustSalesAreaTax`
- **Label:** Customer Sales Area Tax
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `Customer` |  |  | `String(10)` | Y | Customer |  | _Customer | S/4 only entity |
| `SalesOrganization` |  |  | `String(4)` | Y | Sales Organization |  | _SalesOrganization | S/4 only entity |
| `DistributionChannel` |  |  | `String(2)` | Y | RefDistCh-Cust/Mat. |  | _DistributionChannel | S/4 only entity |
| `Division` |  |  | `String(2)` | Y | Division |  | _Division | S/4 only entity |
| `DepartureCountry` |  |  | `String(3)` | Y | Departure Ctry/Reg. |  | _Country | S/4 only entity |
| `CustomerTaxCategory` |  |  | `String(4)` | Y | Tax Condition Type |  |  | S/4 only entity |
| `CustomerTaxClassification` |  |  | `String(1)` |  | Tax Classification |  |  | S/4 only entity |
| `AuthorizationGroup` |  |  | `String(4)` |  | Authorization |  |  | S/4 only entity |
| `IsBusinessPurposeCompleted` |  |  | `Boolean` |  | Purpose Completed |  |  | S/4 only entity |


## Entity: `CustomerUnloadingPoint`

- **ABAP Name:** `I_CustomerUnloadingPoint`
- **Label:** Customer Unloading Point
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `Customer` |  |  | `String(10)` | Y | Customer |  | _Customer | S/4 only entity |
| `UnloadingPointName` |  |  | `String(25)` | Y | Unloading Point |  |  | S/4 only entity |
| `CustomerFactoryCalenderCode` |  |  | `String(2)` |  | Cust.fact.calendar |  |  | S/4 only entity |
| `BPGoodsReceivingHoursCode` |  |  | `String(3)` |  | Goods receiving hrs |  |  | S/4 only entity |
| `IsDfltBPUnloadingPoint` |  |  | `Boolean` |  | Default unloading pt |  |  | S/4 only entity |
| `MondayMorningOpeningTime` |  |  | `String(6)` |  | Monday |  |  | S/4 only entity |
| `MondayMorningClosingTime` |  |  | `String(6)` |  | Monday |  |  | S/4 only entity |
| `MondayAfternoonOpeningTime` |  |  | `String(6)` |  | Monday |  |  | S/4 only entity |
| `MondayAfternoonClosingTime` |  |  | `String(6)` |  | Monday |  |  | S/4 only entity |
| `TuesdayMorningOpeningTime` |  |  | `String(6)` |  | Tuesday |  |  | S/4 only entity |
| `TuesdayMorningClosingTime` |  |  | `String(6)` |  | Tuesday |  |  | S/4 only entity |
| `TuesdayAfternoonOpeningTime` |  |  | `String(6)` |  | Tuesday |  |  | S/4 only entity |
| `TuesdayAfternoonClosingTime` |  |  | `String(6)` |  | Tuesday |  |  | S/4 only entity |
| `WednesdayMorningOpeningTime` |  |  | `String(6)` |  | Wednesday |  |  | S/4 only entity |
| `WednesdayMorningClosingTime` |  |  | `String(6)` |  | Wednesday |  |  | S/4 only entity |
| `WednesdayAfternoonOpeningTime` |  |  | `String(6)` |  | Wednesday |  |  | S/4 only entity |
| `WednesdayAfternoonClosingTime` |  |  | `String(6)` |  | Wednesday |  |  | S/4 only entity |
| `ThursdayMorningOpeningTime` |  |  | `String(6)` |  | Thursday |  |  | S/4 only entity |
| `ThursdayMorningClosingTime` |  |  | `String(6)` |  | Thursday |  |  | S/4 only entity |
| `ThursdayAfternoonOpeningTime` |  |  | `String(6)` |  | Thursday |  |  | S/4 only entity |
| `ThursdayAfternoonClosingTime` |  |  | `String(6)` |  | Thursday |  |  | S/4 only entity |
| `FridayMorningOpeningTime` |  |  | `String(6)` |  | Friday |  |  | S/4 only entity |
| `FridayMorningClosingTime` |  |  | `String(6)` |  | Friday |  |  | S/4 only entity |
| `FridayAfternoonOpeningTime` |  |  | `String(6)` |  | Friday |  |  | S/4 only entity |
| `FridayAfternoonClosingTime` |  |  | `String(6)` |  | Friday |  |  | S/4 only entity |
| `SaturdayMorningOpeningTime` |  |  | `String(6)` |  | Saturday |  |  | S/4 only entity |
| `SaturdayMorningClosingTime` |  |  | `String(6)` |  | Saturday |  |  | S/4 only entity |
| `SaturdayAfternoonOpeningTime` |  |  | `String(6)` |  | Saturday |  |  | S/4 only entity |
| `SaturdayAfternoonClosingTime` |  |  | `String(6)` |  | Saturday |  |  | S/4 only entity |
| `SundayMorningOpeningTime` |  |  | `String(6)` |  | Sunday |  |  | S/4 only entity |
| `SundayMorningClosingTime` |  |  | `String(6)` |  | Sunday |  |  | S/4 only entity |
| `SundayAfternoonOpeningTime` |  |  | `String(6)` |  | Sunday |  |  | S/4 only entity |
| `SundayAfternoonClosingTime` |  |  | `String(6)` |  | Sunday |  |  | S/4 only entity |


## Entity: `CustomerWithHoldingTax`

- **ABAP Name:** `I_CustomerWithTax`
- **Label:** Customer WithHolding Tax
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `Customer` |  |  | `String(10)` | Y | Customer |  | _Customer | S/4 only entity |
| `CompanyCode` | `T001` | `BUKRS` | `String(4)` | Y | Company Code |  | _CompanyCode |  |
| `WithholdingTaxType` |  |  | `String(2)` | Y | Withholding Tax Type |  |  | S/4 only entity |
| `WithholdingTaxCode` |  |  | `String(2)` |  | W/Tax Code |  |  | S/4 only entity |
| `WithholdingTaxAgent` |  |  | `Boolean` |  | WTax Agent |  |  | S/4 only entity |
| `ObligationDateBegin` |  |  | `Date` |  | W/Tax Obligated Frm |  |  | S/4 only entity |
| `ObligationDateEnd` |  |  | `Date` |  | Oblig.to W/Tax Until |  |  | S/4 only entity |
| `WithholdingTaxNumber` |  |  | `String(16)` |  | W/tax number |  |  | S/4 only entity |
| `WithholdingTaxCertificate` |  |  | `String(25)` |  | Exemption Number |  |  | S/4 only entity |
| `WithholdingTaxExmptPercent` |  |  | `Decimal(5,2)` |  | Exemption Rate |  |  | S/4 only entity |
| `ExemptionDateBegin` |  |  | `Date` |  | Exemption Start Date |  |  | S/4 only entity |
| `ExemptionDateEnd` |  |  | `Date` |  | Exemption End Date |  |  | S/4 only entity |
| `ExemptionReason` |  |  | `String(2)` |  | Exemption Reason |  |  | S/4 only entity |
