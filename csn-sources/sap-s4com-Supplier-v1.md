# Supplier

> Source file: `sap-s4com-Supplier-v1.json`

**Technical Name:** `` | **Data Category:** `DIMENSION` | **VDM Type:** `BASIC` | **Size:** `XL`


## Entity: `Supplier`

- **ABAP CDS Name:** `I_Supplier`
- **Label:** Supplier
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** ADRC, LFA1

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Supplier` | `LIFNR` | `LFA1` | `LIFNR` |  |  | `String(10)` | Y | Supplier |  |  |
| `SupplierAccountGroup` | `KTOKK` | `LFA1` | `KTOKK` |  |  | `String(4)` |  | Account Group |  |  |
| `SupplierName` | `MD_SUPPLIER_NAME` |  |  |  |  | `String(80)` |  | Name of Supplier |  |  |
| `SupplierFullName` | `MD_SUPPLIER_FULL_NAME` | `LFA1` | `NAME1` |  |  | `String(220)` |  | Supplier Name |  |  |
| `BPSupplierName` | `SUPPLIERNAME_2` |  |  |  |  | `String(81)` |  | Business Partner - Supplier Name |  |  |
| `BPSupplierFullName` | `SUPPLIERFULLNAME_2` |  |  |  |  | `String(163)` |  | Business Partner - Supplier Full Name |  |  |
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
| `IsBusinessPurposeCompleted` |  |  |  |  |  | `Boolean` |  | Purpose Completed |  |  |
| `CreatedByUser` | `ERNAM_RF` |  |  |  |  | `String(12)` |  | Created By |  |  |
| `CreationDate` | `ERDAT_RF` |  |  |  |  | `Date` |  | Created On |  |  |
| `IsOneTimeAccount` | `XCPDK` |  |  |  |  | `Boolean` |  | One-Time Account |  |  |
| `AuthorizationGroup` | `BRGRU` |  |  |  |  | `String(4)` |  | Authorization |  |  |
| `VATRegistration` | `STCEG` |  |  |  |  | `String(20)` |  | VAT Registration No. |  |  |
| `AccountIsBlockedForPosting` | `SPERB_X` |  |  |  |  | `Boolean` |  | Posting Block(Deprecated) |  |  |
| `TaxJurisdiction` | `TXJCD` |  |  |  |  | `String(15)` |  | Tax Jurisdiction |  |  |
| `SupplierStandardCarrierAccess` | `SCACD` |  |  |  |  | `String(4)` |  | SCAC |  |  |
| `SupplierFwdAgentFreightGroup` | `SFRGR` |  |  |  |  | `String(4)` |  | Carrier freight grp |  |  |
| `SupplierAgentProcedureGroup` | `DLGRP` |  |  |  |  | `String(4)` |  | ServAgntProcGrp |  |  |
| `SupplIsSocialInsuranceRegtrd` | `J_1AREGSS` |  |  |  |  | `Boolean` |  | Social Insurance |  |  |
| `SocialInsuranceActivityCode` | `J_1AACTSS` |  |  |  |  | `String(3)` |  | Social Ins. Code |  |  |
| `SupplierCorporateGroup` | `KONZS` |  |  |  |  | `String(10)` |  | Group Key |  |  |
| `Customer` | `KUNNR` |  |  |  |  | `String(10)` |  | Customer |  |  |
| `Industry` | `BRSCH` |  |  |  |  | `String(4)` |  | Industry |  |  |
| `TaxNumber1` | `STCD1` | `LFA1` | `STCD1` |  |  | `String(16)` |  | Tax Number 1 |  |  |
| `TaxNumber2` | `STCD2` |  |  |  |  | `String(11)` |  | Tax Number 2 |  |  |
| `TaxNumber3` | `STCD3` |  |  |  |  | `String(18)` |  | Tax Number 3 |  |  |
| `TaxNumber4` | `STCD4` |  |  |  |  | `String(18)` |  | Tax Number 4 |  |  |
| `TaxNumber5` | `STCD5` |  |  |  |  | `String(60)` |  | Tax Number 5 |  |  |
| `TaxNumber6` | `STCD6` |  |  |  |  | `String(20)` |  | Tax Number 6 |  |  |
| `PostingIsBlocked` | `SPERB_X` |  |  |  |  | `Boolean` |  | Posting Block |  |  |
| `PurchasingIsBlocked` | `SPERM_X` |  |  |  |  | `Boolean` |  | Purch. Block |  |  |
| `InternationalLocationNumber1` | `BBBNR` |  |  |  |  | `String(7)` |  | Int. location no. 1 |  |  |
| `InternationalLocationNumber2` | `BBSNR` |  |  |  |  | `String(5)` |  | Int. location no. 2 |  |  |
| `InternationalLocationNumber3` | `BUBKZ` |  |  |  |  | `String(1)` |  | Check Digit |  |  |
| `AddressID` | `ADRNR` | `ADRC` | `ADDRNUMBER` |  |  | `String(10)` |  | Address |  |  |
| `Region` | `REGIO` | `LFA1` | `REGIO` |  |  | `String(3)` |  | Region |  |  |
| `OrganizationBPName1` | `NAME1_GP` |  |  |  |  | `String(35)` |  | Name |  |  |
| `OrganizationBPName2` | `NAME2_GP` |  |  |  |  | `String(35)` |  | Name 2 |  |  |
| `CityName` | `ORT01_GP` | `LFA1` | `ORT01` |  |  | `String(35)` |  | City |  |  |
| `PostalCode` | `PSTLZ` | `LFA1` | `PSTLZ` |  |  | `String(10)` |  | Postal Code |  |  |
| `StreetName` | `STRAS_GP` | `LFA1` | `STRAS` |  |  | `String(35)` |  | Street |  |  |
| `Country` | `LAND1_GP` | `LFA1` | `LAND1` |  |  | `String(3)` |  | Country/Region Key |  |  |
| `ConcatenatedInternationalLocNo` | `MD_INTERNATIONAL_LOC` |  |  |  |  | `String(20)` |  | Int. Location No. |  |  |
| `SupplierProcurementBlock` | `QSPERRFKT` |  |  |  |  | `String(2)` |  | Block Function |  |  |
| `SuplrQualityManagementSystem` | `QSSYS_IST` |  |  |  |  | `String(4)` |  | Actual QM System |  |  |
| `SuplrQltyInProcmtCertfnValidTo` | `QQSSYSDAT` |  |  |  |  | `Date` |  | QM System Valid To |  |  |
| `SupplierLanguage` | `SPRAS` |  |  |  |  | `String(2)` |  | Language Key |  |  |
| `AlternativePayeeAccountNumber` | `LNRZA` |  |  |  |  | `String(10)` |  | Alternative Payee |  |  |
| `PhoneNumber1` | `TELF1` | `LFA1` | `TELF1` |  |  | `String(16)` |  | Telephone 1 |  |  |
| `FaxNumber` | `TELFX` |  |  |  |  | `String(31)` |  | Fax Number |  |  |
| `IsNaturalPerson` |  |  |  |  |  | `Boolean` |  | Natural Person |  |  |
| `TaxNumberResponsible` | `STENR` |  |  |  |  | `String(18)` |  | Tax Number |  |  |
| `UK_ContractorBusinessType` | `CIS_CATEGORY` |  |  |  |  | `String(12)` |  | Business Type |  |  |
| `UK_PartnerTradingName` | `CIS_PARTNER_NAME` |  |  |  |  | `String(30)` |  | Prtnr's Trading Name |  |  |
| `UK_PartnerTaxReference` | `CIS_PARTNER_UTR` |  |  |  |  | `String(20)` |  | Partner's UTR |  |  |
| `UK_VerificationStatus` | `CIS_VFNSTATUS` |  |  |  |  | `String(3)` |  | Verification Status |  |  |
| `UK_VerificationNumber` | `GB_CIS_SC_VFNNUM` |  |  |  |  | `String(20)` |  | Verification Number |  |  |
| `UK_CompanyRegistrationNumber` | `GB_CIS_CRN` |  |  |  |  | `String(8)` |  | Comp. House Reg. No. |  |  |
| `UK_VerifiedTaxStatus` | `CIS_VFN_ID` |  |  |  |  | `String(1)` |  | Tax Status |  |  |
| `FormOfAddress` | `ANRED` |  |  |  |  | `String(15)` |  | Title |  |  |
| `ReferenceAccountGroup` | `KTOCK` |  |  |  |  | `String(4)` |  | Reference Acct Group |  |  |
| `VATLiability` | `STKZU` |  |  |  |  | `Boolean` |  | Liable for VAT |  |  |
| `ResponsibleType` | `J_1AFITP_D` |  |  |  |  | `String(2)` |  | Tax Type |  |  |
| `TaxNumberType` | `J_1ATOID` |  |  |  |  | `String(2)` |  | Tax Number Type |  |  |
| `FiscalAddress` | `FISKN_K` |  |  |  |  | `String(10)` |  | Fiscal Address |  |  |
| `BusinessType` | `GESTYP` |  |  |  |  | `String(30)` |  | Type of Business |  |  |
| `BirthDate` | `GBDAT_Q` |  |  |  |  | `Date` |  | Date of Birth |  |  |
| `PaymentIsBlockedForSupplier` | `SPERZ` |  |  |  |  | `Boolean` |  | Payment Block |  |  |
| `SortField` | `SORTL` |  |  |  |  | `String(10)` |  | Search Term |  |  |
| `PhoneNumber2` | `TELF2` |  |  |  |  | `String(16)` |  | Telephone 2 |  |  |
| `DeletionIndicator` | `LOEVM_X` |  |  |  |  | `Boolean` |  | Deletion Flag |  |  |
| `TaxInvoiceRepresentativeName` | `REPRES` |  |  |  |  | `String(10)` |  | Rep's Name |  |  |
| `IndustryType` | `INDTYP` |  |  |  |  | `String(30)` |  | Type of Industry |  |  |
| `IN_GSTSupplierClassification` | `J_1IGTAKLD` |  |  |  |  | `String(1)` |  | GST Ven Class. |  |  |
| `SuplrProofOfDelivRlvtCode` | `PODKZB` |  |  |  |  | `String(1)` |  | Relevant for POD |  |  |
| `TradingPartner` | `RASSC` |  |  |  |  | `String(6)` |  | Trading Partner No. |  |  |
| `BR_TaxIsSplit` | `J_1BINDEQU` |  |  |  |  | `Boolean` |  | Tax Split |  |  |
| `AU_PayerIsPayingToCarryOnEnt` | `FIAPAU_CARRY_ENT` |  |  |  |  | `String(1)` |  | Enterprise in AU |  |  |
| `AU_IndividualIsUnder18` | `FIAPAU_IND_UNDER_18` |  |  |  |  | `String(1)` |  | Individual |  |  |
| `AU_PaymentIsExceeding75` | `FIAPAU_PMNT_NOT_EXCEED` |  |  |  |  | `String(1)` |  | Payment Does not Exc |  |  |
| `AU_PaymentIsWhollyInputTaxed` | `FIAPAU_INPUT_TAXED` |  |  |  |  | `String(1)` |  | Wholly Input Taxed |  |  |
| `AU_PartnerIsSupplyWithoutGain` | `FIAPAU_PARTNER_NO_GAIN` |  |  |  |  | `String(1)` |  | Individual w/o Gain |  |  |
| `AU_SupplierIsEntitledToABN` | `FIAPAU_ABN_ELIGIBLE` |  |  |  |  | `String(1)` |  | ABN Eligible |  |  |
| `AU_PaymentIsIncomeExempted` | `FIAPAU_PMNT_EXEMPT` |  |  |  |  | `String(1)` |  | Payment Exempt |  |  |
| `AU_SupplyIsMadeAsPrivateHobby` | `FIAPAU_PVT_HOBBY` |  |  |  |  | `String(1)` |  | Hobby |  |  |
| `AU_SupplyMadeIsOfDmstcNature` | `FIAPAU_DOM_NATURE` |  |  |  |  | `String(1)` |  | Domestic |  |  |
| `IsToBeAcceptedAtOrigin` | `WEORA` |  |  |  |  | `Boolean` |  | Origin Acceptance |  |  |
| `BPIsEqualizationTaxSubject` | `XFELD` |  |  |  |  | `Boolean` |  |  |  |  |
| `BRSpcfcTaxBasePercentageCode` | `TAXBS` |  |  |  |  | `String(1)` |  | Tax Base |  |  |
| `SupplierProfession` | `PROFS` |  |  |  |  | `String(30)` |  | Profession |  |  |
| `SuplrManufacturerExternalName` | `EMNFR` |  |  |  |  | `String(10)` |  | Ext. manufacturer |  |  |
| `DataMediumExchangeIndicator` | `DTAMS` |  |  |  |  | `String(1)` |  | DME Recipient Code |  |  |
| `DataExchangeInstructionKey` | `DTAWS` |  |  |  |  | `String(2)` |  | Instruction Key |  |  |
| `SupplierIsSubRangeRelevant` | `LTSNA` |  |  |  |  | `Boolean` |  | VSR Relevant |  |  |
| `TrainStationName` | `BAHNS` |  |  |  |  | `String(25)` |  | Train Station |  |  |
| `AlternativePayeeIsAllowed` | `XZEMP` |  |  |  |  | `Boolean` |  | Payee in Document |  |  |
| `PaytSlipWthRefSubscriber` | `ESRNR` |  |  |  |  | `String(11)` |  | PBC/ISR Number |  |  |
| `TranspServiceAgentStstcGrp` | `STGDL` |  |  |  |  | `String(2)` |  | Stat. Grp, Agent |  |  |
| `SupplierIsPlantRelevant` | `WERKR` |  |  |  |  | `Boolean` |  | Plant Level Relevant |  |  |
| `SuplrTaxAuthorityAccountNumber` | `FISKU` |  |  |  |  | `String(10)` |  | Tax Office |  |  |
| `SuplrCarrierConfirmIsExpected` |  |  |  |  |  | `String(1)` |  | Carrier confirmation |  |  |
| `SupplierPlant` | `WERKS_EXT` |  |  |  |  | `String(4)` |  | Plant |  |  |
| `FactoryCalendar` | `FABKL` |  |  |  |  | `String(2)` |  | Factory Calendar |  |  |
| `PaymentReason` | `FARP_PAYT_RSN` |  |  |  |  | `String(4)` |  | Payment Reason |  |  |
| `SupplierCentralDeletionIsBlock` | `NODEL_X` |  |  |  |  | `Boolean` |  | Central Del. Block |  |  |
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
| `SupplierTransportationChain` | `WRF_PSCD_TC_ID` |  |  |  |  | `String(10)` |  | Transportation Chain |  |  |
| `SupplierStagingTimeInDays` | `WRF_PSCD_MST` |  |  |  |  | `Decimal(3,0)` |  | Staging Time |  |  |
| `SupplierSchedulingProcedure` | `WRF_PSCD_SCHED_TYPE` |  |  |  |  | `String(1)` |  | Scheduling Procedure |  |  |
| `CollectiveNumberingIsRelevant` | `WRF_SUBMI_RELEVANT` |  |  |  |  | `Boolean` |  | Rel. for Coll. No. |  |  |
| `BusinessPartnerPanNumber` | `J_1IPANNO` |  |  |  |  | `String(40)` |  | PAN |  |  |
| `BPPanReferenceNumber` | `J_1IPANREF` |  |  |  |  | `String(40)` |  | PAN Reference Number |  |  |
| `BPPanValidFromDate` | `J_1IPANVALDT` |  |  |  |  | `Date` |  | PAN Valid From Date |  |  |


## Entity: `SupplierCompanyCode`

- **ABAP CDS Name:** `I_SupplierCompany`
- **Label:** Supplier Company
- **VDM Type:** `BASIC` | **Data Category:** `FACT`
- **ECC Source Tables:** LFB1, T001

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Supplier` | `LIFNR` | `LFB1` | `LIFNR` |  |  | `String(10)` | Y | Supplier |  |  |
| `CompanyCode` | `BUKRS` | `T001` | `BUKRS` |  |  | `String(4)` | Y | Company Code |  |  |
| `AuthorizationGroup` | `BRGRU` |  |  |  |  | `String(4)` |  | Authorization |  |  |
| `CompanyCodeName` | `BUTXT` |  |  |  |  | `String(25)` |  | Company Name |  |  |
| `PaymentBlockingReason` | `DZAHLS` | `LFB1` | `ZAHLS` |  |  | `String(1)` |  | Payment Block |  |  |
| `SupplierIsBlockedForPosting` | `SPERB_B` |  |  |  |  | `Boolean` |  | Co.code post.block |  |  |
| `IsBusinessPurposeCompleted` |  |  |  |  |  | `Boolean` |  | Purpose Completed |  |  |
| `AccountingClerk` | `BUSAB` |  |  |  |  | `String(2)` |  | Clerk Abbrev. |  |  |
| `AccountingClerkFaxNumber` | `TLFXS` |  |  |  |  | `String(31)` |  | Acctg clerk's fax |  |  |
| `AccountingClerkPhoneNumber` | `TLFNS` |  |  |  |  | `String(30)` |  | Acct.clerks tel.no. |  |  |
| `AccountingClerkInternetAddress` | `INTAD` |  |  |  |  | `String(130)` |  | Clrk's internet add. |  |  |
| `SupplierClerk` | `DZSABE_K` |  |  |  |  | `String(15)` |  | Clerk at vendor |  |  |
| `SupplierClerkURL` | `INTAD` |  |  |  |  | `String(130)` |  | Clrk's internet add. |  |  |
| `PaymentMethodsList` | `DZWELS` |  |  |  |  | `String(10)` |  | Payment Methods |  |  |
| `PaymentTerms` | `DZTERM` | `LFB1` | `ZTERM` |  |  | `String(4)` |  | Terms of Payment |  |  |
| `ClearCustomerSupplier` | `XVERR_LFB1` |  |  |  |  | `Boolean` |  | Clearing w/ Customer |  |  |
| `IsToBeLocallyProcessed` | `XDEZV` |  |  |  |  | `Boolean` |  | Local Processing |  |  |
| `ItemIsToBePaidSeparately` | `XPORE` |  |  |  |  | `Boolean` |  | Individual Payment |  |  |
| `PaymentIsToBeSentByEDI` | `XEDIP` |  |  |  |  | `Boolean` |  | Pmnt advice by EDI |  |  |
| `HouseBank` | `HBKID` |  |  |  |  | `String(5)` |  | House Bank |  |  |
| `CheckPaidDurationInDays` | `KULTG` |  |  |  |  | `Decimal(3,0)` |  | Check Cashing Time |  |  |
| `Currency` | `WAERS` | `LFB1` | `WAERS` |  |  | `String(5)` |  | Currency |  |  |
| `BillOfExchLmtAmtInCoCodeCrcy` | `WEBTR_CS` |  |  |  |  | `Decimal(34,4)` |  | Bill/Ex. Limit | Currency |  |
| `SupplierClerkIDBySupplier` | `EIKTO_K` |  |  |  |  | `String(12)` |  | Account with vendor |  |  |
| `IsDoubleInvoice` | `REPRF` |  |  |  |  | `Boolean` |  | Check Double Invoice |  |  |
| `CustomerSupplierClearingIsUsed` | `XVERR_LFB1` |  |  |  |  | `Boolean` |  | Clearing w/ Customer |  |  |
| `ReconciliationAccount` | `AKONT` | `LFB1` | `AKONT` |  |  | `String(10)` |  | Reconciliation Acct |  |  |
| `InterestCalculationCode` | `VZSKZ` |  |  |  |  | `String(2)` |  | Interest Indicator |  |  |
| `InterestCalculationDate` | `DZINDT` |  |  |  |  | `Date` |  | Last Key Date |  |  |
| `IntrstCalcFrequencyInMonths` | `DZINRT` |  |  |  |  | `String(2)` |  | Int.Calc.Freq. |  |  |
| `SupplierHeadOffice` | `LNRZE` |  |  |  |  | `String(10)` |  | Head Office |  |  |
| `AlternativePayee` | `LNRZB` |  |  |  |  | `String(10)` |  | Alternative payee |  |  |
| `LayoutSortingRule` | `DZUAWA` |  |  |  |  | `String(3)` |  | Sort key |  |  |
| `APARToleranceGroup` | `TOGRU` |  |  |  |  | `String(4)` |  | Tolerance Group |  |  |
| `SuplrInvcVerificatTolGroup` | `TOGRR` |  |  |  |  | `String(4)` |  | Tolerance Group |  |  |
| `SupplierCertificationDate` | `CERDT` |  |  |  |  | `Date` |  | Certification Date |  |  |
| `SupplierAccountNote` | `KVERM` |  |  |  |  | `String(30)` |  | Account Memo |  |  |
| `WithholdingTaxCountry` | `QLAND` |  |  |  |  | `String(3)` |  | WTax C/R Key |  |  |
| `DeletionIndicator` | `LOEVM_B` |  |  |  |  | `Boolean` |  | Co.Cde Deletion Flag |  |  |
| `CashPlanningGroup` | `FDGRV` |  |  |  |  | `String(10)` |  | Planning Group |  |  |
| `IsToBeCheckedForDuplicates` | `REPRF` |  |  |  |  | `Boolean` |  | Check Double Invoice |  |  |
| `PersonnelNumber` | `PERNR_D` |  |  |  |  | `String(8)` |  | Personnel Number |  |  |
| `PreviousAccountNumber` | `ALTKN` |  |  |  |  | `String(10)` |  | Previous Account No. |  |  |
| `MinorityGroup` | `MINDK` |  |  |  |  | `String(3)` |  | Minority Indicator |  |  |
| `LastInterestCalcRunDate` | `DATLZ` |  |  |  |  | `Date` |  | Last Int. Calc. |  |  |
| `US_ForeignSuplrHasPartnership` | `FIWTUS_PARTNERSHIP_IND` |  |  |  |  | `String(1)` |  | Partnership Int Ind |  |  |
| `US_SecondTINNoticeIsIssued` | `FIWTUS_SECOND_TIN_NOTICE` |  |  |  |  | `String(1)` |  | Second TIN Notice |  |  |
| `US_ForeignSuplrLmtnOnBnftCode` | `FIWTUS_LOB_CODE` |  |  |  |  | `String(2)` |  | LOB Treaty Code |  |  |
| `SupplierReleaseGroup` | `FRGRP` |  |  |  |  | `String(4)` |  | Release Group |  |  |
| `CreditMemoPaymentTerms` | `GUZTE` |  |  |  |  | `String(4)` |  | Credit Memo Pyt Term |  |  |
| `PaymentMethodSupplement` | `UZAWE` |  |  |  |  | `String(2)` |  | Pmt Meth. Supplement |  |  |
| `US_FrgnAcctTaxFilingIsRequired` | `FIWTUS_FATCA_IND` |  |  |  |  | `String(1)` |  | FATCA Ind |  |  |
| `US_RecipientForeignTaxID` | `FIWTUS_RECIPIENT_FTID` |  |  |  |  | `String(22)` |  | US Recipient FTID |  |  |
| `US_FW9ReceiveDate` | `FIWTUS_W9_RECV_DATE` |  |  |  |  | `Date` |  | W9 Form Rec Date |  |  |
| `US_FW8BENReceiveDate` | `FIWTUS_W8_RECV_DATE` |  |  |  |  | `Date` |  | W8 Form Rec Date |  |  |
| `US_FrgnAcctTaxRcpntCntry` | `LAND1` |  |  |  |  | `String(3)` |  | Country/Region Key |  |  |
| `US_GlobIntermediaryIdnNumber` | `FIWTUS_RECIPIENT_GIIN` |  |  |  |  | `String(19)` |  | US Recipient GIIN |  |  |
| `US_LobTreatyCode` | `FIWTUS_LOB_CODE` |  |  |  |  | `String(2)` |  | LOB Treaty Code |  |  |
| `US_Chapter4StatusCode` | `FIWTUS_CHAP4_STATUS_CODE` |  |  |  |  | `String(2)` |  | Chaptr 4 Status Code |  |  |
| `PaymentClearingGroup` | `FAR_PAYMENT_CLEARING_GROUP` |  |  |  |  | `String(8)` |  | Payment Clrg Grp ID |  |  |
| `PaymentReason` | `FARP_PAYT_RSN` |  |  |  |  | `String(4)` |  | Payment Reason |  |  |
| `DeletionIsBlocked` | `NODEL_B` |  |  |  |  | `Boolean` |  | CoCd Deletion Block |  |  |
| `IsActiveEntity` | `SDRAFT_IS_ACTIVE` |  |  |  |  | `Boolean` |  | Is active |  |  |
| `UK_ContractorBusinessType` | `CIS_CATEGORY` |  |  |  |  | `String(12)` |  | Business Type |  |  |
| `UK_PartnerTradingName` | `CIS_PARTNER_NAME` |  |  |  |  | `String(30)` |  | Prtnr's Trading Name |  |  |
| `UK_PartnerTaxReference` | `CIS_PARTNER_UTR` |  |  |  |  | `String(20)` |  | Partner's UTR |  |  |
| `UK_VerificationStatus` | `CIS_VFNSTATUS` |  |  |  |  | `String(3)` |  | Verification Status |  |  |
| `UK_VerificationNumber` | `GB_CIS_SC_VFNNUM` |  |  |  |  | `String(20)` |  | Verification Number |  |  |
| `UK_CompanyRegistrationNumber` | `GB_CIS_CRN` |  |  |  |  | `String(8)` |  | Comp. House Reg. No. |  |  |
| `UK_VerifiedTaxStatus` | `CIS_VFN_ID` |  |  |  |  | `String(1)` |  | Tax Status |  |  |


