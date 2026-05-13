# JournalEntryHeader

> Source file: `sap-s4com-JournalEntryHeader-v1.json`

**Technical Name:** `IFIJOURNALENT` | **Data Category:** `DIMENSION` | **VDM Type:** `BASIC` | **Size:** `XXL`


## Entity: `JournalEntry`

- **ABAP Name:** `I_JournalEntry`
- **Technical Name:** `IFIJOURNALENT`
- **Label:** Journal Entry
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** BKPF

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `CompanyCode` | `BKPF` | `BUKRS` | `String(4)` | Y | Company Code |  | _CompanyCode |  |
| `FiscalYear` | `BKPF` | `GJAHR` | `String(4)` | Y | Fiscal Year |  | _FiscalYear |  |
| `AccountingDocument` | `BKPF` | `BELNR` | `String(10)` | Y | Journal Entry |  |  |  |
| `AccountingDocumentType` | `BKPF` | `BLART` | `String(2)` |  | Journal Entry Type |  | _AccountingDocumentType |  |
| `DocumentDate` | `BKPF` | `BLDAT` | `Date` |  | Journal Entry Date |  |  |  |
| `PostingDate` | `BKPF` | `BUDAT` | `Date` |  | Posting Date |  |  |  |
| `FiscalPeriod` | `BKPF` | `MONAT` | `String(3)` |  | Fiscal Period |  | _FiscalPeriod | ECC BKPF.MONAT unpadded ('3'); S/4 zero-padded ('003') |
| `AccountingDocumentCreationDate` | `BKPF` | `CPUDT` | `Date` |  | Entered On |  |  |  |
| `CreationTime` | `BKPF` | `CPUTM` | `String(6)` |  | Creation Time |  |  |  |
| `LastManualChangeDate` |  |  | `Date` |  | Manual Change Date |  |  |  |
| `LastAutomaticChangeDate` |  |  | `Date` |  | Autom. Change Date |  |  |  |
| `LastChangeDate` | `BKPF` | `AEDAT` | `Date` |  | Last Change Date |  |  |  |
| `ExchangeRateDate` | `BKPF` | `WWERT` | `Date` |  | Exchange Rate Date |  |  |  |
| `AccountingDocCreatedByUser` | `BKPF` | `USNAM` | `String(12)` |  | Journal Entry Created By |  |  |  |
| `TransactionCode` | `BKPF` | `TCODE` | `String(20)` |  | Transaction Code |  |  |  |
| `IntercompanyTransaction` | `BKPF` | `BVORG` | `String(16)` |  | Intercompany Transac |  |  |  |
| `DocumentReferenceID` | `BKPF` | `XBLNR` | `String(16)` |  | Document Reference ID |  |  |  |
| `RecurringAccountingDocument` | `BKPF` | `DBBLG` | `String(10)` |  | Recurring Journal Entry |  |  |  |
| `RecrrgJournalEntryCompanyCode` |  |  | `String(4)` |  | Recurring Journal Entry Company Code |  |  |  |
| `RecrrgJournalEntryFiscalYear` |  |  | `String(4)` |  | Recurring Journal Entry Fiscal Year |  |  |  |
| `ReverseDocument` | `BKPF` | `STBLG` | `String(10)` |  | Reverse Document |  |  |  |
| `ReverseDocumentFiscalYear` | `BKPF` | `STJAH` | `String(4)` |  | Reverse Document Fiscal Year |  |  |  |
| `AccountingDocumentHeaderText` | `BKPF` | `BKTXT` | `String(25)` |  | Document Header Text |  |  |  |
| `TransactionCurrency` | `BKPF` | `WAERS` | `String(5)` |  | Currency |  | _TransactionCurrency |  |
| `AbsoluteExchangeRate` | `BKPF` | `KURSF` | `Decimal(9,5)` |  | Absolute Exchange Rate |  |  |  |
| `ExchangeRate` | `BKPF` | `KURSF` | `Decimal(9,5)` |  | Exchange Rate |  |  |  |
| `ExchRateIsIndirectQuotation` |  |  | `Boolean` |  | Exchange Rate Is Indirect Quotation |  |  |  |
| `EffectiveExchangeRate` | `BKPF` | `KURSF` | `Decimal(12,5)` |  | Effective Exch. Rate |  |  |  |
| `AccountingDocumentCategory` | `BKPF` | `BLART` | `String(1)` |  | Journal Entry Category |  | _AccountingDocumentCategory |  |
| `NetAmountIsPosted` | `BKPF` | `XNEGP` | `Boolean` |  | Net Amount Is Posted |  |  |  |
| `JrnlEntryIsPostedToPrevPeriod` |  |  | `Boolean` |  | Journal Entry Is Posted To Prev. Period |  |  |  |
| `BusinessTransactionType` | `BKPF` | `GLVOR` | `String(4)` |  | Bus. Trans. Category |  | _BusinessTransactionType |  |
| `BatchInputSession` | `BKPF` | `BVORG` | `String(12)` |  | Batch Input Session |  |  |  |
| `ReferenceDocumentType` | `BKPF` | `AWTYP` | `String(5)` |  | Reference Document Type |  | _ReferenceDocumentType |  |
| `OriginalReferenceDocument` | `BKPF` | `AWKEY` | `String(20)` |  | Object Key |  |  |  |
| `FinancialManagementArea` | `BKPF` | `FIKRS` | `String(4)` |  | FM Area |  | _FinancialManagementArea |  |
| `CompanyCodeCurrency` | `T001` | `WAERS` | `String(5)` |  | Company Code Currency |  | _CompanyCodeCurrency |  |
| `AdditionalCurrency1` | `BKPF` | `HWAE2` | `String(5)` |  | Additional Crcy 1 |  |  |  |
| `AdditionalCurrency2` | `BKPF` | `HWAE3` | `String(5)` |  | Additional Crcy 2 |  |  |  |
| `ReversalIsPlanned` | `BKPF` | `XSTOV` | `Boolean` |  | Reversal Is Planned |  |  |  |
| `PlannedReversalDate` | `BKPF` | `STODT` | `Date` |  | Planned Reversal Dte |  |  |  |
| `TaxIsCalculatedAutomatically` | `BKPF` | `XMWST` | `Boolean` |  | Tax Is Automatically Calculated |  |  |  |
| `AdditionalCurrency1Role` |  |  | `String(2)` |  | LC2 Currency Type |  |  |  |
| `AdditionalCurrency2Role` |  |  | `String(2)` |  | LC3 Currency Type |  |  |  |
| `TaxBaseAmountIsNetAmount` | `BKPF` | `XNEGP` | `Boolean` |  | Tax Base Amount is Net Amount |  |  |  |
| `SourceCompanyCode` | `BKPF` | `AUSBK` | `String(4)` |  | Source Company Code |  |  |  |
| `LogicalSystem` | `BKPF` | `LOGSYS` | `String(10)` |  | Logical System |  | _LogicalSystem |  |
| `ReferenceDocumentLogicalSystem` |  |  | `String(10)` |  | Ref. Doc. Lgcl Syst. |  | _RefDocumentLogicalSystem |  |
| `TaxAbsoluteExchangeRate` | `BKPF` | `KURSF` | `Decimal(9,5)` |  | Absolute Tax Exchange Rate |  |  |  |
| `TaxExchangeRate` | `BKPF` | `KURSF` | `Decimal(9,5)` |  | Tax Exchange Rate |  |  |  |
| `TaxExchRateIsIndirectQuotation` |  |  | `Boolean` |  | Tax Exchange Rate Is Indirect Quotation |  |  |  |
| `TaxEffectiveExchangeRate` |  |  | `Decimal(12,5)` |  | Effective Tax Exchange Rate |  |  |  |
| `CtryCrcyTxAbsoluteExchangeRate` |  |  | `Decimal(9,5)` |  | Absolute Tax Exch. Rate in C/R Cur. |  |  |  |
| `CtryCrcyTaxEffctvExchangeRate` |  |  | `Decimal(12,5)` |  | Effective Tax Exch. Rate in C/R Cur. |  |  |  |
| `ReversalReason` | `BKPF` | `STGRD` | `String(2)` |  | Reversal Reason |  |  |  |
| `ParkedByUser` | `BKPF` | `USNAM` | `String(12)` |  | JE Parked By |  |  |  |
| `ParkingDate` | `BKPF` | `CPUDT` | `Date` |  | Parked On |  |  |  |
| `ParkingTime` |  |  | `String(6)` |  | Time of Parking |  |  |  |
| `ParkingTransactionCode` | `BKPF` | `TCODE` | `String(20)` |  | Parking Transaction Code |  |  |  |
| `Branch` | `BKPF` | `BRNCH` | `String(4)` |  | Branch |  |  |  |
| `NmbrOfPages` | `BKPF` | `NUMPG` | `String(3)` |  | Number of Pages |  |  |  |
| `IsDiscountDocument` | `BKPF` | `REINF` | `String(1)` |  | discount document |  |  |  |
| `Reference1InDocumentHeader` | `BKPF` | `XBLNR` | `String(20)` |  | Reference 1 |  |  |  |
| `Reference2InDocumentHeader` |  |  | `String(20)` |  | Reference 2 |  |  |  |
| `InvoiceReceiptDate` |  |  | `Date` |  | Invoice Receipt Date |  |  |  |
| `Ledger` |  |  | `String(2)` |  | Ledger |  | _Ledger | S/4 only — no ECC equivalent |
| `LedgerGroup` |  |  | `String(4)` |  | Ledger Group |  |  |  |
| `AlternativeReferenceDocument` |  |  | `String(26)` |  | Alternative Reference Document |  |  |  |
| `TaxReportingDate` |  |  | `Date` |  | Tax Reporting Date |  |  |  |
| `TaxFulfillmentDate` |  |  | `Date` |  | Tax Fulfill. Date |  |  |  |
| `AccountingDocumentClass` |  |  | `String(6)` |  | Acctg Document Class |  |  |  |
| `ExchangeRateType` |  |  | `String(4)` |  | Exchange Rate Type |  |  |  |
| `MarketDataAbsoluteExchangeRate` |  |  | `Decimal(28,14)` |  | Absolute Market Data Exch. Rate |  |  |  |
| `MktDataEffectiveExchangeRate` |  |  | `Decimal(31,14)` |  | Effective Market Data Exch. Rate |  |  |  |
| `SenderLogicalSystem` |  |  | `String(10)` |  | Sender Logical System |  |  |  |
| `SenderCompanyCode` |  |  | `String(4)` |  | Sender CoCode |  |  |  |
| `SenderAccountingDocument` |  |  | `String(10)` |  | Sender Journal Entry |  |  |  |
| `SenderFiscalYear` |  |  | `String(4)` |  | Fiscal Year in Sender System |  |  |  |
| `ReversalReferenceDocumentCntxt` |  |  | `String(10)` |  | Reversal Organizatns |  |  |  |
| `ReversalReferenceDocument` |  |  | `String(10)` |  | Reversal Ref. No. |  |  |  |
| `LatePaymentReason` |  |  | `String(2)` |  | Late Payment Reason |  |  |  |
| `SalesDocumentCondition` |  |  | `String(10)` |  | Sales Document Condition |  |  |  |
| `IsReversal` |  |  | `Boolean` |  | Is Reversing |  |  |  |
| `IsReversed` |  |  | `Boolean` |  | Is Reversed |  |  |  |
| `GLBusinessTransactionGroup` |  |  | `String(1)` |  | GL Business Transaction Group |  |  |  |
| `CostAccountingValuationDate` |  |  | `Date` |  | Valuation Date |  |  |  |
| `TaxCountry` |  |  | `String(3)` |  | Tax Country/Region |  |  |  |
| `JournalEntryLastChangeDateTime` |  |  | `DateTime` |  | Journal Entry Last Change Date Time |  |  |  |
| `JournalEntryReprocessingStatus` |  |  | `String(1)` |  | Journal Entry Reprocessing Status |  |  |  |
| `JrnlEntryCntrySpecificRef1` |  |  | `String(80)` |  | Country/Region Specific Reference 1 |  |  |  |
| `JrnlEntryCntrySpecificDate1` |  |  | `Date` |  | Country/Region Specific Date 1 |  |  |  |
| `JrnlEntryCntrySpecificRef2` |  |  | `String(25)` |  | Country/Region Specific Reference 2 |  |  |  |
| `JrnlEntryCntrySpecificDate2` |  |  | `Date` |  | Country/Region Specific Date 2 |  |  |  |
| `JrnlEntryCntrySpecificRef3` |  |  | `String(25)` |  | Country/Region Specific Reference 3 |  |  |  |
| `JrnlEntryCntrySpecificDate3` |  |  | `Date` |  | Country/Region Specific Date 3 |  |  |  |
| `JrnlEntryCntrySpecificRef4` |  |  | `String(50)` |  | Country/Region Specific Reference 4 |  |  |  |
| `JrnlEntryCntrySpecificDate4` |  |  | `Date` |  | Country/Region Specific Date 4 |  |  |  |
| `JrnlEntryCntrySpecificRef5` |  |  | `String(50)` |  | Country/Region Specific Reference 5 |  |  |  |
| `JrnlEntryCntrySpecificDate5` |  |  | `Date` |  | Country/Region Specific Date 5 |  |  |  |
| `JrnlEntryCntrySpecificBP1` |  |  | `String(10)` |  | Ctry/Reg. Specific Business Partner 1 |  |  |  |
| `JrnlEntryCntrySpecificBP2` |  |  | `String(10)` |  | Ctry/Reg. Specific Business Partner 2 |  |  |  |
| `WithholdingTaxReportingDate` |  |  | `Date` |  | Wtax Reporting Date |  |  |  |


