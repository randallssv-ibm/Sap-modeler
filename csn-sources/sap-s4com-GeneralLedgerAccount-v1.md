# GeneralLedgerAccount

> Source file: `sap-s4com-GeneralLedgerAccount-v1.json`


## Entity: `ChartOfAccounts`

- **ABAP Name:** `I_ChartOfAccounts`
- **Label:** Chart Of Accounts
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `ChartOfAccounts` | `T001` | `KTOPL` | `String(4)` | Y | Chart of Accounts |  |  |  |
| `CorporateGroupChartOfAccounts` |  |  | `String(4)` |  | Group Chart of Accts |  |  | S/4 only entity |
| `ChartOfAcctsIsBlocked` |  |  | `Boolean` |  | Blocked |  |  | S/4 only entity |
| `MaintenanceLanguage` |  |  | `String(2)` |  | Maint.Language |  |  | S/4 only entity |


## Entity: `ChartOfAccountsText`

- **ABAP Name:** `I_ChartOfAccountsText`
- **Label:** Chart Of Accounts - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `ChartOfAccounts` | `T001` | `KTOPL` | `String(4)` | Y | Chart of Accounts |  | _ChartOfAccounts |  |
| `Language` |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity |
| `ChartOfAccountsName` |  |  | `String(50)` |  | Chart of Accounts Description |  |  | S/4 only entity |


## Entity: `FinancialStatementHierNode`

- **ABAP Name:** `I_FinancialStatementHierNode`
- **Label:** Financial Statement Hierarchy Node
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `FinancialStatementHierarchy` |  |  | `String(42)` | Y | Hierarchy ID |  | _Hierarchy | S/4 only entity |
| `HierarchyNode` |  |  | `String(50)` | Y | Node |  |  | S/4 only entity |
| `ValidityEndDate` |  |  | `Date` | Y | Valid To |  |  | S/4 only entity |
| `ValidityStartDate` |  |  | `Date` |  | Validity Start Date |  |  | S/4 only entity |
| `ParentNode` |  |  | `String(50)` |  | Par. Node |  |  | S/4 only entity |
| `HierarchyVersion` |  |  | `String(15)` |  | Version |  |  | S/4 only entity |
| `FinancialStatementLeafItem` |  |  | `String(50)` |  | Node |  |  | S/4 only entity |
| `SequenceNumber` |  |  | `String(56)` |  |  |  |  | S/4 only entity |
| `SignIsInverted` |  |  | `Boolean` |  | Attribute Value |  |  | S/4 only entity |
| `ChartOfAccounts` | `T001` | `KTOPL` | `String(12)` |  | Node Class |  |  |  |
| `FinancialStatementNodeType` |  |  | `String(1)` |  | Node Type |  |  | S/4 only entity |
| `FinStmntNodeFormattedID` |  |  | `String(32)` |  | Node for Extraction |  |  | S/4 only entity |
| `HierarchyNodeVal` |  |  | `String(40)` |  | Value |  |  | S/4 only entity |
| `HierarchyNodeSequence` |  |  | `String(6)` |  | Sequence Number |  |  | S/4 only entity |
| `HierarchyLevel` |  |  | `String(6)` |  | Hierarchy Level |  |  | S/4 only entity |
| `DebitCreditCode` |  |  | `String(1)` |  | Balance |  |  | S/4 only entity |


## Entity: `FinancialStatementHierNodeText`

- **ABAP Name:** `I_FinancialStatementHierNodeT`
- **Label:** Financial Statement Hierarchy Node - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `FinancialStatementHierarchy` |  |  | `String(42)` | Y | Hierarchy ID |  | _Hierarchy | S/4 only entity |
| `HierarchyNode` |  |  | `String(50)` | Y | Node |  |  | S/4 only entity |
| `ValidityEndDate` |  |  | `Date` | Y | Valid To |  |  | S/4 only entity |
| `Language` |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity |
| `HierarchyNodeText` |  |  | `String(50)` |  | Description |  |  | S/4 only entity |
| `HierarchyNodeShortText` |  |  | `String(20)` |  |  |  |  | S/4 only entity |
| `ValidityStartDate` |  |  | `Date` |  | Valid From |  |  | S/4 only entity |
| `FinStmntNodeFormattedID` |  |  | `String(32)` |  | Node for Extraction |  |  | S/4 only entity |


## Entity: `FinancialStatementHierText`

- **ABAP Name:** `I_FinancialStatementHierT`
- **Label:** Financial Statement Hierarchy - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `FinancialStatementHierarchy` |  |  | `String(42)` | Y | Hierarchy ID |  |  | S/4 only entity |
| `ValidityEndDate` |  |  | `Date` | Y | Valid To |  |  | S/4 only entity |
| `Language` |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity |
| `ValidityStartDate` |  |  | `Date` |  | Valid From |  |  | S/4 only entity |
| `FinancialStmntHierarchyName` |  |  | `String(50)` |  | Financial Statement Description |  |  | S/4 only entity |


## Entity: `FinancialStatementHierarchy`

- **ABAP Name:** `I_FinancialStatementHier`
- **Label:** Financial Statement Hierarchy
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `FinancialStatementHierarchy` |  |  | `String(42)` | Y | Hierarchy ID |  |  | S/4 only entity |
| `ValidityEndDate` |  |  | `Date` | Y | Validity End Date |  |  | S/4 only entity |
| `ValidityStartDate` |  |  | `Date` |  | Validity Start Date |  |  | S/4 only entity |
| `HierarchyType` |  |  | `String(4)` |  | Hierarchy Type |  |  | S/4 only entity |
| `LastChangedByUser` |  |  | `String(12)` |  | Last Changed By |  |  | S/4 only entity |
| `LastChangeTime` |  |  | `DateTime` |  | Updated At |  |  | S/4 only entity |
| `LastChangeDateTime` |  |  | `DateTime` |  | Updated At |  |  | S/4 only entity |
| `ChartOfAccounts` | `T001` | `KTOPL` | `String(80)` |  | Char80 |  |  |  |
| `FinancialStatementAssetsItem` |  |  | `String(80)` |  | Char80 |  |  | S/4 only entity |
| `FinStatementLiabilitiesItem` |  |  | `String(80)` |  | Char80 |  |  | S/4 only entity |
| `FinancialStatementNetLossItem` |  |  | `String(80)` |  | Char80 |  |  | S/4 only entity |
| `FinStatementNetProfitItem` |  |  | `String(80)` |  | Char80 |  |  | S/4 only entity |
| `FinStatementProfitAndLossItem` |  |  | `String(80)` |  | Char80 |  |  | S/4 only entity |
| `FinancialStatementOrphansItem` |  |  | `String(80)` |  | Char80 |  |  | S/4 only entity |
| `FinancialStatementNotesItem` |  |  | `String(80)` |  | Char80 |  |  | S/4 only entity |
| `GroupChartOfAccountIsUsed` |  |  | `Boolean` |  | Char80 |  |  | S/4 only entity |
| `FunctionalAreaIsUsed` |  |  | `Boolean` |  | Char80 |  |  | S/4 only entity |


## Entity: `GLAccountHierNodeBySemanticTag`

- **ABAP Name:** `I_GLAccountHierNodeBySemTag`
- **Label:** GLAccount Hierarchy Node By Semantic Tag
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `GLAccountHierarchy` |  |  | `String(42)` | Y | Hierarchy ID |  | _Hierarchy | S/4 only entity |
| `HierarchyNode` |  |  | `String(50)` | Y | Node |  |  | S/4 only entity |
| `SemanticTag` |  |  | `String(10)` | Y | Semantic Tag |  | _SemanticTag | S/4 only entity |
| `HierarchyNodeType` |  |  | `String(30)` |  | Field Name |  |  | S/4 only entity |


## Entity: `GLAccountHierarchyNode`

- **ABAP Name:** `I_GLAccountHierarchyNode`
- **Label:** G/L Account Hierarchy Node
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `GLAccountHierarchy` |  |  | `String(42)` | Y | G/L Account Hierarchy |  | _Hierarchy | S/4 only entity |
| `HierarchyNode` |  |  | `String(50)` | Y | Node |  |  | S/4 only entity |
| `ValidityEndDate` |  |  | `Date` | Y | Validity End Date |  |  | S/4 only entity |
| `ParentNode` |  |  | `String(50)` |  | Par. Node |  |  | S/4 only entity |
| `HierarchyVersion` |  |  | `String(15)` |  | Version |  |  | S/4 only entity |
| `ValidityStartDate` |  |  | `Date` |  | Validity Start Date |  |  | S/4 only entity |
| `ChartOfAccounts` | `T001` | `KTOPL` | `String(4)` |  | Chart of Accounts |  | _ChartOfAccounts |  |
| `GLAccount` |  |  | `String(10)` |  | G/L Account |  | _GLAccountInChartOfAccounts | S/4 only entity |
| `SequenceNumber` |  |  | `String(56)` |  |  |  |  | S/4 only entity |
| `HierarchyNodeSequence` |  |  | `String(6)` |  | Sequence Number |  |  | S/4 only entity |
| `HierarchyNodeLevel` |  |  | `String(6)` |  | Hierarchy Level |  |  | S/4 only entity |
| `NodeType` |  |  | `String(1)` |  | Node Type |  |  | S/4 only entity |
| `SignIsInverted` |  |  | `Boolean` |  | Attribute Value |  |  | S/4 only entity |
| `HierarchyNodeVal` |  |  | `String(40)` |  | Value |  |  | S/4 only entity |


## Entity: `GLAccountHierarchyNodeText`

- **ABAP Name:** `I_GLAccountHierarchyNodeT`
- **Label:** G/L Account Hierarchy Node - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `GLAccountHierarchy` |  |  | `String(42)` | Y | G/L Account Hierarchy |  | _Hierarchy | S/4 only entity |
| `HierarchyNode` |  |  | `String(50)` | Y | Node |  |  | S/4 only entity |
| `ValidityEndDate` |  |  | `Date` | Y | Valid To |  |  | S/4 only entity |
| `Language` |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity |
| `HierarchyNodeText` |  |  | `String(50)` |  | Description |  |  | S/4 only entity |
| `HierarchyNodeShortText` |  |  | `String(20)` |  |  |  |  | S/4 only entity |
| `ValidityStartDate` |  |  | `Date` |  | Valid From |  |  | S/4 only entity |


## Entity: `GLAccountHierarchyText`

