# Supplier

> Source file: `sap-s4com-Supplier-v1.json`

**Technical Name:** `` | **Data Category:** `DIMENSION` | **VDM Type:** `BASIC` | **Size:** `XL`


## Entity: `Supplier`

- **ABAP Name:** `I_Supplier`
- **Label:** Supplier
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** LFA1, ADRC

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `Supplier` | `LFA1` | `LIFNR` | `String(10)` | Y | Supplier |  |  |  |
| `SupplierAccountGroup` | `LFA1` | `KTOKK` | `String(4)` |  | Account Group |  |  |  |
| `SupplierName` |  |  | `String(80)` |  | Name of Supplier |  |  |  |
| `SupplierFullName` | `LFA1` | `NAME1` | `String(220)` |  | Supplier Name |  |  |  |
| `BPSupplierName` |  |  | `String(81)` |  | Business Partner - Supplier Name |  |  |  |
| `BPSupplierFullName` |  |  | `String(163)` |  | Business Partner - Supplier Full Name |  |  |  |
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
| `IsBusinessPurposeCompleted` |  |  | `Boolean` |  | Purpose Completed |  |  |  |
| `CreatedByUser` |  |  | `String(12)` |  | Created By |  |  |  |
| `CreationDate` |  |  | `Date` |  | Created On |  |  |  |
| `IsOneTimeAccount` |  |  | `Boolean` |  | One-Time Account |  |  |  |
| `AuthorizationGroup` |  |  | `String(4)` |  | Authorization |  |  |  |
| `VATRegistration` |  |  | `String(20)` |  | VAT Registration No. |  |  |  |
| `AccountIsBlockedForPosting` |  |  | `Boolean` |  | Posting Block(Deprecated) |  |  |  |
| `TaxJurisdiction` |  |  | `String(15)` |  | Tax Jurisdiction |  |  |  |
| `SupplierStandardCarrierAccess` |  |  | `String(4)` |  | SCAC |  |  |  |
| `SupplierFwdAgentFreightGroup` |  |  | `String(4)` |  | Carrier freight grp |  |  |  |
| `SupplierAgentProcedureGroup` |  |  | `String(4)` |  | ServAgntProcGrp |  |  |  |
| `SupplIsSocialInsuranceRegtrd` |  |  | `Boolean` |  | Social Insurance |  |  |  |
| `SocialInsuranceActivityCode` |  |  | `String(3)` |  | Social Ins. Code |  |  |  |
| `SupplierCorporateGroup` |  |  | `String(10)` |  | Group Key |  |  |  |
| `Customer` |  |  | `String(10)` |  | Customer |  |  |  |
| `Industry` |  |  | `String(4)` |  | Industry |  |  |  |
| `TaxNumber1` |  |  | `String(16)` |  | Tax Number 1 |  |  |  |
| `TaxNumber2` |  |  | `String(11)` |  | Tax Number 2 |  |  |  |
| `TaxNumber3` |  |  | `String(18)` |  | Tax Number 3 |  |  |  |
| `TaxNumber4` |  |  | `String(18)` |  | Tax Number 4 |  |  |  |
| `TaxNumber5` |  |  | `String(60)` |  | Tax Number 5 |  |  |  |
| `TaxNumber6` |  |  | `String(20)` |  | Tax Number 6 |  |  |  |
| `PostingIsBlocked` |  |  | `Boolean` |  | Posting Block |  |  |  |
| `PurchasingIsBlocked` |  |  | `Boolean` |  | Purch. Block |  |  |  |
| `InternationalLocationNumber1` |  |  | `String(7)` |  | Int. location no. 1 |  |  |  |
| `InternationalLocationNumber2` |  |  | `String(5)` |  | Int. location no. 2 |  |  |  |
| `InternationalLocationNumber3` |  |  | `String(1)` |  | Check Digit |  |  |  |
| `AddressID` |  |  | `String(10)` |  | Address |  |  |  |
| `Region` | `LFA1` | `REGIO` | `String(3)` |  | Region |  |  |  |
| `OrganizationBPName1` |  |  | `String(35)` |  | Name |  |  |  |
| `OrganizationBPName2` |  |  | `String(35)` |  | Name 2 |  |  |  |
| `CityName` | `LFA1` | `ORT01` | `String(35)` |  | City |  |  |  |
| `PostalCode` | `LFA1` | `PSTLZ` | `String(10)` |  | Postal Code |  |  |  |
| `StreetName` | `LFA1` | `STRAS` | `String(35)` |  | Street |  |  |  |
| `Country` | `LFA1` | `LAND1` | `String(3)` |  | Country/Region Key |  |  |  |
| `ConcatenatedInternationalLocNo` |  |  | `String(20)` |  | Int. Location No. |  |  |  |
| `SupplierProcurementBlock` |  |  | `String(2)` |  | Block Function |  |  |  |
| `SuplrQualityManagementSystem` |  |  | `String(4)` |  | Actual QM System |  |  |  |
| `SuplrQltyInProcmtCertfnValidTo` |  |  | `Date` |  | QM System Valid To |  |  |  |
| `SupplierLanguage` |  |  | `String(2)` |  | Language Key |  |  |  |
| `AlternativePayeeAccountNumber` |  |  | `String(10)` |  | Alternative Payee |  |  |  |
| `PhoneNumber1` | `LFA1` | `TELF1` | `String(16)` |  | Telephone 1 |  |  |  |
| `FaxNumber` |  |  | `String(31)` |  | Fax Number |  |  |  |
| `IsNaturalPerson` |  |  | `Boolean` |  | Natural Person |  |  |  |
| `TaxNumberResponsible` |  |  | `String(18)` |  | Tax Number |  |  |  |
| `UK_ContractorBusinessType` |  |  | `String(12)` |  | Business Type |  |  |  |
| `UK_PartnerTradingName` |  |  | `String(30)` |  | Prtnr's Trading Name |  |  |  |
| `UK_PartnerTaxReference` |  |  | `String(20)` |  | Partner's UTR |  |  |  |
| `UK_VerificationStatus` |  |  | `String(3)` |  | Verification Status |  |  |  |
| `UK_VerificationNumber` |  |  | `String(20)` |  | Verification Number |  |  |  |
| `UK_CompanyRegistrationNumber` |  |  | `String(8)` |  | Comp. House Reg. No. |  |  |  |
| `UK_VerifiedTaxStatus` |  |  | `String(1)` |  | Tax Status |  |  |  |
| `FormOfAddress` |  |  | `String(15)` |  | Title |  |  |  |
| `ReferenceAccountGroup` |  |  | `String(4)` |  | Reference Acct Group |  |  |  |
| `VATLiability` |  |  | `Boolean` |  | Liable for VAT |  |  |  |
| `ResponsibleType` |  |  | `String(2)` |  | Tax Type |  |  |  |
| `TaxNumberType` |  |  | `String(2)` |  | Tax Number Type |  |  |  |
| `FiscalAddress` |  |  | `String(10)` |  | Fiscal Address |  |  |  |
| `BusinessType` |  |  | `String(30)` |  | Type of Business |  |  |  |
| `BirthDate` |  |  | `Date` |  | Date of Birth |  |  |  |
| `PaymentIsBlockedForSupplier` |  |  | `Boolean` |  | Payment Block |  |  |  |
| `SortField` |  |  | `String(10)` |  | Search Term |  |  |  |
| `PhoneNumber2` |  |  | `String(16)` |  | Telephone 2 |  |  |  |
| `DeletionIndicator` |  |  | `Boolean` |  | Deletion Flag |  |  |  |
| `TaxInvoiceRepresentativeName` |  |  | `String(10)` |  | Rep's Name |  |  |  |
| `IndustryType` |  |  | `String(30)` |  | Type of Industry |  |  |  |
| `IN_GSTSupplierClassification` |  |  | `String(1)` |  | GST Ven Class. |  |  |  |
| `SuplrProofOfDelivRlvtCode` |  |  | `String(1)` |  | Relevant for POD |  |  |  |
| `TradingPartner` |  |  | `String(6)` |  | Trading Partner No. |  |  |  |
| `BR_TaxIsSplit` |  |  | `Boolean` |  | Tax Split |  |  |  |
| `AU_PayerIsPayingToCarryOnEnt` |  |  | `String(1)` |  | Enterprise in AU |  |  |  |
| `AU_IndividualIsUnder18` |  |  | `String(1)` |  | Individual |  |  |  |
| `AU_PaymentIsExceeding75` |  |  | `String(1)` |  | Payment Does not Exc |  |  |  |
| `AU_PaymentIsWhollyInputTaxed` |  |  | `String(1)` |  | Wholly Input Taxed |  |  |  |
| `AU_PartnerIsSupplyWithoutGain` |  |  | `String(1)` |  | Individual w/o Gain |  |  |  |
| `AU_SupplierIsEntitledToABN` |  |  | `String(1)` |  | ABN Eligible |  |  |  |
| `AU_PaymentIsIncomeExempted` |  |  | `String(1)` |  | Payment Exempt |  |  |  |
| `AU_SupplyIsMadeAsPrivateHobby` |  |  | `String(1)` |  | Hobby |  |  |  |
| `AU_SupplyMadeIsOfDmstcNature` |  |  | `String(1)` |  | Domestic |  |  |  |
| `IsToBeAcceptedAtOrigin` |  |  | `Boolean` |  | Origin Acceptance |  |  |  |
| `BPIsEqualizationTaxSubject` |  |  | `Boolean` |  |  |  |  |  |
| `BRSpcfcTaxBasePercentageCode` |  |  | `String(1)` |  | Tax Base |  |  |  |
| `SupplierProfession` |  |  | `String(30)` |  | Profession |  |  |  |
| `SuplrManufacturerExternalName` |  |  | `String(10)` |  | Ext. manufacturer |  |  |  |
| `DataMediumExchangeIndicator` |  |  | `String(1)` |  | DME Recipient Code |  |  |  |
| `DataExchangeInstructionKey` |  |  | `String(2)` |  | Instruction Key |  |  |  |
| `SupplierIsSubRangeRelevant` |  |  | `Boolean` |  | VSR Relevant |  |  |  |
| `TrainStationName` |  |  | `String(25)` |  | Train Station |  |  |  |
| `AlternativePayeeIsAllowed` |  |  | `Boolean` |  | Payee in Document |  |  |  |
| `PaytSlipWthRefSubscriber` |  |  | `String(11)` |  | PBC/ISR Number |  |  |  |
| `TranspServiceAgentStstcGrp` |  |  | `String(2)` |  | Stat. Grp, Agent |  |  |  |
| `SupplierIsPlantRelevant` |  |  | `Boolean` |  | Plant Level Relevant |  |  |  |
| `SuplrTaxAuthorityAccountNumber` |  |  | `String(10)` |  | Tax Office |  |  |  |
| `SuplrCarrierConfirmIsExpected` |  |  | `String(1)` |  | Carrier confirmation |  |  |  |
| `SupplierPlant` |  |  | `String(4)` |  | Plant |  |  |  |
| `FactoryCalendar` |  |  | `String(2)` |  | Factory Calendar |  |  |  |
| `PaymentReason` |  |  | `String(4)` |  | Payment Reason |  |  |  |
| `SupplierCentralDeletionIsBlock` |  |  | `Boolean` |  | Central Del. Block |  |  |  |
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
| `SupplierTransportationChain` |  |  | `String(10)` |  | Transportation Chain |  |  |  |
| `SupplierStagingTimeInDays` |  |  | `Decimal(3,0)` |  | Staging Time |  |  |  |
| `SupplierSchedulingProcedure` |  |  | `String(1)` |  | Scheduling Procedure |  |  |  |
| `CollectiveNumberingIsRelevant` |  |  | `Boolean` |  | Rel. for Coll. No. |  |  |  |
| `BusinessPartnerPanNumber` |  |  | `String(40)` |  | PAN |  |  |  |
| `BPPanReferenceNumber` |  |  | `String(40)` |  | PAN Reference Number |  |  |  |
| `BPPanValidFromDate` |  |  | `Date` |  | PAN Valid From Date |  |  |  |