## Entity: `SupplierPurchasingOrganization`

- **ABAP CDS Name:** `I_SupplierPurchasingOrg`
- **Label:** Supplier Purchasing Organization
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** LFA1, LFM1

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Supplier` | `ELIFN` | `LFA1` | `LIFNR` |  |  | `String(10)` | Y | Supplier |  |  |
| `PurchasingOrganization` | `EKORG` | `LFM1` | `EKORG` |  |  | `String(4)` | Y | Purch. Organization |  |  |
| `PurchasingGroup` | `EKGRP` |  |  |  |  | `String(3)` |  | Purchasing Group |  |  |
| `MaterialPlannedDeliveryDurn` | `PLIFZ` |  |  |  |  | `Decimal(3,0)` |  | Planned Deliv. Time |  |  |
| `PurchasingIsBlockedForSupplier` | `SPERM_M` |  |  |  |  | `Boolean` |  | Pur. block POrg |  |  |
| `SupplierRespSalesPersonName` | `EVERK` |  |  |  |  | `String(30)` |  | Salesperson |  |  |
| `SupplierPhoneNumber` | `TELFE` |  |  |  |  | `String(16)` |  | Telephone |  |  |
| `PurchaseOrderCurrency` | `BSTWA` |  |  |  |  | `String(5)` |  | Order currency |  |  |
| `MinimumOrderAmount` | `MINBW` |  |  |  |  | `Decimal(34,4)` |  | Minimum order value | PurchaseOrderCurrency |  |
| `CalculationSchemaGroupCode` | `KALSK` |  |  |  |  | `String(2)` |  | Schema Grp, Supplier |  |  |
| `PaymentTerms` | `DZTERM` |  |  |  |  | `String(4)` |  | Terms of Payment |  |  |
| `PricingDateControl` | `MEPRF` |  |  |  |  | `String(1)` |  | Pricing Date Control |  |  |
| `SupplierABCClassificationCode` | `LFABC` |  |  |  |  | `String(1)` |  | ABC indicator |  |  |
| `ShippingCondition` | `VSBED` |  |  |  |  | `String(2)` |  | Shipping Conditions |  |  |
| `PurOrdAutoGenerationIsAllowed` | `KZAUT` |  |  |  |  | `Boolean` |  | Automatic PO |  |  |
| `InvoiceIsGoodsReceiptBased` | `WEBRE` |  |  |  |  | `Boolean` |  | GR-Based Inv. Verif. |  |  |
| `IncotermsClassification` | `INCO1` |  |  |  |  | `String(3)` |  | Incoterms |  |  |
| `IncotermsTransferLocation` | `INCO2` |  |  |  |  | `String(28)` |  | Incoterms (Part 2) |  |  |
| `IncotermsVersion` | `INCOV` |  |  |  |  | `String(4)` |  | Incoterms Version |  |  |
| `IncotermsLocation1` | `INCO2_L` |  |  |  |  | `String(70)` |  | Incoterms Location 1 |  |  |
| `IncotermsLocation2` | `INCO3_L` |  |  |  |  | `String(70)` |  | Incoterms Location 2 |  |  |
| `DeletionIndicator` | `LOEVM_M` |  |  |  |  | `Boolean` |  | Del. flag POrg. |  |  |
| `PlannedDeliveryDurationInDays` | `PLIFZ` |  |  |  |  | `Decimal(3,0)` |  | Planned Deliv. Time |  |  |
| `ContactPersonPhoneNumber` | `TELFE` |  |  |  |  | `String(16)` |  | Telephone |  |  |
| `SupplierConfirmationControlKey` | `BSTAE` |  |  |  |  | `String(4)` |  | Confirmation Control |  |  |
| `IsOrderAcknRqd` | `KZABS` |  |  |  |  | `Boolean` |  | Acknowledgment Reqd. |  |  |
| `EvaldReceiptSettlementIsActive` | `XERSY` |  |  |  |  | `Boolean` |  | Eval. Receipt Sett. |  |  |
| `AutomaticEvaluatedRcptSettlmt` | `XERSR` |  |  |  |  | `Boolean` |  | Aut. ev. GRSetmt.Ret |  |  |
| `SupplierAccountNumber` | `EIKTO_M` |  |  |  |  | `String(12)` |  | Acc. with supplier |  |  |
| `SuplrIsSubjToSubsqntSettlement` | `BOLRE` |  |  |  |  | `Boolean` |  | Subseq. settlement |  |  |
| `SuplrPurgOrgAgrmtOfBusVolIsRqd` | `UMSAE` |  |  |  |  | `Boolean` |  | B.vol.comp./ag.nec. |  |  |
| `SuplrInvcRevalIsAllowed` | `XNBWY` |  |  |  |  | `Boolean` |  | Revaluation |  |  |
| `SuplrPurgOrgIsRlvtForPriceDetn` | `PRFRE_LH` |  |  |  |  | `Boolean` |  | Price determination |  |  |
| `IntrastatCrsBorderTrMode` | `EXPVZ` |  |  |  |  | `String(1)` |  | Mode of Transport |  |  |
| `ProductUnitGroup` | `MEGRU` |  |  |  |  | `String(4)` |  | Unit of Measure Grp |  |  |
| `RoundingProfile` | `RDPRF` |  |  |  |  | `String(4)` |  | Rounding Profile |  |  |
| `PlanningCycle` | `LFRHY` |  |  |  |  | `String(3)` |  | Planning Cycle |  |  |
| `SuplrDiscountInKindIsGranted` | `XFELD` |  |  |  |  | `Boolean` |  |  |  |  |
| `SuplrIsRlvtForSettlmtMgmt` | `AGREL` |  |  |  |  | `Boolean` |  | Settlement Mgmt. |  |  |
| `InvoiceIsMMServiceEntryBased` | `LEBRE` |  |  |  |  | `Boolean` |  | Srv.-Based Inv. Ver. |  |  |
| `ProdStockAndSlsDataTransfPrfl` | `WVMI_PAPRF` |  |  |  |  | `String(4)` |  | PROACT control prof. |  |  |
| `EvaldRcptSettlementProfile` | `VALID_PRO` |  |  |  |  | `String(4)` |  | Settlement profile |  |  |
| `AbsoluteHandlingSurchargeAmt` | `HSCABS` |  |  |  |  | `Decimal(34,4)` |  | Absolute surcharge | PurchaseOrderCurrency |  |
| `PercentageHandlingSurchargeAmt` | `HSCPE` |  |  |  |  | `Decimal(5,2)` |  | Percentage HSC |  |  |
| `MinimumHandlingSurchargeAmt` | `HSCMIN` |  |  |  |  | `Decimal(34,4)` |  | Minimum HSC | PurchaseOrderCurrency |  |
| `MaximumHandlingSurchargeAmt` | `HSCMAX` |  |  |  |  | `Decimal(34,4)` |  | Max. HSC | PurchaseOrderCurrency |  |
| `AutomDebitCrtnIsEnbldOnGI` | `AUBEL` |  |  |  |  | `Boolean` |  | Auto. debit |  |  |
| `SupplierIsReturnsSupplier` | `KZRET` |  |  |  |  | `Boolean` |  | Returns supplier |  |  |
| `IsActiveEntity` | `SDRAFT_IS_ACTIVE` |  |  |  |  | `Boolean` |  | Is active |  |  |
| `IncotermsSupChnLoc1AddlUUID` |  |  |  |  |  | `UUID` |  | Location UUID |  |  |
| `IncotermsSupChnLoc2AddlUUID` |  |  |  |  |  | `UUID` |  | Location UUID |  |  |
| `IncotermsSupChnDvtgLocAddlUUID` |  |  |  |  |  | `UUID` |  | Location UUID |  |  |
| `AuthorizationGroup` | `BRGRU` |  |  |  |  | `String(4)` |  | Authorization |  |  |


## Entity: `SupplierWithHoldingTax`

- **ABAP CDS Name:** `I_SupplierWithHoldingTax`
- **Label:** Supplier WithHolding Tax
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Supplier` | `LIFNR` |  |  |  |  | `String(10)` | Y | Supplier |  | S/4 only entity |
| `CompanyCode` | `BUKRS` |  |  |  |  | `String(4)` | Y | Company Code |  | S/4 only entity |
| `WithholdingTaxType` | `WITHT` |  |  |  |  | `String(2)` | Y | Withholding Tax Type |  | S/4 only entity |
| `WithholdingTaxNumber` | `WT_WTSTCD` |  |  |  |  | `String(16)` |  | W/tax number |  | S/4 only entity |
| `WithholdingTaxCode` | `WT_WITHCD` |  |  |  |  | `String(2)` |  | W/Tax Code |  | S/4 only entity |
| `IsWithholdingTaxSubject` | `WT_SUBJCT` |  |  |  |  | `Boolean` |  | Subject to W/Tx |  | S/4 only entity |
| `RecipientType` | `WT_QSREC` |  |  |  |  | `String(2)` |  | Recipient Type |  | S/4 only entity |
| `WithholdingTaxCertificate` | `WT_EXNR` |  |  |  |  | `String(25)` |  | Exemption Number |  | S/4 only entity |
| `WithholdingTaxExmptPercent` | `WT_EXRT` |  |  |  |  | `Decimal(5,2)` |  | Exemption Rate |  | S/4 only entity |
| `ExemptionDateBegin` | `WT_EXDF` |  |  |  |  | `Date` |  | Exemption Start Date |  | S/4 only entity |
| `ExemptionDateEnd` | `WT_EXDT` |  |  |  |  | `Date` |  | Exemption End Date |  | S/4 only entity |
| `ExemptionReason` | `WT_WTEXRS` |  |  |  |  | `String(2)` |  | Exemption Reason |  | S/4 only entity |
