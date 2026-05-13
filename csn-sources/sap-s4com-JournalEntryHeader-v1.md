# JournalEntryHeader

> Source file: `sap-s4com-JournalEntryHeader-v1.json`

**Technical Name:** `IFIJOURNALENT` | **Data Category:** `DIMENSION` | **VDM Type:** `BASIC` | **Size:** `XXL`


## Entity: `JournalEntry`

- **ABAP CDS Name:** `I_JournalEntry`
- **Technical Name:** `IFIJOURNALENT`
- **Label:** Journal Entry
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** BKPF

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `CompanyCode` | `FIS_BUKRS` | `BKPF` | `BUKRS` | `ACDOCA` | `RBUKRS` | `String(4)` | Y | Company Code |  |  |
| `FiscalYear` | `FIS_GJAHR_NO_CONV` | `BKPF` | `GJAHR` | `ACDOCA` | `GJAHR` | `String(4)` | Y | Fiscal Year |  |  |
| `AccountingDocument` | `FARP_BELNR_D` | `BKPF` | `BELNR` | `ACDOCA` | `BELNR` | `String(10)` | Y | Journal Entry |  |  |
| `AccountingDocumentType` | `FARP_BLART` | `BKPF` | `BLART` | `ACDOCA` | `BLART` | `String(2)` |  | Journal Entry Type |  |  |
| `DocumentDate` | `FIS_BLDAT` | `BKPF` | `BLDAT` | `ACDOCA` | `BLDAT` | `Date` |  | Journal Entry Date |  |  |
| `PostingDate` | `FIS_BUDAT` | `BKPF` | `BUDAT` | `ACDOCA` | `BUDAT` | `Date` |  | Posting Date |  |  |
| `FiscalPeriod` | `FINS_FISCALPERIOD` | `BKPF` | `MONAT` | `ACDOCA` | `POPER` | `String(3)` |  | Fiscal Period |  | ECC MONAT unpadded '3'; S/4 ACDOCA.POPER zero-padded '003' |
| `AccountingDocumentCreationDate` | `FARP_CPUDT` | `BKPF` | `CPUDT` | `ACDOCA` | `TIMESTAMP` | `Date` |  | Entered On |  |  |
| `CreationTime` | `TTET_DT_CR_TIME` |  |  |  |  | `String(6)` |  | Creation Time |  |  |
| `LastManualChangeDate` | `FIS_LASTMANUALCHANGEDATE` |  |  |  |  | `Date` |  | Manual Change Date |  |  |
| `LastAutomaticChangeDate` | `FIS_LASTAUTOMATICCHANGEDATE` |  |  |  |  | `Date` |  | Autom. Change Date |  |  |
| `LastChangeDate` | `TTET_DT_CHG_DATE` |  |  |  |  | `Date` |  | Last Change Date |  |  |
| `ExchangeRateDate` | `VDM_V_EXCHANGE_RATE_DATE` | `BKPF` | `WWERT` | `ACDOCA` | `WWERT` | `Date` |  | Exchange Rate Date |  |  |
| `AccountingDocCreatedByUser` | `FIS_USNAM` | `BKPF` | `USNAM` | `ACDOCA` | `USNAM` | `String(12)` |  | Journal Entry Created By |  |  |
| `TransactionCode` | `TCODE` | `BKPF` | `TCODE` | `ACDOCA` |  | `String(20)` |  | Transaction Code |  |  |
| `IntercompanyTransaction` | `FAC_BVORG` | `BKPF` | `BVORG` | `ACDOCA` |  | `String(16)` |  | Intercompany Transac |  |  |
| `DocumentReferenceID` | `FIS_XBLNR1` | `BKPF` | `XBLNR` | `ACDOCA` | `AWREF` | `String(16)` |  | Document Reference ID |  |  |
| `RecurringAccountingDocument` | `FIS_RJET_ID` | `BKPF` | `DBBLG` | `ACDOCA` |  | `String(10)` |  | Recurring Journal Entry |  |  |
| `RecrrgJournalEntryCompanyCode` | `FIS_DBBLG_BUKRS` |  |  |  |  | `String(4)` |  | Recurring Journal Entry Company Code |  |  |
| `RecrrgJournalEntryFiscalYear` | `FIS_DBBLG_GJAHR` |  |  |  |  | `String(4)` |  | Recurring Journal Entry Fiscal Year |  |  |
| `ReverseDocument` | `FIS_STBLG` | `BKPF` | `STBLG` | `ACDOCA` | `AWREF_REV` | `String(10)` |  | Reverse Document |  |  |
| `ReverseDocumentFiscalYear` | `FIS_STJAH_NO_CONV` | `BKPF` | `STJAH` | `ACDOCA` |  | `String(4)` |  | Reverse Document Fiscal Year |  |  |
| `AccountingDocumentHeaderText` | `BKTXT` | `BKPF` | `BKTXT` | `ACDOCA` |  | `String(25)` |  | Document Header Text |  |  |
| `TransactionCurrency` | `WAERS` | `BKPF` | `WAERS` | `ACDOCA` | `RWCUR` | `String(5)` |  | Currency |  |  |
| `AbsoluteExchangeRate` | `FIS_ABSOLUTE_EXCHANGERATE` | `BKPF` | `KURSF` | `ACDOCA` |  | `Decimal(9,5)` |  | Absolute Exchange Rate |  |  |
| `ExchangeRate` | `UKURS_CURR` | `BKPF` | `KURSF` | `ACDOCA` |  | `Decimal(9,5)` |  | Exchange Rate |  |  |
| `ExchRateIsIndirectQuotation` |  |  |  |  |  | `Boolean` |  | Exchange Rate Is Indirect Quotation |  |  |
| `EffectiveExchangeRate` | `FIS_EFFECTIVE_EXCHANGERATE` |  |  |  |  | `Decimal(12,5)` |  | Effective Exch. Rate |  |  |
| `AccountingDocumentCategory` | `FIS_BSTAT` | `BKPF` | `BSTAT` | `ACDOCA` | `BSTAT` | `String(1)` |  | Journal Entry Category |  |  |
| `NetAmountIsPosted` | `FIS_XNETB` |  |  |  |  | `Boolean` |  | Net Amount Is Posted |  |  |
| `JrnlEntryIsPostedToPrevPeriod` | `FIS_XRUEB` |  |  |  |  | `Boolean` |  | Journal Entry Is Posted To Prev. Period |  |  |
| `BusinessTransactionType` | `FINS_BTTYPE` | `BKPF` | `GLVOR` | `ACDOCA` | `BTTYPE` | `String(4)` |  | Bus. Trans. Category |  |  |
| `BatchInputSession` | `FIS_GRPID` | `BKPF` | `GRPID` | `ACDOCA` |  | `String(12)` |  | Batch Input Session |  |  |
| `ReferenceDocumentType` | `FIS_AWTYP` | `BKPF` | `AWTYP` | `ACDOCA` | `AWTYP` | `String(5)` |  | Reference Document Type |  |  |
| `OriginalReferenceDocument` | `FAC_AWKEY` | `BKPF` | `AWKEY` | `ACDOCA` | `AWORG` | `String(20)` |  | Object Key |  |  |
| `FinancialManagementArea` | `FIKRS` | `BKPF` | `FIKRS` | `ACDOCA` |  | `String(4)` |  | FM Area |  |  |
| `CompanyCodeCurrency` | `FIS_HWAER` | `T001` | `WAERS` | `ACDOCA` | `RHCUR` | `String(5)` |  | Company Code Currency |  |  |
| `AdditionalCurrency1` | `FIS_HWAE2` | `BKPF` | `HWAE2` | `ACDOCA` | `ROCUR` | `String(5)` |  | Additional Crcy 1 |  |  |
| `AdditionalCurrency2` | `FIS_HWAE3` | `BKPF` | `HWAE3` | `ACDOCA` | `RVCUR` | `String(5)` |  | Additional Crcy 2 |  |  |
| `ReversalIsPlanned` | `FIS_XSTOV` | `BKPF` | `XSTOV` | `ACDOCA` |  | `Boolean` |  | Reversal Is Planned |  |  |
| `PlannedReversalDate` | `FIS_STODT` | `BKPF` | `STODT` | `ACDOCA` |  | `Date` |  | Planned Reversal Dte |  |  |
| `TaxIsCalculatedAutomatically` | `FIS_XMWST` |  |  |  |  | `Boolean` |  | Tax Is Automatically Calculated |  |  |
| `AdditionalCurrency1Role` | `CURT2` |  |  |  |  | `String(2)` |  | LC2 Currency Type |  |  |
| `AdditionalCurrency2Role` | `CURT3` |  |  |  |  | `String(2)` |  | LC3 Currency Type |  |  |
| `TaxBaseAmountIsNetAmount` | `FIS_XMWSN` |  |  |  |  | `Boolean` |  | Tax Base Amount is Net Amount |  |  |
| `SourceCompanyCode` | `AUSBK` | `BKPF` | `AUSBK` | `ACDOCA` | `PREC_BUKRS` | `String(4)` |  | Source Company Code |  |  |
| `LogicalSystem` | `LOGSYSTEM` | `BKPF` | `LOGSYS` | `ACDOCA` | `AWSYS` | `String(10)` |  | Logical System |  |  |
| `ReferenceDocumentLogicalSystem` | `FIS_AWSYS` |  |  |  |  | `String(10)` |  | Ref. Doc. Lgcl Syst. |  |  |
| `TaxAbsoluteExchangeRate` | `FIS_ABSOLUTE_TXKRS_BKPF` |  |  |  |  | `Decimal(9,5)` |  | Absolute Tax Exchange Rate |  |  |
| `TaxExchangeRate` | `FIS_TXKRS_BKPF` |  |  |  |  | `Decimal(9,5)` |  | Tax Exchange Rate |  |  |
| `TaxExchRateIsIndirectQuotation` |  |  |  |  |  | `Boolean` |  | Tax Exchange Rate Is Indirect Quotation |  |  |
| `TaxEffectiveExchangeRate` | `FIS_TAX_EFFECTIVE_EXCHANGERATE` |  |  |  |  | `Decimal(12,5)` |  | Effective Tax Exchange Rate |  |  |
| `CtryCrcyTxAbsoluteExchangeRate` | `CTRYCRCYTXABSOLUTEEXCHANGERATE` |  |  |  |  | `Decimal(9,5)` |  | Absolute Tax Exch. Rate in C/R Cur. |  |  |
| `CtryCrcyTaxEffctvExchangeRate` | `CTRYCRCYTAXEFFCTVEXCHANGERATE` |  |  |  |  | `Decimal(12,5)` |  | Effective Tax Exch. Rate in C/R Cur. |  |  |
| `ReversalReason` | `STGRD` | `BKPF` | `STGRD` | `ACDOCA` |  | `String(2)` |  | Reversal Reason |  |  |
| `ParkedByUser` | `FIS_PPNAM` |  |  |  |  | `String(12)` |  | JE Parked By |  |  |
| `ParkingDate` | `PPDATE` |  |  |  |  | `Date` |  | Parked On |  |  |
| `ParkingTime` | `PPTME` |  |  |  |  | `String(6)` |  | Time of Parking |  |  |
| `ParkingTransactionCode` | `FIS_PPTCOD` |  |  |  |  | `String(20)` |  | Parking Transaction Code |  |  |
| `Branch` | `FIS_J_1ABRNCH` | `BKPF` | `BRNCH` | `ACDOCA` |  | `String(4)` |  | Branch |  |  |
| `NmbrOfPages` | `J_1ANOPG` |  |  |  |  | `String(3)` |  | Number of Pages |  |  |
| `IsDiscountDocument` |  |  |  |  |  | `String(1)` |  | discount document |  |  |
| `Reference1InDocumentHeader` | `FINS_XREF1_HD` |  |  |  |  | `String(20)` |  | Reference 1 |  |  |
| `Reference2InDocumentHeader` | `FINS_XREF2_HD` |  |  |  |  | `String(20)` |  | Reference 2 |  |  |
| `InvoiceReceiptDate` | `FIS_REINDAT` |  |  |  |  | `Date` |  | Invoice Receipt Date |  |  |
| `Ledger` | `FIS_RLDNR` |  |  | `ACDOCA` | `RLDNR` | `String(2)` |  | Ledger |  |  |
| `LedgerGroup` | `FAGL_LDGRP` |  |  |  |  | `String(4)` |  | Ledger Group |  |  |
| `AlternativeReferenceDocument` | `FIS_XBLNR_ALT_ALPHA` |  |  |  |  | `String(26)` |  | Alternative Reference Document |  |  |
| `TaxReportingDate` | `VATDATE` | `BKPF` | `VATDATE` | `ACDOCA` |  | `Date` |  | Tax Reporting Date |  |  |
| `TaxFulfillmentDate` | `FOT_FULFILLDATE` |  |  |  |  | `Date` |  | Tax Fulfill. Date |  |  |
| `AccountingDocumentClass` | `FIS_ACCDOC_CLASS` |  |  |  |  | `String(6)` |  | Acctg Document Class |  |  |
| `ExchangeRateType` | `KURST` |  |  |  |  | `String(4)` |  | Exchange Rate Type |  |  |
| `MarketDataAbsoluteExchangeRate` | `MARKETDATAABSOLUTEEXCHANGERATE` |  |  |  |  | `Decimal(28,14)` |  | Absolute Market Data Exch. Rate |  |  |
| `MktDataEffectiveExchangeRate` | `MKTDATAEFFECTIVEEXCHANGERATE` |  |  |  |  | `Decimal(31,14)` |  | Effective Market Data Exch. Rate |  |  |
| `SenderLogicalSystem` | `FIS_LOGSYSTEM_SENDER` |  |  |  |  | `String(10)` |  | Sender Logical System |  |  |
| `SenderCompanyCode` | `BUKRS_SENDER` | `BKPF` | `AUSBK` | `ACDOCA` | `PREC_BUKRS` | `String(4)` |  | Sender CoCode |  |  |
| `SenderAccountingDocument` | `FIS_BELNR_SENDER` |  |  |  |  | `String(10)` |  | Sender Journal Entry |  |  |
| `SenderFiscalYear` | `FIS_GJAHR_SENDER_NO_CONV` |  |  |  |  | `String(4)` |  | Fiscal Year in Sender System |  |  |
| `ReversalReferenceDocumentCntxt` | `AWORG_REV` | `BKPF` | `AWORG` | `ACDOCA` | `AWORG_REV` | `String(10)` |  | Reversal Organizatns |  |  |
| `ReversalReferenceDocument` | `AWREF_REV` | `BKPF` | `STBLG` | `ACDOCA` | `AWREF_REV` | `String(10)` |  | Reversal Ref. No. |  |  |
| `LatePaymentReason` | `FIS_PENRC` |  |  |  |  | `String(2)` |  | Late Payment Reason |  |  |
| `SalesDocumentCondition` | `FIS_KNUMV` |  |  |  |  | `String(10)` |  | Sales Document Condition |  |  |
| `IsReversal` | `FINS_XREVERSING` | `BKPF` | `XREVERSAL` | `ACDOCA` | `XREVERSING` | `Boolean` |  | Is Reversing |  |  |
| `IsReversed` | `FINS_XREVERSED` |  |  | `ACDOCA` | `XREVERSED` | `Boolean` |  | Is Reversed |  |  |
| `GLBusinessTransactionGroup` | `FIS_GLBTGRP` |  |  |  |  | `String(1)` |  | GL Business Transaction Group |  |  |
| `CostAccountingValuationDate` | `CO_VALDT` |  |  |  |  | `Date` |  | Valuation Date |  |  |
| `TaxCountry` | `FIS_TAX_COUNTRY_HD` |  |  |  |  | `String(3)` |  | Tax Country/Region |  |  |
| `JournalEntryLastChangeDateTime` | `FIS_JE_LASTCHANGE_DATETIME` |  |  |  |  | `DateTime` |  | Journal Entry Last Change Date Time |  |  |
| `JournalEntryReprocessingStatus` | `FIS_JE_REPROCESSING_STATUS` |  |  |  |  | `String(1)` |  | Journal Entry Reprocessing Status |  |  |
| `JrnlEntryCntrySpecificRef1` | `FAC_GLO_REF1_HD` |  |  |  |  | `String(80)` |  | Country/Region Specific Reference 1 |  |  |
| `JrnlEntryCntrySpecificDate1` | `FAC_GLO_DAT1_HD` |  |  |  |  | `Date` |  | Country/Region Specific Date 1 |  |  |
| `JrnlEntryCntrySpecificRef2` | `FAC_GLO_REF2_HD` |  |  |  |  | `String(25)` |  | Country/Region Specific Reference 2 |  |  |
| `JrnlEntryCntrySpecificDate2` | `FAC_GLO_DAT2_HD` |  |  |  |  | `Date` |  | Country/Region Specific Date 2 |  |  |
| `JrnlEntryCntrySpecificRef3` | `FAC_GLO_REF3_HD` |  |  |  |  | `String(25)` |  | Country/Region Specific Reference 3 |  |  |
| `JrnlEntryCntrySpecificDate3` | `FAC_GLO_DAT3_HD` |  |  |  |  | `Date` |  | Country/Region Specific Date 3 |  |  |
| `JrnlEntryCntrySpecificRef4` | `FAC_GLO_REF4_HD` |  |  |  |  | `String(50)` |  | Country/Region Specific Reference 4 |  |  |
| `JrnlEntryCntrySpecificDate4` | `FAC_GLO_DAT4_HD` |  |  |  |  | `Date` |  | Country/Region Specific Date 4 |  |  |
| `JrnlEntryCntrySpecificRef5` | `FAC_GLO_REF5_HD` |  |  |  |  | `String(50)` |  | Country/Region Specific Reference 5 |  |  |
| `JrnlEntryCntrySpecificDate5` | `FAC_GLO_DAT5_HD` |  |  |  |  | `Date` |  | Country/Region Specific Date 5 |  |  |
| `JrnlEntryCntrySpecificBP1` | `FAC_GLO_BP1_HD` |  |  |  |  | `String(10)` |  | Ctry/Reg. Specific Business Partner 1 |  |  |
| `JrnlEntryCntrySpecificBP2` | `FAC_GLO_BP2_HD` |  |  |  |  | `String(10)` |  | Ctry/Reg. Specific Business Partner 2 |  |  |
| `WithholdingTaxReportingDate` | `WHTDATE` |  |  |  |  | `Date` |  | Wtax Reporting Date |  |  |