## Entity: `SupplierCompanyCode`

- **ABAP Name:** `I_SupplierCompany`
- **Label:** Supplier Company
- **VDM Type:** `BASIC` | **Data Category:** `FACT`
- **ECC Source Tables:** t001, lfb1

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `Supplier` | `LFA1` | `LIFNR` | `String(10)` | Y | Supplier |  | _Supplier |  |
| `CompanyCode` | `LFB1` | `BUKRS` | `String(4)` | Y | Company Code |  | _CompanyCode |  |
| `AuthorizationGroup` |  |  | `String(4)` |  | Authorization |  |  |  |
| `CompanyCodeName` |  |  | `String(25)` |  | Company Name |  |  |  |
| `PaymentBlockingReason` | `LFB1` | `ZAHLS` | `String(1)` |  | Payment Block |  |  |  |
| `SupplierIsBlockedForPosting` |  |  | `Boolean` |  | Co.code post.block |  |  |  |
| `IsBusinessPurposeCompleted` |  |  | `Boolean` |  | Purpose Completed |  |  |  |
| `AccountingClerk` |  |  | `String(2)` |  | Clerk Abbrev. |  |  |  |
| `AccountingClerkFaxNumber` |  |  | `String(31)` |  | Acctg clerk's fax |  |  |  |
| `AccountingClerkPhoneNumber` |  |  | `String(30)` |  | Acct.clerks tel.no. |  |  |  |
| `AccountingClerkInternetAddress` |  |  | `String(130)` |  | Clrk's internet add. |  |  |  |
| `SupplierClerk` |  |  | `String(15)` |  | Clerk at vendor |  |  |  |
| `SupplierClerkURL` |  |  | `String(130)` |  | Clrk's internet add. |  |  |  |
| `PaymentMethodsList` |  |  | `String(10)` |  | Payment Methods |  |  |  |
| `PaymentTerms` | `LFB1` | `ZTERM` | `String(4)` |  | Terms of Payment |  |  |  |
| `ClearCustomerSupplier` |  |  | `Boolean` |  | Clearing w/ Customer |  |  |  |
| `IsToBeLocallyProcessed` |  |  | `Boolean` |  | Local Processing |  |  |  |
| `ItemIsToBePaidSeparately` |  |  | `Boolean` |  | Individual Payment |  |  |  |
| `PaymentIsToBeSentByEDI` |  |  | `Boolean` |  | Pmnt advice by EDI |  |  |  |
| `HouseBank` |  |  | `String(5)` |  | House Bank |  |  |  |
| `CheckPaidDurationInDays` |  |  | `Decimal(3,0)` |  | Check Cashing Time |  |  |  |
| `Currency` | `LFB1` | `WAERS` | `String(5)` |  | Currency |  |  |  |
| `BillOfExchLmtAmtInCoCodeCrcy` |  |  | `Decimal(34,4)` |  | Bill/Ex. Limit | Currency |  |  |
| `SupplierClerkIDBySupplier` |  |  | `String(12)` |  | Account with vendor |  |  |  |
| `IsDoubleInvoice` |  |  | `Boolean` |  | Check Double Invoice |  |  |  |
| `CustomerSupplierClearingIsUsed` |  |  | `Boolean` |  | Clearing w/ Customer |  |  |  |
| `ReconciliationAccount` | `LFB1` | `AKONT` | `String(10)` |  | Reconciliation Acct |  |  |  |
| `InterestCalculationCode` |  |  | `String(2)` |  | Interest Indicator |  |  |  |
| `InterestCalculationDate` |  |  | `Date` |  | Last Key Date |  |  |  |
| `IntrstCalcFrequencyInMonths` |  |  | `String(2)` |  | Int.Calc.Freq. |  |  |  |
| `SupplierHeadOffice` |  |  | `String(10)` |  | Head Office |  |  |  |
| `AlternativePayee` |  |  | `String(10)` |  | Alternative payee |  |  |  |
| `LayoutSortingRule` |  |  | `String(3)` |  | Sort key |  |  |  |
| `APARToleranceGroup` |  |  | `String(4)` |  | Tolerance Group |  |  |  |
| `SuplrInvcVerificatTolGroup` |  |  | `String(4)` |  | Tolerance Group |  |  |  |
| `SupplierCertificationDate` |  |  | `Date` |  | Certification Date |  |  |  |
| `SupplierAccountNote` |  |  | `String(30)` |  | Account Memo |  |  |  |
| `WithholdingTaxCountry` |  |  | `String(3)` |  | WTax C/R Key |  |  |  |
| `DeletionIndicator` |  |  | `Boolean` |  | Co.Cde Deletion Flag |  |  |  |
| `CashPlanningGroup` |  |  | `String(10)` |  | Planning Group |  |  |  |
| `IsToBeCheckedForDuplicates` |  |  | `Boolean` |  | Check Double Invoice |  |  |  |
| `PersonnelNumber` |  |  | `String(8)` |  | Personnel Number |  |  |  |
| `PreviousAccountNumber` |  |  | `String(10)` |  | Previous Account No. |  |  |  |
| `MinorityGroup` |  |  | `String(3)` |  | Minority Indicator |  |  |  |
| `LastInterestCalcRunDate` |  |  | `Date` |  | Last Int. Calc. |  |  |  |
| `US_ForeignSuplrHasPartnership` |  |  | `String(1)` |  | Partnership Int Ind |  |  |  |
| `US_SecondTINNoticeIsIssued` |  |  | `String(1)` |  | Second TIN Notice |  |  |  |
| `US_ForeignSuplrLmtnOnBnftCode` |  |  | `String(2)` |  | LOB Treaty Code |  |  |  |
| `SupplierReleaseGroup` |  |  | `String(4)` |  | Release Group |  |  |  |
| `CreditMemoPaymentTerms` |  |  | `String(4)` |  | Credit Memo Pyt Term |  |  |  |
| `PaymentMethodSupplement` |  |  | `String(2)` |  | Pmt Meth. Supplement |  |  |  |
| `US_FrgnAcctTaxFilingIsRequired` |  |  | `String(1)` |  | FATCA Ind |  |  |  |
| `US_RecipientForeignTaxID` |  |  | `String(22)` |  | US Recipient FTID |  |  |  |
| `US_FW9ReceiveDate` |  |  | `Date` |  | W9 Form Rec Date |  |  |  |
| `US_FW8BENReceiveDate` |  |  | `Date` |  | W8 Form Rec Date |  |  |  |
| `US_FrgnAcctTaxRcpntCntry` |  |  | `String(3)` |  | Country/Region Key |  |  |  |
| `US_GlobIntermediaryIdnNumber` |  |  | `String(19)` |  | US Recipient GIIN |  |  |  |
| `US_LobTreatyCode` |  |  | `String(2)` |  | LOB Treaty Code |  |  |  |
| `US_Chapter4StatusCode` |  |  | `String(2)` |  | Chaptr 4 Status Code |  |  |  |
| `PaymentClearingGroup` |  |  | `String(8)` |  | Payment Clrg Grp ID |  |  |  |
| `PaymentReason` |  |  | `String(4)` |  | Payment Reason |  |  |  |
| `DeletionIsBlocked` |  |  | `Boolean` |  | CoCd Deletion Block |  |  |  |
| `IsActiveEntity` |  |  | `Boolean` |  | Is active |  |  |  |
| `UK_ContractorBusinessType` |  |  | `String(12)` |  | Business Type |  |  |  |
| `UK_PartnerTradingName` |  |  | `String(30)` |  | Prtnr's Trading Name |  |  |  |
| `UK_PartnerTaxReference` |  |  | `String(20)` |  | Partner's UTR |  |  |  |
| `UK_VerificationStatus` |  |  | `String(3)` |  | Verification Status |  |  |  |
| `UK_VerificationNumber` |  |  | `String(20)` |  | Verification Number |  |  |  |
| `UK_CompanyRegistrationNumber` |  |  | `String(8)` |  | Comp. House Reg. No. |  |  |  |
| `UK_VerifiedTaxStatus` |  |  | `String(1)` |  | Tax Status |  |  |  |