## Entity: `JournalEntryItemBillOfExchange`

- **ABAP Name:** `I_BillOfExchange`
- **Label:** Bill of Exchange
- **VDM Type:** `BASIC` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `CompanyCode` | `T001` | `BUKRS` | `String(4)` | Y | Company Code |  |  |  |
| `AccountingDocument` |  |  | `String(10)` | Y | Document Number |  |  | S/4 only entity |
| `FiscalYear` |  |  | `String(4)` | Y | Fiscal Year |  |  | S/4 only entity |
| `AccountingDocumentItem` |  |  | `String(3)` | Y | Item |  |  | S/4 only entity |
| `Cheque` |  |  | `String(13)` |  | Check number |  |  | S/4 only entity |
| `BillOfExchangeIssueDate` |  |  | `Date` |  | Issue Date |  |  | S/4 only entity |
| `BillOfExchangeUsageDate` |  |  | `Date` |  | Used On |  |  | S/4 only entity |
| `BillOfExchangeUsage` |  |  | `String(1)` |  | Bill/Exchange Usage |  |  | S/4 only entity |
| `PlannedBillOfExchangeUsage` |  |  | `String(1)` |  | Planned Usage |  |  | S/4 only entity |
| `BillOfExchangeDrawer` |  |  | `String(30)` |  | Drawer |  |  | S/4 only entity |
| `BillOfExchangeDrawerCityName` |  |  | `String(30)` |  | City of Drawer |  |  | S/4 only entity |
| `BillOfExchangeDrawee` |  |  | `String(30)` |  | Drawee |  |  | S/4 only entity |
| `BillOfExchangeDraweeCityName` |  |  | `String(30)` |  | City of Drawee |  |  | S/4 only entity |
| `BillOfExchangeDomicileText` |  |  | `String(60)` |  | Domicile |  |  | S/4 only entity |
| `BillOfExchangeIsAccepted` |  |  | `Boolean` |  | Accepted |  |  | S/4 only entity |
| `Region` |  |  | `String(3)` |  | Region |  |  | S/4 only entity |
| `BillOfExchangeDocumentStatus` |  |  | `String(1)` |  | Bill/Ex. Status |  |  | S/4 only entity |
| `BillOfExchangeIsProtested` |  |  | `String(1)` |  | Bill Protest ID |  |  | S/4 only entity |
| `BillOfExchangeIsOnDemand` |  |  | `Boolean` |  | Bill on Demand |  |  | S/4 only entity |
| `BusinessPlace` |  |  | `String(4)` |  | Business Place |  |  | S/4 only entity |
| `BusinessSectionCode` |  |  | `String(4)` |  | Section Code |  |  | S/4 only entity |
| `BillOfExchangePortfolio` |  |  | `String(10)` |  | Bill Portfolio |  |  | S/4 only entity |
| `BillOfExchangeCntrlBankLocText` |  |  | `String(60)` |  | Cen.Bank Loc. |  |  | S/4 only entity |
| `BOEDraweeBankKey` |  |  | `String(15)` |  | Bank Key |  |  | S/4 only entity |
| `BillOfExchangeDataAgingDate` |  |  | `Date` |  | Data Aging |  |  | S/4 only entity |
| `IsBusinessPurposeCompleted` |  |  | `Boolean` |  | Purpose Completed |  |  | S/4 only entity |
| `AuthorizationGroup` |  |  | `String(4)` |  | Authorization |  |  | S/4 only entity |
