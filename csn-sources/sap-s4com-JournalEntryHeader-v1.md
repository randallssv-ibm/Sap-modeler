# JournalEntryHeader

> Source file: `sap-s4com-JournalEntryHeader-v1.json`

**Technical Name:** `IFIJOURNALENT` | **Data Category:** `DIMENSION` | **VDM Type:** `BASIC` | **Size:** `XXL`


## Entity: `JournalEntry`

- **ABAP Name:** `I_JournalEntry`
- **Technical Name:** `IFIJOURNALENT`
- **Label:** Journal Entry
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** BKPF

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `CompanyCode` | `FIS_BUKRS` | `BUKRS` | `BKPF` | `String(4)` | Y | Company Code |  | _CompanyCode |  |
| `FiscalYear` | `FIS_GJAHR_NO_CONV` | `GJAHR` | `BKPF` | `String(4)` | Y | Fiscal Year |  | _FiscalYear |  |
| `AccountingDocument` | `FARP_BELNR_D` | `BELNR` | `BKPF` | `String(10)` | Y | Journal Entry |  |  |  |
| `AccountingDocumentType` | `FARP_BLART` | `BLART` | `BKPF` | `String(2)` |  | Journal Entry Type |  | _AccountingDocumentType |  |
| `DocumentDate` | `FIS_BLDAT` | `BLDAT` | `BKPF` | `Date` |  | Journal Entry Date |  |  |  |
| `PostingDate` | `FIS_BUDAT` | `BUDAT` | `BKPF` | `Date` |  | Posting Date |  |  |  |
| `FiscalPeriod` | `FINS_FISCALPERIOD` | `FISCALPERIOD` | `BKPF` | `String(3)` |  | Fiscal Period |  | _FiscalPeriod | ECC: unpadded '3' (MONAT); S/4: zero-padded '003' |
| `AccountingDocumentCreationDate` | `FARP_CPUDT` | `CPUDT` | `BKPF` | `Date` |  | Entered On |  |  |  |
| `CreationTime` | `TTET_DT_CR_TIME` | `CR_TIME` | `BKPF` | `String(6)` |  | Creation Time |  |  |  |
| `LastManualChangeDate` | `FIS_LASTMANUALCHANGEDATE` | `LASTMANUALCHANGEDATE` | `BKPF` | `Date` |  | Manual Change Date |  |  |  |
| `LastAutomaticChangeDate` | `FIS_LASTAUTOMATICCHANGEDATE` | `LASTAUTOMATICCHANGEDATE` | `BKPF` | `Date` |  | Autom. Change Date |  |  |  |
| `LastChangeDate` | `TTET_DT_CHG_DATE` | `CHG_DATE` | `BKPF` | `Date` |  | Last Change Date |  |  |  |
| `ExchangeRateDate` | `VDM_V_EXCHANGE_RATE_DATE` | `EXCHANGE_RATE_DATE` | `BKPF` | `Date` |  | Exchange Rate Date |  |  |  |
| `AccountingDocCreatedByUser` | `FIS_USNAM` | `USNAM` | `BKPF` | `String(12)` |  | Journal Entry Created By |  |  |  |
| `TransactionCode` | `TCODE` | `TCODE` | `BKPF` | `String(20)` |  | Transaction Code |  |  |  |
| `IntercompanyTransaction` | `FAC_BVORG` | `BVORG` | `BKPF` | `String(16)` |  | Intercompany Transac |  |  |  |
| `DocumentReferenceID` | `FIS_XBLNR1` | `XBLNR1` | `BKPF` | `String(16)` |  | Document Reference ID |  |  |  |
| `RecurringAccountingDocument` | `FIS_RJET_ID` | `RJET_ID` | `BKPF` | `String(10)` |  | Recurring Journal Entry |  |  |  |
| `RecrrgJournalEntryCompanyCode` | `FIS_DBBLG_BUKRS` | `DBBLG_BUKRS` | `BKPF` | `String(4)` |  | Recurring Journal Entry Company Code |  |  |  |
| `RecrrgJournalEntryFiscalYear` | `FIS_DBBLG_GJAHR` | `DBBLG_GJAHR` | `BKPF` | `String(4)` |  | Recurring Journal Entry Fiscal Year |  |  |  |
| `ReverseDocument` | `FIS_STBLG` | `STBLG` | `BKPF` | `String(10)` |  | Reverse Document |  |  |  |
| `ReverseDocumentFiscalYear` | `FIS_STJAH_NO_CONV` | `STJAH` | `BKPF` | `String(4)` |  | Reverse Document Fiscal Year |  |  |  |
| `AccountingDocumentHeaderText` | `BKTXT` | `BKTXT` | `BKPF` | `String(25)` |  | Document Header Text |  |  |  |
| `TransactionCurrency` | `WAERS` | `WAERS` | `BKPF` | `String(5)` |  | Currency |  | _TransactionCurrency |  |
| `AbsoluteExchangeRate` | `FIS_ABSOLUTE_EXCHANGERATE` | `ABSOLUTE_EXCHANGERATE` | `BKPF` | `Decimal(9,5)` |  | Absolute Exchange Rate |  |  |  |
| `ExchangeRate` | `UKURS_CURR` | `UKURS_CURR` | `BKPF` | `Decimal(9,5)` |  | Exchange Rate |  |  |  |
| `ExchRateIsIndirectQuotation` |  |  |  | `Boolean` |  | Exchange Rate Is Indirect Quotation |  |  |  |
| `EffectiveExchangeRate` | `FIS_EFFECTIVE_EXCHANGERATE` | `EFFECTIVE_EXCHANGERATE` | `BKPF` | `Decimal(12,5)` |  | Effective Exch. Rate |  |  |  |
| `AccountingDocumentCategory` | `FIS_BSTAT` | `BSTAT` | `BKPF` | `String(1)` |  | Journal Entry Category |  | _AccountingDocumentCategory |  |
| `NetAmountIsPosted` | `FIS_XNETB` | `XNETB` | `BKPF` | `Boolean` |  | Net Amount Is Posted |  |  |  |
| `JrnlEntryIsPostedToPrevPeriod` | `FIS_XRUEB` | `XRUEB` | `BKPF` | `Boolean` |  | Journal Entry Is Posted To Prev. Period |  |  |  |
| `BusinessTransactionType` | `FINS_BTTYPE` | `BTTYPE` | `BKPF` | `String(4)` |  | Bus. Trans. Category |  | _BusinessTransactionType |  |
| `BatchInputSession` | `FIS_GRPID` | `GRPID` | `BKPF` | `String(12)` |  | Batch Input Session |  |  |  |
| `ReferenceDocumentType` | `FIS_AWTYP` | `AWTYP` | `BKPF` | `String(5)` |  | Reference Document Type |  | _ReferenceDocumentType |  |
| `OriginalReferenceDocument` | `FAC_AWKEY` | `AWKEY` | `BKPF` | `String(20)` |  | Object Key |  |  |  |
| `FinancialManagementArea` | `FIKRS` | `FIKRS` | `BKPF` | `String(4)` |  | FM Area |  | _FinancialManagementArea |  |
| `CompanyCodeCurrency` | `FIS_HWAER` | `HWAER` | `BKPF` | `String(5)` |  | Company Code Currency |  | _CompanyCodeCurrency |  |
| `AdditionalCurrency1` | `FIS_HWAE2` | `HWAE2` | `BKPF` | `String(5)` |  | Additional Crcy 1 |  |  |  |
| `AdditionalCurrency2` | `FIS_HWAE3` | `HWAE3` | `BKPF` | `String(5)` |  | Additional Crcy 2 |  |  |  |
| `ReversalIsPlanned` | `FIS_XSTOV` | `XSTOV` | `BKPF` | `Boolean` |  | Reversal Is Planned |  |  |  |
| `PlannedReversalDate` | `FIS_STODT` | `STODT` | `BKPF` | `Date` |  | Planned Reversal Dte |  |  |  |
| `TaxIsCalculatedAutomatically` | `FIS_XMWST` | `XMWST` | `BKPF` | `Boolean` |  | Tax Is Automatically Calculated |  |  |  |
| `AdditionalCurrency1Role` | `CURT2` | `CURT2` | `BKPF` | `String(2)` |  | LC2 Currency Type |  |  |  |
| `AdditionalCurrency2Role` | `CURT3` | `CURT3` | `BKPF` | `String(2)` |  | LC3 Currency Type |  |  |  |
| `TaxBaseAmountIsNetAmount` | `FIS_XMWSN` | `XMWSN` | `BKPF` | `Boolean` |  | Tax Base Amount is Net Amount |  |  |  |
| `SourceCompanyCode` | `AUSBK` | `AUSBK` | `BKPF` | `String(4)` |  | Source Company Code |  |  |  |
| `LogicalSystem` | `LOGSYSTEM` | `LOGSYSTEM` | `BKPF` | `String(10)` |  | Logical System |  | _LogicalSystem |  |
| `ReferenceDocumentLogicalSystem` | `FIS_AWSYS` | `AWSYS` | `BKPF` | `String(10)` |  | Ref. Doc. Lgcl Syst. |  | _RefDocumentLogicalSystem |  |
| `TaxAbsoluteExchangeRate` | `FIS_ABSOLUTE_TXKRS_BKPF` | `ABSOLUTE_TXKRS_BKPF` | `BKPF` | `Decimal(9,5)` |  | Absolute Tax Exchange Rate |  |  |  |
| `TaxExchangeRate` | `FIS_TXKRS_BKPF` | `TXKRS_BKPF` | `BKPF` | `Decimal(9,5)` |  | Tax Exchange Rate |  |  |  |
| `TaxExchRateIsIndirectQuotation` |  |  |  | `Boolean` |  | Tax Exchange Rate Is Indirect Quotation |  |  |  |
| `TaxEffectiveExchangeRate` | `FIS_TAX_EFFECTIVE_EXCHANGERATE` | `TAX_EFFECTIVE_EXCHANGERATE` | `BKPF` | `Decimal(12,5)` |  | Effective Tax Exchange Rate |  |  |  |
| `CtryCrcyTxAbsoluteExchangeRate` | `CTRYCRCYTXABSOLUTEEXCHANGERATE` | `CTRYCRCYTXABSOLUTEEXCHANGERATE` | `BKPF` | `Decimal(9,5)` |  | Absolute Tax Exch. Rate in C/R Cur. |  |  |  |
| `CtryCrcyTaxEffctvExchangeRate` | `CTRYCRCYTAXEFFCTVEXCHANGERATE` | `CTRYCRCYTAXEFFCTVEXCHANGERATE` | `BKPF` | `Decimal(12,5)` |  | Effective Tax Exch. Rate in C/R Cur. |  |  |  |
| `ReversalReason` | `STGRD` | `STGRD` | `BKPF` | `String(2)` |  | Reversal Reason |  |  |  |
| `ParkedByUser` | `FIS_PPNAM` | `PPNAM` | `BKPF` | `String(12)` |  | JE Parked By |  |  |  |
| `ParkingDate` | `PPDATE` | `PPDATE` | `BKPF` | `Date` |  | Parked On |  |  |  |
| `ParkingTime` | `PPTME` | `PPTME` | `BKPF` | `String(6)` |  | Time of Parking |  |  |  |
| `ParkingTransactionCode` | `FIS_PPTCOD` | `PPTCOD` | `BKPF` | `String(20)` |  | Parking Transaction Code |  |  |  |
| `Branch` | `FIS_J_1ABRNCH` | `J_1ABRNCH` | `BKPF` | `String(4)` |  | Branch |  |  |  |
| `NmbrOfPages` | `J_1ANOPG` | `J_1ANOPG` | `BKPF` | `String(3)` |  | Number of Pages |  |  |  |
| `IsDiscountDocument` |  |  |  | `String(1)` |  | discount document |  |  |  |
| `Reference1InDocumentHeader` | `FINS_XREF1_HD` | `XREF1_HD` | `BKPF` | `String(20)` |  | Reference 1 |  |  |  |
| `Reference2InDocumentHeader` | `FINS_XREF2_HD` | `XREF2_HD` | `BKPF` | `String(20)` |  | Reference 2 |  |  |  |
| `InvoiceReceiptDate` | `FIS_REINDAT` | `REINDAT` | `BKPF` | `Date` |  | Invoice Receipt Date |  |  |  |
| `Ledger` | `FIS_RLDNR` | `RLDNR` | `BKPF` | `String(2)` |  | Ledger |  | _Ledger |  |
| `LedgerGroup` | `FAGL_LDGRP` | `LDGRP` | `BKPF` | `String(4)` |  | Ledger Group |  |  |  |
| `AlternativeReferenceDocument` | `FIS_XBLNR_ALT_ALPHA` | `XBLNR_ALT` | `BKPF` | `String(26)` |  | Alternative Reference Document |  |  |  |
| `TaxReportingDate` | `VATDATE` | `VATDATE` | `BKPF` | `Date` |  | Tax Reporting Date |  |  |  |
| `TaxFulfillmentDate` | `FOT_FULFILLDATE` | `FULFILLDATE` | `BKPF` | `Date` |  | Tax Fulfill. Date |  |  |  |
| `AccountingDocumentClass` | `FIS_ACCDOC_CLASS` | `ACCDOC_CLASS` | `BKPF` | `String(6)` |  | Acctg Document Class |  |  |  |
| `ExchangeRateType` | `KURST` | `KURST` | `BKPF` | `String(4)` |  | Exchange Rate Type |  |  |  |
| `MarketDataAbsoluteExchangeRate` | `MARKETDATAABSOLUTEEXCHANGERATE` | `ABSOLUTEEXCHANGERATE` | `BKPF` | `Decimal(28,14)` |  | Absolute Market Data Exch. Rate |  |  |  |
| `MktDataEffectiveExchangeRate` | `MKTDATAEFFECTIVEEXCHANGERATE` | `EFFECTIVEEXCHANGERATE` | `BKPF` | `Decimal(31,14)` |  | Effective Market Data Exch. Rate |  |  |  |
| `SenderLogicalSystem` | `FIS_LOGSYSTEM_SENDER` | `LOGSYSTEM_SENDER` | `BKPF` | `String(10)` |  | Sender Logical System |  |  |  |
| `SenderCompanyCode` | `BUKRS_SENDER` | `BUKRS_SENDER` | `BKPF` | `String(4)` |  | Sender CoCode |  |  |  |
| `SenderAccountingDocument` | `FIS_BELNR_SENDER` | `BELNR_SENDER` | `BKPF` | `String(10)` |  | Sender Journal Entry |  |  |  |
| `SenderFiscalYear` | `FIS_GJAHR_SENDER_NO_CONV` | `GJAHR_SENDER` | `BKPF` | `String(4)` |  | Fiscal Year in Sender System |  |  |  |
| `ReversalReferenceDocumentCntxt` | `AWORG_REV` | `AWORG_REV` | `BKPF` | `String(10)` |  | Reversal Organizatns |  |  |  |
| `ReversalReferenceDocument` | `AWREF_REV` | `AWREF_REV` | `BKPF` | `String(10)` |  | Reversal Ref. No. |  |  |  |
| `LatePaymentReason` | `FIS_PENRC` | `PENRC` | `BKPF` | `String(2)` |  | Late Payment Reason |  |  |  |
| `SalesDocumentCondition` | `FIS_KNUMV` | `KNUMV` | `BKPF` | `String(10)` |  | Sales Document Condition |  |  |  |
| `IsReversal` | `FINS_XREVERSING` | `XREVERSING` | `BKPF` | `Boolean` |  | Is Reversing |  |  |  |
| `IsReversed` | `FINS_XREVERSED` | `XREVERSED` | `BKPF` | `Boolean` |  | Is Reversed |  |  |  |
| `GLBusinessTransactionGroup` | `FIS_GLBTGRP` | `GLBTGRP` | `BKPF` | `String(1)` |  | GL Business Transaction Group |  |  |  |
| `CostAccountingValuationDate` | `CO_VALDT` | `CO_VALDT` | `BKPF` | `Date` |  | Valuation Date |  |  |  |
| `TaxCountry` | `FIS_TAX_COUNTRY_HD` | `TAX_COUNTRY_HD` | `BKPF` | `String(3)` |  | Tax Country/Region |  |  |  |
| `JournalEntryLastChangeDateTime` | `FIS_JE_LASTCHANGE_DATETIME` | `JE_LASTCHANGE_DATETIME` | `BKPF` | `DateTime` |  | Journal Entry Last Change Date Time |  |  |  |
| `JournalEntryReprocessingStatus` | `FIS_JE_REPROCESSING_STATUS` | `JE_REPROCESSING_STATUS` | `BKPF` | `String(1)` |  | Journal Entry Reprocessing Status |  |  |  |
| `JrnlEntryCntrySpecificRef1` | `FAC_GLO_REF1_HD` | `GLO_REF1_HD` | `BKPF` | `String(80)` |  | Country/Region Specific Reference 1 |  |  |  |
| `JrnlEntryCntrySpecificDate1` | `FAC_GLO_DAT1_HD` | `GLO_DAT1_HD` | `BKPF` | `Date` |  | Country/Region Specific Date 1 |  |  |  |
| `JrnlEntryCntrySpecificRef2` | `FAC_GLO_REF2_HD` | `GLO_REF2_HD` | `BKPF` | `String(25)` |  | Country/Region Specific Reference 2 |  |  |  |
| `JrnlEntryCntrySpecificDate2` | `FAC_GLO_DAT2_HD` | `GLO_DAT2_HD` | `BKPF` | `Date` |  | Country/Region Specific Date 2 |  |  |  |
| `JrnlEntryCntrySpecificRef3` | `FAC_GLO_REF3_HD` | `GLO_REF3_HD` | `BKPF` | `String(25)` |  | Country/Region Specific Reference 3 |  |  |  |
| `JrnlEntryCntrySpecificDate3` | `FAC_GLO_DAT3_HD` | `GLO_DAT3_HD` | `BKPF` | `Date` |  | Country/Region Specific Date 3 |  |  |  |
| `JrnlEntryCntrySpecificRef4` | `FAC_GLO_REF4_HD` | `GLO_REF4_HD` | `BKPF` | `String(50)` |  | Country/Region Specific Reference 4 |  |  |  |
| `JrnlEntryCntrySpecificDate4` | `FAC_GLO_DAT4_HD` | `GLO_DAT4_HD` | `BKPF` | `Date` |  | Country/Region Specific Date 4 |  |  |  |
| `JrnlEntryCntrySpecificRef5` | `FAC_GLO_REF5_HD` | `GLO_REF5_HD` | `BKPF` | `String(50)` |  | Country/Region Specific Reference 5 |  |  |  |
| `JrnlEntryCntrySpecificDate5` | `FAC_GLO_DAT5_HD` | `GLO_DAT5_HD` | `BKPF` | `Date` |  | Country/Region Specific Date 5 |  |  |  |
| `JrnlEntryCntrySpecificBP1` | `FAC_GLO_BP1_HD` | `GLO_BP1_HD` | `BKPF` | `String(10)` |  | Ctry/Reg. Specific Business Partner 1 |  |  |  |
| `JrnlEntryCntrySpecificBP2` | `FAC_GLO_BP2_HD` | `GLO_BP2_HD` | `BKPF` | `String(10)` |  | Ctry/Reg. Specific Business Partner 2 |  |  |  |
| `WithholdingTaxReportingDate` | `WHTDATE` | `WHTDATE` | `BKPF` | `Date` |  | Wtax Reporting Date |  |  |  |


