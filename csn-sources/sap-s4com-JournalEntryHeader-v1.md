# JournalEntryHeader

> Source file: `sap-s4com-JournalEntryHeader-v1.json`

**Technical Name:** `IFIJOURNALENT` | **Data Category:** `DIMENSION` | **VDM Type:** `BASIC` | **Size:** `XXL`


## Entity: `JournalEntry`

- **ABAP Name:** `I_JournalEntry`
- **Technical Name:** `IFIJOURNALENT`
- **Label:** Journal Entry
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** BKPF

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `CompanyCode` | `CompanyCode` | `String(4)` | Y | Company Code |  | _CompanyCode |  |
| `FiscalYear` | `FiscalYear` | `String(4)` | Y | Fiscal Year |  | _FiscalYear |  |
| `AccountingDocument` | `AccountingDocument` | `String(10)` | Y | Journal Entry |  |  |  |
| `AccountingDocumentType` | `AccountingDocumentType` | `String(2)` |  | Journal Entry Type |  | _AccountingDocumentType |  |
| `DocumentDate` | `DocumentDate` | `Date` |  | Journal Entry Date |  |  |  |
| `PostingDate` | `PostingDate` | `Date` |  | Posting Date |  |  |  |
| `FiscalPeriod` | `FiscalPeriod` | `String(3)` |  | Fiscal Period |  | _FiscalPeriod | ECC: BKPF.MONAT (unpadded '3'); S/4: zero-padded '003' |
| `AccountingDocumentCreationDate` | `AccountingDocumentCreationDate` | `Date` |  | Entered On |  |  |  |
| `CreationTime` | `CreationTime` | `String(6)` |  | Creation Time |  |  |  |
| `LastManualChangeDate` | `LastManualChangeDate` | `Date` |  | Manual Change Date |  |  |  |
| `LastAutomaticChangeDate` | `LastAutomaticChangeDate` | `Date` |  | Autom. Change Date |  |  |  |
| `LastChangeDate` | `LastChangeDate` | `Date` |  | Last Change Date |  |  |  |
| `ExchangeRateDate` | `ExchangeRateDate` | `Date` |  | Exchange Rate Date |  |  |  |
| `AccountingDocCreatedByUser` | `AccountingDocCreatedByUser` | `String(12)` |  | Journal Entry Created By |  |  |  |
| `TransactionCode` | `TransactionCode` | `String(20)` |  | Transaction Code |  |  |  |
| `IntercompanyTransaction` | `IntercompanyTransaction` | `String(16)` |  | Intercompany Transac |  |  |  |
| `DocumentReferenceID` | `DocumentReferenceID` | `String(16)` |  | Document Reference ID |  |  |  |
| `RecurringAccountingDocument` | `RecurringAccountingDocument` | `String(10)` |  | Recurring Journal Entry |  |  |  |
| `RecrrgJournalEntryCompanyCode` | `RecrrgJournalEntryCompanyCode` | `String(4)` |  | Recurring Journal Entry Company Code |  |  |  |
| `RecrrgJournalEntryFiscalYear` | `RecrrgJournalEntryFiscalYear` | `String(4)` |  | Recurring Journal Entry Fiscal Year |  |  |  |
| `ReverseDocument` | `ReverseDocument` | `String(10)` |  | Reverse Document |  |  |  |
| `ReverseDocumentFiscalYear` | `ReverseDocumentFiscalYear` | `String(4)` |  | Reverse Document Fiscal Year |  |  |  |
| `AccountingDocumentHeaderText` | `AccountingDocumentHeaderText` | `String(25)` |  | Document Header Text |  |  |  |
| `TransactionCurrency` | `TransactionCurrency` | `String(5)` |  | Currency |  | _TransactionCurrency |  |
| `AbsoluteExchangeRate` | `AbsoluteExchangeRate` | `Decimal(9,5)` |  | Absolute Exchange Rate |  |  |  |
| `ExchangeRate` | `ExchangeRate` | `Decimal(9,5)` |  | Exchange Rate |  |  |  |
| `ExchRateIsIndirectQuotation` | `ExchRateIsIndirectQuotation` | `Boolean` |  | Exchange Rate Is Indirect Quotation |  |  |  |
| `EffectiveExchangeRate` | `EffectiveExchangeRate` | `Decimal(12,5)` |  | Effective Exch. Rate |  |  |  |
| `AccountingDocumentCategory` | `AccountingDocumentCategory` | `String(1)` |  | Journal Entry Category |  | _AccountingDocumentCategory |  |
| `NetAmountIsPosted` | `NetAmountIsPosted` | `Boolean` |  | Net Amount Is Posted |  |  |  |
| `JrnlEntryIsPostedToPrevPeriod` | `JrnlEntryIsPostedToPrevPeriod` | `Boolean` |  | Journal Entry Is Posted To Prev. Period |  |  |  |
| `BusinessTransactionType` | `BusinessTransactionType` | `String(4)` |  | Bus. Trans. Category |  | _BusinessTransactionType |  |
| `BatchInputSession` | `BatchInputSession` | `String(12)` |  | Batch Input Session |  |  |  |
| `ReferenceDocumentType` | `ReferenceDocumentType` | `String(5)` |  | Reference Document Type |  | _ReferenceDocumentType |  |
| `OriginalReferenceDocument` | `OriginalReferenceDocument` | `String(20)` |  | Object Key |  |  |  |
| `FinancialManagementArea` | `FinancialManagementArea` | `String(4)` |  | FM Area |  | _FinancialManagementArea |  |
| `CompanyCodeCurrency` | `CompanyCodeCurrency` | `String(5)` |  | Company Code Currency |  | _CompanyCodeCurrency |  |
| `AdditionalCurrency1` | `AdditionalCurrency1` | `String(5)` |  | Additional Crcy 1 |  |  |  |
| `AdditionalCurrency2` | `AdditionalCurrency2` | `String(5)` |  | Additional Crcy 2 |  |  |  |
| `ReversalIsPlanned` | `ReversalIsPlanned` | `Boolean` |  | Reversal Is Planned |  |  |  |
| `PlannedReversalDate` | `PlannedReversalDate` | `Date` |  | Planned Reversal Dte |  |  |  |
| `TaxIsCalculatedAutomatically` | `TaxIsCalculatedAutomatically` | `Boolean` |  | Tax Is Automatically Calculated |  |  |  |
| `AdditionalCurrency1Role` | `AdditionalCurrency1Role` | `String(2)` |  | LC2 Currency Type |  |  |  |
| `AdditionalCurrency2Role` | `AdditionalCurrency2Role` | `String(2)` |  | LC3 Currency Type |  |  |  |
| `TaxBaseAmountIsNetAmount` | `TaxBaseAmountIsNetAmount` | `Boolean` |  | Tax Base Amount is Net Amount |  |  |  |
| `SourceCompanyCode` | `SourceCompanyCode` | `String(4)` |  | Source Company Code |  |  |  |
| `LogicalSystem` | `LogicalSystem` | `String(10)` |  | Logical System |  | _LogicalSystem |  |
| `ReferenceDocumentLogicalSystem` | `ReferenceDocumentLogicalSystem` | `String(10)` |  | Ref. Doc. Lgcl Syst. |  | _RefDocumentLogicalSystem |  |
| `TaxAbsoluteExchangeRate` | `TaxAbsoluteExchangeRate` | `Decimal(9,5)` |  | Absolute Tax Exchange Rate |  |  |  |
| `TaxExchangeRate` | `TaxExchangeRate` | `Decimal(9,5)` |  | Tax Exchange Rate |  |  |  |
| `TaxExchRateIsIndirectQuotation` | `TaxExchRateIsIndirectQuotation` | `Boolean` |  | Tax Exchange Rate Is Indirect Quotation |  |  |  |
| `TaxEffectiveExchangeRate` | `TaxEffectiveExchangeRate` | `Decimal(12,5)` |  | Effective Tax Exchange Rate |  |  |  |
| `CtryCrcyTxAbsoluteExchangeRate` | `CtryCrcyTxAbsoluteExchangeRate` | `Decimal(9,5)` |  | Absolute Tax Exch. Rate in C/R Cur. |  |  |  |
| `CtryCrcyTaxEffctvExchangeRate` | `CtryCrcyTaxEffctvExchangeRate` | `Decimal(12,5)` |  | Effective Tax Exch. Rate in C/R Cur. |  |  |  |
| `ReversalReason` | `ReversalReason` | `String(2)` |  | Reversal Reason |  |  |  |
| `ParkedByUser` | `ParkedByUser` | `String(12)` |  | JE Parked By |  |  |  |
| `ParkingDate` | `ParkingDate` | `Date` |  | Parked On |  |  |  |
| `ParkingTime` | `ParkingTime` | `String(6)` |  | Time of Parking |  |  |  |
| `ParkingTransactionCode` | `ParkingTransactionCode` | `String(20)` |  | Parking Transaction Code |  |  |  |
| `Branch` | `Branch` | `String(4)` |  | Branch |  |  |  |
| `NmbrOfPages` | `NmbrOfPages` | `String(3)` |  | Number of Pages |  |  |  |
| `IsDiscountDocument` | `IsDiscountDocument` | `String(1)` |  | discount document |  |  |  |
| `Reference1InDocumentHeader` | `Reference1InDocumentHeader` | `String(20)` |  | Reference 1 |  |  |  |
| `Reference2InDocumentHeader` | `Reference2InDocumentHeader` | `String(20)` |  | Reference 2 |  |  |  |
| `InvoiceReceiptDate` | `InvoiceReceiptDate` | `Date` |  | Invoice Receipt Date |  |  |  |
| `Ledger` | `Ledger` | `String(2)` |  | Ledger |  | _Ledger | S/4 only — no ECC equivalent |
| `LedgerGroup` | `LedgerGroup` | `String(4)` |  | Ledger Group |  |  |  |
| `AlternativeReferenceDocument` | `AlternativeReferenceDocument` | `String(26)` |  | Alternative Reference Document |  |  |  |
| `TaxReportingDate` | `TaxReportingDate` | `Date` |  | Tax Reporting Date |  |  |  |
| `TaxFulfillmentDate` | `TaxFulfillmentDate` | `Date` |  | Tax Fulfill. Date |  |  |  |
| `AccountingDocumentClass` | `AccountingDocumentClass` | `String(6)` |  | Acctg Document Class |  |  |  |
| `ExchangeRateType` | `ExchangeRateType` | `String(4)` |  | Exchange Rate Type |  |  |  |
| `MarketDataAbsoluteExchangeRate` | `MarketDataAbsoluteExchangeRate` | `Decimal(28,14)` |  | Absolute Market Data Exch. Rate |  |  |  |
| `MktDataEffectiveExchangeRate` | `MktDataEffectiveExchangeRate` | `Decimal(31,14)` |  | Effective Market Data Exch. Rate |  |  |  |
| `SenderLogicalSystem` | `SenderLogicalSystem` | `String(10)` |  | Sender Logical System |  |  |  |
| `SenderCompanyCode` | `SenderCompanyCode` | `String(4)` |  | Sender CoCode |  |  |  |
| `SenderAccountingDocument` | `SenderAccountingDocument` | `String(10)` |  | Sender Journal Entry |  |  |  |
| `SenderFiscalYear` | `SenderFiscalYear` | `String(4)` |  | Fiscal Year in Sender System |  |  |  |
| `ReversalReferenceDocumentCntxt` | `ReversalReferenceDocumentCntxt` | `String(10)` |  | Reversal Organizatns |  |  |  |
| `ReversalReferenceDocument` | `ReversalReferenceDocument` | `String(10)` |  | Reversal Ref. No. |  |  |  |
| `LatePaymentReason` | `LatePaymentReason` | `String(2)` |  | Late Payment Reason |  |  |  |
| `SalesDocumentCondition` | `SalesDocumentCondition` | `String(10)` |  | Sales Document Condition |  |  |  |
| `IsReversal` | `IsReversal` | `Boolean` |  | Is Reversing |  |  |  |
| `IsReversed` | `IsReversed` | `Boolean` |  | Is Reversed |  |  |  |
| `GLBusinessTransactionGroup` | `GLBusinessTransactionGroup` | `String(1)` |  | GL Business Transaction Group |  |  |  |
| `CostAccountingValuationDate` | `CostAccountingValuationDate` | `Date` |  | Valuation Date |  |  |  |
| `TaxCountry` | `TaxCountry` | `String(3)` |  | Tax Country/Region |  |  |  |
| `JournalEntryLastChangeDateTime` | `JournalEntryLastChangeDateTime` | `DateTime` |  | Journal Entry Last Change Date Time |  |  |  |
| `JournalEntryReprocessingStatus` | `JournalEntryReprocessingStatus` | `String(1)` |  | Journal Entry Reprocessing Status |  |  |  |
| `JrnlEntryCntrySpecificRef1` | `JrnlEntryCntrySpecificRef1` | `String(80)` |  | Country/Region Specific Reference 1 |  |  |  |
| `JrnlEntryCntrySpecificDate1` | `JrnlEntryCntrySpecificDate1` | `Date` |  | Country/Region Specific Date 1 |  |  |  |
| `JrnlEntryCntrySpecificRef2` | `JrnlEntryCntrySpecificRef2` | `String(25)` |  | Country/Region Specific Reference 2 |  |  |  |
| `JrnlEntryCntrySpecificDate2` | `JrnlEntryCntrySpecificDate2` | `Date` |  | Country/Region Specific Date 2 |  |  |  |
| `JrnlEntryCntrySpecificRef3` | `JrnlEntryCntrySpecificRef3` | `String(25)` |  | Country/Region Specific Reference 3 |  |  |  |
| `JrnlEntryCntrySpecificDate3` | `JrnlEntryCntrySpecificDate3` | `Date` |  | Country/Region Specific Date 3 |  |  |  |
| `JrnlEntryCntrySpecificRef4` | `JrnlEntryCntrySpecificRef4` | `String(50)` |  | Country/Region Specific Reference 4 |  |  |  |
| `JrnlEntryCntrySpecificDate4` | `JrnlEntryCntrySpecificDate4` | `Date` |  | Country/Region Specific Date 4 |  |  |  |
| `JrnlEntryCntrySpecificRef5` | `JrnlEntryCntrySpecificRef5` | `String(50)` |  | Country/Region Specific Reference 5 |  |  |  |
| `JrnlEntryCntrySpecificDate5` | `JrnlEntryCntrySpecificDate5` | `Date` |  | Country/Region Specific Date 5 |  |  |  |
| `JrnlEntryCntrySpecificBP1` | `JrnlEntryCntrySpecificBP1` | `String(10)` |  | Ctry/Reg. Specific Business Partner 1 |  |  |  |
| `JrnlEntryCntrySpecificBP2` | `JrnlEntryCntrySpecificBP2` | `String(10)` |  | Ctry/Reg. Specific Business Partner 2 |  |  |  |
| `WithholdingTaxReportingDate` | `WithholdingTaxReportingDate` | `Date` |  | Wtax Reporting Date |  |  |  |