- **ABAP Name:** `I_GLAccountHierarchyText`
- **Label:** G/L Account Hierarchy - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `GLAccountHierarchy` |  |  | `String(42)` | Y | G/L Account Hierarchy |  |  | S/4 only entity |
| `ValidityEndDate` |  |  | `Date` | Y | Valid To |  |  | S/4 only entity |
| `Language` |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity |
| `ValidityStartDate` |  |  | `Date` |  | Valid From |  |  | S/4 only entity |
| `GLAccountHierarchyName` |  |  | `String(50)` |  | Description |  |  | S/4 only entity |


## Entity: `GLAccountTypeFlowType`

- **ABAP Name:** `I_GLAccountTypeFlowType`
- **Label:** Flow Type for G/L Account Type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `GLAccountTypeFlowType` |  |  | `String(12)` | Y | GLAcct Type FlowType |  |  | S/4 only entity |


## Entity: `GeneralLedgerAccount`

- **ABAP Name:** `I_GLAccountInChartOfAccounts`
- **Label:** G/L Account In Chart Of Accounts
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `ChartOfAccounts` | `SKA1` | `KTOPL` | `String(4)` | Y | Chart of Accounts |  | _ChartOfAccounts |  |
| `GLAccount` | `SKA1` | `SAKNR` | `String(10)` | Y | G/L Account |  |  |  |
| `IsBalanceSheetAccount` | `SKA1` | `XBILK` | `Boolean` |  | Balance sheet acct |  |  |  |
| `GLAccountGroup` | `SKA1` | `KTOKS` | `String(4)` |  | Account Group |  |  |  |
| `CorporateGroupChartOfAccounts` |  |  | `String(4)` |  | Group Chart of Accts |  | _CorporateGroupChartOfAccounts | S/4 only entity |
| `CorporateGroupAccount` |  |  | `String(10)` |  | Group Account Number |  |  | S/4 only entity |
| `ProfitLossAccountType` | `SKA1` | `GVTYP` | `String(2)` |  | P&L state. acct |  |  |  |
| `SampleGLAccount` | `SKA1` | `MUSTR` | `String(10)` |  | Sample Account |  |  |  |
| `AccountIsMarkedForDeletion` |  |  | `Boolean` |  | Deletion Flag |  |  | S/4 only entity |
| `AccountIsBlockedForCreation` |  |  | `Boolean` |  | Creation Block |  |  | S/4 only entity |
| `AccountIsBlockedForPosting` |  |  | `Boolean` |  | Posting Block |  |  | S/4 only entity |
| `AccountIsBlockedForPlanning` |  |  | `Boolean` |  | Planning Block |  |  | S/4 only entity |
| `PartnerCompany` |  |  | `String(6)` |  | Trading Partner No. |  |  | S/4 only entity |
| `FunctionalArea` | `SKA1` | `FUNC_AREA` | `String(16)` |  | Functional Area |  |  |  |
| `CreationDate` |  |  | `Date` |  | Created On |  |  | S/4 only entity |
| `CreatedByUser` |  |  | `String(12)` |  | Created By |  |  | S/4 only entity |
| `LastChangeDateTime` |  |  | `DateTime` |  | Time Stamp |  |  | S/4 only entity |
| `GLAccountType` |  |  | `String(1)` |  | G/L Account Type |  |  | S/4 only entity |
| `GLAccountSubtype` |  |  | `String(1)` |  | G/L Account Subtype |  |  | S/4 only entity |
| `GLAccountExternal` |  |  | `String(10)` |  | G/L Acct External ID |  |  | S/4 only entity |
| `BankReconciliationAccount` |  |  | `String(10)` |  | Reconciliation Acct |  |  | S/4 only entity |
| `IsProfitLossAccount` |  |  | `Boolean` |  | Profit Loss Account |  |  | S/4 only entity |


## Entity: `GeneralLedgerAccountFlowType`

- **ABAP Name:** `I_GLAccountFlowType`
- **Label:** GLAccount Flow Type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `GLAccountFlowType` |  |  | `String(10)` | Y | G/L Acct. Flow Type |  |  | S/4 only entity |


## Entity: `GeneralLedgerAccountHierarchy`

- **ABAP Name:** `I_GLAccountHierarchy`
- **Label:** General Ledger Account Hierarchy
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `GLAccountHierarchy` |  |  | `String(42)` | Y | G/L Account Hierarchy |  |  | S/4 only entity |
| `ValidityEndDate` |  |  | `Date` | Y | Valid To |  |  | S/4 only entity |
| `ValidityStartDate` |  |  | `Date` |  | Valid From |  |  | S/4 only entity |
| `HierarchyType` |  |  | `String(4)` |  | Hierarchy Type |  |  | S/4 only entity |
| `LastChangedByUser` |  |  | `String(12)` |  | Last Changed By |  |  | S/4 only entity |
| `LastChangeTime` |  |  | `DateTime` |  | Updated At |  |  | S/4 only entity |
| `LastChangeDateTime` |  |  | `DateTime` |  | Updated At |  |  | S/4 only entity |
| `HierarchyShortID` |  |  | `String(20)` |  | Hierarchy ID |  |  | S/4 only entity |
| `FunctionalAreaIsUsed` |  |  | `Boolean` |  | Functional Area |  |  | S/4 only entity |
| `SemanticTagIsUsed` |  |  | `Boolean` |  | Sem. Tag Assigned |  |  | S/4 only entity |
| `ChartOfAccounts` | `T001` | `KTOPL` | `String(4)` |  | Chart of Accounts |  | _ChartOfAccounts |  |


## Entity: `GeneralLedgerAccountLineItem`

