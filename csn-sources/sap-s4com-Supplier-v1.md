# Supplier

> Source file: `sap-s4com-Supplier-v1.json`

**Technical Name:** `` | **Data Category:** `DIMENSION` | **VDM Type:** `BASIC` | **Size:** `XL`


## Entity: `Supplier`

- **ABAP Name:** `I_Supplier`
- **Label:** Supplier
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** LFA1, ADRC

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Supplier` | `Supplier` | `String(10)` | Y | Supplier |  |  |  |
| `SupplierAccountGroup` | `SupplierAccountGroup` | `String(4)` |  | Account Group |  |  |  |
| `SupplierName` | `SupplierName` | `String(80)` |  | Name of Supplier |  |  |  |
| `SupplierFullName` | `SupplierFullName` | `String(220)` |  | Supplier Name |  |  |  |
| `BPSupplierName` | `BPSupplierName` | `String(81)` |  | Business Partner - Supplier Name |  |  |  |
| `BPSupplierFullName` | `BPSupplierFullName` | `String(163)` |  | Business Partner - Supplier Full Name |  |  |  |
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
| `IsBusinessPurposeCompleted` | `IsBusinessPurposeCompleted` | `Boolean` |  | Purpose Completed |  |  |  |
| `CreatedByUser` | `CreatedByUser` | `String(12)` |  | Created By |  |  |  |
| `CreationDate` | `CreationDate` | `Date` |  | Created On |  |  |  |
| `IsOneTimeAccount` | `IsOneTimeAccount` | `Boolean` |  | One-Time Account |  |  |  |
| `AuthorizationGroup` | `AuthorizationGroup` | `String(4)` |  | Authorization |  |  |  |
| `VATRegistration` | `VATRegistration` | `String(20)` |  | VAT Registration No. |  |  |  |
| `AccountIsBlockedForPosting` | `AccountIsBlockedForPosting` | `Boolean` |  | Posting Block(Deprecated) |  |  |  |
| `TaxJurisdiction` | `TaxJurisdiction` | `String(15)` |  | Tax Jurisdiction |  |  |  |
| `SupplierStandardCarrierAccess` | `SupplierStandardCarrierAccess` | `String(4)` |  | SCAC |  |  |  |
| `SupplierFwdAgentFreightGroup` | `SupplierFwdAgentFreightGroup` | `String(4)` |  | Carrier freight grp |  |  |  |
| `SupplierAgentProcedureGroup` | `SupplierAgentProcedureGroup` | `String(4)` |  | ServAgntProcGrp |  |  |  |
| `SupplIsSocialInsuranceRegtrd` | `SupplIsSocialInsuranceRegtrd` | `Boolean` |  | Social Insurance |  |  |  |
| `SocialInsuranceActivityCode` | `SocialInsuranceActivityCode` | `String(3)` |  | Social Ins. Code |  |  |  |
| `SupplierCorporateGroup` | `SupplierCorporateGroup` | `String(10)` |  | Group Key |  |  |  |
| `Customer` | `Customer` | `String(10)` |  | Customer |  |  |  |
| `Industry` | `Industry` | `String(4)` |  | Industry |  |  |  |
| `TaxNumber1` | `TaxNumber1` | `String(16)` |  | Tax Number 1 |  |  |  |
| `TaxNumber2` | `TaxNumber2` | `String(11)` |  | Tax Number 2 |  |  |  |
| `TaxNumber3` | `TaxNumber3` | `String(18)` |  | Tax Number 3 |  |  |  |
| `TaxNumber4` | `TaxNumber4` | `String(18)` |  | Tax Number 4 |  |  |  |
| `TaxNumber5` | `TaxNumber5` | `String(60)` |  | Tax Number 5 |  |  |  |
| `TaxNumber6` | `TaxNumber6` | `String(20)` |  | Tax Number 6 |  |  |  |
| `PostingIsBlocked` | `PostingIsBlocked` | `Boolean` |  | Posting Block |  |  |  |
| `PurchasingIsBlocked` | `PurchasingIsBlocked` | `Boolean` |  | Purch. Block |  |  |  |
| `InternationalLocationNumber1` | `InternationalLocationNumber1` | `String(7)` |  | Int. location no. 1 |  |  |  |
| `InternationalLocationNumber2` | `InternationalLocationNumber2` | `String(5)` |  | Int. location no. 2 |  |  |  |
| `InternationalLocationNumber3` | `InternationalLocationNumber3` | `String(1)` |  | Check Digit |  |  |  |
| `AddressID` | `AddressID` | `String(10)` |  | Address |  |  |  |
| `Region` | `Region` | `String(3)` |  | Region |  |  |  |
| `OrganizationBPName1` | `OrganizationBPName1` | `String(35)` |  | Name |  |  |  |
| `OrganizationBPName2` | `OrganizationBPName2` | `String(35)` |  | Name 2 |  |  |  |
| `CityName` | `CityName` | `String(35)` |  | City |  |  |  |
| `PostalCode` | `PostalCode` | `String(10)` |  | Postal Code |  |  |  |
| `StreetName` | `StreetName` | `String(35)` |  | Street |  |  |  |
| `Country` | `Country` | `String(3)` |  | Country/Region Key |  |  |  |
| `ConcatenatedInternationalLocNo` | `ConcatenatedInternationalLocNo` | `String(20)` |  | Int. Location No. |  |  |  |
| `SupplierProcurementBlock` | `SupplierProcurementBlock` | `String(2)` |  | Block Function |  |  |  |
| `SuplrQualityManagementSystem` | `SuplrQualityManagementSystem` | `String(4)` |  | Actual QM System |  |  |  |
| `SuplrQltyInProcmtCertfnValidTo` | `SuplrQltyInProcmtCertfnValidTo` | `Date` |  | QM System Valid To |  |  |  |
| `SupplierLanguage` | `SupplierLanguage` | `String(2)` |  | Language Key |  |  |  |
| `AlternativePayeeAccountNumber` | `AlternativePayeeAccountNumber` | `String(10)` |  | Alternative Payee |  |  |  |
| `PhoneNumber1` | `PhoneNumber1` | `String(16)` |  | Telephone 1 |  |  |  |
| `FaxNumber` | `FaxNumber` | `String(31)` |  | Fax Number |  |  |  |
| `IsNaturalPerson` | `IsNaturalPerson` | `Boolean` |  | Natural Person |  |  |  |
| `TaxNumberResponsible` | `TaxNumberResponsible` | `String(18)` |  | Tax Number |  |  |  |
| `UK_ContractorBusinessType` | `UK_ContractorBusinessType` | `String(12)` |  | Business Type |  |  |  |
| `UK_PartnerTradingName` | `UK_PartnerTradingName` | `String(30)` |  | Prtnr's Trading Name |  |  |  |
| `UK_PartnerTaxReference` | `UK_PartnerTaxReference` | `String(20)` |  | Partner's UTR |  |  |  |
| `UK_VerificationStatus` | `UK_VerificationStatus` | `String(3)` |  | Verification Status |  |  |  |
| `UK_VerificationNumber` | `UK_VerificationNumber` | `String(20)` |  | Verification Number |  |  |  |
| `UK_CompanyRegistrationNumber` | `UK_CompanyRegistrationNumber` | `String(8)` |  | Comp. House Reg. No. |  |  |  |
| `UK_VerifiedTaxStatus` | `UK_VerifiedTaxStatus` | `String(1)` |  | Tax Status |  |  |  |
| `FormOfAddress` | `FormOfAddress` | `String(15)` |  | Title |  |  |  |
| `ReferenceAccountGroup` | `ReferenceAccountGroup` | `String(4)` |  | Reference Acct Group |  |  |  |
| `VATLiability` | `VATLiability` | `Boolean` |  | Liable for VAT |  |  |  |
| `ResponsibleType` | `ResponsibleType` | `String(2)` |  | Tax Type |  |  |  |
| `TaxNumberType` | `TaxNumberType` | `String(2)` |  | Tax Number Type |  |  |  |
| `FiscalAddress` | `FiscalAddress` | `String(10)` |  | Fiscal Address |  |  |  |
| `BusinessType` | `BusinessType` | `String(30)` |  | Type of Business |  |  |  |
| `BirthDate` | `BirthDate` | `Date` |  | Date of Birth |  |  |  |
| `PaymentIsBlockedForSupplier` | `PaymentIsBlockedForSupplier` | `Boolean` |  | Payment Block |  |  |  |
| `SortField` | `SortField` | `String(10)` |  | Search Term |  |  |  |
| `PhoneNumber2` | `PhoneNumber2` | `String(16)` |  | Telephone 2 |  |  |  |
| `DeletionIndicator` | `DeletionIndicator` | `Boolean` |  | Deletion Flag |  |  |  |
| `TaxInvoiceRepresentativeName` | `TaxInvoiceRepresentativeName` | `String(10)` |  | Rep's Name |  |  |  |
| `IndustryType` | `IndustryType` | `String(30)` |  | Type of Industry |  |  |  |
| `IN_GSTSupplierClassification` | `IN_GSTSupplierClassification` | `String(1)` |  | GST Ven Class. |  |  |  |
| `SuplrProofOfDelivRlvtCode` | `SuplrProofOfDelivRlvtCode` | `String(1)` |  | Relevant for POD |  |  |  |
| `TradingPartner` | `TradingPartner` | `String(6)` |  | Trading Partner No. |  |  |  |
| `BR_TaxIsSplit` | `BR_TaxIsSplit` | `Boolean` |  | Tax Split |  |  |  |
| `AU_PayerIsPayingToCarryOnEnt` | `AU_PayerIsPayingToCarryOnEnt` | `String(1)` |  | Enterprise in AU |  |  |  |
| `AU_IndividualIsUnder18` | `AU_IndividualIsUnder18` | `String(1)` |  | Individual |  |  |  |
| `AU_PaymentIsExceeding75` | `AU_PaymentIsExceeding75` | `String(1)` |  | Payment Does not Exc |  |  |  |
| `AU_PaymentIsWhollyInputTaxed` | `AU_PaymentIsWhollyInputTaxed` | `String(1)` |  | Wholly Input Taxed |  |  |  |
| `AU_PartnerIsSupplyWithoutGain` | `AU_PartnerIsSupplyWithoutGain` | `String(1)` |  | Individual w/o Gain |  |  |  |
| `AU_SupplierIsEntitledToABN` | `AU_SupplierIsEntitledToABN` | `String(1)` |  | ABN Eligible |  |  |  |
| `AU_PaymentIsIncomeExempted` | `AU_PaymentIsIncomeExempted` | `String(1)` |  | Payment Exempt |  |  |  |
| `AU_SupplyIsMadeAsPrivateHobby` | `AU_SupplyIsMadeAsPrivateHobby` | `String(1)` |  | Hobby |  |  |  |
| `AU_SupplyMadeIsOfDmstcNature` | `AU_SupplyMadeIsOfDmstcNature` | `String(1)` |  | Domestic |  |  |  |
| `IsToBeAcceptedAtOrigin` | `IsToBeAcceptedAtOrigin` | `Boolean` |  | Origin Acceptance |  |  |  |
| `BPIsEqualizationTaxSubject` | `BPIsEqualizationTaxSubject` | `Boolean` |  |  |  |  |  |
| `BRSpcfcTaxBasePercentageCode` | `BRSpcfcTaxBasePercentageCode` | `String(1)` |  | Tax Base |  |  |  |
| `SupplierProfession` | `SupplierProfession` | `String(30)` |  | Profession |  |  |  |
| `SuplrManufacturerExternalName` | `SuplrManufacturerExternalName` | `String(10)` |  | Ext. manufacturer |  |  |  |
| `DataMediumExchangeIndicator` | `DataMediumExchangeIndicator` | `String(1)` |  | DME Recipient Code |  |  |  |
| `DataExchangeInstructionKey` | `DataExchangeInstructionKey` | `String(2)` |  | Instruction Key |  |  |  |
| `SupplierIsSubRangeRelevant` | `SupplierIsSubRangeRelevant` | `Boolean` |  | VSR Relevant |  |  |  |
| `TrainStationName` | `TrainStationName` | `String(25)` |  | Train Station |  |  |  |
| `AlternativePayeeIsAllowed` | `AlternativePayeeIsAllowed` | `Boolean` |  | Payee in Document |  |  |  |
| `PaytSlipWthRefSubscriber` | `PaytSlipWthRefSubscriber` | `String(11)` |  | PBC/ISR Number |  |  |  |
| `TranspServiceAgentStstcGrp` | `TranspServiceAgentStstcGrp` | `String(2)` |  | Stat. Grp, Agent |  |  |  |
| `SupplierIsPlantRelevant` | `SupplierIsPlantRelevant` | `Boolean` |  | Plant Level Relevant |  |  |  |
| `SuplrTaxAuthorityAccountNumber` | `SuplrTaxAuthorityAccountNumber` | `String(10)` |  | Tax Office |  |  |  |
| `SuplrCarrierConfirmIsExpected` | `SuplrCarrierConfirmIsExpected` | `String(1)` |  | Carrier confirmation |  |  |  |
| `SupplierPlant` | `SupplierPlant` | `String(4)` |  | Plant |  |  |  |
| `FactoryCalendar` | `FactoryCalendar` | `String(2)` |  | Factory Calendar |  |  |  |
| `PaymentReason` | `PaymentReason` | `String(4)` |  | Payment Reason |  |  |  |
| `SupplierCentralDeletionIsBlock` | `SupplierCentralDeletionIsBlock` | `Boolean` |  | Central Del. Block |  |  |  |
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
| `SupplierTransportationChain` | `SupplierTransportationChain` | `String(10)` |  | Transportation Chain |  |  |  |
| `SupplierStagingTimeInDays` | `SupplierStagingTimeInDays` | `Decimal(3,0)` |  | Staging Time |  |  |  |
| `SupplierSchedulingProcedure` | `SupplierSchedulingProcedure` | `String(1)` |  | Scheduling Procedure |  |  |  |
| `CollectiveNumberingIsRelevant` | `CollectiveNumberingIsRelevant` | `Boolean` |  | Rel. for Coll. No. |  |  |  |
| `BusinessPartnerPanNumber` | `BusinessPartnerPanNumber` | `String(40)` |  | PAN |  |  |  |
| `BPPanReferenceNumber` | `BPPanReferenceNumber` | `String(40)` |  | PAN Reference Number |  |  |  |
| `BPPanValidFromDate` | `BPPanValidFromDate` | `Date` |  | PAN Valid From Date |  |  |  |


## Entity: `SupplierCompanyCode`

- **ABAP Name:** `I_SupplierCompany`
- **Label:** Supplier Company
- **VDM Type:** `BASIC` | **Data Category:** `FACT`
- **ECC Source Tables:** t001, lfb1

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Supplier` | `Supplier` | `String(10)` | Y | Supplier |  | _Supplier |  |
| `CompanyCode` | `CompanyCode` | `String(4)` | Y | Company Code |  | _CompanyCode |  |
| `AuthorizationGroup` | `AuthorizationGroup` | `String(4)` |  | Authorization |  |  |  |
| `CompanyCodeName` | `CompanyCodeName` | `String(25)` |  | Company Name |  |  |  |
| `PaymentBlockingReason` | `PaymentBlockingReason` | `String(1)` |  | Payment Block |  |  |  |
| `SupplierIsBlockedForPosting` | `SupplierIsBlockedForPosting` | `Boolean` |  | Co.code post.block |  |  |  |
| `IsBusinessPurposeCompleted` | `IsBusinessPurposeCompleted` | `Boolean` |  | Purpose Completed |  |  |  |
| `AccountingClerk` | `AccountingClerk` | `String(2)` |  | Clerk Abbrev. |  |  |  |
| `AccountingClerkFaxNumber` | `AccountingClerkFaxNumber` | `String(31)` |  | Acctg clerk's fax |  |  |  |
| `AccountingClerkPhoneNumber` | `AccountingClerkPhoneNumber` | `String(30)` |  | Acct.clerks tel.no. |  |  |  |
| `AccountingClerkInternetAddress` | `AccountingClerkInternetAddress` | `String(130)` |  | Clrk's internet add. |  |  |  |
| `SupplierClerk` | `SupplierClerk` | `String(15)` |  | Clerk at vendor |  |  |  |
| `SupplierClerkURL` | `SupplierClerkURL` | `String(130)` |  | Clrk's internet add. |  |  |  |
| `PaymentMethodsList` | `PaymentMethodsList` | `String(10)` |  | Payment Methods |  |  |  |
| `PaymentTerms` | `PaymentTerms` | `String(4)` |  | Terms of Payment |  |  |  |
| `ClearCustomerSupplier` | `ClearCustomerSupplier` | `Boolean` |  | Clearing w/ Customer |  |  |  |
| `IsToBeLocallyProcessed` | `IsToBeLocallyProcessed` | `Boolean` |  | Local Processing |  |  |  |
| `ItemIsToBePaidSeparately` | `ItemIsToBePaidSeparately` | `Boolean` |  | Individual Payment |  |  |  |
| `PaymentIsToBeSentByEDI` | `PaymentIsToBeSentByEDI` | `Boolean` |  | Pmnt advice by EDI |  |  |  |
| `HouseBank` | `HouseBank` | `String(5)` |  | House Bank |  |  |  |
| `CheckPaidDurationInDays` | `CheckPaidDurationInDays` | `Decimal(3,0)` |  | Check Cashing Time |  |  |  |
| `Currency` | `Currency` | `String(5)` |  | Currency |  |  |  |
| `BillOfExchLmtAmtInCoCodeCrcy` | `BillOfExchLmtAmtInCoCodeCrcy` | `Decimal(34,4)` |  | Bill/Ex. Limit | Currency |  |  |
| `SupplierClerkIDBySupplier` | `SupplierClerkIDBySupplier` | `String(12)` |  | Account with vendor |  |  |  |
| `IsDoubleInvoice` | `IsDoubleInvoice` | `Boolean` |  | Check Double Invoice |  |  |  |
| `CustomerSupplierClearingIsUsed` | `CustomerSupplierClearingIsUsed` | `Boolean` |  | Clearing w/ Customer |  |  |  |
| `ReconciliationAccount` | `ReconciliationAccount` | `String(10)` |  | Reconciliation Acct |  |  |  |
| `InterestCalculationCode` | `InterestCalculationCode` | `String(2)` |  | Interest Indicator |  |  |  |
| `InterestCalculationDate` | `InterestCalculationDate` | `Date` |  | Last Key Date |  |  |  |
| `IntrstCalcFrequencyInMonths` | `IntrstCalcFrequencyInMonths` | `String(2)` |  | Int.Calc.Freq. |  |  |  |
| `SupplierHeadOffice` | `SupplierHeadOffice` | `String(10)` |  | Head Office |  |  |  |
| `AlternativePayee` | `AlternativePayee` | `String(10)` |  | Alternative payee |  |  |  |
| `LayoutSortingRule` | `LayoutSortingRule` | `String(3)` |  | Sort key |  |  |  |
| `APARToleranceGroup` | `APARToleranceGroup` | `String(4)` |  | Tolerance Group |  |  |  |
| `SuplrInvcVerificatTolGroup` | `SuplrInvcVerificatTolGroup` | `String(4)` |  | Tolerance Group |  |  |  |
| `SupplierCertificationDate` | `SupplierCertificationDate` | `Date` |  | Certification Date |  |  |  |
| `SupplierAccountNote` | `SupplierAccountNote` | `String(30)` |  | Account Memo |  |  |  |
| `WithholdingTaxCountry` | `WithholdingTaxCountry` | `String(3)` |  | WTax C/R Key |  |  |  |
| `DeletionIndicator` | `DeletionIndicator` | `Boolean` |  | Co.Cde Deletion Flag |  |  |  |
| `CashPlanningGroup` | `CashPlanningGroup` | `String(10)` |  | Planning Group |  |  |  |
| `IsToBeCheckedForDuplicates` | `IsToBeCheckedForDuplicates` | `Boolean` |  | Check Double Invoice |  |  |  |
| `PersonnelNumber` | `PersonnelNumber` | `String(8)` |  | Personnel Number |  |  |  |
| `PreviousAccountNumber` | `PreviousAccountNumber` | `String(10)` |  | Previous Account No. |  |  |  |
| `MinorityGroup` | `MinorityGroup` | `String(3)` |  | Minority Indicator |  |  |  |
| `LastInterestCalcRunDate` | `LastInterestCalcRunDate` | `Date` |  | Last Int. Calc. |  |  |  |
| `US_ForeignSuplrHasPartnership` | `US_ForeignSuplrHasPartnership` | `String(1)` |  | Partnership Int Ind |  |  |  |
| `US_SecondTINNoticeIsIssued` | `US_SecondTINNoticeIsIssued` | `String(1)` |  | Second TIN Notice |  |  |  |
| `US_ForeignSuplrLmtnOnBnftCode` | `US_ForeignSuplrLmtnOnBnftCode` | `String(2)` |  | LOB Treaty Code |  |  |  |
| `SupplierReleaseGroup` | `SupplierReleaseGroup` | `String(4)` |  | Release Group |  |  |  |
| `CreditMemoPaymentTerms` | `CreditMemoPaymentTerms` | `String(4)` |  | Credit Memo Pyt Term |  |  |  |
| `PaymentMethodSupplement` | `PaymentMethodSupplement` | `String(2)` |  | Pmt Meth. Supplement |  |  |  |
| `US_FrgnAcctTaxFilingIsRequired` | `US_FrgnAcctTaxFilingIsRequired` | `String(1)` |  | FATCA Ind |  |  |  |
| `US_RecipientForeignTaxID` | `US_RecipientForeignTaxID` | `String(22)` |  | US Recipient FTID |  |  |  |
| `US_FW9ReceiveDate` | `US_FW9ReceiveDate` | `Date` |  | W9 Form Rec Date |  |  |  |
| `US_FW8BENReceiveDate` | `US_FW8BENReceiveDate` | `Date` |  | W8 Form Rec Date |  |  |  |
| `US_FrgnAcctTaxRcpntCntry` | `US_FrgnAcctTaxRcpntCntry` | `String(3)` |  | Country/Region Key |  |  |  |
| `US_GlobIntermediaryIdnNumber` | `US_GlobIntermediaryIdnNumber` | `String(19)` |  | US Recipient GIIN |  |  |  |
| `US_LobTreatyCode` | `US_LobTreatyCode` | `String(2)` |  | LOB Treaty Code |  |  |  |
| `US_Chapter4StatusCode` | `US_Chapter4StatusCode` | `String(2)` |  | Chaptr 4 Status Code |  |  |  |
| `PaymentClearingGroup` | `PaymentClearingGroup` | `String(8)` |  | Payment Clrg Grp ID |  |  |  |
| `PaymentReason` | `PaymentReason` | `String(4)` |  | Payment Reason |  |  |  |
| `DeletionIsBlocked` | `DeletionIsBlocked` | `Boolean` |  | CoCd Deletion Block |  |  |  |
| `IsActiveEntity` | `IsActiveEntity` | `Boolean` |  | Is active |  |  |  |
| `UK_ContractorBusinessType` | `UK_ContractorBusinessType` | `String(12)` |  | Business Type |  |  |  |
| `UK_PartnerTradingName` | `UK_PartnerTradingName` | `String(30)` |  | Prtnr's Trading Name |  |  |  |
| `UK_PartnerTaxReference` | `UK_PartnerTaxReference` | `String(20)` |  | Partner's UTR |  |  |  |
| `UK_VerificationStatus` | `UK_VerificationStatus` | `String(3)` |  | Verification Status |  |  |  |
| `UK_VerificationNumber` | `UK_VerificationNumber` | `String(20)` |  | Verification Number |  |  |  |
| `UK_CompanyRegistrationNumber` | `UK_CompanyRegistrationNumber` | `String(8)` |  | Comp. House Reg. No. |  |  |  |
| `UK_VerifiedTaxStatus` | `UK_VerifiedTaxStatus` | `String(1)` |  | Tax Status |  |  |  |


