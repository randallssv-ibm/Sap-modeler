# Supplier

> Source file: `sap-s4com-Supplier-v1.json`

**Technical Name:** `` | **Data Category:** `DIMENSION` | **VDM Type:** `BASIC` | **Size:** `XL`


## Entity: `Supplier`

- **ABAP Name:** `I_Supplier`
- **Label:** Supplier
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** ADRC, LFA1

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Supplier` | `LIFNR` | `LIFNR` | `LFA1` | `String(10)` | Y | Supplier |  |  |  |
| `SupplierAccountGroup` | `KTOKK` | `KTOKK` | `LFA1` | `String(4)` |  | Account Group |  |  |  |
| `SupplierName` | `MD_SUPPLIER_NAME` | `MD_SUPPLIER_NAME` | `LFA1` | `String(80)` |  | Name of Supplier |  |  |  |
| `SupplierFullName` | `MD_SUPPLIER_FULL_NAME` | `MD_SUPPLIER_FULL_NAME` | `LFA1` | `String(220)` |  | Supplier Name |  |  |  |
| `BPSupplierName` | `SUPPLIERNAME_2` | `SUPPLIERNAME_2` | `LFA1` | `String(81)` |  | Business Partner - Supplier Name |  |  |  |
| `BPSupplierFullName` | `SUPPLIERFULLNAME_2` | `SUPPLIERFULLNAME_2` | `LFA1` | `String(163)` |  | Business Partner - Supplier Full Name |  |  |  |
| `BusinessPartnerName1` | `AD_NAME1` | `AD_NAME1` | `LFA1` | `String(40)` |  | Business Partner Organization  - Name 1 |  |  |  |
| `BusinessPartnerName2` | `AD_NAME2` | `AD_NAME2` | `LFA1` | `String(40)` |  | Business Partner Organization  - Name 2 |  |  |  |
| `BusinessPartnerName3` | `AD_NAME3` | `AD_NAME3` | `LFA1` | `String(40)` |  | Business Partner Organization  - Name 3 |  |  |  |
| `BusinessPartnerName4` | `AD_NAME4` | `AD_NAME4` | `LFA1` | `String(40)` |  | Business Partner Organization  - Name 4 |  |  |  |
| `BPAddrCityName` | `AD_CITY1` | `AD_CITY1` | `LFA1` | `String(40)` |  | Business Partner Address – City |  |  |  |
| `BPAddrStreetName` | `AD_STREET` | `AD_STREET` | `LFA1` | `String(60)` |  | Business Partner Address – Street |  |  |  |
| `AddressSearchTerm1` | `AD_SORT1` | `AD_SORT1` | `LFA1` | `String(20)` |  | Business Partner Address - Search Term 1 |  |  |  |
| `AddressSearchTerm2` | `AD_SORT2` | `AD_SORT2` | `LFA1` | `String(20)` |  | Business Partner Address - Search Term 2 |  |  |  |
| `DistrictName` | `AD_CITY2` | `AD_CITY2` | `LFA1` | `String(40)` |  | Business Partner Address – District |  |  |  |
| `POBoxDeviatingCityName` | `AD_POBXLOC` | `AD_POBXLOC` | `LFA1` | `String(40)` |  | Business Partner Address - PO Box Deviating City |  |  |  |
| `BusinessPartnerFormOfAddress` | `AD_TITLE` | `AD_TITLE` | `LFA1` | `String(4)` |  | Business Partner - Form of Address |  |  |  |
| `IsBusinessPurposeCompleted` |  |  |  | `Boolean` |  | Purpose Completed |  |  |  |
| `CreatedByUser` | `ERNAM_RF` | `ERNAM_RF` | `LFA1` | `String(12)` |  | Created By |  |  |  |
| `CreationDate` | `ERDAT_RF` | `ERDAT_RF` | `LFA1` | `Date` |  | Created On |  |  |  |
| `IsOneTimeAccount` | `XCPDK` | `XCPDK` | `LFA1` | `Boolean` |  | One-Time Account |  |  |  |
| `AuthorizationGroup` | `BRGRU` | `BRGRU` | `LFA1` | `String(4)` |  | Authorization |  |  |  |
| `VATRegistration` | `STCEG` | `STCEG` | `LFA1` | `String(20)` |  | VAT Registration No. |  |  |  |
| `AccountIsBlockedForPosting` | `SPERB_X` | `SPERB_X` | `LFA1` | `Boolean` |  | Posting Block(Deprecated) |  |  |  |
| `TaxJurisdiction` | `TXJCD` | `TXJCD` | `LFA1` | `String(15)` |  | Tax Jurisdiction |  |  |  |
| `SupplierStandardCarrierAccess` | `SCACD` | `SCACD` | `LFA1` | `String(4)` |  | SCAC |  |  |  |
| `SupplierFwdAgentFreightGroup` | `SFRGR` | `SFRGR` | `LFA1` | `String(4)` |  | Carrier freight grp |  |  |  |
| `SupplierAgentProcedureGroup` | `DLGRP` | `DLGRP` | `LFA1` | `String(4)` |  | ServAgntProcGrp |  |  |  |
| `SupplIsSocialInsuranceRegtrd` | `J_1AREGSS` | `J_1AREGSS` | `LFA1` | `Boolean` |  | Social Insurance |  |  |  |
| `SocialInsuranceActivityCode` | `J_1AACTSS` | `J_1AACTSS` | `LFA1` | `String(3)` |  | Social Ins. Code |  |  |  |
| `SupplierCorporateGroup` | `KONZS` | `KONZS` | `LFA1` | `String(10)` |  | Group Key |  |  |  |
| `Customer` | `KUNNR` | `KUNNR` | `LFA1` | `String(10)` |  | Customer |  |  |  |
| `Industry` | `BRSCH` | `BRSCH` | `LFA1` | `String(4)` |  | Industry |  |  |  |
| `TaxNumber1` | `STCD1` | `STCD1` | `LFA1` | `String(16)` |  | Tax Number 1 |  |  |  |
| `TaxNumber2` | `STCD2` | `STCD2` | `LFA1` | `String(11)` |  | Tax Number 2 |  |  |  |
| `TaxNumber3` | `STCD3` | `STCD3` | `LFA1` | `String(18)` |  | Tax Number 3 |  |  |  |
| `TaxNumber4` | `STCD4` | `STCD4` | `LFA1` | `String(18)` |  | Tax Number 4 |  |  |  |
| `TaxNumber5` | `STCD5` | `STCD5` | `LFA1` | `String(60)` |  | Tax Number 5 |  |  |  |
| `TaxNumber6` | `STCD6` | `STCD6` | `LFA1` | `String(20)` |  | Tax Number 6 |  |  |  |
| `PostingIsBlocked` | `SPERB_X` | `SPERB_X` | `LFA1` | `Boolean` |  | Posting Block |  |  |  |
| `PurchasingIsBlocked` | `SPERM_X` | `SPERM_X` | `LFA1` | `Boolean` |  | Purch. Block |  |  |  |
| `InternationalLocationNumber1` | `BBBNR` | `BBBNR` | `LFA1` | `String(7)` |  | Int. location no. 1 |  |  |  |
| `InternationalLocationNumber2` | `BBSNR` | `BBSNR` | `LFA1` | `String(5)` |  | Int. location no. 2 |  |  |  |
| `InternationalLocationNumber3` | `BUBKZ` | `BUBKZ` | `LFA1` | `String(1)` |  | Check Digit |  |  |  |
| `AddressID` | `ADRNR` | `ADDRNUMBER` | `ADRC` | `String(10)` |  | Address |  |  |  |
| `Region` | `REGIO` | `REGIO` | `LFA1` | `String(3)` |  | Region |  |  |  |
| `OrganizationBPName1` | `NAME1_GP` | `NAME1_GP` | `LFA1` | `String(35)` |  | Name |  |  |  |
| `OrganizationBPName2` | `NAME2_GP` | `NAME2_GP` | `LFA1` | `String(35)` |  | Name 2 |  |  |  |
| `CityName` | `ORT01_GP` | `ORT01_GP` | `LFA1` | `String(35)` |  | City |  |  |  |
| `PostalCode` | `PSTLZ` | `PSTLZ` | `LFA1` | `String(10)` |  | Postal Code |  |  |  |
| `StreetName` | `STRAS_GP` | `STRAS_GP` | `LFA1` | `String(35)` |  | Street |  |  |  |
| `Country` | `LAND1_GP` | `LAND1_GP` | `LFA1` | `String(3)` |  | Country/Region Key |  |  |  |
| `ConcatenatedInternationalLocNo` | `MD_INTERNATIONAL_LOC` | `MD_INTERNATIONAL_LOC` | `LFA1` | `String(20)` |  | Int. Location No. |  |  |  |
| `SupplierProcurementBlock` | `QSPERRFKT` | `QSPERRFKT` | `LFA1` | `String(2)` |  | Block Function |  |  |  |
| `SuplrQualityManagementSystem` | `QSSYS_IST` | `QSSYS_IST` | `LFA1` | `String(4)` |  | Actual QM System |  |  |  |
| `SuplrQltyInProcmtCertfnValidTo` | `QQSSYSDAT` | `QQSSYSDAT` | `LFA1` | `Date` |  | QM System Valid To |  |  |  |
| `SupplierLanguage` | `SPRAS` | `SPRAS` | `LFA1` | `String(2)` |  | Language Key |  |  |  |
| `AlternativePayeeAccountNumber` | `LNRZA` | `LNRZA` | `LFA1` | `String(10)` |  | Alternative Payee |  |  |  |
| `PhoneNumber1` | `TELF1` | `TELF1` | `LFA1` | `String(16)` |  | Telephone 1 |  |  |  |
| `FaxNumber` | `TELFX` | `TELFX` | `LFA1` | `String(31)` |  | Fax Number |  |  |  |
| `IsNaturalPerson` |  |  |  | `Boolean` |  | Natural Person |  |  |  |
| `TaxNumberResponsible` | `STENR` | `STENR` | `LFA1` | `String(18)` |  | Tax Number |  |  |  |
| `UK_ContractorBusinessType` | `CIS_CATEGORY` | `CIS_CATEGORY` | `LFA1` | `String(12)` |  | Business Type |  |  |  |
| `UK_PartnerTradingName` | `CIS_PARTNER_NAME` | `CIS_PARTNER_NAME` | `LFA1` | `String(30)` |  | Prtnr's Trading Name |  |  |  |
| `UK_PartnerTaxReference` | `CIS_PARTNER_UTR` | `CIS_PARTNER_UTR` | `LFA1` | `String(20)` |  | Partner's UTR |  |  |  |
| `UK_VerificationStatus` | `CIS_VFNSTATUS` | `CIS_VFNSTATUS` | `LFA1` | `String(3)` |  | Verification Status |  |  |  |
| `UK_VerificationNumber` | `GB_CIS_SC_VFNNUM` | `GB_CIS_SC_VFNNUM` | `LFA1` | `String(20)` |  | Verification Number |  |  |  |
| `UK_CompanyRegistrationNumber` | `GB_CIS_CRN` | `GB_CIS_CRN` | `LFA1` | `String(8)` |  | Comp. House Reg. No. |  |  |  |
| `UK_VerifiedTaxStatus` | `CIS_VFN_ID` | `CIS_VFN_ID` | `LFA1` | `String(1)` |  | Tax Status |  |  |  |
| `FormOfAddress` | `ANRED` | `ANRED` | `LFA1` | `String(15)` |  | Title |  |  |  |
| `ReferenceAccountGroup` | `KTOCK` | `KTOCK` | `LFA1` | `String(4)` |  | Reference Acct Group |  |  |  |
| `VATLiability` | `STKZU` | `STKZU` | `LFA1` | `Boolean` |  | Liable for VAT |  |  |  |
| `ResponsibleType` | `J_1AFITP_D` | `J_1AFITP` | `LFA1` | `String(2)` |  | Tax Type |  |  |  |
| `TaxNumberType` | `J_1ATOID` | `J_1ATOID` | `LFA1` | `String(2)` |  | Tax Number Type |  |  |  |
| `FiscalAddress` | `FISKN_K` | `FISKN_K` | `LFA1` | `String(10)` |  | Fiscal Address |  |  |  |
| `BusinessType` | `GESTYP` | `GESTYP` | `LFA1` | `String(30)` |  | Type of Business |  |  |  |
| `BirthDate` | `GBDAT_Q` | `GBDAT_Q` | `LFA1` | `Date` |  | Date of Birth |  |  |  |
| `PaymentIsBlockedForSupplier` | `SPERZ` | `SPERZ` | `LFA1` | `Boolean` |  | Payment Block |  |  |  |
| `SortField` | `SORTL` | `SORTL` | `LFA1` | `String(10)` |  | Search Term |  |  |  |
| `PhoneNumber2` | `TELF2` | `TELF2` | `LFA1` | `String(16)` |  | Telephone 2 |  |  |  |
| `DeletionIndicator` | `LOEVM_X` | `LOEVM_X` | `LFA1` | `Boolean` |  | Deletion Flag |  |  |  |
| `TaxInvoiceRepresentativeName` | `REPRES` | `REPRES` | `LFA1` | `String(10)` |  | Rep's Name |  |  |  |
| `IndustryType` | `INDTYP` | `INDTYP` | `LFA1` | `String(30)` |  | Type of Industry |  |  |  |
| `IN_GSTSupplierClassification` | `J_1IGTAKLD` | `J_1IGTAKLD` | `LFA1` | `String(1)` |  | GST Ven Class. |  |  |  |
| `SuplrProofOfDelivRlvtCode` | `PODKZB` | `PODKZB` | `LFA1` | `String(1)` |  | Relevant for POD |  |  |  |
| `TradingPartner` | `RASSC` | `RASSC` | `LFA1` | `String(6)` |  | Trading Partner No. |  |  |  |
| `BR_TaxIsSplit` | `J_1BINDEQU` | `J_1BINDEQU` | `LFA1` | `Boolean` |  | Tax Split |  |  |  |
| `AU_PayerIsPayingToCarryOnEnt` | `FIAPAU_CARRY_ENT` | `FIAPAU_CARRY_ENT` | `LFA1` | `String(1)` |  | Enterprise in AU |  |  |  |
| `AU_IndividualIsUnder18` | `FIAPAU_IND_UNDER_18` | `FIAPAU_IND_UNDER_18` | `LFA1` | `String(1)` |  | Individual |  |  |  |
| `AU_PaymentIsExceeding75` | `FIAPAU_PMNT_NOT_EXCEED` | `FIAPAU_PMNT_NOT_EXCEED` | `LFA1` | `String(1)` |  | Payment Does not Exc |  |  |  |
| `AU_PaymentIsWhollyInputTaxed` | `FIAPAU_INPUT_TAXED` | `FIAPAU_INPUT_TAXED` | `LFA1` | `String(1)` |  | Wholly Input Taxed |  |  |  |
| `AU_PartnerIsSupplyWithoutGain` | `FIAPAU_PARTNER_NO_GAIN` | `FIAPAU_PARTNER_NO_GAIN` | `LFA1` | `String(1)` |  | Individual w/o Gain |  |  |  |
| `AU_SupplierIsEntitledToABN` | `FIAPAU_ABN_ELIGIBLE` | `FIAPAU_ABN_ELIGIBLE` | `LFA1` | `String(1)` |  | ABN Eligible |  |  |  |
| `AU_PaymentIsIncomeExempted` | `FIAPAU_PMNT_EXEMPT` | `FIAPAU_PMNT_EXEMPT` | `LFA1` | `String(1)` |  | Payment Exempt |  |  |  |
| `AU_SupplyIsMadeAsPrivateHobby` | `FIAPAU_PVT_HOBBY` | `FIAPAU_PVT_HOBBY` | `LFA1` | `String(1)` |  | Hobby |  |  |  |
| `AU_SupplyMadeIsOfDmstcNature` | `FIAPAU_DOM_NATURE` | `FIAPAU_DOM_NATURE` | `LFA1` | `String(1)` |  | Domestic |  |  |  |
| `IsToBeAcceptedAtOrigin` | `WEORA` | `WEORA` | `LFA1` | `Boolean` |  | Origin Acceptance |  |  |  |
| `BPIsEqualizationTaxSubject` | `XFELD` | `XFELD` | `LFA1` | `Boolean` |  |  |  |  |  |
| `BRSpcfcTaxBasePercentageCode` | `TAXBS` | `TAXBS` | `LFA1` | `String(1)` |  | Tax Base |  |  |  |
| `SupplierProfession` | `PROFS` | `PROFS` | `LFA1` | `String(30)` |  | Profession |  |  |  |
| `SuplrManufacturerExternalName` | `EMNFR` | `EMNFR` | `LFA1` | `String(10)` |  | Ext. manufacturer |  |  |  |
| `DataMediumExchangeIndicator` | `DTAMS` | `DTAMS` | `LFA1` | `String(1)` |  | DME Recipient Code |  |  |  |
| `DataExchangeInstructionKey` | `DTAWS` | `DTAWS` | `LFA1` | `String(2)` |  | Instruction Key |  |  |  |
| `SupplierIsSubRangeRelevant` | `LTSNA` | `LTSNA` | `LFA1` | `Boolean` |  | VSR Relevant |  |  |  |
| `TrainStationName` | `BAHNS` | `BAHNS` | `LFA1` | `String(25)` |  | Train Station |  |  |  |
| `AlternativePayeeIsAllowed` | `XZEMP` | `XZEMP` | `LFA1` | `Boolean` |  | Payee in Document |  |  |  |
| `PaytSlipWthRefSubscriber` | `ESRNR` | `ESRNR` | `LFA1` | `String(11)` |  | PBC/ISR Number |  |  |  |
| `TranspServiceAgentStstcGrp` | `STGDL` | `STGDL` | `LFA1` | `String(2)` |  | Stat. Grp, Agent |  |  |  |
| `SupplierIsPlantRelevant` | `WERKR` | `WERKR` | `LFA1` | `Boolean` |  | Plant Level Relevant |  |  |  |
| `SuplrTaxAuthorityAccountNumber` | `FISKU` | `FISKU` | `LFA1` | `String(10)` |  | Tax Office |  |  |  |
| `SuplrCarrierConfirmIsExpected` |  |  |  | `String(1)` |  | Carrier confirmation |  |  |  |
| `SupplierPlant` | `WERKS_EXT` | `WERKS_EXT` | `LFA1` | `String(4)` |  | Plant |  |  |  |
| `FactoryCalendar` | `FABKL` | `FABKL` | `LFA1` | `String(2)` |  | Factory Calendar |  |  |  |
| `PaymentReason` | `FARP_PAYT_RSN` | `PAYT_RSN` | `LFA1` | `String(4)` |  | Payment Reason |  |  |  |
| `SupplierCentralDeletionIsBlock` | `NODEL_X` | `NODEL_X` | `LFA1` | `Boolean` |  | Central Del. Block |  |  |  |
| `DataControllerSet` | `BU_XDCSET` | `BU_XDCSET` | `LFA1` | `String(1)` |  | Data Ctrlr. Set |  |  |  |
| `DataController1` | `BU_DATA_CONTROLLER` | `BU_DATA_CONTROLLER` | `LFA1` | `String(30)` |  | Data Controller |  |  |  |
| `DataController2` | `BU_DATA_CONTROLLER` | `BU_DATA_CONTROLLER` | `LFA1` | `String(30)` |  | Data Controller |  |  |  |
| `DataController3` | `BU_DATA_CONTROLLER` | `BU_DATA_CONTROLLER` | `LFA1` | `String(30)` |  | Data Controller |  |  |  |
| `DataController4` | `BU_DATA_CONTROLLER` | `BU_DATA_CONTROLLER` | `LFA1` | `String(30)` |  | Data Controller |  |  |  |
| `DataController5` | `BU_DATA_CONTROLLER` | `BU_DATA_CONTROLLER` | `LFA1` | `String(30)` |  | Data Controller |  |  |  |
| `DataController6` | `BU_DATA_CONTROLLER` | `BU_DATA_CONTROLLER` | `LFA1` | `String(30)` |  | Data Controller |  |  |  |
| `DataController7` | `BU_DATA_CONTROLLER` | `BU_DATA_CONTROLLER` | `LFA1` | `String(30)` |  | Data Controller |  |  |  |
| `DataController8` | `BU_DATA_CONTROLLER` | `BU_DATA_CONTROLLER` | `LFA1` | `String(30)` |  | Data Controller |  |  |  |
| `DataController9` | `BU_DATA_CONTROLLER` | `BU_DATA_CONTROLLER` | `LFA1` | `String(30)` |  | Data Controller |  |  |  |
| `DataController10` | `BU_DATA_CONTROLLER` | `BU_DATA_CONTROLLER` | `LFA1` | `String(30)` |  | Data Controller |  |  |  |
| `SupplierTransportationChain` | `WRF_PSCD_TC_ID` | `WRF_PSCD_TC_ID` | `LFA1` | `String(10)` |  | Transportation Chain |  |  |  |
| `SupplierStagingTimeInDays` | `WRF_PSCD_MST` | `WRF_PSCD_MST` | `LFA1` | `Decimal(3,0)` |  | Staging Time |  |  |  |
| `SupplierSchedulingProcedure` | `WRF_PSCD_SCHED_TYPE` | `WRF_PSCD_SCHED_TYPE` | `LFA1` | `String(1)` |  | Scheduling Procedure |  |  |  |
| `CollectiveNumberingIsRelevant` | `WRF_SUBMI_RELEVANT` | `WRF_SUBMI_RELEVANT` | `LFA1` | `Boolean` |  | Rel. for Coll. No. |  |  |  |
| `BusinessPartnerPanNumber` | `J_1IPANNO` | `J_1IPANNO` | `LFA1` | `String(40)` |  | PAN |  |  |  |
| `BPPanReferenceNumber` | `J_1IPANREF` | `J_1IPANREF` | `LFA1` | `String(40)` |  | PAN Reference Number |  |  |  |
| `BPPanValidFromDate` | `J_1IPANVALDT` | `J_1IPANVALDT` | `LFA1` | `Date` |  | PAN Valid From Date |  |  |  |


## Entity: `SupplierCompanyCode`

- **ABAP Name:** `I_SupplierCompany`
- **Label:** Supplier Company
- **VDM Type:** `BASIC` | **Data Category:** `FACT`
- **ECC Source Tables:** LFB1, T001

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Supplier` | `LIFNR` | `LIFNR` | `LFB1` | `String(10)` | Y | Supplier |  | _Supplier |  |
| `CompanyCode` | `BUKRS` | `BUKRS` | `T001` | `String(4)` | Y | Company Code |  | _CompanyCode |  |
| `AuthorizationGroup` | `BRGRU` | `BRGRU` | `LFB1` | `String(4)` |  | Authorization |  |  |  |
| `CompanyCodeName` | `BUTXT` | `BUTXT` | `LFB1` | `String(25)` |  | Company Name |  |  |  |
| `PaymentBlockingReason` | `DZAHLS` | `DZAHLS` | `LFB1` | `String(1)` |  | Payment Block |  |  |  |
| `SupplierIsBlockedForPosting` | `SPERB_B` | `SPERB_B` | `LFB1` | `Boolean` |  | Co.code post.block |  |  |  |
| `IsBusinessPurposeCompleted` |  |  |  | `Boolean` |  | Purpose Completed |  |  |  |
| `AccountingClerk` | `BUSAB` | `BUSAB` | `LFB1` | `String(2)` |  | Clerk Abbrev. |  |  |  |
| `AccountingClerkFaxNumber` | `TLFXS` | `TLFXS` | `LFB1` | `String(31)` |  | Acctg clerk's fax |  |  |  |
| `AccountingClerkPhoneNumber` | `TLFNS` | `TLFNS` | `LFB1` | `String(30)` |  | Acct.clerks tel.no. |  |  |  |
| `AccountingClerkInternetAddress` | `INTAD` | `INTAD` | `LFB1` | `String(130)` |  | Clrk's internet add. |  |  |  |
| `SupplierClerk` | `DZSABE_K` | `DZSABE_K` | `LFB1` | `String(15)` |  | Clerk at vendor |  |  |  |
| `SupplierClerkURL` | `INTAD` | `INTAD` | `LFB1` | `String(130)` |  | Clrk's internet add. |  |  |  |
| `PaymentMethodsList` | `DZWELS` | `DZWELS` | `LFB1` | `String(10)` |  | Payment Methods |  |  |  |
| `PaymentTerms` | `DZTERM` | `DZTERM` | `LFB1` | `String(4)` |  | Terms of Payment |  |  |  |
| `ClearCustomerSupplier` | `XVERR_LFB1` | `XVERR_LFB1` | `LFB1` | `Boolean` |  | Clearing w/ Customer |  |  |  |
| `IsToBeLocallyProcessed` | `XDEZV` | `XDEZV` | `LFB1` | `Boolean` |  | Local Processing |  |  |  |
| `ItemIsToBePaidSeparately` | `XPORE` | `XPORE` | `LFB1` | `Boolean` |  | Individual Payment |  |  |  |
| `PaymentIsToBeSentByEDI` | `XEDIP` | `XEDIP` | `LFB1` | `Boolean` |  | Pmnt advice by EDI |  |  |  |
| `HouseBank` | `HBKID` | `HBKID` | `LFB1` | `String(5)` |  | House Bank |  |  |  |
| `CheckPaidDurationInDays` | `KULTG` | `KULTG` | `LFB1` | `Decimal(3,0)` |  | Check Cashing Time |  |  |  |
| `Currency` | `WAERS` | `WAERS` | `LFB1` | `String(5)` |  | Currency |  |  |  |
| `BillOfExchLmtAmtInCoCodeCrcy` | `WEBTR_CS` | `WEBTR_CS` | `LFB1` | `Decimal(34,4)` |  | Bill/Ex. Limit | Currency |  |  |
| `SupplierClerkIDBySupplier` | `EIKTO_K` | `EIKTO_K` | `LFB1` | `String(12)` |  | Account with vendor |  |  |  |
| `IsDoubleInvoice` | `REPRF` | `REPRF` | `LFB1` | `Boolean` |  | Check Double Invoice |  |  |  |
| `CustomerSupplierClearingIsUsed` | `XVERR_LFB1` | `XVERR_LFB1` | `LFB1` | `Boolean` |  | Clearing w/ Customer |  |  |  |
| `ReconciliationAccount` | `AKONT` | `AKONT` | `LFB1` | `String(10)` |  | Reconciliation Acct |  |  |  |
| `InterestCalculationCode` | `VZSKZ` | `VZSKZ` | `LFB1` | `String(2)` |  | Interest Indicator |  |  |  |
| `InterestCalculationDate` | `DZINDT` | `DZINDT` | `LFB1` | `Date` |  | Last Key Date |  |  |  |
| `IntrstCalcFrequencyInMonths` | `DZINRT` | `DZINRT` | `LFB1` | `String(2)` |  | Int.Calc.Freq. |  |  |  |
| `SupplierHeadOffice` | `LNRZE` | `LNRZE` | `LFB1` | `String(10)` |  | Head Office |  |  |  |
| `AlternativePayee` | `LNRZB` | `LNRZB` | `LFB1` | `String(10)` |  | Alternative payee |  |  |  |
| `LayoutSortingRule` | `DZUAWA` | `DZUAWA` | `LFB1` | `String(3)` |  | Sort key |  |  |  |
| `APARToleranceGroup` | `TOGRU` | `TOGRU` | `LFB1` | `String(4)` |  | Tolerance Group |  |  |  |
| `SuplrInvcVerificatTolGroup` | `TOGRR` | `TOGRR` | `LFB1` | `String(4)` |  | Tolerance Group |  |  |  |
| `SupplierCertificationDate` | `CERDT` | `CERDT` | `LFB1` | `Date` |  | Certification Date |  |  |  |
| `SupplierAccountNote` | `KVERM` | `KVERM` | `LFB1` | `String(30)` |  | Account Memo |  |  |  |
| `WithholdingTaxCountry` | `QLAND` | `QLAND` | `LFB1` | `String(3)` |  | WTax C/R Key |  |  |  |
| `DeletionIndicator` | `LOEVM_B` | `LOEVM_B` | `LFB1` | `Boolean` |  | Co.Cde Deletion Flag |  |  |  |
| `CashPlanningGroup` | `FDGRV` | `FDGRV` | `LFB1` | `String(10)` |  | Planning Group |  |  |  |
| `IsToBeCheckedForDuplicates` | `REPRF` | `REPRF` | `LFB1` | `Boolean` |  | Check Double Invoice |  |  |  |
| `PersonnelNumber` | `PERNR_D` | `PERNR` | `LFB1` | `String(8)` |  | Personnel Number |  |  |  |
| `PreviousAccountNumber` | `ALTKN` | `ALTKN` | `LFB1` | `String(10)` |  | Previous Account No. |  |  |  |
| `MinorityGroup` | `MINDK` | `MINDK` | `LFB1` | `String(3)` |  | Minority Indicator |  |  |  |
| `LastInterestCalcRunDate` | `DATLZ` | `DATLZ` | `LFB1` | `Date` |  | Last Int. Calc. |  |  |  |
| `US_ForeignSuplrHasPartnership` | `FIWTUS_PARTNERSHIP_IND` | `FIWTUS_PARTNERSHIP_IND` | `LFB1` | `String(1)` |  | Partnership Int Ind |  |  |  |
| `US_SecondTINNoticeIsIssued` | `FIWTUS_SECOND_TIN_NOTICE` | `FIWTUS_SECOND_TIN_NOTICE` | `LFB1` | `String(1)` |  | Second TIN Notice |  |  |  |
| `US_ForeignSuplrLmtnOnBnftCode` | `FIWTUS_LOB_CODE` | `FIWTUS_LOB_CODE` | `LFB1` | `String(2)` |  | LOB Treaty Code |  |  |  |
| `SupplierReleaseGroup` | `FRGRP` | `FRGRP` | `LFB1` | `String(4)` |  | Release Group |  |  |  |
| `CreditMemoPaymentTerms` | `GUZTE` | `GUZTE` | `LFB1` | `String(4)` |  | Credit Memo Pyt Term |  |  |  |
| `PaymentMethodSupplement` | `UZAWE` | `UZAWE` | `LFB1` | `String(2)` |  | Pmt Meth. Supplement |  |  |  |
| `US_FrgnAcctTaxFilingIsRequired` | `FIWTUS_FATCA_IND` | `FIWTUS_FATCA_IND` | `LFB1` | `String(1)` |  | FATCA Ind |  |  |  |
| `US_RecipientForeignTaxID` | `FIWTUS_RECIPIENT_FTID` | `FIWTUS_RECIPIENT_FTID` | `LFB1` | `String(22)` |  | US Recipient FTID |  |  |  |
| `US_FW9ReceiveDate` | `FIWTUS_W9_RECV_DATE` | `FIWTUS_W9_RECV_DATE` | `LFB1` | `Date` |  | W9 Form Rec Date |  |  |  |
| `US_FW8BENReceiveDate` | `FIWTUS_W8_RECV_DATE` | `FIWTUS_W8_RECV_DATE` | `LFB1` | `Date` |  | W8 Form Rec Date |  |  |  |
| `US_FrgnAcctTaxRcpntCntry` | `LAND1` | `LAND1` | `LFB1` | `String(3)` |  | Country/Region Key |  |  |  |
| `US_GlobIntermediaryIdnNumber` | `FIWTUS_RECIPIENT_GIIN` | `FIWTUS_RECIPIENT_GIIN` | `LFB1` | `String(19)` |  | US Recipient GIIN |  |  |  |
| `US_LobTreatyCode` | `FIWTUS_LOB_CODE` | `FIWTUS_LOB_CODE` | `LFB1` | `String(2)` |  | LOB Treaty Code |  |  |  |
| `US_Chapter4StatusCode` | `FIWTUS_CHAP4_STATUS_CODE` | `FIWTUS_CHAP4_STATUS_CODE` | `LFB1` | `String(2)` |  | Chaptr 4 Status Code |  |  |  |
| `PaymentClearingGroup` | `FAR_PAYMENT_CLEARING_GROUP` | `FAR_PAYMENT_CLEARING_GROUP` | `LFB1` | `String(8)` |  | Payment Clrg Grp ID |  |  |  |
| `PaymentReason` | `FARP_PAYT_RSN` | `PAYT_RSN` | `LFB1` | `String(4)` |  | Payment Reason |  |  |  |
| `DeletionIsBlocked` | `NODEL_B` | `NODEL_B` | `LFB1` | `Boolean` |  | CoCd Deletion Block |  |  |  |
| `IsActiveEntity` | `SDRAFT_IS_ACTIVE` | `SDRAFT_IS_ACTIVE` | `LFB1` | `Boolean` |  | Is active |  |  |  |
| `UK_ContractorBusinessType` | `CIS_CATEGORY` | `CIS_CATEGORY` | `LFB1` | `String(12)` |  | Business Type |  |  |  |
| `UK_PartnerTradingName` | `CIS_PARTNER_NAME` | `CIS_PARTNER_NAME` | `LFB1` | `String(30)` |  | Prtnr's Trading Name |  |  |  |
| `UK_PartnerTaxReference` | `CIS_PARTNER_UTR` | `CIS_PARTNER_UTR` | `LFB1` | `String(20)` |  | Partner's UTR |  |  |  |
| `UK_VerificationStatus` | `CIS_VFNSTATUS` | `CIS_VFNSTATUS` | `LFB1` | `String(3)` |  | Verification Status |  |  |  |
| `UK_VerificationNumber` | `GB_CIS_SC_VFNNUM` | `GB_CIS_SC_VFNNUM` | `LFB1` | `String(20)` |  | Verification Number |  |  |  |
| `UK_CompanyRegistrationNumber` | `GB_CIS_CRN` | `GB_CIS_CRN` | `LFB1` | `String(8)` |  | Comp. House Reg. No. |  |  |  |
| `UK_VerifiedTaxStatus` | `CIS_VFN_ID` | `CIS_VFN_ID` | `LFB1` | `String(1)` |  | Tax Status |  |  |  |