## Entity: `JournalEntryItemBillOfExchange`

- **ABAP Name:** `I_BillOfExchange`
- **Label:** Bill of Exchange
- **VDM Type:** `BASIC` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `CompanyCode` | `CompanyCode` | `String(4)` | Y | Company Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `AccountingDocument` | `AccountingDocument` | `String(10)` | Y | Document Number |  |  | S/4 only entity (no ECC CDC mapping) |
| `FiscalYear` | `FiscalYear` | `String(4)` | Y | Fiscal Year |  |  | S/4 only entity (no ECC CDC mapping) |
| `AccountingDocumentItem` | `AccountingDocumentItem` | `String(3)` | Y | Item |  |  | S/4 only entity (no ECC CDC mapping) |
| `Cheque` | `Cheque` | `String(13)` |  | Check number |  |  | S/4 only entity (no ECC CDC mapping) |
| `BillOfExchangeIssueDate` | `BillOfExchangeIssueDate` | `Date` |  | Issue Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `BillOfExchangeUsageDate` | `BillOfExchangeUsageDate` | `Date` |  | Used On |  |  | S/4 only entity (no ECC CDC mapping) |
| `BillOfExchangeUsage` | `BillOfExchangeUsage` | `String(1)` |  | Bill/Exchange Usage |  |  | S/4 only entity (no ECC CDC mapping) |
| `PlannedBillOfExchangeUsage` | `PlannedBillOfExchangeUsage` | `String(1)` |  | Planned Usage |  |  | S/4 only entity (no ECC CDC mapping) |
| `BillOfExchangeDrawer` | `BillOfExchangeDrawer` | `String(30)` |  | Drawer |  |  | S/4 only entity (no ECC CDC mapping) |
| `BillOfExchangeDrawerCityName` | `BillOfExchangeDrawerCityName` | `String(30)` |  | City of Drawer |  |  | S/4 only entity (no ECC CDC mapping) |
| `BillOfExchangeDrawee` | `BillOfExchangeDrawee` | `String(30)` |  | Drawee |  |  | S/4 only entity (no ECC CDC mapping) |
| `BillOfExchangeDraweeCityName` | `BillOfExchangeDraweeCityName` | `String(30)` |  | City of Drawee |  |  | S/4 only entity (no ECC CDC mapping) |
| `BillOfExchangeDomicileText` | `BillOfExchangeDomicileText` | `String(60)` |  | Domicile |  |  | S/4 only entity (no ECC CDC mapping) |
| `BillOfExchangeIsAccepted` | `BillOfExchangeIsAccepted` | `Boolean` |  | Accepted |  |  | S/4 only entity (no ECC CDC mapping) |
| `Region` | `Region` | `String(3)` |  | Region |  |  | S/4 only entity (no ECC CDC mapping) |
| `BillOfExchangeDocumentStatus` | `BillOfExchangeDocumentStatus` | `String(1)` |  | Bill/Ex. Status |  |  | S/4 only entity (no ECC CDC mapping) |
| `BillOfExchangeIsProtested` | `BillOfExchangeIsProtested` | `String(1)` |  | Bill Protest ID |  |  | S/4 only entity (no ECC CDC mapping) |
| `BillOfExchangeIsOnDemand` | `BillOfExchangeIsOnDemand` | `Boolean` |  | Bill on Demand |  |  | S/4 only entity (no ECC CDC mapping) |
| `BusinessPlace` | `BusinessPlace` | `String(4)` |  | Business Place |  |  | S/4 only entity (no ECC CDC mapping) |
| `BusinessSectionCode` | `BusinessSectionCode` | `String(4)` |  | Section Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `BillOfExchangePortfolio` | `BillOfExchangePortfolio` | `String(10)` |  | Bill Portfolio |  |  | S/4 only entity (no ECC CDC mapping) |
| `BillOfExchangeCntrlBankLocText` | `BillOfExchangeCntrlBankLocText` | `String(60)` |  | Cen.Bank Loc. |  |  | S/4 only entity (no ECC CDC mapping) |
| `BOEDraweeBankKey` | `BOEDraweeBankKey` | `String(15)` |  | Bank Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `BillOfExchangeDataAgingDate` | `BillOfExchangeDataAgingDate` | `Date` |  | Data Aging |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsBusinessPurposeCompleted` | `IsBusinessPurposeCompleted` | `Boolean` |  | Purpose Completed |  |  | S/4 only entity (no ECC CDC mapping) |
| `AuthorizationGroup` | `AuthorizationGroup` | `String(4)` |  | Authorization |  |  | S/4 only entity (no ECC CDC mapping) |