## Entity: `SupplierPurchasingOrganization`

- **ABAP Name:** `I_SupplierPurchasingOrg`
- **Label:** Supplier Purchasing Organization
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** LFA1, LFM1

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Supplier` | `Supplier` | `String(10)` | Y | Supplier |  | _Supplier |  |
| `PurchasingOrganization` | `PurchasingOrganization` | `String(4)` | Y | Purch. Organization |  |  |  |
| `PurchasingGroup` | `PurchasingGroup` | `String(3)` |  | Purchasing Group |  |  |  |
| `MaterialPlannedDeliveryDurn` | `MaterialPlannedDeliveryDurn` | `Decimal(3,0)` |  | Planned Deliv. Time |  |  |  |
| `PurchasingIsBlockedForSupplier` | `PurchasingIsBlockedForSupplier` | `Boolean` |  | Pur. block POrg |  |  |  |
| `SupplierRespSalesPersonName` | `SupplierRespSalesPersonName` | `String(30)` |  | Salesperson |  |  |  |
| `SupplierPhoneNumber` | `SupplierPhoneNumber` | `String(16)` |  | Telephone |  |  |  |
| `PurchaseOrderCurrency` | `PurchaseOrderCurrency` | `String(5)` |  | Order currency |  |  |  |
| `MinimumOrderAmount` | `MinimumOrderAmount` | `Decimal(34,4)` |  | Minimum order value | PurchaseOrderCurrency |  |  |
| `CalculationSchemaGroupCode` | `CalculationSchemaGroupCode` | `String(2)` |  | Schema Grp, Supplier |  |  |  |
| `PaymentTerms` | `PaymentTerms` | `String(4)` |  | Terms of Payment |  |  |  |
| `PricingDateControl` | `PricingDateControl` | `String(1)` |  | Pricing Date Control |  |  |  |
| `SupplierABCClassificationCode` | `SupplierABCClassificationCode` | `String(1)` |  | ABC indicator |  |  |  |
| `ShippingCondition` | `ShippingCondition` | `String(2)` |  | Shipping Conditions |  |  |  |
| `PurOrdAutoGenerationIsAllowed` | `PurOrdAutoGenerationIsAllowed` | `Boolean` |  | Automatic PO |  |  |  |
| `InvoiceIsGoodsReceiptBased` | `InvoiceIsGoodsReceiptBased` | `Boolean` |  | GR-Based Inv. Verif. |  |  |  |
| `IncotermsClassification` | `IncotermsClassification` | `String(3)` |  | Incoterms |  |  |  |
| `IncotermsTransferLocation` | `IncotermsTransferLocation` | `String(28)` |  | Incoterms (Part 2) |  |  |  |
| `IncotermsVersion` | `IncotermsVersion` | `String(4)` |  | Incoterms Version |  |  |  |
| `IncotermsLocation1` | `IncotermsLocation1` | `String(70)` |  | Incoterms Location 1 |  |  |  |
| `IncotermsLocation2` | `IncotermsLocation2` | `String(70)` |  | Incoterms Location 2 |  |  |  |
| `DeletionIndicator` | `DeletionIndicator` | `Boolean` |  | Del. flag POrg. |  |  |  |
| `PlannedDeliveryDurationInDays` | `PlannedDeliveryDurationInDays` | `Decimal(3,0)` |  | Planned Deliv. Time |  |  |  |
| `ContactPersonPhoneNumber` | `ContactPersonPhoneNumber` | `String(16)` |  | Telephone |  |  |  |
| `SupplierConfirmationControlKey` | `SupplierConfirmationControlKey` | `String(4)` |  | Confirmation Control |  |  |  |
| `IsOrderAcknRqd` | `IsOrderAcknRqd` | `Boolean` |  | Acknowledgment Reqd. |  |  |  |
| `EvaldReceiptSettlementIsActive` | `EvaldReceiptSettlementIsActive` | `Boolean` |  | Eval. Receipt Sett. |  |  |  |
| `AutomaticEvaluatedRcptSettlmt` | `AutomaticEvaluatedRcptSettlmt` | `Boolean` |  | Aut. ev. GRSetmt.Ret |  |  |  |
| `SupplierAccountNumber` | `SupplierAccountNumber` | `String(12)` |  | Acc. with supplier |  |  |  |
| `SuplrIsSubjToSubsqntSettlement` | `SuplrIsSubjToSubsqntSettlement` | `Boolean` |  | Subseq. settlement |  |  |  |
| `SuplrPurgOrgAgrmtOfBusVolIsRqd` | `SuplrPurgOrgAgrmtOfBusVolIsRqd` | `Boolean` |  | B.vol.comp./ag.nec. |  |  |  |
| `SuplrInvcRevalIsAllowed` | `SuplrInvcRevalIsAllowed` | `Boolean` |  | Revaluation |  |  |  |
| `SuplrPurgOrgIsRlvtForPriceDetn` | `SuplrPurgOrgIsRlvtForPriceDetn` | `Boolean` |  | Price determination |  |  |  |
| `IntrastatCrsBorderTrMode` | `IntrastatCrsBorderTrMode` | `String(1)` |  | Mode of Transport |  |  |  |
| `ProductUnitGroup` | `ProductUnitGroup` | `String(4)` |  | Unit of Measure Grp |  |  |  |
| `RoundingProfile` | `RoundingProfile` | `String(4)` |  | Rounding Profile |  |  |  |
| `PlanningCycle` | `PlanningCycle` | `String(3)` |  | Planning Cycle |  |  |  |
| `SuplrDiscountInKindIsGranted` | `SuplrDiscountInKindIsGranted` | `Boolean` |  |  |  |  |  |
| `SuplrIsRlvtForSettlmtMgmt` | `SuplrIsRlvtForSettlmtMgmt` | `Boolean` |  | Settlement Mgmt. |  |  |  |
| `InvoiceIsMMServiceEntryBased` | `InvoiceIsMMServiceEntryBased` | `Boolean` |  | Srv.-Based Inv. Ver. |  |  |  |
| `ProdStockAndSlsDataTransfPrfl` | `ProdStockAndSlsDataTransfPrfl` | `String(4)` |  | PROACT control prof. |  |  |  |
| `EvaldRcptSettlementProfile` | `EvaldRcptSettlementProfile` | `String(4)` |  | Settlement profile |  |  |  |
| `AbsoluteHandlingSurchargeAmt` | `AbsoluteHandlingSurchargeAmt` | `Decimal(34,4)` |  | Absolute surcharge | PurchaseOrderCurrency |  |  |
| `PercentageHandlingSurchargeAmt` | `PercentageHandlingSurchargeAmt` | `Decimal(5,2)` |  | Percentage HSC |  |  |  |
| `MinimumHandlingSurchargeAmt` | `MinimumHandlingSurchargeAmt` | `Decimal(34,4)` |  | Minimum HSC | PurchaseOrderCurrency |  |  |
| `MaximumHandlingSurchargeAmt` | `MaximumHandlingSurchargeAmt` | `Decimal(34,4)` |  | Max. HSC | PurchaseOrderCurrency |  |  |
| `AutomDebitCrtnIsEnbldOnGI` | `AutomDebitCrtnIsEnbldOnGI` | `Boolean` |  | Auto. debit |  |  |  |
| `SupplierIsReturnsSupplier` | `SupplierIsReturnsSupplier` | `Boolean` |  | Returns supplier |  |  |  |
| `IsActiveEntity` | `IsActiveEntity` | `Boolean` |  | Is active |  |  |  |
| `IncotermsSupChnLoc1AddlUUID` | `IncotermsSupChnLoc1AddlUUID` | `UUID` |  | Location UUID |  |  |  |
| `IncotermsSupChnLoc2AddlUUID` | `IncotermsSupChnLoc2AddlUUID` | `UUID` |  | Location UUID |  |  |  |
| `IncotermsSupChnDvtgLocAddlUUID` | `IncotermsSupChnDvtgLocAddlUUID` | `UUID` |  | Location UUID |  |  |  |
| `AuthorizationGroup` | `AuthorizationGroup` | `String(4)` |  | Authorization |  |  |  |


## Entity: `SupplierWithHoldingTax`

- **ABAP Name:** `I_SupplierWithHoldingTax`
- **Label:** Supplier WithHolding Tax
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Supplier` | `Supplier` | `String(10)` | Y | Supplier |  | _Supplier | S/4 only entity (no ECC CDC mapping) |
| `CompanyCode` | `CompanyCode` | `String(4)` | Y | Company Code |  | _CompanyCode | S/4 only entity (no ECC CDC mapping) |
| `WithholdingTaxType` | `WithholdingTaxType` | `String(2)` | Y | Withholding Tax Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `WithholdingTaxNumber` | `WithholdingTaxNumber` | `String(16)` |  | W/tax number |  |  | S/4 only entity (no ECC CDC mapping) |
| `WithholdingTaxCode` | `WithholdingTaxCode` | `String(2)` |  | W/Tax Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsWithholdingTaxSubject` | `IsWithholdingTaxSubject` | `Boolean` |  | Subject to W/Tx |  |  | S/4 only entity (no ECC CDC mapping) |
| `RecipientType` | `RecipientType` | `String(2)` |  | Recipient Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `WithholdingTaxCertificate` | `WithholdingTaxCertificate` | `String(25)` |  | Exemption Number |  |  | S/4 only entity (no ECC CDC mapping) |
| `WithholdingTaxExmptPercent` | `WithholdingTaxExmptPercent` | `Decimal(5,2)` |  | Exemption Rate |  |  | S/4 only entity (no ECC CDC mapping) |
| `ExemptionDateBegin` | `ExemptionDateBegin` | `Date` |  | Exemption Start Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `ExemptionDateEnd` | `ExemptionDateEnd` | `Date` |  | Exemption End Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `ExemptionReason` | `ExemptionReason` | `String(2)` |  | Exemption Reason |  |  | S/4 only entity (no ECC CDC mapping) |