- **ABAP Name:** `I_GLAccountLineItemRawData`
- **Label:** Raw Data of G/L Account Line Item
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `SourceLedger` |  |  | `String(2)` | Y | Source Ledger |  |  | S/4 only — no ECC equivalent; Filter SourceLedger='0L' for leading ledger in S/4 |
| `CompanyCode` | `BKPF` | `BUKRS` | `String(4)` | Y | Company Code |  |  |  |
| `FiscalYear` | `BKPF` | `GJAHR` | `String(4)` | Y | Fiscal Year |  |  |  |
| `AccountingDocument` | `BKPF` | `BELNR` | `String(10)` | Y | Journal Entry |  |  |  |
| `LedgerGLLineItem` | `BSEG` | `BUZEI` | `String(6)` | Y | Journal Entry Item |  |  |  |
| `LedgerFiscalYear` |  |  | `String(4)` |  | Fiscal Year of Ledger |  |  | S/4 only — no ECC equivalent |
| `GLRecordType` |  |  | `String(1)` |  | Record Type |  |  | S/4 only entity |
| `JrnlEntrAltvFYConsecutiveID` |  |  | `String(10)` |  | Shifted Fiscal Year Consecutive ID |  |  | S/4 only entity |
| `ChartOfAccounts` | `T001` | `KTOPL` | `String(4)` |  | Chart of Accounts |  | _ChartOfAccounts |  |
| `ControllingArea` | `BSEG` | `KOKRS` | `String(4)` |  | Controlling Area |  |  |  |
| `FinancialTransactionType` |  |  | `String(3)` |  | Financial Transaction Type |  |  | S/4 only entity |
| `GLBusinessTransactionType` |  |  | `String(4)` |  | Transaction Type for General Ledger |  |  | S/4 only entity |
| `BusinessTransactionCategory` |  |  | `String(4)` |  | Business Transaction Category |  |  | S/4 only entity |
| `BusinessTransactionType` |  |  | `String(4)` |  | Business Transaction Type |  |  | S/4 only entity |
| `FinancialClosingStep` |  |  | `String(3)` |  | Financial Closing Step |  |  | S/4 only entity |
| `ControllingBusTransacType` |  |  | `String(4)` |  | Business Transaction |  |  | S/4 only entity |
| `ReferenceDocumentType` |  |  | `String(5)` |  | Reference Document Type |  |  | S/4 only entity |
| `LogicalSystem` |  |  | `String(10)` |  | Logical System |  |  | S/4 only entity |
| `ReferenceDocumentContext` |  |  | `String(10)` |  | Reference Document Context |  |  | S/4 only entity |
| `ReferenceDocument` | `BKPF` | `XBLNR` | `String(10)` |  | Reference Document |  |  |  |
| `ReferenceDocumentItem` |  |  | `String(6)` |  | Reference Document Item |  |  | S/4 only entity |
| `ReferenceDocumentItemGroup` |  |  | `String(6)` |  | Reference Document Item Group |  |  | S/4 only entity |
| `TransactionSubitem` |  |  | `String(6)` |  | Sub Transaction |  |  | S/4 only entity |
| `AccountingNotificationUUID` |  |  | `UUID` |  | Accounting Notification UUID |  |  | S/4 only entity |
| `OffsettingLedgerGLLineItem` |  |  | `String(6)` |  | G/L Offsetting Entry Line Item |  |  | S/4 only entity |
| `IsReversal` |  |  | `Boolean` |  | Is Reversing |  |  | S/4 only entity |
| `IsReversed` |  |  | `Boolean` |  | Is Reversed |  |  | S/4 only entity |
| `ReversalReferenceDocumentType` |  |  | `String(5)` |  | Reversal Reference Document Type |  |  | S/4 only entity |
| `ReversalReferenceDocumentCntxt` |  |  | `String(10)` |  | Reversal Reference Document Context |  |  | S/4 only entity |
| `ReversalReferenceDocument` |  |  | `String(10)` |  | Reversal Reference Document |  |  | S/4 only entity |
| `ReversalTransactionSubitem` |  |  | `String(6)` |  | Reversal Transaction Sub Item |  |  | S/4 only entity |
| `IsSettlement` |  |  | `Boolean` |  | Is Settling |  |  | S/4 only entity |
| `IsSettled` |  |  | `Boolean` |  | Is Settled |  |  | S/4 only entity |
| `PredecessorReferenceDocType` |  |  | `String(5)` |  | Predecessor Reference Document Type |  |  | S/4 only entity |
| `PredecessorReferenceDocCntxt` |  |  | `String(10)` |  | Predecessor Reference Document Context |  |  | S/4 only entity |
| `PredecessorReferenceDocument` |  |  | `String(10)` |  | Predecessor Reference Document |  |  | S/4 only entity |
| `PredecessorReferenceDocItem` |  |  | `String(6)` |  | Predecessor Reference Document Item |  |  | S/4 only entity |
| `PrdcssrJournalEntryCompanyCode` |  |  | `String(4)` |  | Predecessor Journal Entry Company Code |  |  | S/4 only entity |
| `PrdcssrJournalEntryFiscalYear` |  |  | `String(4)` |  | Predecessor Journal Entry Fiscal Year |  |  | S/4 only entity |
| `PredecessorJournalEntry` |  |  | `String(10)` |  | Predecessor Journal Entry |  |  | S/4 only entity |
| `PredecessorJournalEntryItem` |  |  | `String(6)` |  | Predecessor Journal Entry Item |  |  | S/4 only entity |
| `SourceReferenceDocumentType` |  |  | `String(5)` |  | Source Reference Document Type |  |  | S/4 only entity |
| `SourceLogicalSystem` |  |  | `String(10)` |  | Source Logical System |  |  | S/4 only entity |
| `SourceReferenceDocumentCntxt` |  |  | `String(10)` |  | Source Reference Document Context |  |  | S/4 only entity |
| `SourceReferenceDocument` |  |  | `String(10)` |  | Source Reference Document |  |  | S/4 only entity |
| `SourceReferenceDocumentItem` |  |  | `String(6)` |  | Source Reference Document Item |  |  | S/4 only entity |
| `SourceReferenceDocSubitem` |  |  | `String(6)` |  | Source Reference Document Subitem |  |  | S/4 only entity |
| `IsCommitment` |  |  | `Boolean` |  | Is Commitment |  |  | S/4 only entity |
| `JrnlEntryItemObsoleteReason` |  |  | `String(1)` |  | Obsolete Reason |  |  | S/4 only entity |
| `JournalEntryIsSecondaryEntry` |  |  | `Boolean` |  | Is Secondary Journal Entry |  |  | S/4 only entity |
| `JrnlPeriodEndClosingRunLogUUID` |  |  | `UUID` |  | Closing Run UUID |  |  | S/4 only entity |
| `OrganizationalChange` |  |  | `String(10)` |  | Organizational Change |  |  | S/4 only entity |
| `GLAccount` | `BSEG` | `HKONT` | `String(10)` |  | G/L Account |  | _GLAccountInChartOfAccounts |  |
| `CostCenter` | `BSEG` | `KOSTL` | `String(10)` |  | Cost Center |  |  |  |
| `ProfitCenter` | `BSEG` | `PRCTR` | `String(10)` |  | Profit Center |  |  |  |
| `FunctionalArea` | `BSEG` | `FKBER` | `String(16)` |  | Functional Area |  |  |  |
| `BusinessArea` | `BSEG` | `GSBER` | `String(4)` |  | Business Area |  |  |  |
| `Segment` | `BSEG` | `SEGMENT` | `String(10)` |  | Segment |  |  |  |
| `PartnerCostCenter` |  |  | `String(10)` |  | Partner Cost Center |  |  | S/4 only entity |
| `PartnerProfitCenter` |  |  | `String(10)` |  | Partner Profit Center |  |  | S/4 only entity |
| `PartnerFunctionalArea` |  |  | `String(16)` |  | Partner Func. Area |  |  | S/4 only entity |
| `PartnerBusinessArea` |  |  | `String(4)` |  | Partner Bus. Area |  |  | S/4 only entity |
| `PartnerCompany` |  |  | `String(6)` |  | Trading Partner |  |  | S/4 only entity |
| `PartnerSegment` |  |  | `String(10)` |  | Partner Segment |  |  | S/4 only entity |
| `BalanceTransactionCurrency` |  |  | `String(5)` |  | Balance Transaction Currency |  |  | S/4 only entity |
| `AmountInBalanceTransacCrcy` |  |  | `Decimal(34,4)` |  | Amount in Balance Transaction Currency | BalanceTransactionCurrency |  | S/4 only entity |
| `TransactionCurrency` | `BKPF` | `WAERS` | `String(5)` |  | Transaction Currency |  |  |  |
| `AmountInTransactionCurrency` | `BSEG` | `WRBTR` | `Decimal(34,4)` |  | Amount in Transaction Currency | TransactionCurrency |  |  |
| `CompanyCodeCurrency` | `T001` | `WAERS` | `String(5)` |  | Company Code Currency |  |  |  |
| `AmountInCompanyCodeCurrency` | `BSEG` | `DMBTR` | `Decimal(34,4)` |  | Amount in Company Code Currency | CompanyCodeCurrency |  |  |
| `GlobalCurrency` |  |  | `String(5)` |  | Global Currency |  |  | S/4 only — no ECC equivalent |
| `AmountInGlobalCurrency` |  |  | `Decimal(34,4)` |  | Amount in Global Currency | GlobalCurrency |  | S/4 only — no ECC equivalent |
| `FunctionalCurrency` |  |  | `String(5)` |  | Functional Currency |  |  | S/4 only entity |
| `AmountInFunctionalCurrency` |  |  | `Decimal(34,4)` |  | Amount in Functional Currency | FunctionalCurrency |  | S/4 only entity |
| `FreeDefinedCurrency1` |  |  | `String(5)` |  | Freely Defined Currency 1 |  |  | S/4 only — no ECC equivalent |
| `AmountInFreeDefinedCurrency1` |  |  | `Decimal(34,4)` |  | Amount in Freely Defined Currency 1 | FreeDefinedCurrency1 |  | S/4 only — no ECC equivalent |
| `FreeDefinedCurrency2` |  |  | `String(5)` |  | Freely Defined Currency 2 |  |  | S/4 only — no ECC equivalent |
| `AmountInFreeDefinedCurrency2` |  |  | `Decimal(34,4)` |  | Amount in Freely Defined Currency 2 | FreeDefinedCurrency2 |  | S/4 only — no ECC equivalent |
| `FreeDefinedCurrency3` |  |  | `String(5)` |  | Freely Defined Currency 3 |  |  | S/4 only — no ECC equivalent |
| `AmountInFreeDefinedCurrency3` |  |  | `Decimal(34,4)` |  | Amount in Freely Defined Currency 3 | FreeDefinedCurrency3 |  | S/4 only — no ECC equivalent |
| `FreeDefinedCurrency4` |  |  | `String(5)` |  | Freely Defined Currency 4 |  |  | S/4 only entity |
| `AmountInFreeDefinedCurrency4` |  |  | `Decimal(34,4)` |  | Amount in Freely Defined Currency 4 | FreeDefinedCurrency4 |  | S/4 only entity |
| `FreeDefinedCurrency5` |  |  | `String(5)` |  | Freely Defined Currency 5 |  |  | S/4 only entity |
| `AmountInFreeDefinedCurrency5` |  |  | `Decimal(34,4)` |  | Amount in Freely Defined Currency 5 | FreeDefinedCurrency5 |  | S/4 only entity |
| `FreeDefinedCurrency6` |  |  | `String(5)` |  | Freely Defined Currency 6 |  |  | S/4 only entity |
| `AmountInFreeDefinedCurrency6` |  |  | `Decimal(34,4)` |  | Amount in Freely Defined Currency 6 | FreeDefinedCurrency6 |  | S/4 only entity |
| `FreeDefinedCurrency7` |  |  | `String(5)` |  | Freely Defined Currency 7 |  |  | S/4 only entity |
| `AmountInFreeDefinedCurrency7` |  |  | `Decimal(34,4)` |  | Amount in Freely Defined Currency 7 | FreeDefinedCurrency7 |  | S/4 only entity |
| `FreeDefinedCurrency8` |  |  | `String(5)` |  | Freely Defined Currency 8 |  |  | S/4 only entity |
| `AmountInFreeDefinedCurrency8` |  |  | `Decimal(34,4)` |  | Amount in Freely Defined Currency 8 | FreeDefinedCurrency8 |  | S/4 only entity |
| `FixedAmountInGlobalCrcy` |  |  | `Decimal(34,4)` |  | Fixed Amount in Global Currency | GlobalCurrency |  | S/4 only entity |
| `GrpValnFixedAmtInGlobCrcy` |  |  | `Decimal(34,4)` |  | Group Val. Fixed Amount in Global Cur. | GlobalCurrency |  | S/4 only entity |
| `PrftCtrValnFxdAmtInGlobCrcy` |  |  | `Decimal(34,4)` |  | PC Val. Fixed Amount in Global Currency | GlobalCurrency |  | S/4 only entity |
| `FixedAmountInCoCodeCrcy` |  |  | `Decimal(34,4)` |  | Fixed Amount in Company Currency | CompanyCodeCurrency |  | S/4 only entity |
| `FixedAmountInTransCrcy` |  |  | `Decimal(34,4)` |  | Fixed Amount in Transaction Currency | TransactionCurrency |  | S/4 only entity |
| `TotalPriceVarcInGlobalCrcy` |  |  | `Decimal(34,4)` |  | Total Price Variance in Global Currency | GlobalCurrency |  | S/4 only entity |
| `GrpValnTotPrcVarcInGlobCrcy` |  |  | `Decimal(34,4)` |  | GV Total Price Var. in Global Currency | GlobalCurrency |  | S/4 only entity |
| `PrftCtrValnTotPrcVarcInGlbCrcy` |  |  | `Decimal(34,4)` |  | PC Val. Total Price Var. in Global Cur. | GlobalCurrency |  | S/4 only entity |
| `FixedPriceVarcInGlobalCrcy` |  |  | `Decimal(34,4)` |  | Fixed Price Variance in Global Currency | GlobalCurrency |  | S/4 only entity |
| `GrpValnFixedPrcVarcInGlobCrcy` |  |  | `Decimal(34,4)` |  | GV Fixed Price Var. in Global Currency | GlobalCurrency |  | S/4 only entity |
| `PrftCtrValnFxdPrcVarcInGlbCrcy` |  |  | `Decimal(34,4)` |  | PC Val. Fixed Price Var. in Global Cur. | GlobalCurrency |  | S/4 only entity |
| `ControllingObjectCurrency` |  |  | `String(5)` |  | CO Object Currency |  |  | S/4 only entity |
| `AmountInObjectCurrency` |  |  | `Decimal(34,4)` |  | Amount in Object Currency | ControllingObjectCurrency |  | S/4 only entity |
| `GrantCurrency` |  |  | `String(5)` |  | Grant Currency |  |  | S/4 only entity |
| `AmountInGrantCurrency` |  |  | `Decimal(34,4)` |  | Amount in Grant Crcy | GrantCurrency |  | S/4 only entity |
| `BaseUnit` | `BSEG` | `MEINS` | `String(3)` |  | Base Unit of Measure |  |  |  |
| `Quantity` | `BSEG` | `MENGE` | `Decimal(23,3)` |  | Quantity | BaseUnit |  |  |
| `FixedQuantity` |  |  | `Decimal(23,3)` |  | Fixed Quantity | BaseUnit |  | S/4 only entity |
| `CostSourceUnit` |  |  | `String(3)` |  | Cost Source Unit |  |  | S/4 only entity |
| `ValuationQuantity` |  |  | `Decimal(23,3)` |  | Valuation Quantity | CostSourceUnit |  | S/4 only entity |
| `ValuationFixedQuantity` |  |  | `Decimal(23,3)` |  | Valuation Fixed Quantity | CostSourceUnit |  | S/4 only entity |
| `ReferenceQuantityUnit` |  |  | `String(3)` |  | Reference Qty UoM |  |  | S/4 only entity |
| `ReferenceQuantity` |  |  | `Decimal(23,3)` |  | Reference quantity | ReferenceQuantityUnit |  | S/4 only entity |
| `AdditionalQuantity1Unit` |  |  | `String(3)` |  | Additional Quantity 1 Unit |  |  | S/4 only entity |
| `AdditionalQuantity1` |  |  | `Decimal(23,3)` |  | Additional Quantity 1 | AdditionalQuantity1Unit |  | S/4 only entity |
| `AdditionalQuantity2Unit` |  |  | `String(3)` |  | Additional Quantity 2 Unit |  |  | S/4 only entity |
| `AdditionalQuantity2` |  |  | `Decimal(23,3)` |  | Additional Quantity 2 | AdditionalQuantity2Unit |  | S/4 only entity |
| `AdditionalQuantity3Unit` |  |  | `String(3)` |  | Additional Quantity 3 Unit |  |  | S/4 only entity |
| `AdditionalQuantity3` |  |  | `Decimal(23,3)` |  | Additional Quantity 3 | AdditionalQuantity3Unit |  | S/4 only entity |
| `IncmpltSummableValnQtyUnt` |  |  | `String(3)` |  | Incomplete Sum. Valuation Quantity Unit |  |  | S/4 only entity |
| `IncmpltSummableValnQty` |  |  | `Decimal(23,3)` |  | Incomplete Summable Valuation Quantity | IncmpltSummableValnQtyUnt |  | S/4 only entity |
| `IncmpltSummableValnFxdQty` |  |  | `Decimal(23,3)` |  | Incomplete Sum. Valuation Fix Quantity | IncmpltSummableValnQtyUnt |  | S/4 only entity |
| `DebitCreditCode` | `BSEG` | `SHKZG` | `String(1)` |  | Debit/Credit Code |  |  |  |
| `FiscalPeriod` | `BKPF` | `MONAT` | `String(3)` |  | Fiscal Period |  |  |  |
| `FiscalYearVariant` |  |  | `String(2)` |  | Fiscal Year Variant |  |  | S/4 only entity |
| `FiscalYearPeriod` | `BKPF` | `GJAHR+MONAT` | `String(7)` |  | Fiscal Year Period |  |  |  |
| `PostingDate` | `BKPF` | `BUDAT` | `Date` |  | Posting Date |  |  |  |
| `DocumentDate` | `BKPF` | `BLDAT` | `Date` |  | Journal Entry Date |  |  |  |
| `AccountingDocumentType` | `BKPF` | `BLART` | `String(2)` |  | Journal Entry Type |  |  |  |
| `AccountingDocumentItem` | `BSEG` | `BUZEI` | `String(3)` |  | Posting View Item |  |  |  |
| `AssignmentReference` | `BSEG` | `ZUONR` | `String(18)` |  | Assignment Reference |  |  |  |
| `AccountingDocumentCategory` |  |  | `String(1)` |  | Journal Entry Category |  |  | S/4 only entity |
| `JournalEntryItemCategory` |  |  | `String(5)` |  | Journal Entry Item Category |  |  | S/4 only entity |
| `PostingKey` |  |  | `String(2)` |  | Posting Key |  |  | S/4 only entity |
| `TransactionTypeDetermination` | `BSEG` | `BEWAR` | `String(3)` |  | Transaction Key |  |  |  |
| `SubLedgerAcctLineItemType` |  |  | `String(5)` |  | SLA Line Item Type |  |  | S/4 only entity |
| `AccountingDocCreatedByUser` |  |  | `String(12)` |  | Journal Entry Created By |  |  | S/4 only entity |
| `LastChangeDateTime` |  |  | `DateTime` |  | Last Change Date Time |  |  | S/4 only entity |
| `CreationDateTime` |  |  | `DateTime` |  | Creation Date Time |  |  | S/4 only entity |
| `CreationDate` |  |  | `Date` |  | Creation Date |  |  | S/4 only entity |
| `EliminationProfitCenter` |  |  | `String(10)` |  | Elimination Profit Center |  |  | S/4 only entity |
| `OriginObjectType` |  |  | `String(2)` |  | Origin Object Type |  |  | S/4 only entity |
| `GLAccountType` |  |  | `String(1)` |  | G/L Account Type |  |  | S/4 only entity |
| `AlternativeGLAccount` |  |  | `String(10)` |  | Alternative G/L Account |  | _AlternativeGLAccount | S/4 only entity |
| `CountryChartOfAccounts` |  |  | `String(4)` |  | Alternative Chart of Accounts |  | _CountryChartOfAccounts | S/4 only entity |
| `ItemIsSplit` |  |  | `Boolean` |  | Itm chngd by Doc Spl |  |  | S/4 only entity |
| `ConsolidationUnit` |  |  | `String(18)` |  | Consolidation Unit |  |  | S/4 only entity |
| `PartnerConsolidationUnit` |  |  | `String(18)` |  | Partner Consolidation Unit |  |  | S/4 only entity |
| `Company` |  |  | `String(6)` |  | Company |  |  | S/4 only entity |
| `ConsolidationChartOfAccounts` |  |  | `String(2)` |  | Consolidation Chart of Accounts |  |  | S/4 only entity |
| `CnsldtnFinancialStatementItem` |  |  | `String(10)` |  | Consolidation Financial Statement Item |  |  | S/4 only entity |
| `CnsldtnSubitemCategory` |  |  | `String(3)` |  | Consolidation Subitem Category |  |  | S/4 only entity |
| `CnsldtnSubitem` |  |  | `String(10)` |  | Consolidation Subitem |  |  | S/4 only entity |
| `InvoiceReference` | `BSEG` | `REBZG` | `String(10)` |  | Invoice Reference |  |  |  |
| `InvoiceReferenceFiscalYear` | `BSEG` | `REBZJ` | `String(4)` |  | Invoice Reference Fiscal Year |  |  |  |
| `FollowOnDocumentType` |  |  | `String(1)` |  | Follow-On Document Type |  |  | S/4 only entity |
| `InvoiceItemReference` |  |  | `String(3)` |  | Invoice Item Reference |  |  | S/4 only entity |
| `ReferencePurchaseOrderCategory` |  |  | `String(3)` |  | Reference Purchase Order Category |  |  | S/4 only entity |
| `PurchasingDocument` | `BSEG` | `EBELN` | `String(10)` |  | Purchasing Document |  |  |  |
| `PurchasingDocumentItem` | `BSEG` | `EBELP` | `String(5)` |  | Purchasing Doc. Item |  |  |  |
| `AccountAssignmentNumber` |  |  | `String(2)` |  | Account Assignment Number |  |  | S/4 only entity |
| `DocumentItemText` | `BSEG` | `SGTXT` | `String(50)` |  | Item Text |  |  |  |
| `SalesDocument` | `BSEG` | `VBELN` | `String(10)` |  | Sales Document |  |  |  |
| `SalesDocumentItem` | `BSEG` | `VBPOS` | `String(6)` |  | Sales Document Item |  |  |  |
| `Product` |  |  | `String(40)` |  | Product |  |  | S/4 only entity |
| `Plant` | `BSEG` | `WERKS` | `String(4)` |  | Plant |  |  |  |
| `Supplier` | `BSEG` | `LIFNR` | `String(10)` |  | Supplier |  |  |  |
| `Customer` | `BSEG` | `KUNNR` | `String(10)` |  | Customer |  |  |  |
| `ServicesRenderedDate` |  |  | `Date` |  | Serv. Rendered Date |  |  | S/4 only entity |
| `PerformancePeriodStartDate` |  |  | `Date` |  | Per. of Perf. Start |  |  | S/4 only entity |
| `PerformancePeriodEndDate` |  |  | `Date` |  | Per. of Perf. End |  |  | S/4 only entity |
| `ConditionContract` |  |  | `String(10)` |  | Condition Contract |  |  | S/4 only entity |
| `ExchangeRateDate` |  |  | `Date` |  | Translation Date |  |  | S/4 only entity |
| `ComponentBreakdown` |  |  | `String(16)` |  | Component Breakdown |  |  | S/4 only entity |
| `CompBreakdownScaleNumerator` |  |  | `Decimal(23,3)` |  | Component Breakdown Scale Numerator |  |  | S/4 only entity |
| `FinancialAccountType` |  |  | `String(1)` |  | Account Type |  |  | S/4 only entity |
| `SpecialGLCode` |  |  | `String(1)` |  | Special G/L |  |  | S/4 only entity |
| `TaxCode` | `BSEG` | `MWSKZ` | `String(2)` |  | Tax Code |  |  |  |
| `TaxCountry` |  |  | `String(3)` |  | Tax Ctry/Reg. |  |  | S/4 only entity |
| `HouseBank` |  |  | `String(5)` |  | House Bank |  |  | S/4 only entity |
| `HouseBankAccount` |  |  | `String(5)` |  | House Bank Account |  |  | S/4 only entity |
| `IsOpenItemManaged` |  |  | `Boolean` |  | Open Item Management |  |  | S/4 only entity |
| `ClearingDate` | `BSEG` | `AUGDT` | `Date` |  | Clearing Date |  |  |  |
| `ClearingDocFiscalYear` |  |  | `String(4)` |  | Fiscal Year of Clearing JE (Depr.) |  |  | S/4 only entity |
| `ClearingAccountingDocument` | `BSEG` | `AUGBL` | `String(10)` |  | Clearing Journal Entry (Deprecated) |  |  |  |
| `ClearingJournalEntryFiscalYear` |  |  | `String(4)` |  | Fiscal Year of Clearing Journal Entry |  |  | S/4 only entity |
| `ClearingJournalEntry` |  |  | `String(10)` |  | Clearing Journal Entry |  |  | S/4 only entity |
| `ValueDate` |  |  | `Date` |  | Value date |  |  | S/4 only entity |
| `GeneralLedgerAgingScope` |  |  | `String(10)` |  | General Ledger Aging Scope |  |  | S/4 only entity |
| `GeneralLedgerAgingIncrement` |  |  | `String(15)` |  | General Ledger Aging Increment |  |  | S/4 only entity |
| `AssetDepreciationArea` |  |  | `String(2)` |  | Depreciation Area |  |  | S/4 only entity |
| `MasterFixedAsset` | `BSEG` | `ANLN1` | `String(12)` |  | Fixed Asset |  |  |  |
| `FixedAsset` | `BSEG` | `ANLN2` | `String(4)` |  | Asset Subnumber |  |  |  |
| `AssetValueDate` |  |  | `Date` |  | Asset Value Date |  |  | S/4 only entity |
| `AssetTransactionType` |  |  | `String(3)` |  | Asset Transaction Type |  |  | S/4 only entity |
| `AssetAcctTransClassfctn` |  |  | `String(2)` |  | Trans. Type Category |  |  | S/4 only entity |
| `DepreciationFiscalPeriod` |  |  | `String(3)` |  | Depreciation Fiscal Period |  |  | S/4 only entity |
| `GroupMasterFixedAsset` |  |  | `String(12)` |  | Group Asset |  |  | S/4 only entity |
| `GroupFixedAsset` |  |  | `String(4)` |  | Group Asset Subnmbr |  |  | S/4 only entity |
| `AssetClass` |  |  | `String(8)` |  | Asset Class |  |  | S/4 only entity |
| `PartnerMasterFixedAsset` |  |  | `String(12)` |  | Partner Master Fixed Asset |  |  | S/4 only entity |
| `PartnerFixedAsset` |  |  | `String(4)` |  | Partner Fixed Asset |  |  | S/4 only entity |
| `CostEstimate` |  |  | `String(12)` |  | Cost Estimate |  |  | S/4 only entity |
| `InventorySpecialStockValnType` |  |  | `String(1)` |  | Inventory Special Stock Valuation Type |  |  | S/4 only entity |
| `IsSupplierStockValuation` |  |  | `Boolean` |  | Is Supplier Stock Valuation |  |  | S/4 only entity |
| `InventorySpecialStockType` |  |  | `String(1)` |  | Inventory Special Stock Type |  |  | S/4 only entity |
| `InventorySpclStkSalesDocument` |  |  | `String(10)` |  | Inventory Special Stock Sales Document |  |  | S/4 only entity |
| `InventorySpclStkSalesDocItm` |  |  | `String(6)` |  | Inventory Spcl Stock Sales Document Item |  |  | S/4 only entity |
| `InvtrySpclStockWBSElmntIntID` |  |  | `String(8)` |  | Inv. Special Stock WBS Element Int. ID |  |  | S/4 only entity |
| `InventorySpclStockWBSElement` |  |  | `String(24)` |  | Inventory WBS Element |  |  | S/4 only entity |
| `InventorySpecialStockSupplier` |  |  | `String(10)` |  | Inventory Special Stock Supplier |  |  | S/4 only entity |
| `InventoryValuationType` |  |  | `String(10)` |  | Inventory Valuation Type |  |  | S/4 only entity |
| `ValuationArea` |  |  | `String(4)` |  | Valuation Area |  |  | S/4 only entity |
| `MaterialLedgerProcessType` |  |  | `String(4)` |  | Material Ledger Process Type |  |  | S/4 only entity |
| `MaterialLedgerCategory` |  |  | `String(2)` |  | Material Ledger Category |  |  | S/4 only entity |
| `SlsPriceAmountInCoCodeCrcy` |  |  | `Decimal(34,4)` |  | Sales Price Amount in Company Code Crcy | CompanyCodeCurrency |  | S/4 only entity |
| `ProductPriceControl` |  |  | `String(1)` |  | Product Price Control |  |  | S/4 only entity |
| `ProcurementAlternative` |  |  | `String(12)` |  | Procurement Alternative |  |  | S/4 only entity |
| `ProductionProcess` |  |  | `String(12)` |  | Production Process |  |  | S/4 only entity |
| `SenderCompanyCode` |  |  | `String(4)` |  | Company Code in Sender System |  |  | S/4 only entity |
| `SenderGLAccount` |  |  | `String(10)` |  | Sender G/L Account |  |  | S/4 only entity |
| `SenderAccountAssignment` |  |  | `String(30)` |  | Sender Account Assignment |  |  | S/4 only entity |
| `SenderAccountAssignmentType` |  |  | `String(2)` |  | Sender Account Assignment Type |  |  | S/4 only entity |
| `ControllingObject` |  |  | `String(22)` |  | Controlling Object |  |  | S/4 only entity |
| `ControllingKeySubNumber` |  |  | `String(14)` |  | CO subkey |  |  | S/4 only entity |
| `CostOriginGroup` |  |  | `String(4)` |  | Origin Group |  |  | S/4 only entity |
| `OriginSenderObject` |  |  | `String(22)` |  | Origin Sender Object |  |  | S/4 only entity |
| `ControllingDebitCreditCode` |  |  | `String(1)` |  | Controlling Debit Credit Code |  |  | S/4 only entity |
| `OriginCtrlgDebitCreditCode` |  |  | `String(1)` |  | Dr/Cr Ind. (Origin) |  |  | S/4 only entity |
| `ControllingObjectDebitType` |  |  | `String(1)` |  | Controlling Object Debit Type |  |  | S/4 only entity |
| `QuantityIsIncomplete` |  |  | `Boolean` |  | Qty Is Incomplete |  |  | S/4 only entity |
| `OffsettingAccount` |  |  | `String(10)` |  | Offsetting Account |  |  | S/4 only entity |
| `OffsettingAccountType` |  |  | `String(1)` |  | Offsetting Account Type |  |  | S/4 only entity |
| `OffsettingChartOfAccounts` |  |  | `String(4)` |  | Offsetting Chart of Accounts |  | _OffsettingChartOfAccounts | S/4 only entity |
| `LineItemIsCompleted` |  |  | `Boolean` |  | Line Item is Completed |  |  | S/4 only entity |
| `PersonnelNumber` |  |  | `String(8)` |  | Personnel Number |  |  | S/4 only entity |
| `ProfitabilitySegment` |  |  | `String(10)` |  | Profitability Segment |  |  | S/4 only entity |
| `ControllingObjectClass` |  |  | `String(2)` |  | Controlling Object Class |  |  | S/4 only entity |
| `PartnerCompanyCode` |  |  | `String(4)` |  | Partner Company Code |  |  | S/4 only entity |
| `PartnerControllingObjectClass` |  |  | `String(2)` |  | Partner Controlling Object Class |  |  | S/4 only entity |
| `OriginProfitCenter` |  |  | `String(10)` |  | Origin Profit Center |  |  | S/4 only entity |
| `OriginOrder` |  |  | `String(12)` |  | Origin Order |  |  | S/4 only entity |
| `OriginCostCtrActivityType` |  |  | `String(6)` |  | Origin Cost Center Activity Type |  |  | S/4 only entity |
| `OriginCostCenter` |  |  | `String(10)` |  | Origin Cost Center |  |  | S/4 only entity |
| `OriginProduct` |  |  | `String(40)` |  | Origin Product |  |  | S/4 only entity |
| `VarianceOriginGLAccount` |  |  | `String(10)` |  | Origin G/L Account of a Variance |  |  | S/4 only entity |
| `AccountAssignment` |  |  | `String(30)` |  | Account Assignment |  |  | S/4 only entity |
| `AccountAssignmentType` |  |  | `String(2)` |  | Account Assignment Type |  |  | S/4 only entity |
| `CostCtrActivityType` |  |  | `String(6)` |  | Activity Type |  |  | S/4 only entity |
| `OrderID` | `BSEG` | `AUFNR` | `String(12)` |  | Order ID |  |  |  |
| `OrderCategory` |  |  | `String(2)` |  | Order category |  |  | S/4 only entity |
| `WBSElementInternalID` |  |  | `String(8)` |  | WBS Element Internal ID |  |  | S/4 only entity |
| `WBSElement` | `BSEG` | `PS_PSP_PNR` | `String(24)` |  | WBS Element |  |  |  |
| `PartnerWBSElementInternalID` |  |  | `String(8)` |  | Partner WBS Element Internal ID |  |  | S/4 only entity |
| `PartnerWBSElement` |  |  | `String(24)` |  | Partner WBS Element |  |  | S/4 only entity |
| `ProjectInternalID` |  |  | `String(8)` |  | Project Internal ID |  |  | S/4 only entity |
| `Project` |  |  | `String(24)` |  | Project |  |  | S/4 only entity |
| `PartnerProjectInternalID` |  |  | `String(8)` |  | Partner Project Internal ID |  |  | S/4 only entity |
| `PartnerProject` |  |  | `String(24)` |  | Partner Project |  |  | S/4 only entity |
| `OperatingConcern` |  |  | `String(4)` |  | Operating concern |  |  | S/4 only entity |
| `ProjectNetwork` |  |  | `String(12)` |  | Network |  |  | S/4 only entity |
| `RelatedNetworkActivity` |  |  | `String(4)` |  | Related Network Activity |  |  | S/4 only entity |
| `BusinessProcess` |  |  | `String(12)` |  | Business Process |  |  | S/4 only entity |
| `CostObject` |  |  | `String(12)` |  | Cost Object |  |  | S/4 only entity |
| `BillableControl` |  |  | `String(2)` |  | Billable Control |  |  | S/4 only entity |
| `CostAnalysisResource` |  |  | `String(10)` |  | Cost Analysis Resource |  |  | S/4 only entity |
| `CustomerServiceNotification` |  |  | `String(12)` |  | Customer Service Notification |  |  | S/4 only entity |
| `ServiceDocumentType` |  |  | `String(4)` |  | Service Doc. Type |  |  | S/4 only entity |
| `ServiceDocument` |  |  | `String(10)` |  | Service Document |  |  | S/4 only entity |
| `ServiceDocumentItem` |  |  | `String(6)` |  | Service Doc. Item |  |  | S/4 only entity |
| `PartnerServiceDocumentType` |  |  | `String(4)` |  | Partner Service Document Type |  |  | S/4 only entity |
| `PartnerServiceDocument` |  |  | `String(10)` |  | Partner Service Document |  |  | S/4 only entity |
| `PartnerServiceDocumentItem` |  |  | `String(6)` |  | Partner Service Document Item |  |  | S/4 only entity |
| `ServiceContractType` |  |  | `String(4)` |  | Serv. Contract Type |  |  | S/4 only entity |
| `ServiceContract` |  |  | `String(10)` |  | Service Contract |  |  | S/4 only entity |
| `ServiceContractItem` |  |  | `String(6)` |  | Srv Contract Item |  |  | S/4 only entity |
| `BusinessSolutionOrder` |  |  | `String(10)` |  | Solution Order |  |  | S/4 only entity |
| `BusinessSolutionOrderItem` |  |  | `String(6)` |  | Solution Order Item |  |  | S/4 only entity |
| `ProviderContract` |  |  | `String(20)` |  | Provider Contract |  |  | S/4 only entity |
| `ProviderContractItem` |  |  | `String(6)` |  | Provider Contract Item |  |  | S/4 only entity |
| `RevenueAccountingContract` |  |  | `String(14)` |  | Revenue Accounting Contract |  |  | S/4 only entity |
| `PerformanceObligation` |  |  | `String(16)` |  | Performance Obligation |  |  | S/4 only entity |
| `TimeSheetOvertimeCategory` |  |  | `String(4)` |  | Overtime Category |  |  | S/4 only entity |
| `PartnerAccountAssignment` |  |  | `String(30)` |  | Partner Account Assignment |  |  | S/4 only entity |
| `PartnerAccountAssignmentType` |  |  | `String(2)` |  | Partner Account Assignment Type |  |  | S/4 only entity |
| `StstclAccountAssignmentType1` |  |  | `String(2)` |  | Statistical Account Assignment Type 1 |  |  | S/4 only entity |
| `StstclAccountAssignmentType2` |  |  | `String(2)` |  | Statistical Account Assignment Type 2 |  |  | S/4 only entity |
| `StstclAccountAssignmentType3` |  |  | `String(2)` |  | Statistical Account Assignment Type 3 |  |  | S/4 only entity |
| `WorkPackage` |  |  | `String(50)` |  | Plan Item |  |  | S/4 only entity |
| `WorkItem` |  |  | `String(10)` |  | Work Item ID |  |  | S/4 only entity |
| `PartnerCostCtrActivityType` |  |  | `String(6)` |  | Partner Cost Center Activity Type |  |  | S/4 only entity |
| `PartnerOrder` |  |  | `String(12)` |  | Partner Order |  |  | S/4 only entity |
| `PartnerOrderCategory` |  |  | `String(2)` |  | Partner Order Cat. |  |  | S/4 only entity |
| `PartnerSalesDocument` |  |  | `String(10)` |  | Partner Sales Doc. |  |  | S/4 only entity |
| `PartnerSalesDocumentItem` |  |  | `String(6)` |  | Partner Sales Document Item |  |  | S/4 only entity |
| `PartnerProjectNetwork` |  |  | `String(12)` |  | Partner Project Network |  |  | S/4 only entity |
| `PartnerProjectNetworkActivity` |  |  | `String(4)` |  | Partner Project Network Activity |  |  | S/4 only entity |
| `PartnerBusinessProcess` |  |  | `String(12)` |  | Partner Business Process |  |  | S/4 only entity |
| `PartnerCostObject` |  |  | `String(12)` |  | Partner Cost Object |  |  | S/4 only entity |
| `ControllingDocumentItem` |  |  | `String(3)` |  | Controlling Doc Item |  |  | S/4 only entity |
| `VarianceOriginGroup` |  |  | `String(4)` |  | Varc. Origin Group |  |  | S/4 only entity |
| `BillingDocumentType` |  |  | `String(4)` |  | Billing Type |  |  | S/4 only entity |
| `SalesOrganization` |  |  | `String(4)` |  | Sales Organization |  |  | S/4 only entity |
| `DistributionChannel` |  |  | `String(2)` |  | Distribution Channel |  |  | S/4 only entity |
| `OrganizationDivision` |  |  | `String(2)` |  | Division |  |  | S/4 only entity |
| `SoldProduct` |  |  | `String(40)` |  | Product Sold |  |  | S/4 only entity |
| `SoldProductGroup` |  |  | `String(9)` |  | Product Sold Group |  |  | S/4 only entity |
| `CustomerGroup` |  |  | `String(2)` |  | Customer Group |  |  | S/4 only entity |
| `CustomerSupplierCountry` |  |  | `String(3)` |  | Customer or Supplier Country/Region |  |  | S/4 only entity |
| `CustomerSupplierIndustry` |  |  | `String(4)` |  | Customer Supplier Industry |  |  | S/4 only entity |
| `SalesDistrict` |  |  | `String(6)` |  | Sales District |  |  | S/4 only entity |
| `BillToParty` |  |  | `String(10)` |  | Bill-to Party |  |  | S/4 only entity |
| `ShipToParty` |  |  | `String(10)` |  | Ship-to Party |  |  | S/4 only entity |
| `CustomerSupplierCorporateGroup` |  |  | `String(10)` |  | Customer Supplier Corporate Group |  |  | S/4 only entity |
| `CashLedgerCompanyCode` |  |  | `String(4)` |  | Cash Origin CoCode |  |  | S/4 only entity |
| `CashLedgerAccount` |  |  | `String(10)` |  | Cash Origin Account |  | _CashLedgerAccount | S/4 only entity |
| `FinancialManagementArea` |  |  | `String(4)` |  | FM Area |  |  | S/4 only entity |
| `CommitmentItem` |  |  | `String(24)` |  | Commitment Item |  |  | S/4 only entity |
| `FundsCenter` |  |  | `String(16)` |  | Funds Center |  |  | S/4 only entity |
| `FundedProgram` |  |  | `String(24)` |  | Funded Program |  |  | S/4 only entity |
| `Fund` |  |  | `String(10)` |  | Fund |  |  | S/4 only entity |
| `GrantID` |  |  | `String(20)` |  | Grant |  |  | S/4 only entity |
| `BudgetPeriod` |  |  | `String(10)` |  | Budget Period |  |  | S/4 only entity |
| `PartnerFund` |  |  | `String(10)` |  | Partner Fund |  |  | S/4 only entity |
| `PartnerGrant` |  |  | `String(20)` |  | Partner Grant |  |  | S/4 only entity |
| `PartnerBudgetPeriod` |  |  | `String(10)` |  | Partner Budget Period |  |  | S/4 only entity |
| `PubSecBudgetAccount` |  |  | `String(10)` |  | Budget Account |  |  | S/4 only entity |
| `PubSecBudgetAccountCoCode` |  |  | `String(4)` |  | Company Code for Budget Account |  |  | S/4 only entity |
| `PubSecBudgetCnsmpnDate` |  |  | `Date` |  | Budget Consumption Date |  |  | S/4 only entity |
| `PubSecBudgetCnsmpnFsclPeriod` |  |  | `String(3)` |  | Posting Period for Budget Consumption |  |  | S/4 only entity |
| `PubSecBudgetCnsmpnFsclYear` |  |  | `String(4)` |  | Year of Budget Consumption |  |  | S/4 only entity |
| `PubSecBudgetIsRelevant` |  |  | `Boolean` |  | Budget-Relevant |  |  | S/4 only entity |
| `PubSecBudgetCnsmpnType` |  |  | `String(2)` |  | Budget Consumption Type |  |  | S/4 only entity |
| `PubSecBudgetCnsmpnAmtType` |  |  | `String(4)` |  | Amount Type for Budget Consumption |  |  | S/4 only entity |
| `SponsoredProgram` |  |  | `String(20)` |  | Sponsored Program |  |  | S/4 only entity |
| `SponsoredClass` |  |  | `String(20)` |  | Sponsored Class |  |  | S/4 only entity |
| `GteeMBudgetValidityNumber` |  |  | `String(3)` |  | Bdgt Validty No. |  |  | S/4 only entity |
| `EarmarkedFundsDocument` |  |  | `String(10)` |  | Earmarked Funds Document |  |  | S/4 only entity |
| `EarmarkedFundsDocumentItem` |  |  | `String(3)` |  | Earmarked Funds Document Item |  |  | S/4 only entity |
| `FinancialServicesProductGroup` |  |  | `String(10)` |  | Financial Services Product Group |  |  | S/4 only entity |
| `FinancialServicesBranch` |  |  | `String(10)` |  | Financial Services Branch |  |  | S/4 only entity |
| `FinancialDataSource` |  |  | `String(10)` |  | Financial Data Source |  |  | S/4 only entity |
| `JointVenture` |  |  | `String(6)` |  | Joint venture |  |  | S/4 only entity |
| `JointVentureEquityGroup` |  |  | `String(3)` |  | Joint Venture Equity Group |  |  | S/4 only entity |
| `JointVentureCostRecoveryCode` |  |  | `String(2)` |  | Joint Venture Cost Recovery Code |  |  | S/4 only entity |
| `JointVenturePartner` |  |  | `String(10)` |  | Joint Venture Partner |  |  | S/4 only entity |
| `JointVentureBillingType` |  |  | `String(2)` |  | Joint Venture Billing Type |  |  | S/4 only entity |
| `JointVentureEquityType` |  |  | `String(3)` |  | Joint Venture Equity Type |  |  | S/4 only entity |
| `JointVentureProductionDate` |  |  | `Date` |  | Joint Venture Production Date |  |  | S/4 only entity |
| `JointVentureBillingDate` |  |  | `Date` |  | Joint Venture Billing Date |  |  | S/4 only entity |
| `JointVentureOperationalDate` |  |  | `Date` |  | Joint Venture Operational Date |  |  | S/4 only entity |
| `CutbackRun` |  |  | `Timestamp` |  | Cutback Run |  |  | S/4 only entity |
| `JointVentureAccountingActivity` |  |  | `String(2)` |  | Joint Venture Accounting Activity |  |  | S/4 only entity |
| `PartnerVenture` |  |  | `String(6)` |  | PartnerVenture |  |  | S/4 only entity |
| `PartnerEquityGroup` |  |  | `String(3)` |  | Partner Equity Group |  |  | S/4 only entity |
| `SenderCostRecoveryCode` |  |  | `String(2)` |  | Sender Cost Recovery Code |  |  | S/4 only entity |
| `CutbackAccount` |  |  | `String(10)` |  | Cutback Account |  |  | S/4 only entity |
| `CutbackCostObject` |  |  | `String(22)` |  | Cutback Cost Object |  |  | S/4 only entity |
| `REBusinessEntity` |  |  | `String(8)` |  | RE Business Entity |  |  | S/4 only entity |
| `RealEstateBuilding` |  |  | `String(8)` |  | Real Estate Building |  |  | S/4 only entity |
| `RealEstateProperty` |  |  | `String(8)` |  | Real Estate Property |  |  | S/4 only entity |
| `RERentalObject` |  |  | `String(8)` |  | RE Rental Object |  |  | S/4 only entity |
| `RealEstateContract` |  |  | `String(13)` |  | Real Estate Contract |  |  | S/4 only entity |
| `REServiceChargeKey` |  |  | `String(4)` |  | RE Service Charge Key |  |  | S/4 only entity |
| `RESettlementUnitID` |  |  | `String(5)` |  | RE Settlement Unit |  |  | S/4 only entity |
| `SettlementReferenceDate` |  |  | `Date` |  | Settlement Reference Date |  |  | S/4 only entity |
| `REPartnerBusinessEntity` |  |  | `String(8)` |  | RE Partner Business Entity |  |  | S/4 only entity |
| `RealEstatePartnerBuilding` |  |  | `String(8)` |  | Real Estate Partner Building |  |  | S/4 only entity |
| `RealEstatePartnerProperty` |  |  | `String(8)` |  | Real Estate Partner Property |  |  | S/4 only entity |
| `REPartnerRentalObject` |  |  | `String(8)` |  | RE Partner Rental Object |  |  | S/4 only entity |
| `RealEstatePartnerContract` |  |  | `String(13)` |  | Real Estate Partner Contract |  |  | S/4 only entity |
| `REPartnerServiceChargeKey` |  |  | `String(4)` |  | RE Partner Service Charge Key |  |  | S/4 only entity |
| `REPartnerSettlementUnitID` |  |  | `String(5)` |  | RE Partner Settlement Unit |  |  | S/4 only entity |
| `PartnerSettlementReferenceDate` |  |  | `Date` |  | Ptnr. Reference Date |  |  | S/4 only entity |
| `AccrualObjectType` |  |  | `String(4)` |  | Accrual Object Type |  |  | S/4 only entity |
| `AccrualObjectLogicalSystem` |  |  | `String(10)` |  | Logical Syst. AcrObj |  |  | S/4 only entity |
| `AccrualObject` |  |  | `String(32)` |  | Accrual Object |  |  | S/4 only entity |
| `AccrualSubobject` |  |  | `String(32)` |  | Accrual Subobject |  |  | S/4 only entity |
| `AccrualItemType` |  |  | `String(11)` |  | Accrual Item Type |  |  | S/4 only entity |
| `AccrualReferenceObject` |  |  | `String(32)` |  | Accrual Reference Object |  |  | S/4 only entity |
| `AccrualValueDate` |  |  | `Date` |  | Accrual Value Date |  |  | S/4 only entity |
| `FinancialValuationObjectType` |  |  | `String(4)` |  | Financial Valuation Object Type |  |  | S/4 only entity |
| `FinancialValuationObject` |  |  | `String(32)` |  | Financial Valuation Object |  |  | S/4 only entity |
| `FinancialValuationSubobject` |  |  | `String(32)` |  | Financial Valuation Subobject |  |  | S/4 only entity |
| `NetDueDate` |  |  | `Date` |  | Net Due Date |  |  | S/4 only entity |
| `CreditRiskClass` |  |  | `String(3)` |  | Credit Risk Class |  |  | S/4 only entity |
| `WorkCenterInternalID` |  |  | `String(8)` |  | Object ID |  |  | S/4 only entity |
| `OrderOperation` |  |  | `String(4)` |  | Order Operation |  |  | S/4 only entity |
| `OrderItem` |  |  | `String(4)` |  | Order item number |  |  | S/4 only entity |
| `PartnerOrderItem` |  |  | `String(4)` |  | Partner Order item |  |  | S/4 only entity |
| `OrderSuboperation` |  |  | `String(4)` |  | Order Suboperation |  |  | S/4 only entity |
| `Equipment` |  |  | `String(18)` |  | Equipment |  |  | S/4 only entity |
| `FunctionalLocation` |  |  | `String(30)` |  | Functional Location |  |  | S/4 only entity |
| `Assembly` |  |  | `String(40)` |  | Assembly |  |  | S/4 only entity |
| `MaintenanceActivityType` |  |  | `String(3)` |  | MaintActivityType |  |  | S/4 only entity |
| `MaintenanceOrderPlanningCode` |  |  | `String(1)` |  | Order planning ind. |  |  | S/4 only entity |
| `MaintPriorityType` |  |  | `String(2)` |  | Priority Type |  |  | S/4 only entity |
| `MaintPriority` |  |  | `String(1)` |  | Priority |  |  | S/4 only entity |
| `SuperiorOrder` |  |  | `String(12)` |  | Superior Order |  |  | S/4 only entity |
| `ProductGroup` |  |  | `String(9)` |  | Product Group |  |  | S/4 only entity |
| `MaintenanceOrderIsPlanned` |  |  | `Boolean` |  | Planned Parts/Work |  |  | S/4 only entity |
| `OriginOrderOperation` |  |  | `String(4)` |  | Origin Order Operation |  |  | S/4 only entity |
| `JrnlEntryItemMigrationSource` |  |  | `String(1)` |  | Journal Entry Item Migration Source |  |  | S/4 only entity |
| `USFedCommitmentString` |  |  | `String(62)` |  | Commitment string |  |  | S/4 only entity |
| `USFedBudgetaryLedgerStatus` |  |  | `String(5)` |  | BL Status |  |  | S/4 only entity |
| `USFedFiscalYearBlank` |  |  | `String(4)` |  | FMA Fiscal Year |  |  | S/4 only entity |
| `USFedObjectClass` |  |  | `String(24)` |  | Obj Class US Fed |  |  | S/4 only entity |
| `USFedStandardGLAccount` |  |  | `String(6)` |  | SGL account |  |  | S/4 only entity |
| `USFedAgencyLocationCode` |  |  | `String(8)` |  | Agency Location Code |  |  | S/4 only entity |
| `USFedApplOfSecdrySrceFunds` |  |  | `String(16)` |  | Application of Funds |  |  | S/4 only entity |
| `USFedFundType` |  |  | `String(6)` |  | Fund Type |  |  | S/4 only entity |
| `USFedPaymentOffice` |  |  | `String(5)` |  | Payment Office |  |  | S/4 only entity |
| `USFedAgency` |  |  | `String(3)` |  | Agency Identifier |  |  | S/4 only entity |
| `USFedMainAccount` |  |  | `String(4)` |  | Main Account |  |  | S/4 only entity |
| `USFedSubAccount` |  |  | `String(3)` |  | Sub account |  |  | S/4 only entity |
| `USFedBeginPerdOfAvailability` |  |  | `String(4)` |  | Begin Prd of Avail |  |  | S/4 only entity |
| `USFedEndPerdOfAvaily` |  |  | `String(4)` |  | Ending Prd of Avail |  |  | S/4 only entity |
| `USFedAvailabilityType` |  |  | `String(1)` |  | Avail Type Code |  |  | S/4 only entity |
| `USFedBusEventTypeCode` |  |  | `String(10)` |  | Business Evt Typ Cd |  |  | S/4 only entity |
| `USFedSubLevelPrefix` |  |  | `String(2)` |  | Sublevel Prefix |  |  | S/4 only entity |
| `USFedAuthorityType` |  |  | `String(1)` |  | Authority Type |  |  | S/4 only entity |
| `USFedApportionmentCategory` |  |  | `String(1)` |  | Apportionment Cat |  |  | S/4 only entity |
| `USFedApprtmtCatDetailPgmCode` |  |  | `String(4)` |  | Category B Detail |  |  | S/4 only entity |
| `USFedYearOfBdgtAuthorityCode` |  |  | `String(4)` |  | Yr of Budget Auth |  |  | S/4 only entity |
| `USFedAvailabilityTimeType` |  |  | `String(1)` |  | Availability Time |  |  | S/4 only entity |
| `USFedPriorYearAdjmtCode` |  |  | `String(1)` |  | Prior Year Adj. Cd |  |  | S/4 only entity |
| `USFedBudgetEnforcementActCat` |  |  | `String(1)` |  | BEA Category |  |  | S/4 only entity |
| `USFedReductionType` |  |  | `String(3)` |  | Reduction Type |  |  | S/4 only entity |
| `USFedBorrowingSource` |  |  | `String(1)` |  | Borrowing Source |  |  | S/4 only entity |
| `USFedRptgYearForCohort` |  |  | `String(4)` |  | Year Cohort |  |  | S/4 only entity |
| `USFedAllocTransfAgencyID` |  |  | `String(3)` |  | Alloc Transfr Agency |  |  | S/4 only entity |
| `USFedReimbursable` |  |  | `String(1)` |  | Reimbursable |  |  | S/4 only entity |
| `USFedBudgetImpact` |  |  | `String(1)` |  | Budget Impact |  |  | S/4 only entity |
| `USFedDisasterEmergencyFundCode` |  |  | `String(3)` |  | Disastr Emer Fnd Cde |  |  | S/4 only entity |
| `USFedPgmReportingCat` |  |  | `String(3)` |  | Prog.Rpt.Category |  |  | S/4 only entity |
| `USFedCustodialIndicator` |  |  | `String(1)` |  | Custodial indicator |  |  | S/4 only entity |
| `USFedPostingSequenceNumber` |  |  | `String(10)` |  | Sequence Nbr |  |  | S/4 only entity |
| `USFedExchangeIndicator` |  |  | `String(1)` |  | Exchange Indicator |  |  | S/4 only entity |
| `USFedFederalNonFederalCode` |  |  | `String(1)` |  | Federal/Nonfederal |  |  | S/4 only entity |
| `USFedTradingPartnerAgency` |  |  | `String(3)` |  | Agency ID (TP) |  |  | S/4 only entity |
| `USFedTrdgPartMainAccount` |  |  | `String(4)` |  | Main Account (TP) |  |  | S/4 only entity |
| `USFedTrdgPartSubAccount` |  |  | `String(3)` |  | Subaccount (TP) |  |  | S/4 only entity |
| `USFedTrdgPartBeginPerdOfAvaily` |  |  | `String(4)` |  | Begin Prd Avail (TP) |  |  | S/4 only entity |
| `USFedTrdgPartEndPerdOfAvaily` |  |  | `String(4)` |  | End Prd Avail (TP) |  |  | S/4 only entity |
| `USFedAllocTransfAgencyTrdgPart` |  |  | `String(3)` |  | AllcTrnsfrAgncy (TP) |  |  | S/4 only entity |
| `USFedTrdgPartAvailabilityType` |  |  | `String(1)` |  | Avail Type Code (TP) |  |  | S/4 only entity |
| `USFedTrdgPartBusEventTypeCode` |  |  | `String(10)` |  | BusinessEvtTypCd(TP) |  |  | S/4 only entity |
| `USFedTrdgPartSubLevelPrefix` |  |  | `String(2)` |  | Sublevel Prefix (TP) |  |  | S/4 only entity |
| `USFedPgmActivityReportingKey` |  |  | `String(15)` |  | Prog Act Rep Key |  |  | S/4 only entity |
| `GeneralLedgerAccountLineItemOID` |  |  | `String(128)` |  |  |  |  | S/4 only entity |