## Entity: `SupplierPurchasingOrganization`

- **ABAP Name:** `I_SupplierPurchasingOrg`
- **Label:** Supplier Purchasing Organization
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** LFA1, LFM1

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `Supplier` |  |  | `String(10)` | Y | Supplier |  | _Supplier |  |
| `PurchasingOrganization` |  |  | `String(4)` | Y | Purch. Organization |  |  |  |
| `PurchasingGroup` |  |  | `String(3)` |  | Purchasing Group |  |  |  |
| `MaterialPlannedDeliveryDurn` |  |  | `Decimal(3,0)` |  | Planned Deliv. Time |  |  |  |
| `PurchasingIsBlockedForSupplier` |  |  | `Boolean` |  | Pur. block POrg |  |  |  |
| `SupplierRespSalesPersonName` |  |  | `String(30)` |  | Salesperson |  |  |  |
| `SupplierPhoneNumber` |  |  | `String(16)` |  | Telephone |  |  |  |
| `PurchaseOrderCurrency` |  |  | `String(5)` |  | Order currency |  |  |  |
| `MinimumOrderAmount` |  |  | `Decimal(34,4)` |  | Minimum order value | PurchaseOrderCurrency |  |  |
| `CalculationSchemaGroupCode` |  |  | `String(2)` |  | Schema Grp, Supplier |  |  |  |
| `PaymentTerms` |  |  | `String(4)` |  | Terms of Payment |  |  |  |
| `PricingDateControl` |  |  | `String(1)` |  | Pricing Date Control |  |  |  |
| `SupplierABCClassificationCode` |  |  | `String(1)` |  | ABC indicator |  |  |  |
| `ShippingCondition` |  |  | `String(2)` |  | Shipping Conditions |  |  |  |
| `PurOrdAutoGenerationIsAllowed` |  |  | `Boolean` |  | Automatic PO |  |  |  |
| `InvoiceIsGoodsReceiptBased` |  |  | `Boolean` |  | GR-Based Inv. Verif. |  |  |  |
| `IncotermsClassification` |  |  | `String(3)` |  | Incoterms |  |  |  |
| `IncotermsTransferLocation` |  |  | `String(28)` |  | Incoterms (Part 2) |  |  |  |
| `IncotermsVersion` |  |  | `String(4)` |  | Incoterms Version |  |  |  |
| `IncotermsLocation1` |  |  | `String(70)` |  | Incoterms Location 1 |  |  |  |
| `IncotermsLocation2` |  |  | `String(70)` |  | Incoterms Location 2 |  |  |  |
| `DeletionIndicator` |  |  | `Boolean` |  | Del. flag POrg. |  |  |  |
| `PlannedDeliveryDurationInDays` |  |  | `Decimal(3,0)` |  | Planned Deliv. Time |  |  |  |
| `ContactPersonPhoneNumber` |  |  | `String(16)` |  | Telephone |  |  |  |
| `SupplierConfirmationControlKey` |  |  | `String(4)` |  | Confirmation Control |  |  |  |
| `IsOrderAcknRqd` |  |  | `Boolean` |  | Acknowledgment Reqd. |  |  |  |
| `EvaldReceiptSettlementIsActive` |  |  | `Boolean` |  | Eval. Receipt Sett. |  |  |  |
| `AutomaticEvaluatedRcptSettlmt` |  |  | `Boolean` |  | Aut. ev. GRSetmt.Ret |  |  |  |
| `SupplierAccountNumber` |  |  | `String(12)` |  | Acc. with supplier |  |  |  |
| `SuplrIsSubjToSubsqntSettlement` |  |  | `Boolean` |  | Subseq. settlement |  |  |  |
| `SuplrPurgOrgAgrmtOfBusVolIsRqd` |  |  | `Boolean` |  | B.vol.comp./ag.nec. |  |  |  |
| `SuplrInvcRevalIsAllowed` |  |  | `Boolean` |  | Revaluation |  |  |  |
| `SuplrPurgOrgIsRlvtForPriceDetn` |  |  | `Boolean` |  | Price determination |  |  |  |
| `IntrastatCrsBorderTrMode` |  |  | `String(1)` |  | Mode of Transport |  |  |  |
| `ProductUnitGroup` |  |  | `String(4)` |  | Unit of Measure Grp |  |  |  |
| `RoundingProfile` |  |  | `String(4)` |  | Rounding Profile |  |  |  |
| `PlanningCycle` |  |  | `String(3)` |  | Planning Cycle |  |  |  |
| `SuplrDiscountInKindIsGranted` |  |  | `Boolean` |  |  |  |  |  |
| `SuplrIsRlvtForSettlmtMgmt` |  |  | `Boolean` |  | Settlement Mgmt. |  |  |  |
| `InvoiceIsMMServiceEntryBased` |  |  | `Boolean` |  | Srv.-Based Inv. Ver. |  |  |  |
| `ProdStockAndSlsDataTransfPrfl` |  |  | `String(4)` |  | PROACT control prof. |  |  |  |
| `EvaldRcptSettlementProfile` |  |  | `String(4)` |  | Settlement profile |  |  |  |
| `AbsoluteHandlingSurchargeAmt` |  |  | `Decimal(34,4)` |  | Absolute surcharge | PurchaseOrderCurrency |  |  |
| `PercentageHandlingSurchargeAmt` |  |  | `Decimal(5,2)` |  | Percentage HSC |  |  |  |
| `MinimumHandlingSurchargeAmt` |  |  | `Decimal(34,4)` |  | Minimum HSC | PurchaseOrderCurrency |  |  |
| `MaximumHandlingSurchargeAmt` |  |  | `Decimal(34,4)` |  | Max. HSC | PurchaseOrderCurrency |  |  |
| `AutomDebitCrtnIsEnbldOnGI` |  |  | `Boolean` |  | Auto. debit |  |  |  |
| `SupplierIsReturnsSupplier` |  |  | `Boolean` |  | Returns supplier |  |  |  |
| `IsActiveEntity` |  |  | `Boolean` |  | Is active |  |  |  |
| `IncotermsSupChnLoc1AddlUUID` |  |  | `UUID` |  | Location UUID |  |  |  |
| `IncotermsSupChnLoc2AddlUUID` |  |  | `UUID` |  | Location UUID |  |  |  |
| `IncotermsSupChnDvtgLocAddlUUID` |  |  | `UUID` |  | Location UUID |  |  |  |
| `AuthorizationGroup` |  |  | `String(4)` |  | Authorization |  |  |  |


