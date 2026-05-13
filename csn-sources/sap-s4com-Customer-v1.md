# Customer

> Source file: `sap-s4com-Customer-v1.json`

**Technical Name:** `` | **Data Category:** `DIMENSION` | **VDM Type:** `BASIC` | **Size:** `XL`


## Entity: `Customer`

- **ABAP Name:** `I_Customer`
- **Label:** Customer
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** KNA1, ADRC

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Customer` | `Customer` | `String(10)` | Y | Customer |  |  |  |
| `CustomerName` | `CustomerName` | `String(80)` |  | Name of Customer |  |  |  |
| `CustomerFullName` | `CustomerFullName` | `String(220)` |  | Customer Name |  |  |  |
| `BPCustomerName` | `BPCustomerName` | `String(81)` |  | Business Partner - Customer Name |  |  |  |
| `BPCustomerFullName` | `BPCustomerFullName` | `String(220)` |  | Business Partner - Customer Full Name |  |  |  |
| `CreatedByUser` | `CreatedByUser` | `String(12)` |  | Created by |  |  |  |
| `CreationDate` | `CreationDate` | `Date` |  | Created On |  |  |  |
| `AddressID` | `AddressID` | `String(10)` |  | Address |  |  |  |
| `CustomerClassification` | `CustomerClassification` | `String(2)` |  | Customer Classific. |  | _CustomerClassification |  |
| `VATRegistration` | `VATRegistration` | `String(20)` |  | VAT Registration No. |  |  |  |
| `CustomerAccountGroup` | `CustomerAccountGroup` | `String(4)` |  | Account Group |  |  |  |
| `AuthorizationGroup` | `AuthorizationGroup` | `String(4)` |  | Authorization |  |  |  |
| `DeliveryIsBlocked` | `DeliveryIsBlocked` | `String(2)` |  | Delivery block |  |  |  |
| `PostingIsBlocked` | `PostingIsBlocked` | `Boolean` |  | Posting Block |  |  |  |
| `BillingIsBlockedForCustomer` | `BillingIsBlockedForCustomer` | `String(2)` |  | Billing Block |  |  |  |
| `OrderIsBlockedForCustomer` | `OrderIsBlockedForCustomer` | `String(2)` |  | Order Block |  |  |  |
| `InternationalLocationNumber1` | `InternationalLocationNumber1` | `String(7)` |  | Int. location no. 1 |  |  |  |
| `IsOneTimeAccount` | `IsOneTimeAccount` | `Boolean` |  | One-Time Account |  |  |  |
| `TaxJurisdiction` | `TaxJurisdiction` | `String(15)` |  | Tax Jurisdiction |  |  |  |
| `Industry` | `Industry` | `String(4)` |  | Industry |  |  |  |
| `TaxNumberType` | `TaxNumberType` | `String(2)` |  | Tax Number Type |  |  |  |
| `TaxNumber1` | `TaxNumber1` | `String(16)` |  | Tax Number 1 |  |  |  |
| `TaxNumber2` | `TaxNumber2` | `String(11)` |  | Tax Number 2 |  |  |  |
| `TaxNumber3` | `TaxNumber3` | `String(18)` |  | Tax Number 3 |  |  |  |
| `TaxNumber4` | `TaxNumber4` | `String(18)` |  | Tax Number 4 |  |  |  |
| `TaxNumber5` | `TaxNumber5` | `String(60)` |  | Tax Number 5 |  |  |  |
| `TaxNumber6` | `TaxNumber6` | `String(20)` |  | Tax Number 6 |  |  |  |
| `CustomerCorporateGroup` | `CustomerCorporateGroup` | `String(10)` |  | Group Key |  |  |  |
| `Supplier` | `Supplier` | `String(10)` |  | Supplier |  |  |  |
| `NielsenRegion` | `NielsenRegion` | `String(2)` |  | Nielsen Indicator |  |  |  |
| `IndustryCode1` | `IndustryCode1` | `String(10)` |  | Industry Code 1 |  |  |  |
| `IndustryCode2` | `IndustryCode2` | `String(10)` |  | Industry Code 2 |  |  |  |
| `IndustryCode3` | `IndustryCode3` | `String(10)` |  | Industry Code 3 |  |  |  |
| `IndustryCode4` | `IndustryCode4` | `String(10)` |  | Industry Code 4 |  |  |  |
| `IndustryCode5` | `IndustryCode5` | `String(10)` |  | Industry Code 5 |  |  |  |
| `Country` | `Country` | `String(3)` |  | Country/Region Key |  |  |  |
| `OrganizationBPName1` | `OrganizationBPName1` | `String(35)` |  | Name |  |  |  |
| `OrganizationBPName2` | `OrganizationBPName2` | `String(35)` |  | Name 2 |  |  |  |
| `CityName` | `CityName` | `String(35)` |  | City |  |  |  |
| `PostalCode` | `PostalCode` | `String(10)` |  | Postal Code |  |  |  |
| `StreetName` | `StreetName` | `String(35)` |  | Street |  |  |  |
| `SortField` | `SortField` | `String(10)` |  | Search Term |  |  |  |
| `FaxNumber` | `FaxNumber` | `String(31)` |  | Fax Number |  |  |  |
| `BR_SUFRAMACode` | `BR_SUFRAMACode` | `String(9)` |  | Suframa Code |  |  |  |
| `Region` | `Region` | `String(3)` |  | Region |  |  |  |
| `TelephoneNumber1` | `TelephoneNumber1` | `String(16)` |  | Telephone 1 |  |  |  |
| `TelephoneNumber2` | `TelephoneNumber2` | `String(16)` |  | Telephone 2 |  |  |  |
| `AlternativePayerAccount` | `AlternativePayerAccount` | `String(10)` |  | Alternative Payer |  |  |  |
| `DataMediumExchangeIndicator` | `DataMediumExchangeIndicator` | `String(1)` |  | DME Recipient Code |  |  |  |
| `VATLiability` | `VATLiability` | `Boolean` |  | Liable for VAT |  |  |  |
| `IsBusinessPurposeCompleted` | `IsBusinessPurposeCompleted` | `Boolean` |  | Purpose Completed |  |  |  |
| `ResponsibleType` | `ResponsibleType` | `String(2)` |  | Tax Type |  |  |  |
| `FiscalAddress` | `FiscalAddress` | `String(10)` |  | Fiscal address |  |  |  |
| `NFPartnerIsNaturalPerson` | `NFPartnerIsNaturalPerson` | `Boolean` |  | Natural Person |  |  |  |
| `DeletionIndicator` | `DeletionIndicator` | `Boolean` |  | Deletion Flag |  |  |  |
| `Language` | `Language` | `String(2)` |  | Language Key |  |  |  |
| `TradingPartner` | `TradingPartner` | `String(6)` |  | Trading Partner No. |  | _GlobalCompany |  |
| `DeliveryDateTypeRule` | `DeliveryDateTypeRule` | `String(1)` |  | Deliv Date Rule |  |  |  |
| `ExpressTrainStationName` | `ExpressTrainStationName` | `String(25)` |  | Express station |  |  |  |
| `TrainStationName` | `TrainStationName` | `String(25)` |  | Train station |  |  |  |
| `InternationalLocationNumber2` | `InternationalLocationNumber2` | `String(5)` |  | Int. location no. 2 |  |  |  |
| `InternationalLocationNumber3` | `InternationalLocationNumber3` | `String(1)` |  | Check digit |  |  |  |
| `CityCode` | `CityCode` | `String(4)` |  | City Code |  |  |  |
| `County` | `County` | `String(3)` |  | County Code |  |  |  |
| `CustomerHasUnloadingPoint` | `CustomerHasUnloadingPoint` | `Boolean` |  | Unloading points |  |  |  |
| `CustomerWorkingTimeCalendar` | `CustomerWorkingTimeCalendar` | `String(2)` |  | Working times |  |  |  |
| `IsCompetitor` | `IsCompetitor` | `Boolean` |  | Competitors |  |  |  |
| `TaxInvoiceRepresentativeName` | `TaxInvoiceRepresentativeName` | `String(10)` |  | Rep's Name |  |  |  |
| `BusinessType` | `BusinessType` | `String(30)` |  | Type of Business |  |  |  |
| `IndustryType` | `IndustryType` | `String(30)` |  | Type of Industry |  |  |  |
| `TW_CollvBillingIsSupported` | `TW_CollvBillingIsSupported` | `Boolean` |  | Consolidated Invoic. |  |  |  |
| `AlternativePayeeIsAllowed` | `AlternativePayeeIsAllowed` | `Boolean` |  | Alt.payer in doc? |  |  |  |
| `FreeDefinedAttribute01` | `FreeDefinedAttribute01` | `String(2)` |  | Attribute 1 |  |  |  |
| `FreeDefinedAttribute02` | `FreeDefinedAttribute02` | `String(2)` |  | Attribute 2 |  |  |  |
| `FreeDefinedAttribute03` | `FreeDefinedAttribute03` | `String(2)` |  | Attribute 3 |  |  |  |
| `FreeDefinedAttribute04` | `FreeDefinedAttribute04` | `String(2)` |  | Attribute 4 |  |  |  |
| `FreeDefinedAttribute05` | `FreeDefinedAttribute05` | `String(2)` |  | Attribute 5 |  |  |  |
| `FreeDefinedAttribute06` | `FreeDefinedAttribute06` | `String(3)` |  | Attribute 6 |  |  |  |
| `FreeDefinedAttribute07` | `FreeDefinedAttribute07` | `String(3)` |  | Attribute 7 |  |  |  |
| `FreeDefinedAttribute08` | `FreeDefinedAttribute08` | `String(3)` |  | Attribute 8 |  |  |  |
| `FreeDefinedAttribute09` | `FreeDefinedAttribute09` | `String(3)` |  | Attribute 9 |  |  |  |
| `FreeDefinedAttribute10` | `FreeDefinedAttribute10` | `String(3)` |  | Attribute 10 |  |  |  |
| `PaymentReason` | `PaymentReason` | `String(4)` |  | Payment Reason |  |  |  |
| `CustomerConditionGroup1` | `CustomerConditionGroup1` | `String(2)` |  | Condition Group 1 |  |  |  |
| `CustomerConditionGroup2` | `CustomerConditionGroup2` | `String(2)` |  | Condition Group 2 |  |  |  |
| `CustomerConditionGroup3` | `CustomerConditionGroup3` | `String(2)` |  | Condition Group 3 |  |  |  |
| `CustomerConditionGroup4` | `CustomerConditionGroup4` | `String(2)` |  | Condition Group 4 |  |  |  |
| `CustomerConditionGroup5` | `CustomerConditionGroup5` | `String(2)` |  | Condition Group 5 |  |  |  |
| `IsSalesProspect` | `IsSalesProspect` | `Boolean` |  | Prospect |  |  |  |
| `PaymentIsBlockedForCustomer` | `PaymentIsBlockedForCustomer` | `Boolean` |  | Payment block |  |  |  |
| `IsConsumer` | `IsConsumer` | `Boolean` |  | Consumer |  |  |  |
| `DataControllerSet` | `DataControllerSet` | `String(1)` |  | Data Ctrlr. Set |  |  |  |
| `DataController1` | `DataController1` | `String(30)` |  | Data Controller |  |  |  |
| `DataController2` | `DataController2` | `String(30)` |  | Data Controller |  |  |  |
| `DataController3` | `DataController3` | `String(30)` |  | Data Controller |  |  |  |
| `DataController4` | `DataController4` | `String(30)` |  | Data Controller |  |  |  |
| `DataController5` | `DataController5` | `String(30)` |  | Data Controller |  |  |  |
| `DataController6` | `DataController6` | `String(30)` |  | Data Controller |  |  |  |
| `DataController7` | `DataController7` | `String(30)` |  | Data Controller |  |  |  |
| `DataController8` | `DataController8` | `String(30)` |  | Data Controller |  |  |  |
| `DataController9` | `DataController9` | `String(30)` |  | Data Controller |  |  |  |
| `DataController10` | `DataController10` | `String(30)` |  | Data Controller |  |  |  |
| `BusinessPartnerName1` | `BusinessPartnerName1` | `String(40)` |  | Business Partner Organization  - Name 1 |  |  |  |
| `BusinessPartnerName2` | `BusinessPartnerName2` | `String(40)` |  | Business Partner Organization  - Name 2 |  |  |  |
| `BusinessPartnerName3` | `BusinessPartnerName3` | `String(40)` |  | Business Partner Organization  - Name 3 |  |  |  |
| `BusinessPartnerName4` | `BusinessPartnerName4` | `String(40)` |  | Business Partner Organization  - Name 4 |  |  |  |
| `BPAddrCityName` | `BPAddrCityName` | `String(40)` |  | Business Partner Address – City |  |  |  |
| `BPAddrStreetName` | `BPAddrStreetName` | `String(60)` |  | Business Partner Address – Street |  |  |  |
| `AddressSearchTerm1` | `AddressSearchTerm1` | `String(20)` |  | Business Partner Address - Search Term 1 |  |  |  |
| `AddressSearchTerm2` | `AddressSearchTerm2` | `String(20)` |  | Business Partner Address - Search Term 2 |  |  |  |
| `DistrictName` | `DistrictName` | `String(40)` |  | Business Partner Address – District |  |  |  |
| `POBoxDeviatingCityName` | `POBoxDeviatingCityName` | `String(40)` |  | Business Partner Address - PO Box Deviating City |  |  |  |
| `BusinessPartnerFormOfAddress` | `BusinessPartnerFormOfAddress` | `String(4)` |  | Business Partner - Form of Address |  |  |  |
| `BR_ICMSTaxPayerType` | `BR_ICMSTaxPayerType` | `String(2)` |  | ICMS Taxpayer |  |  |  |


## Entity: `CustomerCompanyCode`

- **ABAP Name:** `I_CustomerCompany`
- **Label:** Customer Company
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** KNB5, KNB1

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Customer` | `Customer` | `String(10)` | Y | Customer |  | _Customer |  |
| `CompanyCode` | `CompanyCode` | `String(4)` | Y | Company Code |  |  |  |
| `AccountingClerk` | `AccountingClerk` | `String(2)` |  | Clerk Abbrev. |  |  |  |
| `ReconciliationAccount` | `ReconciliationAccount` | `String(10)` |  | Reconciliation Acct |  |  |  |
| `AuthorizationGroup` | `AuthorizationGroup` | `String(4)` |  | Authorization |  |  |  |
| `CustomerHeadOffice` | `CustomerHeadOffice` | `String(10)` |  | Head Office |  |  |  |
| `AlternativePayerAccount` | `AlternativePayerAccount` | `String(10)` |  | Alternative payer |  |  |  |
| `PaymentBlockingReason` | `PaymentBlockingReason` | `String(1)` |  | Payment Block |  | _PaymentBlockValueHelp |  |
| `InterestCalculationCode` | `InterestCalculationCode` | `String(2)` |  | Interest Indicator |  |  |  |
| `InterestCalculationDate` | `InterestCalculationDate` | `Date` |  | Last Key Date |  |  |  |
| `IntrstCalcFrequencyInMonths` | `IntrstCalcFrequencyInMonths` | `String(2)` |  | Int.Calc.Freq. |  |  |  |
| `CustomerAccountNote` | `CustomerAccountNote` | `String(30)` |  | Account Memo |  |  |  |
| `APARToleranceGroup` | `APARToleranceGroup` | `String(4)` |  | Tolerance Group |  |  |  |
| `HouseBank` | `HouseBank` | `String(5)` |  | House Bank |  |  |  |
| `ItemIsToBePaidSeparately` | `ItemIsToBePaidSeparately` | `Boolean` |  | Individual Payment |  |  |  |
| `PaytAdviceIsSentbyEDI` | `PaytAdviceIsSentbyEDI` | `Boolean` |  | Pmnt advice by EDI |  |  |  |
| `PhysicalInventoryBlockInd` | `PhysicalInventoryBlockInd` | `Boolean` |  | Co.code post.block |  |  |  |
| `UserAtCustomer` | `UserAtCustomer` | `String(15)` |  | User at customer |  |  |  |
| `AccountingClerkPhoneNumber` | `AccountingClerkPhoneNumber` | `String(30)` |  | Acct.clerks tel.no. |  |  |  |
| `AccountingClerkFaxNumber` | `AccountingClerkFaxNumber` | `String(31)` |  | Acctg clerk's fax |  |  |  |
| `AccountingClerkInternetAddress` | `AccountingClerkInternetAddress` | `String(130)` |  | Clrk's internet add. |  |  |  |
| `AccountByCustomer` | `AccountByCustomer` | `String(12)` |  | Account at Customer |  |  |  |
| `IsToBeLocallyProcessed` | `IsToBeLocallyProcessed` | `Boolean` |  | Local Processing |  |  |  |
| `CollectiveInvoiceVariant` | `CollectiveInvoiceVariant` | `String(1)` |  | Coll.Invoice Variant |  |  |  |
| `LayoutSortingRule` | `LayoutSortingRule` | `String(3)` |  | Sort key |  |  |  |
| `PaymentTerms` | `PaymentTerms` | `String(4)` |  | Terms of Payment |  |  |  |
| `CustomerSupplierClearingIsUsed` | `CustomerSupplierClearingIsUsed` | `Boolean` |  | Clearing with vendor |  |  |  |
| `RecordPaymentHistoryIndicator` | `RecordPaymentHistoryIndicator` | `Boolean` |  | Record Pmnt History |  |  |  |
| `PaymentMethodsList` | `PaymentMethodsList` | `String(10)` |  | Payment Methods |  |  |  |
| `DeletionIndicator` | `DeletionIndicator` | `Boolean` |  | Co.Cde Deletion Flag |  |  |  |
| `CreditMemoPaymentTerms` | `CreditMemoPaymentTerms` | `String(4)` |  | Credit Memo Pyt Term |  |  |  |
| `DunningNoticeGroup` | `DunningNoticeGroup` | `String(2)` |  | Grouping Key |  |  |  |
| `LastInterestCalcRunDate` | `LastInterestCalcRunDate` | `Date` |  | Last Int. Calc. |  |  |  |
| `CustPreviousMasterRecordNumber` | `CustPreviousMasterRecordNumber` | `String(10)` |  | Previous Account No. |  |  |  |
| `ValueAdjustmentKey` | `ValueAdjustmentKey` | `String(2)` |  | Value Adjustment |  |  |  |
| `CashPlanningGroup` | `CashPlanningGroup` | `String(10)` |  | Planning Group |  | _CashPlanningGroup |  |
| `SupplierReleaseGroup` | `SupplierReleaseGroup` | `String(4)` |  | Release Group |  |  |  |
| `PersonnelNumber` | `PersonnelNumber` | `String(8)` |  | Personnel Number |  |  |  |
| `BuyingGroupAccountNumber` | `BuyingGroupAccountNumber` | `String(10)` |  | Buying Group |  |  |  |
| `BillExchChargePaymentTerms` | `BillExchChargePaymentTerms` | `String(4)` |  | B/Ex. Charges Terms |  |  |  |
| `CheckPaidDurationInDays` | `CheckPaidDurationInDays` | `Decimal(3,0)` |  | Check Cashing Time |  |  |  |
| `CustomerPaymentBlockingReason` | `CustomerPaymentBlockingReason` | `String(1)` |  | Payment Block |  |  |  |
| `PaymentMethodSupplement` | `PaymentMethodSupplement` | `String(2)` |  | Pmt Meth. Supplement |  |  |  |
| `AcctsReceivablePledgingCode` | `AcctsReceivablePledgingCode` | `String(2)` |  | AR Pledging Ind. |  |  |  |
| `LockboxInternalID` | `LockboxInternalID` | `String(7)` |  | Lockbox |  |  |  |
| `IsBusinessPurposeCompleted` | `IsBusinessPurposeCompleted` | `Boolean` |  | Purpose Completed |  |  |  |
| `WithholdingTaxCountry` | `WithholdingTaxCountry` | `String(3)` |  | WTax C/R Key |  |  |  |
| `KnownOrNegotiatedLeave` | `KnownOrNegotiatedLeave` | `String(4)` |  | Known/Negotiat.Leave |  |  |  |
| `DeletionIsBlocked` | `DeletionIsBlocked` | `Boolean` |  | CoCd Deletion Block |  |  |  |
| `PaymentClearingGroup` | `PaymentClearingGroup` | `String(8)` |  | Payment Clrg Grp ID |  |  |  |
| `PaymentReason` | `PaymentReason` | `String(4)` |  | Payment Reason |  |  |  |
| `BPPeriodicAccountStatement` | `BPPeriodicAccountStatement` | `String(1)` |  | Account Statement |  |  |  |
| `US_FrgnAcctTaxRcpntCntry` | `US_FrgnAcctTaxRcpntCntry` | `String(3)` |  | Country/Region Key |  |  |  |
| `US_GlobIntermediaryIdnNumber` | `US_GlobIntermediaryIdnNumber` | `String(19)` |  | US Recipient GIIN |  |  |  |
| `US_RecipientForeignTaxID` | `US_RecipientForeignTaxID` | `String(22)` |  | US Recipient FTID |  |  |  |
| `US_LobTreatyCode` | `US_LobTreatyCode` | `String(2)` |  | LOB Treaty Code |  |  |  |
| `US_FW8BENReceiveDate` | `US_FW8BENReceiveDate` | `Date` |  | W8 Form Rec Date |  |  |  |
| `US_FW9ReceiveDate` | `US_FW9ReceiveDate` | `Date` |  | W9 Form Rec Date |  |  |  |
| `US_SecondTINNoticeIsIssued` | `US_SecondTINNoticeIsIssued` | `String(1)` |  | Second TIN Notice |  |  |  |
| `US_FrgnRecipientHasPartnership` | `US_FrgnRecipientHasPartnership` | `String(1)` |  | Partnership Int Ind |  |  |  |
| `US_FrgnAcctTaxFilingIsRequired` | `US_FrgnAcctTaxFilingIsRequired` | `String(1)` |  | FATCA Ind |  |  |  |
| `US_Chapter4StatusCode` | `US_Chapter4StatusCode` | `String(2)` |  | Chaptr 4 Status Code |  |  |  |
| `LastDunnedOn` | `LastDunnedOn` | `Date` |  | Last Dunned |  |  |  |
| `DunningProcedure` | `DunningProcedure` | `String(4)` |  | Dunning Procedure |  |  |  |
| `DunningLevel` | `DunningLevel` | `String(1)` |  | Dunning Level |  |  |  |
| `DunningBlock` | `DunningBlock` | `String(1)` |  | Dunning Block |  |  |  |
| `DunningRecipient` | `DunningRecipient` | `String(10)` |  | Dunning Recipient |  |  |  |
| `LegDunningProcedureOn` | `LegDunningProcedureOn` | `Date` |  | Legal Dunn.Proc.From |  |  |  |
| `IsActiveEntity` | `IsActiveEntity` | `Boolean` |  | Is active |  |  |  |