## Entity: `JournalEntryItemBillOfExchange`

- **ABAP CDS Name:** `I_BillOfExchange`
- **Label:** Bill of Exchange
- **VDM Type:** `BASIC` | **Data Category:** ``
- **ECC Source Tables:** BKPF, BSEG

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `CompanyCode` | `BUKRS` |  |  |  |  | `String(4)` | Y | Company Code |  |  |
| `AccountingDocument` | `BELNR_D` |  |  |  |  | `String(10)` | Y | Document Number |  |  |
| `FiscalYear` | `FIS_GJAHR_NO_CONV` |  |  |  |  | `String(4)` | Y | Fiscal Year |  |  |
| `AccountingDocumentItem` | `BUZEI` |  |  |  |  | `String(3)` | Y | Item |  |  |
| `Cheque` | `CHECT` |  |  |  |  | `String(13)` |  | Check number |  |  |
| `BillOfExchangeIssueDate` | `WDATE` |  |  |  |  | `Date` |  | Issue Date |  |  |
| `BillOfExchangeUsageDate` | `WVERD` |  |  |  |  | `Date` |  | Used On |  |  |
| `BillOfExchangeUsage` | `FARP_WVERW` |  |  |  |  | `String(1)` |  | Bill/Exchange Usage |  |  |
| `PlannedBillOfExchangeUsage` | `WEVWV` |  |  |  |  | `String(1)` |  | Planned Usage |  |  |
| `BillOfExchangeDrawer` | `WNAME` |  |  |  |  | `String(30)` |  | Drawer |  |  |
| `BillOfExchangeDrawerCityName` | `WORT1` |  |  |  |  | `String(30)` |  | City of Drawer |  |  |
| `BillOfExchangeDrawee` | `WBZOG` |  |  |  |  | `String(30)` |  | Drawee |  |  |
| `BillOfExchangeDraweeCityName` | `WORT2` |  |  |  |  | `String(30)` |  | City of Drawee |  |  |
| `BillOfExchangeDomicileText` | `WBANK` |  |  |  |  | `String(60)` |  | Domicile |  |  |
| `BillOfExchangeIsAccepted` | `XAKTZ` |  |  |  |  | `Boolean` |  | Accepted |  |  |
| `Region` | `REGIO` |  |  |  |  | `String(3)` |  | Region |  |  |
| `BillOfExchangeDocumentStatus` | `WSTAT` |  |  |  |  | `String(1)` |  | Bill/Ex. Status |  |  |
| `BillOfExchangeIsProtested` |  |  |  |  |  | `String(1)` |  | Bill Protest ID |  |  |
| `BillOfExchangeIsOnDemand` | `XSIWE` |  |  |  |  | `Boolean` |  | Bill on Demand |  |  |
| `BusinessPlace` | `BUPLA` |  |  |  |  | `String(4)` |  | Business Place |  |  |
| `BusinessSectionCode` | `SECCO` |  |  |  |  | `String(4)` |  | Section Code |  |  |
| `BillOfExchangePortfolio` | `PORTFO` |  |  |  |  | `String(10)` |  | Bill Portfolio |  |  |
| `BillOfExchangeCntrlBankLocText` | `WLZBP` |  |  |  |  | `String(60)` |  | Cen.Bank Loc. |  |  |
| `BOEDraweeBankKey` | `BANKK` |  |  |  |  | `String(15)` |  | Bank Key |  |  |
| `BillOfExchangeDataAgingDate` | `DATA_TEMPERATURE` |  |  |  |  | `Date` |  | Data Aging |  |  |
| `IsBusinessPurposeCompleted` |  |  |  |  |  | `Boolean` |  | Purpose Completed |  |  |
| `AuthorizationGroup` | `BRGRU` |  |  |  |  | `String(4)` |  | Authorization |  |  |