## Entity: `GeneralLedgerAccountText`

- **ABAP Name:** `I_GLAccountTextRawData`
- **Label:** General Ledger Account - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `ChartOfAccounts` | `T001` | `KTOPL` | `String(4)` | Y | Chart of Accounts |  | _ChartOfAccounts |  |
| `GLAccount` |  |  | `String(10)` | Y | G/L Account |  |  | S/4 only entity |
| `Language` |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity |
| `GLAccountName` |  |  | `String(20)` |  | G/L Account Name |  |  | S/4 only entity |
| `GLAccountLongName` |  |  | `String(50)` |  | G/L Account Long Name |  |  | S/4 only entity |
| `LastChangeDateTime` |  |  | `DateTime` |  | Time Stamp |  |  | S/4 only entity |


## Entity: `GeneralLedgerAccountTypeText`

- **ABAP Name:** `I_GLAccountTypeText`
- **Label:** G/L Account Type - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `GLAccountType` |  |  | `String(10)` | Y | Lower Value |  |  | S/4 only entity |
| `Language` |  |  | `String(2)` | Y | Lang. |  |  | S/4 only entity |
| `GLAccountTypeName` |  |  | `String(60)` |  | Short Description |  |  | S/4 only entity |
| `DomainValue` |  |  | `String(10)` |  | Lower Value |  |  | S/4 only entity |