## Entity: `CustomerDunning`

- **ABAP Name:** `I_CustomerDunning`
- **Label:** Customer Company Code Dunning Fields
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `CompanyCode` | `CompanyCode` | `String(4)` | Y | Company Code |  | _CustomerCompany | S/4 only entity (no ECC CDC mapping) |
| `Customer` | `Customer` | `String(10)` | Y | Customer |  | _Customer | S/4 only entity (no ECC CDC mapping) |
| `DunningArea` | `DunningArea` | `String(2)` | Y | Dunning Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `LastDunnedOn` | `LastDunnedOn` | `Date` |  | Last Dunned |  |  | S/4 only entity (no ECC CDC mapping) |
| `DunningProcedure` | `DunningProcedure` | `String(4)` |  | Dunning Procedure |  | _DunningProcedure | S/4 only entity (no ECC CDC mapping) |
| `DunningLevel` | `DunningLevel` | `String(1)` |  | Dunning Level |  |  | S/4 only entity (no ECC CDC mapping) |
| `DunningBlock` | `DunningBlock` | `String(1)` |  | Dunning Block |  | _DunningBlock | S/4 only entity (no ECC CDC mapping) |
| `DunningRecipient` | `DunningRecipient` | `String(10)` |  | Dunning Recipient |  | _DunningRecipient | S/4 only entity (no ECC CDC mapping) |
| `LegDunningProcedureOn` | `LegDunningProcedureOn` | `Date` |  | Legal Dunn.Proc.From |  |  | S/4 only entity (no ECC CDC mapping) |
| `DunningClerk` | `DunningClerk` | `String(2)` |  | Dunning Clerk |  | _DunningClerk | S/4 only entity (no ECC CDC mapping) |