## Entity: `JournalEntryItemBillOfExchange`

- **ABAP Name:** `I_BillOfExchange`
- **Label:** Bill of Exchange
- **VDM Type:** `BASIC` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `CompanyCode` | `BUKRS` | `BUKRS` |  | `String(4)` | Y | Company Code |  |  | S/4 only entity — no ECC CDC mapping |
| `AccountingDocument` | `BELNR_D` | `BELNR` |  | `String(10)` | Y | Document Number |  |  | S/4 only entity — no ECC CDC mapping |
| `FiscalYear` | `FIS_GJAHR_NO_CONV` | `GJAHR` |  | `String(4)` | Y | Fiscal Year |  |  | S/4 only entity — no ECC CDC mapping |
| `AccountingDocumentItem` | `BUZEI` | `BUZEI` |  | `String(3)` | Y | Item |  |  | S/4 only entity — no ECC CDC mapping |
| `Cheque` | `CHECT` | `CHECT` |  | `String(13)` |  | Check number |  |  | S/4 only entity — no ECC CDC mapping |
| `BillOfExchangeIssueDate` | `WDATE` | `WDATE` |  | `Date` |  | Issue Date |  |  | S/4 only entity — no ECC CDC mapping |
| `BillOfExchangeUsageDate` | `WVERD` | `WVERD` |  | `Date` |  | Used On |  |  | S/4 only entity — no ECC CDC mapping |
| `BillOfExchangeUsage` | `FARP_WVERW` | `WVERW` |  | `String(1)` |  | Bill/Exchange Usage |  |  | S/4 only entity — no ECC CDC mapping |
| `PlannedBillOfExchangeUsage` | `WEVWV` | `WEVWV` |  | `String(1)` |  | Planned Usage |  |  | S/4 only entity — no ECC CDC mapping |
| `BillOfExchangeDrawer` | `WNAME` | `WNAME` |  | `String(30)` |  | Drawer |  |  | S/4 only entity — no ECC CDC mapping |
| `BillOfExchangeDrawerCityName` | `WORT1` | `WORT1` |  | `String(30)` |  | City of Drawer |  |  | S/4 only entity — no ECC CDC mapping |
| `BillOfExchangeDrawee` | `WBZOG` | `WBZOG` |  | `String(30)` |  | Drawee |  |  | S/4 only entity — no ECC CDC mapping |
| `BillOfExchangeDraweeCityName` | `WORT2` | `WORT2` |  | `String(30)` |  | City of Drawee |  |  | S/4 only entity — no ECC CDC mapping |
| `BillOfExchangeDomicileText` | `WBANK` | `WBANK` |  | `String(60)` |  | Domicile |  |  | S/4 only entity — no ECC CDC mapping |
| `BillOfExchangeIsAccepted` | `XAKTZ` | `XAKTZ` |  | `Boolean` |  | Accepted |  |  | S/4 only entity — no ECC CDC mapping |
| `Region` | `REGIO` | `REGIO` |  | `String(3)` |  | Region |  |  | S/4 only entity — no ECC CDC mapping |
| `BillOfExchangeDocumentStatus` | `WSTAT` | `WSTAT` |  | `String(1)` |  | Bill/Ex. Status |  |  | S/4 only entity — no ECC CDC mapping |
| `BillOfExchangeIsProtested` |  |  |  | `String(1)` |  | Bill Protest ID |  |  | S/4 only entity — no ECC CDC mapping |
| `BillOfExchangeIsOnDemand` | `XSIWE` | `XSIWE` |  | `Boolean` |  | Bill on Demand |  |  | S/4 only entity — no ECC CDC mapping |
| `BusinessPlace` | `BUPLA` | `BUPLA` |  | `String(4)` |  | Business Place |  |  | S/4 only entity — no ECC CDC mapping |
| `BusinessSectionCode` | `SECCO` | `SECCO` |  | `String(4)` |  | Section Code |  |  | S/4 only entity — no ECC CDC mapping |
| `BillOfExchangePortfolio` | `PORTFO` | `PORTFO` |  | `String(10)` |  | Bill Portfolio |  |  | S/4 only entity — no ECC CDC mapping |
| `BillOfExchangeCntrlBankLocText` | `WLZBP` | `WLZBP` |  | `String(60)` |  | Cen.Bank Loc. |  |  | S/4 only entity — no ECC CDC mapping |
| `BOEDraweeBankKey` | `BANKK` | `BANKK` |  | `String(15)` |  | Bank Key |  |  | S/4 only entity — no ECC CDC mapping |
| `BillOfExchangeDataAgingDate` | `DATA_TEMPERATURE` | `DATA_TEMPERATURE` |  | `Date` |  | Data Aging |  |  | S/4 only entity — no ECC CDC mapping |
| `IsBusinessPurposeCompleted` |  |  |  | `Boolean` |  | Purpose Completed |  |  | S/4 only entity — no ECC CDC mapping |
| `AuthorizationGroup` | `BRGRU` | `BRGRU` |  | `String(4)` |  | Authorization |  |  | S/4 only entity — no ECC CDC mapping |