## Entity: `OperatingGeneralLedgerAccount`

- **ABAP Name:** `I_GLAccountInCompanyCode`
- **Label:** General Ledger Account in Company Code
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `GLAccount` |  |  | `String(10)` | Y | G/L Account |  |  | S/4 only entity |
| `CompanyCode` | `T001` | `BUKRS` | `String(4)` | Y | Company Code |  |  |  |
| `AuthorizationGroup` |  |  | `String(4)` |  | Authorization |  |  | S/4 only entity |
| `AccountingClerk` |  |  | `String(2)` |  | Clerk Abbrev. |  |  | S/4 only entity |
| `LastInterestCalcRunDate` |  |  | `Date` |  | Last Int. Calc. |  |  | S/4 only entity |
| `CreationDate` |  |  | `Date` |  | Created On |  |  | S/4 only entity |
| `CreatedByUser` |  |  | `String(12)` |  | Created By |  |  | S/4 only entity |
| `LastChangeDateTime` |  |  | `DateTime` |  | Time Stamp |  |  | S/4 only entity |
| `PlanningLevel` |  |  | `String(2)` |  | Planning Level |  |  | S/4 only entity |
| `HouseBank` |  |  | `String(5)` |  | House Bank |  |  | S/4 only entity |
| `HouseBankAccount` |  |  | `String(5)` |  | Account ID |  |  | S/4 only entity |
| `ExchRateDifferencesAccountDetn` |  |  | `String(4)` |  | E/R Diff. Key |  |  | S/4 only entity |
| `ReconciliationAccountType` |  |  | `String(1)` |  | Reconcil. ID |  |  | S/4 only entity |
| `TaxCategory` |  |  | `String(2)` |  | Tax Category |  |  | S/4 only entity |
| `InterestCalculationCode` |  |  | `String(2)` |  | Interest Indicator |  |  | S/4 only entity |
| `GLAccountCurrency` |  |  | `String(5)` |  | Account Currency |  |  | S/4 only entity |
| `ReconciliationAcctIsChangeable` |  |  | `Boolean` |  | Rec.Act Ready |  |  | S/4 only entity |
| `IsManagedExternally` |  |  | `Boolean` |  | Is Managed Ext. |  |  | S/4 only entity |
| `IsAutomaticallyPosted` |  |  | `Boolean` |  | Auto. Posting |  |  | S/4 only entity |
| `LineItemDisplayIsEnabled` |  |  | `Boolean` |  | Line Items |  |  | S/4 only entity |
| `SupplementIsAllowed` |  |  | `Boolean` |  | Supplement |  |  | S/4 only entity |
| `IsOpenItemManaged` |  |  | `Boolean` |  | OI Management |  |  | S/4 only entity |
| `InterestCalculationDate` |  |  | `Date` |  | Last Key Date |  |  | S/4 only entity |
| `IntrstCalcFrequencyInMonths` |  |  | `String(2)` |  | Int.Calc.Freq. |  |  | S/4 only entity |
| `AcctgDocItmDisplaySequenceRule` |  |  | `String(3)` |  | Sort key |  |  | S/4 only entity |
| `AlternativeGLAccount` |  |  | `String(10)` |  | Alternative G/L Account |  |  | S/4 only entity |
| `JointVentureRecoveryCode` |  |  | `String(2)` |  | Recovery Indicator |  |  | S/4 only entity |
| `CommitmentItem` |  |  | `String(14)` |  | Commitment item |  |  | S/4 only entity |
| `CommitmentItemShortID` |  |  | `String(14)` |  | Commitment Item Short ID |  |  | S/4 only entity |
| `TaxCodeIsRequired` |  |  | `Boolean` |  | Pstg w/o tax allowed |  |  | S/4 only entity |
| `BalanceHasLocalCurrency` |  |  | `Boolean` |  | Balances in LC |  |  | S/4 only entity |
| `ValuationGroup` |  |  | `String(10)` |  | Valuation Group |  |  | S/4 only entity |
| `APARToleranceGroup` |  |  | `String(4)` |  | Tolerance Group |  |  | S/4 only entity |
| `AccountIsBlockedForPosting` |  |  | `Boolean` |  | Posting Block |  |  | S/4 only entity |
| `AccountIsMarkedForDeletion` |  |  | `Boolean` |  | Deletion Flag |  |  | S/4 only entity |
| `ClearingIsLedgerGroupSpecific` |  |  | `Boolean` |  | OI Mgmt by LedgerGrp |  |  | S/4 only entity |
| `CashPlanningGroup` |  |  | `String(10)` |  | Planning Group |  |  | S/4 only entity |
| `IsCashFlowAccount` |  |  | `Boolean` |  | Rel.Cash Flow |  |  | S/4 only entity |
| `GLAcctInflationKey` |  |  | `String(8)` |  | Inflation key |  |  | S/4 only entity |
| `FieldStatusGroup` |  |  | `String(4)` |  | Field status group |  |  | S/4 only entity |
| `MultiCurrencyAccountingCode` |  |  | `String(5)` |  | MCA Key |  |  | S/4 only entity |
| `IsExtendedOpenItemManaged` |  |  | `Boolean` |  | Extended OI Mgmt |  |  | S/4 only entity |