## Entity: `SupplierWithHoldingTax`

- **ABAP Name:** `I_SupplierWithHoldingTax`
- **Label:** Supplier WithHolding Tax
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `Supplier` |  |  | `String(10)` | Y | Supplier |  | _Supplier | S/4 only entity |
| `CompanyCode` | `T001` | `BUKRS` | `String(4)` | Y | Company Code |  | _CompanyCode |  |
| `WithholdingTaxType` |  |  | `String(2)` | Y | Withholding Tax Type |  |  | S/4 only entity |
| `WithholdingTaxNumber` |  |  | `String(16)` |  | W/tax number |  |  | S/4 only entity |
| `WithholdingTaxCode` |  |  | `String(2)` |  | W/Tax Code |  |  | S/4 only entity |
| `IsWithholdingTaxSubject` |  |  | `Boolean` |  | Subject to W/Tx |  |  | S/4 only entity |
| `RecipientType` |  |  | `String(2)` |  | Recipient Type |  |  | S/4 only entity |
| `WithholdingTaxCertificate` |  |  | `String(25)` |  | Exemption Number |  |  | S/4 only entity |
| `WithholdingTaxExmptPercent` |  |  | `Decimal(5,2)` |  | Exemption Rate |  |  | S/4 only entity |
| `ExemptionDateBegin` |  |  | `Date` |  | Exemption Start Date |  |  | S/4 only entity |
| `ExemptionDateEnd` |  |  | `Date` |  | Exemption End Date |  |  | S/4 only entity |
| `ExemptionReason` |  |  | `String(2)` |  | Exemption Reason |  |  | S/4 only entity |