## Entity: `CustomerSalesArea`

- **ABAP Name:** `I_CustomerSalesArea`
- **Label:** Customer Sales Area
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Customer` | `Customer` | `String(10)` | Y | Customer |  | _Customer | S/4 only entity (no ECC CDC mapping) |
| `SalesOrganization` | `SalesOrganization` | `String(4)` | Y | Sales Organization |  | _SalesOrganization | S/4 only entity (no ECC CDC mapping) |
| `DistributionChannel` | `DistributionChannel` | `String(2)` | Y | Distribution Channel |  | _DistributionChannel | S/4 only entity (no ECC CDC mapping) |
| `Division` | `Division` | `String(2)` | Y | Division |  | _Division | S/4 only entity (no ECC CDC mapping) |
| `CustomerABCClassification` | `CustomerABCClassification` | `String(2)` |  | ABC Classification |  |  | S/4 only entity (no ECC CDC mapping) |
| `SalesOffice` | `SalesOffice` | `String(4)` |  | Sales Office |  | _SalesOffice | S/4 only entity (no ECC CDC mapping) |
| `SalesGroup` | `SalesGroup` | `String(3)` |  | Sales Group |  | _SalesGroup | S/4 only entity (no ECC CDC mapping) |
| `OrderIsBlockedForCustomer` | `OrderIsBlockedForCustomer` | `String(2)` |  | Ord.blk:sls ar. |  |  | S/4 only entity (no ECC CDC mapping) |
| `Currency` | `Currency` | `String(5)` |  | Currency |  | _Currency | S/4 only entity (no ECC CDC mapping) |
| `CustomerPriceGroup` | `CustomerPriceGroup` | `String(2)` |  | Customer Price Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `PriceListType` | `PriceListType` | `String(2)` |  | Price List Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `DeliveryPriority` | `DeliveryPriority` | `String(2)` |  | Delivery Priority |  | _DeliveryPriority | S/4 only entity (no ECC CDC mapping) |
| `ShippingCondition` | `ShippingCondition` | `String(2)` |  | Shipping Conditions |  | _ShippingCondition | S/4 only entity (no ECC CDC mapping) |
| `IncotermsClassification` | `IncotermsClassification` | `String(3)` |  | Incoterms |  | _IncotermsClassification | S/4 only entity (no ECC CDC mapping) |
| `SupplyingPlant` | `SupplyingPlant` | `String(4)` |  | Delivering Plant |  | _SupplyingPlant | S/4 only entity (no ECC CDC mapping) |
| `CompleteDeliveryIsDefined` | `CompleteDeliveryIsDefined` | `Boolean` |  | Complete Delivery |  |  | S/4 only entity (no ECC CDC mapping) |
| `DeliveryIsBlockedForCustomer` | `DeliveryIsBlockedForCustomer` | `String(2)` |  | DelBlckSalesAr. |  | _DeliveryIsBlockedForCustomer | S/4 only entity (no ECC CDC mapping) |
| `BillingIsBlockedForCustomer` | `BillingIsBlockedForCustomer` | `String(2)` |  | BBlock for SlsA |  | _BillingIsBlockedForCustomer | S/4 only entity (no ECC CDC mapping) |
| `CustomerPaymentTerms` | `CustomerPaymentTerms` | `String(4)` |  | Terms of Payment |  | _CustomerPaymentTerms | S/4 only entity (no ECC CDC mapping) |
| `CustomerAccountAssignmentGroup` | `CustomerAccountAssignmentGroup` | `String(2)` |  | Acct Assmt Grp Cust. |  |  | S/4 only entity (no ECC CDC mapping) |
| `AccountByCustomer` | `AccountByCustomer` | `String(12)` |  | Account at Customer |  |  | S/4 only entity (no ECC CDC mapping) |
| `CustomerGroup` | `CustomerGroup` | `String(2)` |  | Customer Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `CustomerPricingProcedure` | `CustomerPricingProcedure` | `String(2)` |  | Cust.Pric.Procedure |  |  | S/4 only entity (no ECC CDC mapping) |
| `OrderCombinationIsAllowed` | `OrderCombinationIsAllowed` | `Boolean` |  | Order Combination |  |  | S/4 only entity (no ECC CDC mapping) |
| `PartialDeliveryIsAllowed` | `PartialDeliveryIsAllowed` | `String(1)` |  | Partial Deliv./Item |  |  | S/4 only entity (no ECC CDC mapping) |
| `InvoiceDate` | `InvoiceDate` | `String(2)` |  | Invoicing Dates |  |  | S/4 only entity (no ECC CDC mapping) |
| `PaymentTerms` | `PaymentTerms` | `String(4)` |  | Terms of Payment |  |  | S/4 only entity (no ECC CDC mapping) |
| `IncotermsTransferLocation` | `IncotermsTransferLocation` | `String(28)` |  | Incoterms (Part 2) |  |  | S/4 only entity (no ECC CDC mapping) |
| `ItemOrderProbabilityInPercent` | `ItemOrderProbabilityInPercent` | `String(3)` |  | Order Probability |  |  | S/4 only entity (no ECC CDC mapping) |
| `IncotermsLocation2` | `IncotermsLocation2` | `String(70)` |  | Incoterms Location 2 |  |  | S/4 only entity (no ECC CDC mapping) |
| `RecordCreatedDate` | `RecordCreatedDate` | `Date` |  | Created On |  |  | S/4 only entity (no ECC CDC mapping) |
| `AuthorizationGroup` | `AuthorizationGroup` | `String(4)` |  | Authorization Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `SalesDistrict` | `SalesDistrict` | `String(6)` |  | Sales District |  |  | S/4 only entity (no ECC CDC mapping) |
| `IncotermsVersion` | `IncotermsVersion` | `String(4)` |  | Incoterms Version |  |  | S/4 only entity (no ECC CDC mapping) |
| `IncotermsLocation1` | `IncotermsLocation1` | `String(70)` |  | Incoterms Location 1 |  |  | S/4 only entity (no ECC CDC mapping) |
| `DeletionIndicator` | `DeletionIndicator` | `Boolean` |  | Del.ID SlsArea |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsBusinessPurposeCompleted` | `IsBusinessPurposeCompleted` | `Boolean` |  | Purpose Completed |  |  | S/4 only entity (no ECC CDC mapping) |
| `SalesItemProposal` | `SalesItemProposal` | `String(10)` |  | Item proposal |  |  | S/4 only entity (no ECC CDC mapping) |
| `CustProdProposalProcedure` | `CustProdProposalProcedure` | `String(2)` |  | PP customer proced. |  | _CustProdProposalProcedure | S/4 only entity (no ECC CDC mapping) |
| `ProofOfDeliveryTime` | `ProofOfDeliveryTime` | `String(6)` |  |  |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProofOfDeliveryTimeValue` | `ProofOfDeliveryTimeValue` | `Decimal(6,2)` |  | POD timeframe |  |  | S/4 only entity (no ECC CDC mapping) |
| `MaxNmbrOfPartialDelivery` | `MaxNmbrOfPartialDelivery` | `Decimal(1,0)` |  | Max.Part.Deliveries |  |  | S/4 only entity (no ECC CDC mapping) |
| `UnderdelivTolrtdLmtRatioInPct` | `UnderdelivTolrtdLmtRatioInPct` | `Decimal(3,1)` |  | Underdel. Tolerance |  |  | S/4 only entity (no ECC CDC mapping) |
| `OverdelivTolrtdLmtRatioInPct` | `OverdelivTolrtdLmtRatioInPct` | `Decimal(3,1)` |  | Overdeliv. Tolerance |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsActiveEntity` | `IsActiveEntity` | `Boolean` |  | Is active |  |  | S/4 only entity (no ECC CDC mapping) |
| `AdditionalCustomerGroup1` | `AdditionalCustomerGroup1` | `String(3)` |  | Customer Group 1 |  |  | S/4 only entity (no ECC CDC mapping) |
| `AdditionalCustomerGroup2` | `AdditionalCustomerGroup2` | `String(3)` |  | Customer Group 2 |  |  | S/4 only entity (no ECC CDC mapping) |
| `AdditionalCustomerGroup3` | `AdditionalCustomerGroup3` | `String(3)` |  | Customer Group 3 |  |  | S/4 only entity (no ECC CDC mapping) |
| `AdditionalCustomerGroup4` | `AdditionalCustomerGroup4` | `String(3)` |  | Customer Group 4 |  |  | S/4 only entity (no ECC CDC mapping) |
| `AdditionalCustomerGroup5` | `AdditionalCustomerGroup5` | `String(3)` |  | Customer Group 5 |  |  | S/4 only entity (no ECC CDC mapping) |
| `InvoiceListSchedule` | `InvoiceListSchedule` | `String(2)` |  | Invoice List Sched. |  | _FactoryCalendar | S/4 only entity (no ECC CDC mapping) |
| `ExchangeRateType` | `ExchangeRateType` | `String(4)` |  | Exchange Rate Type |  | _ExchangeRateType | S/4 only entity (no ECC CDC mapping) |
| `PaymentGuaranteeProcedure` | `PaymentGuaranteeProcedure` | `String(4)` |  | Paymt guarant. proc. |  | _PaytGuarProcedVH | S/4 only entity (no ECC CDC mapping) |
| `SuplrIsRlvtForSettlmtMgmt` | `SuplrIsRlvtForSettlmtMgmt` | `Boolean` |  | Settlement Mgmt. |  |  | S/4 only entity (no ECC CDC mapping) |
| `CustIsRlvtForSettlmtMgmt` | `CustIsRlvtForSettlmtMgmt` | `Boolean` |  | Settlement Mgmt. |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductUnitGroup` | `ProductUnitGroup` | `String(4)` |  | Unit of Measure Grp |  |  | S/4 only entity (no ECC CDC mapping) |
| `SlsDocIsRlvtForProofOfDeliv` | `SlsDocIsRlvtForProofOfDeliv` | `Boolean` |  | Relevant for POD |  |  | S/4 only entity (no ECC CDC mapping) |
| `SlsUnlmtdOvrdelivIsAllwd` | `SlsUnlmtdOvrdelivIsAllwd` | `Boolean` |  | Unlimited Tolerance |  |  | S/4 only entity (no ECC CDC mapping) |
| `CreditControlArea` | `CreditControlArea` | `String(4)` |  | Credit Control Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `CustomerIsRebateRelevant` | `CustomerIsRebateRelevant` | `Boolean` |  | Rebate |  |  | S/4 only entity (no ECC CDC mapping) |
| `InspSbstHasNoTimeOrQuantity` | `InspSbstHasNoTimeOrQuantity` | `Boolean` |  | Price determination |  |  | S/4 only entity (no ECC CDC mapping) |
| `ManualInvoiceMaintIsRelevant` | `ManualInvoiceMaintIsRelevant` | `Boolean` |  | Man. Invoice Maint. |  |  | S/4 only entity (no ECC CDC mapping) |
| `IncotermsSupChnLoc1AddlUUID` | `IncotermsSupChnLoc1AddlUUID` | `UUID` |  | Location UUID |  |  | S/4 only entity (no ECC CDC mapping) |
| `IncotermsSupChnLoc2AddlUUID` | `IncotermsSupChnLoc2AddlUUID` | `UUID` |  | Location UUID |  |  | S/4 only entity (no ECC CDC mapping) |
| `IncotermsSupChnDvtgLocAddlUUID` | `IncotermsSupChnDvtgLocAddlUUID` | `UUID` |  | Location UUID |  |  | S/4 only entity (no ECC CDC mapping) |
| `SalesBlockForCustomer` | `SalesBlockForCustomer` | `String(2)` |  | Sales Block |  |  | S/4 only entity (no ECC CDC mapping) |
| `CustomerStatisticsGroup` | `CustomerStatisticsGroup` | `String(1)` |  | Customer Stats.Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `RetailAdditionalCustomerGrp6` | `RetailAdditionalCustomerGrp6` | `String(3)` |  | Customer Group 6 |  |  | S/4 only entity (no ECC CDC mapping) |
| `RetailAdditionalCustomerGrp7` | `RetailAdditionalCustomerGrp7` | `String(3)` |  | Customer Group 7 |  |  | S/4 only entity (no ECC CDC mapping) |
| `RetailAdditionalCustomerGrp8` | `RetailAdditionalCustomerGrp8` | `String(3)` |  | Customer Group 8 |  |  | S/4 only entity (no ECC CDC mapping) |
| `RetailAdditionalCustomerGrp9` | `RetailAdditionalCustomerGrp9` | `String(3)` |  | Customer Group 9 |  |  | S/4 only entity (no ECC CDC mapping) |
| `RetailAdditionalCustomerGrp10` | `RetailAdditionalCustomerGrp10` | `String(3)` |  | Customer Group 10 |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `CustomerSalesAreaTax`

- **ABAP Name:** `I_CustSalesAreaTax`
- **Label:** Customer Sales Area Tax
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Customer` | `Customer` | `String(10)` | Y | Customer |  | _Customer | S/4 only entity (no ECC CDC mapping) |
| `SalesOrganization` | `SalesOrganization` | `String(4)` | Y | Sales Organization |  | _SalesOrganization | S/4 only entity (no ECC CDC mapping) |
| `DistributionChannel` | `DistributionChannel` | `String(2)` | Y | RefDistCh-Cust/Mat. |  | _DistributionChannel | S/4 only entity (no ECC CDC mapping) |
| `Division` | `Division` | `String(2)` | Y | Division |  | _Division | S/4 only entity (no ECC CDC mapping) |
| `DepartureCountry` | `DepartureCountry` | `String(3)` | Y | Departure Ctry/Reg. |  | _Country | S/4 only entity (no ECC CDC mapping) |
| `CustomerTaxCategory` | `CustomerTaxCategory` | `String(4)` | Y | Tax Condition Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `CustomerTaxClassification` | `CustomerTaxClassification` | `String(1)` |  | Tax Classification |  |  | S/4 only entity (no ECC CDC mapping) |
| `AuthorizationGroup` | `AuthorizationGroup` | `String(4)` |  | Authorization |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsBusinessPurposeCompleted` | `IsBusinessPurposeCompleted` | `Boolean` |  | Purpose Completed |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `CustomerUnloadingPoint`

- **ABAP Name:** `I_CustomerUnloadingPoint`
- **Label:** Customer Unloading Point
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Customer` | `Customer` | `String(10)` | Y | Customer |  | _Customer | S/4 only entity (no ECC CDC mapping) |
| `UnloadingPointName` | `UnloadingPointName` | `String(25)` | Y | Unloading Point |  |  | S/4 only entity (no ECC CDC mapping) |
| `CustomerFactoryCalenderCode` | `CustomerFactoryCalenderCode` | `String(2)` |  | Cust.fact.calendar |  |  | S/4 only entity (no ECC CDC mapping) |
| `BPGoodsReceivingHoursCode` | `BPGoodsReceivingHoursCode` | `String(3)` |  | Goods receiving hrs |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsDfltBPUnloadingPoint` | `IsDfltBPUnloadingPoint` | `Boolean` |  | Default unloading pt |  |  | S/4 only entity (no ECC CDC mapping) |
| `MondayMorningOpeningTime` | `MondayMorningOpeningTime` | `String(6)` |  | Monday |  |  | S/4 only entity (no ECC CDC mapping) |
| `MondayMorningClosingTime` | `MondayMorningClosingTime` | `String(6)` |  | Monday |  |  | S/4 only entity (no ECC CDC mapping) |
| `MondayAfternoonOpeningTime` | `MondayAfternoonOpeningTime` | `String(6)` |  | Monday |  |  | S/4 only entity (no ECC CDC mapping) |
| `MondayAfternoonClosingTime` | `MondayAfternoonClosingTime` | `String(6)` |  | Monday |  |  | S/4 only entity (no ECC CDC mapping) |
| `TuesdayMorningOpeningTime` | `TuesdayMorningOpeningTime` | `String(6)` |  | Tuesday |  |  | S/4 only entity (no ECC CDC mapping) |
| `TuesdayMorningClosingTime` | `TuesdayMorningClosingTime` | `String(6)` |  | Tuesday |  |  | S/4 only entity (no ECC CDC mapping) |
| `TuesdayAfternoonOpeningTime` | `TuesdayAfternoonOpeningTime` | `String(6)` |  | Tuesday |  |  | S/4 only entity (no ECC CDC mapping) |
| `TuesdayAfternoonClosingTime` | `TuesdayAfternoonClosingTime` | `String(6)` |  | Tuesday |  |  | S/4 only entity (no ECC CDC mapping) |
| `WednesdayMorningOpeningTime` | `WednesdayMorningOpeningTime` | `String(6)` |  | Wednesday |  |  | S/4 only entity (no ECC CDC mapping) |
| `WednesdayMorningClosingTime` | `WednesdayMorningClosingTime` | `String(6)` |  | Wednesday |  |  | S/4 only entity (no ECC CDC mapping) |
| `WednesdayAfternoonOpeningTime` | `WednesdayAfternoonOpeningTime` | `String(6)` |  | Wednesday |  |  | S/4 only entity (no ECC CDC mapping) |
| `WednesdayAfternoonClosingTime` | `WednesdayAfternoonClosingTime` | `String(6)` |  | Wednesday |  |  | S/4 only entity (no ECC CDC mapping) |
| `ThursdayMorningOpeningTime` | `ThursdayMorningOpeningTime` | `String(6)` |  | Thursday |  |  | S/4 only entity (no ECC CDC mapping) |
| `ThursdayMorningClosingTime` | `ThursdayMorningClosingTime` | `String(6)` |  | Thursday |  |  | S/4 only entity (no ECC CDC mapping) |
| `ThursdayAfternoonOpeningTime` | `ThursdayAfternoonOpeningTime` | `String(6)` |  | Thursday |  |  | S/4 only entity (no ECC CDC mapping) |
| `ThursdayAfternoonClosingTime` | `ThursdayAfternoonClosingTime` | `String(6)` |  | Thursday |  |  | S/4 only entity (no ECC CDC mapping) |
| `FridayMorningOpeningTime` | `FridayMorningOpeningTime` | `String(6)` |  | Friday |  |  | S/4 only entity (no ECC CDC mapping) |
| `FridayMorningClosingTime` | `FridayMorningClosingTime` | `String(6)` |  | Friday |  |  | S/4 only entity (no ECC CDC mapping) |
| `FridayAfternoonOpeningTime` | `FridayAfternoonOpeningTime` | `String(6)` |  | Friday |  |  | S/4 only entity (no ECC CDC mapping) |
| `FridayAfternoonClosingTime` | `FridayAfternoonClosingTime` | `String(6)` |  | Friday |  |  | S/4 only entity (no ECC CDC mapping) |
| `SaturdayMorningOpeningTime` | `SaturdayMorningOpeningTime` | `String(6)` |  | Saturday |  |  | S/4 only entity (no ECC CDC mapping) |
| `SaturdayMorningClosingTime` | `SaturdayMorningClosingTime` | `String(6)` |  | Saturday |  |  | S/4 only entity (no ECC CDC mapping) |
| `SaturdayAfternoonOpeningTime` | `SaturdayAfternoonOpeningTime` | `String(6)` |  | Saturday |  |  | S/4 only entity (no ECC CDC mapping) |
| `SaturdayAfternoonClosingTime` | `SaturdayAfternoonClosingTime` | `String(6)` |  | Saturday |  |  | S/4 only entity (no ECC CDC mapping) |
| `SundayMorningOpeningTime` | `SundayMorningOpeningTime` | `String(6)` |  | Sunday |  |  | S/4 only entity (no ECC CDC mapping) |
| `SundayMorningClosingTime` | `SundayMorningClosingTime` | `String(6)` |  | Sunday |  |  | S/4 only entity (no ECC CDC mapping) |
| `SundayAfternoonOpeningTime` | `SundayAfternoonOpeningTime` | `String(6)` |  | Sunday |  |  | S/4 only entity (no ECC CDC mapping) |
| `SundayAfternoonClosingTime` | `SundayAfternoonClosingTime` | `String(6)` |  | Sunday |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `CustomerWithHoldingTax`

- **ABAP Name:** `I_CustomerWithTax`
- **Label:** Customer WithHolding Tax
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Customer` | `Customer` | `String(10)` | Y | Customer |  | _Customer | S/4 only entity (no ECC CDC mapping) |
| `CompanyCode` | `CompanyCode` | `String(4)` | Y | Company Code |  | _CompanyCode | S/4 only entity (no ECC CDC mapping) |
| `WithholdingTaxType` | `WithholdingTaxType` | `String(2)` | Y | Withholding Tax Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `WithholdingTaxCode` | `WithholdingTaxCode` | `String(2)` |  | W/Tax Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `WithholdingTaxAgent` | `WithholdingTaxAgent` | `Boolean` |  | WTax Agent |  |  | S/4 only entity (no ECC CDC mapping) |
| `ObligationDateBegin` | `ObligationDateBegin` | `Date` |  | W/Tax Obligated Frm |  |  | S/4 only entity (no ECC CDC mapping) |
| `ObligationDateEnd` | `ObligationDateEnd` | `Date` |  | Oblig.to W/Tax Until |  |  | S/4 only entity (no ECC CDC mapping) |
| `WithholdingTaxNumber` | `WithholdingTaxNumber` | `String(16)` |  | W/tax number |  |  | S/4 only entity (no ECC CDC mapping) |
| `WithholdingTaxCertificate` | `WithholdingTaxCertificate` | `String(25)` |  | Exemption Number |  |  | S/4 only entity (no ECC CDC mapping) |
| `WithholdingTaxExmptPercent` | `WithholdingTaxExmptPercent` | `Decimal(5,2)` |  | Exemption Rate |  |  | S/4 only entity (no ECC CDC mapping) |
| `ExemptionDateBegin` | `ExemptionDateBegin` | `Date` |  | Exemption Start Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `ExemptionDateEnd` | `ExemptionDateEnd` | `Date` |  | Exemption End Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `ExemptionReason` | `ExemptionReason` | `String(2)` |  | Exemption Reason |  |  | S/4 only entity (no ECC CDC mapping) |