## Entity: `SemanticTag`

- **ABAP Name:** `I_SemanticTag`
- **Label:** Semantic Tag
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `SemanticTag` |  |  | `String(10)` | Y | Semantic Tag |  |  | S/4 only entity |
| `ParentSemanticTag` |  |  | `String(10)` |  | Parent Semantic Tag |  |  | S/4 only entity |
| `SemanticTagGroup` |  |  | `String(4)` |  | Semantic Tag Group |  |  | S/4 only entity |


## Entity: `SemanticTagFunctionalArea`

- **ABAP Name:** `I_SemTagFuncArea`
- **Label:** Functional Area with Semantic Tag
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `GLAccountHierarchy` |  |  | `String(42)` | Y | FSV |  | _Hierarchy | S/4 only entity |
| `HierarchyNode` |  |  | `String(50)` | Y | Node |  |  | S/4 only entity |
| `SemanticTag` |  |  | `String(10)` | Y | Semantic Tag |  | _SemanticTag | S/4 only entity |
| `ValidityEndDate` |  |  | `Date` | Y | Valid To |  |  | S/4 only entity |
| `ValidityStartDate` |  |  | `Date` | Y | Valid From |  |  | S/4 only entity |
| `FunctionalArea` |  |  | `String(16)` | Y | Functional Area |  |  | S/4 only entity |