## Entity: `SupplierPurchasingOrganization`

- **ABAP Name:** `I_SupplierPurchasingOrg`
- **Label:** Supplier Purchasing Organization
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** LFA1, LFM1

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Supplier` | `ELIFN` | `LIFNR` | `LFA1` | `String(10)` | Y | Supplier |  | _Supplier |  |
| `PurchasingOrganization` | `EKORG` | `EKORG` | `LFM1` | `String(4)` | Y | Purch. Organization |  |  |  |
| `PurchasingGroup` | `EKGRP` | `EKGRP` | `LFM1` | `String(3)` |  | Purchasing Group |  |  |  |
| `MaterialPlannedDeliveryDurn` | `PLIFZ` | `PLIFZ` | `LFM1` | `Decimal(3,0)` |  | Planned Deliv. Time |  |  |  |
| `PurchasingIsBlockedForSupplier` | `SPERM_M` | `SPERM_M` | `LFM1` | `Boolean` |  | Pur. block POrg |  |  |  |
| `SupplierRespSalesPersonName` | `EVERK` | `EVERK` | `LFM1` | `String(30)` |  | Salesperson |  |  |  |
| `SupplierPhoneNumber` | `TELFE` | `TELFE` | `LFM1` | `String(16)` |  | Telephone |  |  |  |
| `PurchaseOrderCurrency` | `BSTWA` | `BSTWA` | `LFM1` | `String(5)` |  | Order currency |  |  |  |
| `MinimumOrderAmount` | `MINBW` | `MINBW` | `LFM1` | `Decimal(34,4)` |  | Minimum order value | PurchaseOrderCurrency |  |  |
| `CalculationSchemaGroupCode` | `KALSK` | `KALSK` | `LFM1` | `String(2)` |  | Schema Grp, Supplier |  |  |  |
| `PaymentTerms` | `DZTERM` | `DZTERM` | `LFM1` | `String(4)` |  | Terms of Payment |  |  |  |
| `PricingDateControl` | `MEPRF` | `MEPRF` | `LFM1` | `String(1)` |  | Pricing Date Control |  |  |  |
| `SupplierABCClassificationCode` | `LFABC` | `LFABC` | `LFM1` | `String(1)` |  | ABC indicator |  |  |  |
| `ShippingCondition` | `VSBED` | `VSBED` | `LFM1` | `String(2)` |  | Shipping Conditions |  |  |  |
| `PurOrdAutoGenerationIsAllowed` | `KZAUT` | `KZAUT` | `LFM1` | `Boolean` |  | Automatic PO |  |  |  |
| `InvoiceIsGoodsReceiptBased` | `WEBRE` | `WEBRE` | `LFM1` | `Boolean` |  | GR-Based Inv. Verif. |  |  |  |
| `IncotermsClassification` | `INCO1` | `INCO1` | `LFM1` | `String(3)` |  | Incoterms |  |  |  |
| `IncotermsTransferLocation` | `INCO2` | `INCO2` | `LFM1` | `String(28)` |  | Incoterms (Part 2) |  |  |  |
| `IncotermsVersion` | `INCOV` | `INCOV` | `LFM1` | `String(4)` |  | Incoterms Version |  |  |  |
| `IncotermsLocation1` | `INCO2_L` | `INCO2_L` | `LFM1` | `String(70)` |  | Incoterms Location 1 |  |  |  |
| `IncotermsLocation2` | `INCO3_L` | `INCO3_L` | `LFM1` | `String(70)` |  | Incoterms Location 2 |  |  |  |
| `DeletionIndicator` | `LOEVM_M` | `LOEVM_M` | `LFM1` | `Boolean` |  | Del. flag POrg. |  |  |  |
| `PlannedDeliveryDurationInDays` | `PLIFZ` | `PLIFZ` | `LFM1` | `Decimal(3,0)` |  | Planned Deliv. Time |  |  |  |
| `ContactPersonPhoneNumber` | `TELFE` | `TELFE` | `LFM1` | `String(16)` |  | Telephone |  |  |  |
| `SupplierConfirmationControlKey` | `BSTAE` | `BSTAE` | `LFM1` | `String(4)` |  | Confirmation Control |  |  |  |
| `IsOrderAcknRqd` | `KZABS` | `KZABS` | `LFM1` | `Boolean` |  | Acknowledgment Reqd. |  |  |  |
| `EvaldReceiptSettlementIsActive` | `XERSY` | `XERSY` | `LFM1` | `Boolean` |  | Eval. Receipt Sett. |  |  |  |
| `AutomaticEvaluatedRcptSettlmt` | `XERSR` | `XERSR` | `LFM1` | `Boolean` |  | Aut. ev. GRSetmt.Ret |  |  |  |
| `SupplierAccountNumber` | `EIKTO_M` | `EIKTO_M` | `LFM1` | `String(12)` |  | Acc. with supplier |  |  |  |
| `SuplrIsSubjToSubsqntSettlement` | `BOLRE` | `BOLRE` | `LFM1` | `Boolean` |  | Subseq. settlement |  |  |  |
| `SuplrPurgOrgAgrmtOfBusVolIsRqd` | `UMSAE` | `UMSAE` | `LFM1` | `Boolean` |  | B.vol.comp./ag.nec. |  |  |  |
| `SuplrInvcRevalIsAllowed` | `XNBWY` | `XNBWY` | `LFM1` | `Boolean` |  | Revaluation |  |  |  |
| `SuplrPurgOrgIsRlvtForPriceDetn` | `PRFRE_LH` | `PRFRE_LH` | `LFM1` | `Boolean` |  | Price determination |  |  |  |
| `IntrastatCrsBorderTrMode` | `EXPVZ` | `EXPVZ` | `LFM1` | `String(1)` |  | Mode of Transport |  |  |  |
| `ProductUnitGroup` | `MEGRU` | `MEGRU` | `LFM1` | `String(4)` |  | Unit of Measure Grp |  |  |  |
| `RoundingProfile` | `RDPRF` | `RDPRF` | `LFM1` | `String(4)` |  | Rounding Profile |  |  |  |
| `PlanningCycle` | `LFRHY` | `LFRHY` | `LFM1` | `String(3)` |  | Planning Cycle |  |  |  |
| `SuplrDiscountInKindIsGranted` | `XFELD` | `XFELD` | `LFM1` | `Boolean` |  |  |  |  |  |
| `SuplrIsRlvtForSettlmtMgmt` | `AGREL` | `AGREL` | `LFM1` | `Boolean` |  | Settlement Mgmt. |  |  |  |
| `InvoiceIsMMServiceEntryBased` | `LEBRE` | `LEBRE` | `LFM1` | `Boolean` |  | Srv.-Based Inv. Ver. |  |  |  |
| `ProdStockAndSlsDataTransfPrfl` | `WVMI_PAPRF` | `WVMI_PAPRF` | `LFM1` | `String(4)` |  | PROACT control prof. |  |  |  |
| `EvaldRcptSettlementProfile` | `VALID_PRO` | `VALID_PRO` | `LFM1` | `String(4)` |  | Settlement profile |  |  |  |
| `AbsoluteHandlingSurchargeAmt` | `HSCABS` | `HSCABS` | `LFM1` | `Decimal(34,4)` |  | Absolute surcharge | PurchaseOrderCurrency |  |  |
| `PercentageHandlingSurchargeAmt` | `HSCPE` | `HSCPE` | `LFM1` | `Decimal(5,2)` |  | Percentage HSC |  |  |  |
| `MinimumHandlingSurchargeAmt` | `HSCMIN` | `HSCMIN` | `LFM1` | `Decimal(34,4)` |  | Minimum HSC | PurchaseOrderCurrency |  |  |
| `MaximumHandlingSurchargeAmt` | `HSCMAX` | `HSCMAX` | `LFM1` | `Decimal(34,4)` |  | Max. HSC | PurchaseOrderCurrency |  |  |
| `AutomDebitCrtnIsEnbldOnGI` | `AUBEL` | `AUBEL` | `LFM1` | `Boolean` |  | Auto. debit |  |  |  |
| `SupplierIsReturnsSupplier` | `KZRET` | `KZRET` | `LFM1` | `Boolean` |  | Returns supplier |  |  |  |
| `IsActiveEntity` | `SDRAFT_IS_ACTIVE` | `SDRAFT_IS_ACTIVE` | `LFM1` | `Boolean` |  | Is active |  |  |  |
| `IncotermsSupChnLoc1AddlUUID` |  |  |  | `UUID` |  | Location UUID |  |  |  |
| `IncotermsSupChnLoc2AddlUUID` |  |  |  | `UUID` |  | Location UUID |  |  |  |
| `IncotermsSupChnDvtgLocAddlUUID` |  |  |  | `UUID` |  | Location UUID |  |  |  |
| `AuthorizationGroup` | `BRGRU` | `BRGRU` | `LFM1` | `String(4)` |  | Authorization |  |  |  |


## Entity: `SupplierWithHoldingTax`

- **ABAP Name:** `I_SupplierWithHoldingTax`
- **Label:** Supplier WithHolding Tax
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Supplier` | `LIFNR` | `LIFNR` |  | `String(10)` | Y | Supplier |  | _Supplier | S/4 only entity — no ECC CDC mapping |
| `CompanyCode` | `BUKRS` | `BUKRS` |  | `String(4)` | Y | Company Code |  | _CompanyCode | S/4 only entity — no ECC CDC mapping |
| `WithholdingTaxType` | `WITHT` | `WITHT` |  | `String(2)` | Y | Withholding Tax Type |  |  | S/4 only entity — no ECC CDC mapping |
| `WithholdingTaxNumber` | `WT_WTSTCD` | `WT_WTSTCD` |  | `String(16)` |  | W/tax number |  |  | S/4 only entity — no ECC CDC mapping |
| `WithholdingTaxCode` | `WT_WITHCD` | `WT_WITHCD` |  | `String(2)` |  | W/Tax Code |  |  | S/4 only entity — no ECC CDC mapping |
| `IsWithholdingTaxSubject` | `WT_SUBJCT` | `WT_SUBJCT` |  | `Boolean` |  | Subject to W/Tx |  |  | S/4 only entity — no ECC CDC mapping |
| `RecipientType` | `WT_QSREC` | `WT_QSREC` |  | `String(2)` |  | Recipient Type |  |  | S/4 only entity — no ECC CDC mapping |
| `WithholdingTaxCertificate` | `WT_EXNR` | `WT_EXNR` |  | `String(25)` |  | Exemption Number |  |  | S/4 only entity — no ECC CDC mapping |
| `WithholdingTaxExmptPercent` | `WT_EXRT` | `WT_EXRT` |  | `Decimal(5,2)` |  | Exemption Rate |  |  | S/4 only entity — no ECC CDC mapping |
| `ExemptionDateBegin` | `WT_EXDF` | `WT_EXDF` |  | `Date` |  | Exemption Start Date |  |  | S/4 only entity — no ECC CDC mapping |
| `ExemptionDateEnd` | `WT_EXDT` | `WT_EXDT` |  | `Date` |  | Exemption End Date |  |  | S/4 only entity — no ECC CDC mapping |
| `ExemptionReason` | `WT_WTEXRS` | `WT_WTEXRS` |  | `String(2)` |  | Exemption Reason |  |  | S/4 only entity — no ECC CDC mapping |