## Entity: `SemanticTagGeneralLedger`

- **ABAP Name:** `I_SemTagGLAccount`
- **Label:** G/L Account with Semantic Tag
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `GLAccountHierarchy` |  |  | `String(42)` | Y | FSV |  | _Hierarchy | S/4 only entity |
| `HierarchyNode` |  |  | `String(50)` | Y | Node |  |  | S/4 only entity |
| `SemanticTag` |  |  | `String(10)` | Y | Semantic Tag |  | _SemanticTag | S/4 only entity |
| `ValidityEndDate` |  |  | `Date` | Y | Valid To |  |  | S/4 only entity |
| `ValidityStartDate` |  |  | `Date` | Y | Valid From |  |  | S/4 only entity |
| `ChartOfAccounts` | `T001` | `KTOPL` | `String(4)` | Y | Chart of Accounts |  | _ChartOfAccounts |  |
| `GLAccount` |  |  | `String(10)` | Y | G/L Account |  | _GLAccountInChartOfAccounts | S/4 only entity |
| `FunctionalAreaIsUsed` |  |  | `Boolean` |  | Functional Area |  |  | S/4 only entity |
| `IsFunctionalAreaPermitted` |  |  | `Boolean` |  | Fun.Area Perm. |  |  | S/4 only entity |


## Entity: `SemanticTagLeafNode`

- **ABAP Name:** `I_SemanticTagLeafNode`
- **Label:** Hierarchy Leaf Node with Semantic Tag
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `GLAccountHierarchy` |  |  | `String(42)` | Y | Hierarchy ID |  | _Hierarchy | S/4 only entity |
| `HierarchyNode` |  |  | `String(50)` | Y | Node |  | _GLAccountHierarchyNode | S/4 only entity |
| `ValidityEndDate` |  |  | `Date` | Y | Valid To |  |  | S/4 only entity |
| `SemanticTag` |  |  | `String(10)` | Y | Semantic Tag |  | _SemanticTag | S/4 only entity |
| `ValidityStartDate` |  |  | `Date` |  | Valid From |  |  | S/4 only entity |
| `ChartOfAccounts` | `T001` | `KTOPL` | `String(4)` |  | Chart of Accounts |  |  |  |
| `GLAccount` |  |  | `String(10)` |  | G/L Account |  |  | S/4 only entity |
| `FunctionalArea` |  |  | `String(16)` |  | Functional Area |  |  | S/4 only entity |


## Entity: `SemanticTagText`

- **ABAP Name:** `I_SemanticTagText`
- **Label:** Semantic Tag - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `Language` |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity |
| `SemanticTag` |  |  | `String(10)` | Y | Semantic Tag |  |  | S/4 only entity |
| `SemanticTagName` |  |  | `String(20)` |  | Semantic Tag Name |  |  | S/4 only entity |
