# GeneralLedgerAccount

> Source file: `sap-s4com-GeneralLedgerAccount-v1.json`


## Entity: `ChartOfAccounts`

- **ABAP CDS Name:** `I_ChartOfAccounts`
- **Label:** Chart Of Accounts
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** T004

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `ChartOfAccounts` |  |  |  |  |  | `String(4)` | Y | Chart of Accounts |  |  |
| `CorporateGroupChartOfAccounts` |  |  |  |  |  | `String(4)` |  | Group Chart of Accts |  |  |
| `ChartOfAcctsIsBlocked` |  |  |  |  |  | `Boolean` |  | Blocked |  |  |
| `MaintenanceLanguage` |  |  |  |  |  | `String(2)` |  | Maint.Language |  |  |


## Entity: `ChartOfAccountsText`

- **ABAP CDS Name:** `I_ChartOfAccountsText`
- **Label:** Chart Of Accounts - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** T004T

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `ChartOfAccounts` |  |  |  |  |  | `String(4)` | Y | Chart of Accounts |  |  |
| `Language` |  |  |  |  |  | `String(2)` | Y | Language Key |  |  |
| `ChartOfAccountsName` |  |  |  |  |  | `String(50)` |  | Chart of Accounts Description |  |  |


## Entity: `FinancialStatementHierNode`

- **ABAP CDS Name:** `I_FinancialStatementHierNode`
- **Label:** Financial Statement Hierarchy Node
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** FINSC_FS_ITEM

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `FinancialStatementHierarchy` |  |  |  |  |  | `String(42)` | Y | Hierarchy ID |  |  |
| `HierarchyNode` |  |  |  |  |  | `String(50)` | Y | Node |  |  |
| `ValidityEndDate` |  |  |  |  |  | `Date` | Y | Valid To |  |  |
| `ValidityStartDate` |  |  |  |  |  | `Date` |  | Validity Start Date |  |  |
| `ParentNode` |  |  |  |  |  | `String(50)` |  | Par. Node |  |  |
| `HierarchyVersion` |  |  |  |  |  | `String(15)` |  | Version |  |  |
| `FinancialStatementLeafItem` |  |  |  |  |  | `String(50)` |  | Node |  |  |
| `SequenceNumber` |  |  |  |  |  | `String(56)` |  |  |  |  |
| `SignIsInverted` |  |  |  |  |  | `Boolean` |  | Attribute Value |  |  |
| `ChartOfAccounts` |  |  |  |  |  | `String(12)` |  | Node Class |  |  |
| `FinancialStatementNodeType` |  |  |  |  |  | `String(1)` |  | Node Type |  |  |
| `FinStmntNodeFormattedID` |  |  |  |  |  | `String(32)` |  | Node for Extraction |  |  |
| `HierarchyNodeVal` |  |  |  |  |  | `String(40)` |  | Value |  |  |
| `HierarchyNodeSequence` |  |  |  |  |  | `String(6)` |  | Sequence Number |  |  |
| `HierarchyLevel` |  |  |  |  |  | `String(6)` |  | Hierarchy Level |  |  |
| `DebitCreditCode` |  |  |  |  |  | `String(1)` |  | Balance |  |  |


## Entity: `FinancialStatementHierNodeText`

- **ABAP CDS Name:** `I_FinancialStatementHierNodeT`
- **Label:** Financial Statement Hierarchy Node - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** FINSC_FS_ITEM

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `FinancialStatementHierarchy` |  |  |  |  |  | `String(42)` | Y | Hierarchy ID |  |  |
| `HierarchyNode` |  |  |  |  |  | `String(50)` | Y | Node |  |  |
| `ValidityEndDate` |  |  |  |  |  | `Date` | Y | Valid To |  |  |
| `Language` |  |  |  |  |  | `String(2)` | Y | Language Key |  |  |
| `HierarchyNodeText` |  |  |  |  |  | `String(50)` |  | Description |  |  |
| `HierarchyNodeShortText` |  |  |  |  |  | `String(20)` |  |  |  |  |
| `ValidityStartDate` |  |  |  |  |  | `Date` |  | Valid From |  |  |
| `FinStmntNodeFormattedID` |  |  |  |  |  | `String(32)` |  | Node for Extraction |  |  |


## Entity: `FinancialStatementHierText`

- **ABAP CDS Name:** `I_FinancialStatementHierT`
- **Label:** Financial Statement Hierarchy - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** FINSC_FS_ITEM

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `FinancialStatementHierarchy` |  |  |  |  |  | `String(42)` | Y | Hierarchy ID |  |  |
| `ValidityEndDate` |  |  |  |  |  | `Date` | Y | Valid To |  |  |
| `Language` |  |  |  |  |  | `String(2)` | Y | Language Key |  |  |
| `ValidityStartDate` |  |  |  |  |  | `Date` |  | Valid From |  |  |
| `FinancialStmntHierarchyName` |  |  |  |  |  | `String(50)` |  | Financial Statement Description |  |  |


## Entity: `FinancialStatementHierarchy`

- **ABAP CDS Name:** `I_FinancialStatementHier`
- **Label:** Financial Statement Hierarchy
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** FINSC_FS_ITEM

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `FinancialStatementHierarchy` |  |  |  |  |  | `String(42)` | Y | Hierarchy ID |  |  |
| `ValidityEndDate` |  |  |  |  |  | `Date` | Y | Validity End Date |  |  |
| `ValidityStartDate` |  |  |  |  |  | `Date` |  | Validity Start Date |  |  |
| `HierarchyType` |  |  |  |  |  | `String(4)` |  | Hierarchy Type |  |  |
| `LastChangedByUser` |  |  |  |  |  | `String(12)` |  | Last Changed By |  |  |
| `LastChangeTime` |  |  |  |  |  | `DateTime` |  | Updated At |  |  |
| `LastChangeDateTime` |  |  |  |  |  | `DateTime` |  | Updated At |  |  |
| `ChartOfAccounts` |  |  |  |  |  | `String(80)` |  | Char80 |  |  |
| `FinancialStatementAssetsItem` |  |  |  |  |  | `String(80)` |  | Char80 |  |  |
| `FinStatementLiabilitiesItem` |  |  |  |  |  | `String(80)` |  | Char80 |  |  |
| `FinancialStatementNetLossItem` |  |  |  |  |  | `String(80)` |  | Char80 |  |  |
| `FinStatementNetProfitItem` |  |  |  |  |  | `String(80)` |  | Char80 |  |  |
| `FinStatementProfitAndLossItem` |  |  |  |  |  | `String(80)` |  | Char80 |  |  |
| `FinancialStatementOrphansItem` |  |  |  |  |  | `String(80)` |  | Char80 |  |  |
| `FinancialStatementNotesItem` |  |  |  |  |  | `String(80)` |  | Char80 |  |  |
| `GroupChartOfAccountIsUsed` |  |  |  |  |  | `Boolean` |  | Char80 |  |  |
| `FunctionalAreaIsUsed` |  |  |  |  |  | `Boolean` |  | Char80 |  |  |


## Entity: `GLAccountHierNodeBySemanticTag`

- **ABAP CDS Name:** `I_GLAccountHierNodeBySemTag`
- **Label:** GLAccount Hierarchy Node By Semantic Tag
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `GLAccountHierarchy` |  |  |  |  |  | `String(42)` | Y | Hierarchy ID |  |  |
| `HierarchyNode` |  |  |  |  |  | `String(50)` | Y | Node |  |  |
| `SemanticTag` |  |  |  |  |  | `String(10)` | Y | Semantic Tag |  |  |
| `HierarchyNodeType` |  |  |  |  |  | `String(30)` |  | Field Name |  |  |


## Entity: `GLAccountHierarchyNode`

- **ABAP CDS Name:** `I_GLAccountHierarchyNode`
- **Label:** G/L Account Hierarchy Node
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** FINSC_HIER, FINSC_HIER_T

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `GLAccountHierarchy` |  |  |  |  |  | `String(42)` | Y | G/L Account Hierarchy |  |  |
| `HierarchyNode` |  |  |  |  |  | `String(50)` | Y | Node |  |  |
| `ValidityEndDate` |  |  |  |  |  | `Date` | Y | Validity End Date |  |  |
| `ParentNode` |  |  |  |  |  | `String(50)` |  | Par. Node |  |  |
| `HierarchyVersion` |  |  |  |  |  | `String(15)` |  | Version |  |  |
| `ValidityStartDate` |  |  |  |  |  | `Date` |  | Validity Start Date |  |  |
| `ChartOfAccounts` |  |  |  |  |  | `String(4)` |  | Chart of Accounts |  |  |
| `GLAccount` |  |  |  |  |  | `String(10)` |  | G/L Account |  |  |
| `SequenceNumber` |  |  |  |  |  | `String(56)` |  |  |  |  |
| `HierarchyNodeSequence` |  |  |  |  |  | `String(6)` |  | Sequence Number |  |  |
| `HierarchyNodeLevel` |  |  |  |  |  | `String(6)` |  | Hierarchy Level |  |  |
| `NodeType` |  |  |  |  |  | `String(1)` |  | Node Type |  |  |
| `SignIsInverted` |  |  |  |  |  | `Boolean` |  | Attribute Value |  |  |
| `HierarchyNodeVal` |  |  |  |  |  | `String(40)` |  | Value |  |  |


## Entity: `GLAccountHierarchyNodeText`

- **ABAP CDS Name:** `I_GLAccountHierarchyNodeT`
- **Label:** G/L Account Hierarchy Node - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** FINSC_HIER_T

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `GLAccountHierarchy` |  |  |  |  |  | `String(42)` | Y | G/L Account Hierarchy |  |  |
| `HierarchyNode` |  |  |  |  |  | `String(50)` | Y | Node |  |  |
| `ValidityEndDate` |  |  |  |  |  | `Date` | Y | Valid To |  |  |
| `Language` |  |  |  |  |  | `String(2)` | Y | Language Key |  |  |
| `HierarchyNodeText` |  |  |  |  |  | `String(50)` |  | Description |  |  |
| `HierarchyNodeShortText` |  |  |  |  |  | `String(20)` |  |  |  |  |
| `ValidityStartDate` |  |  |  |  |  | `Date` |  | Valid From |  |  |


## Entity: `GLAccountHierarchyText`

- **ABAP CDS Name:** `I_GLAccountHierarchyText`
- **Label:** G/L Account Hierarchy - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** FINSC_HIER_T

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `GLAccountHierarchy` |  |  |  |  |  | `String(42)` | Y | G/L Account Hierarchy |  |  |
| `ValidityEndDate` |  |  |  |  |  | `Date` | Y | Valid To |  |  |
| `Language` |  |  |  |  |  | `String(2)` | Y | Language Key |  |  |
| `ValidityStartDate` |  |  |  |  |  | `Date` |  | Valid From |  |  |
| `GLAccountHierarchyName` |  |  |  |  |  | `String(50)` |  | Description |  |  |


## Entity: `GLAccountTypeFlowType`

- **ABAP CDS Name:** `I_GLAccountTypeFlowType`
- **Label:** Flow Type for G/L Account Type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `GLAccountTypeFlowType` |  |  |  |  |  | `String(12)` | Y | GLAcct Type FlowType |  | S/4 only entity |


## Entity: `GeneralLedgerAccount`

- **ABAP CDS Name:** `I_GLAccountInChartOfAccounts`
- **Label:** G/L Account In Chart Of Accounts
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** SKA1, SKAT

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `ChartOfAccounts` |  | `SKA1` | `KTOPL` |  |  | `String(4)` | Y | Chart of Accounts |  |  |
| `GLAccount` |  | `SKA1` | `SAKNR` |  |  | `String(10)` | Y | G/L Account |  |  |
| `IsBalanceSheetAccount` |  | `SKA1` | `XBILK` |  |  | `Boolean` |  | Balance sheet acct |  |  |
| `GLAccountGroup` |  | `SKA1` | `KTOKS` |  |  | `String(4)` |  | Account Group |  |  |
| `CorporateGroupChartOfAccounts` |  |  |  |  |  | `String(4)` |  | Group Chart of Accts |  |  |
| `CorporateGroupAccount` |  |  |  |  |  | `String(10)` |  | Group Account Number |  |  |
| `ProfitLossAccountType` |  | `SKA1` | `GVTYP` |  |  | `String(2)` |  | P&L state. acct |  |  |
| `SampleGLAccount` |  | `SKA1` | `MUSTR` |  |  | `String(10)` |  | Sample Account |  |  |
| `AccountIsMarkedForDeletion` |  |  |  |  |  | `Boolean` |  | Deletion Flag |  |  |
| `AccountIsBlockedForCreation` |  |  |  |  |  | `Boolean` |  | Creation Block |  |  |
| `AccountIsBlockedForPosting` |  |  |  |  |  | `Boolean` |  | Posting Block |  |  |
| `AccountIsBlockedForPlanning` |  |  |  |  |  | `Boolean` |  | Planning Block |  |  |
| `PartnerCompany` |  |  |  |  |  | `String(6)` |  | Trading Partner No. |  |  |
| `FunctionalArea` |  | `SKA1` | `FUNC_AREA` |  |  | `String(16)` |  | Functional Area |  |  |
| `CreationDate` |  |  |  |  |  | `Date` |  | Created On |  |  |
| `CreatedByUser` |  |  |  |  |  | `String(12)` |  | Created By |  |  |
| `LastChangeDateTime` |  |  |  |  |  | `DateTime` |  | Time Stamp |  |  |
| `GLAccountType` |  |  |  |  |  | `String(1)` |  | G/L Account Type |  |  |
| `GLAccountSubtype` |  |  |  |  |  | `String(1)` |  | G/L Account Subtype |  |  |
| `GLAccountExternal` |  |  |  |  |  | `String(10)` |  | G/L Acct External ID |  |  |
| `BankReconciliationAccount` |  |  |  |  |  | `String(10)` |  | Reconciliation Acct |  |  |
| `IsProfitLossAccount` |  |  |  |  |  | `Boolean` |  | Profit Loss Account |  |  |


## Entity: `GeneralLedgerAccountFlowType`

- **ABAP CDS Name:** `I_GLAccountFlowType`
- **Label:** GLAccount Flow Type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `GLAccountFlowType` |  |  |  |  |  | `String(10)` | Y | G/L Acct. Flow Type |  | S/4 only entity |


## Entity: `GeneralLedgerAccountHierarchy`

- **ABAP CDS Name:** `I_GLAccountHierarchy`
- **Label:** General Ledger Account Hierarchy
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `GLAccountHierarchy` |  |  |  |  |  | `String(42)` | Y | G/L Account Hierarchy |  |  |
| `ValidityEndDate` |  |  |  |  |  | `Date` | Y | Valid To |  |  |
| `ValidityStartDate` |  |  |  |  |  | `Date` |  | Valid From |  |  |
| `HierarchyType` |  |  |  |  |  | `String(4)` |  | Hierarchy Type |  |  |
| `LastChangedByUser` |  |  |  |  |  | `String(12)` |  | Last Changed By |  |  |
| `LastChangeTime` |  |  |  |  |  | `DateTime` |  | Updated At |  |  |
| `LastChangeDateTime` |  |  |  |  |  | `DateTime` |  | Updated At |  |  |
| `HierarchyShortID` |  |  |  |  |  | `String(20)` |  | Hierarchy ID |  |  |
| `FunctionalAreaIsUsed` |  |  |  |  |  | `Boolean` |  | Functional Area |  |  |
| `SemanticTagIsUsed` |  |  |  |  |  | `Boolean` |  | Sem. Tag Assigned |  |  |
| `ChartOfAccounts` |  |  |  |  |  | `String(4)` |  | Chart of Accounts |  |  |


## Entity: `GeneralLedgerAccountLineItem`

- **ABAP CDS Name:** `I_GLAccountLineItemRawData`
- **Label:** Raw Data of G/L Account Line Item
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** BKPF, BSEG, ACDOCA

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `SourceLedger` |  |  |  | `ACDOCA` | `RLDNR` | `String(2)` | Y | Source Ledger |  | S/4 only — no ECC equivalent; Filter ACDOCA.RLDNR='0L' for leading ledger |
| `CompanyCode` |  | `BKPF` | `BUKRS` | `ACDOCA` | `RBUKRS` | `String(4)` | Y | Company Code |  |  |
| `FiscalYear` |  | `BKPF` | `GJAHR` | `ACDOCA` | `GJAHR` | `String(4)` | Y | Fiscal Year |  |  |
| `AccountingDocument` |  | `BKPF` | `BELNR` | `ACDOCA` | `BELNR` | `String(10)` | Y | Journal Entry |  |  |
| `LedgerGLLineItem` |  | `BSEG` | `BUZEI` | `ACDOCA` | `DOCLN` | `String(6)` | Y | Journal Entry Item |  |  |
| `LedgerFiscalYear` |  |  |  |  |  | `String(4)` |  | Fiscal Year of Ledger |  |  |
| `GLRecordType` |  |  |  |  |  | `String(1)` |  | Record Type |  |  |
| `JrnlEntrAltvFYConsecutiveID` |  |  |  |  |  | `String(10)` |  | Shifted Fiscal Year Consecutive ID |  |  |
| `ChartOfAccounts` |  | `T001` | `KTOPL` | `ACDOCA` | `KTOPL` | `String(4)` |  | Chart of Accounts |  |  |
| `ControllingArea` |  | `BSEG` | `KOKRS` | `ACDOCA` | `KOKRS` | `String(4)` |  | Controlling Area |  |  |
| `FinancialTransactionType` |  |  |  |  |  | `String(3)` |  | Financial Transaction Type |  |  |
| `GLBusinessTransactionType` |  |  |  |  |  | `String(4)` |  | Transaction Type for General Ledger |  |  |
| `BusinessTransactionCategory` |  |  |  |  |  | `String(4)` |  | Business Transaction Category |  |  |
| `BusinessTransactionType` |  | `BKPF` | `GLVOR` | `ACDOCA` | `BTTYPE` | `String(4)` |  | Business Transaction Type |  |  |
| `FinancialClosingStep` |  |  |  |  |  | `String(3)` |  | Financial Closing Step |  |  |
| `ControllingBusTransacType` |  |  |  |  |  | `String(4)` |  | Business Transaction |  |  |
| `ReferenceDocumentType` |  | `BKPF` | `AWTYP` | `ACDOCA` | `AWTYP` | `String(5)` |  | Reference Document Type |  |  |
| `LogicalSystem` |  |  |  |  |  | `String(10)` |  | Logical System |  |  |
| `ReferenceDocumentContext` |  |  |  |  |  | `String(10)` |  | Reference Document Context |  |  |
| `ReferenceDocument` |  |  |  |  |  | `String(10)` |  | Reference Document |  |  |
| `ReferenceDocumentItem` |  |  |  |  |  | `String(6)` |  | Reference Document Item |  |  |
| `ReferenceDocumentItemGroup` |  |  |  |  |  | `String(6)` |  | Reference Document Item Group |  |  |
| `TransactionSubitem` |  |  |  |  |  | `String(6)` |  | Sub Transaction |  |  |
| `AccountingNotificationUUID` |  |  |  |  |  | `UUID` |  | Accounting Notification UUID |  |  |
| `OffsettingLedgerGLLineItem` |  |  |  |  |  | `String(6)` |  | G/L Offsetting Entry Line Item |  |  |
| `IsReversal` |  | `BKPF` | `XREVERSAL` | `ACDOCA` | `XREVERSING` | `Boolean` |  | Is Reversing |  |  |
| `IsReversed` |  |  |  | `ACDOCA` | `XREVERSED` | `Boolean` |  | Is Reversed |  |  |
| `ReversalReferenceDocumentType` |  |  |  |  |  | `String(5)` |  | Reversal Reference Document Type |  |  |
| `ReversalReferenceDocumentCntxt` |  |  |  |  |  | `String(10)` |  | Reversal Reference Document Context |  |  |
| `ReversalReferenceDocument` |  |  |  |  |  | `String(10)` |  | Reversal Reference Document |  |  |
| `ReversalTransactionSubitem` |  |  |  |  |  | `String(6)` |  | Reversal Transaction Sub Item |  |  |
| `IsSettlement` |  |  |  |  |  | `Boolean` |  | Is Settling |  |  |
| `IsSettled` |  |  |  |  |  | `Boolean` |  | Is Settled |  |  |
| `PredecessorReferenceDocType` |  |  |  |  |  | `String(5)` |  | Predecessor Reference Document Type |  |  |
| `PredecessorReferenceDocCntxt` |  |  |  |  |  | `String(10)` |  | Predecessor Reference Document Context |  |  |
| `PredecessorReferenceDocument` |  |  |  |  |  | `String(10)` |  | Predecessor Reference Document |  |  |
| `PredecessorReferenceDocItem` |  |  |  |  |  | `String(6)` |  | Predecessor Reference Document Item |  |  |
| `PrdcssrJournalEntryCompanyCode` |  |  |  |  |  | `String(4)` |  | Predecessor Journal Entry Company Code |  |  |
| `PrdcssrJournalEntryFiscalYear` |  |  |  |  |  | `String(4)` |  | Predecessor Journal Entry Fiscal Year |  |  |
| `PredecessorJournalEntry` |  |  |  |  |  | `String(10)` |  | Predecessor Journal Entry |  |  |
| `PredecessorJournalEntryItem` |  |  |  |  |  | `String(6)` |  | Predecessor Journal Entry Item |  |  |
| `SourceReferenceDocumentType` |  |  |  |  |  | `String(5)` |  | Source Reference Document Type |  |  |
| `SourceLogicalSystem` |  |  |  |  |  | `String(10)` |  | Source Logical System |  |  |
| `SourceReferenceDocumentCntxt` |  |  |  |  |  | `String(10)` |  | Source Reference Document Context |  |  |
| `SourceReferenceDocument` |  |  |  |  |  | `String(10)` |  | Source Reference Document |  |  |
| `SourceReferenceDocumentItem` |  |  |  |  |  | `String(6)` |  | Source Reference Document Item |  |  |
| `SourceReferenceDocSubitem` |  |  |  |  |  | `String(6)` |  | Source Reference Document Subitem |  |  |
| `IsCommitment` |  |  |  |  |  | `Boolean` |  | Is Commitment |  |  |
| `JrnlEntryItemObsoleteReason` |  |  |  |  |  | `String(1)` |  | Obsolete Reason |  |  |
| `JournalEntryIsSecondaryEntry` |  |  |  |  |  | `Boolean` |  | Is Secondary Journal Entry |  |  |
| `JrnlPeriodEndClosingRunLogUUID` |  |  |  |  |  | `UUID` |  | Closing Run UUID |  |  |
| `OrganizationalChange` |  |  |  |  |  | `String(10)` |  | Organizational Change |  |  |
| `GLAccount` |  | `BSEG` | `HKONT` | `ACDOCA` | `RACCT` | `String(10)` |  | G/L Account |  |  |
| `CostCenter` |  | `BSEG` | `KOSTL` | `ACDOCA` | `RCNTR` | `String(10)` |  | Cost Center |  |  |
| `ProfitCenter` |  | `BSEG` | `PRCTR` | `ACDOCA` | `PRCTR` | `String(10)` |  | Profit Center |  |  |
| `FunctionalArea` |  | `BSEG` | `FKBER` | `ACDOCA` | `RFAREA` | `String(16)` |  | Functional Area |  |  |
| `BusinessArea` |  | `BSEG` | `GSBER` | `ACDOCA` | `RBUSA` | `String(4)` |  | Business Area |  |  |
| `Segment` |  | `BSEG` | `SEGMENT` | `ACDOCA` | `SEGMENT` | `String(10)` |  | Segment |  |  |
| `PartnerCostCenter` |  | `BSEG` | `PARGB` | `ACDOCA` | `SCNTR` | `String(10)` |  | Partner Cost Center |  |  |
| `PartnerProfitCenter` |  |  |  | `ACDOCA` | `PPRCTR` | `String(10)` |  | Partner Profit Center |  |  |
| `PartnerFunctionalArea` |  |  |  | `ACDOCA` | `SFAREA` | `String(16)` |  | Partner Func. Area |  |  |
| `PartnerBusinessArea` |  |  |  | `ACDOCA` | `SBUSA` | `String(4)` |  | Partner Bus. Area |  |  |
| `PartnerCompany` |  |  |  |  |  | `String(6)` |  | Trading Partner |  |  |
| `PartnerSegment` |  |  |  | `ACDOCA` | `PSEGMENT` | `String(10)` |  | Partner Segment |  |  |
| `BalanceTransactionCurrency` |  |  |  |  |  | `String(5)` |  | Balance Transaction Currency |  |  |
| `AmountInBalanceTransacCrcy` |  |  |  |  |  | `Decimal(34,4)` |  | Amount in Balance Transaction Currency | BalanceTransactionCurrency |  |
| `TransactionCurrency` |  | `BKPF` | `WAERS` | `ACDOCA` | `RWCUR` | `String(5)` |  | Transaction Currency |  |  |
| `AmountInTransactionCurrency` |  | `BSEG` | `WRBTR` | `ACDOCA` | `WSL` | `Decimal(34,4)` |  | Amount in Transaction Currency | TransactionCurrency |  |
| `CompanyCodeCurrency` |  | `T001` | `WAERS` | `ACDOCA` | `RHCUR` | `String(5)` |  | Company Code Currency |  |  |
| `AmountInCompanyCodeCurrency` |  | `BSEG` | `DMBTR` | `ACDOCA` | `HSL` | `Decimal(34,4)` |  | Amount in Company Code Currency | CompanyCodeCurrency |  |
| `GlobalCurrency` |  |  |  | `ACDOCA` | `RKCUR` | `String(5)` |  | Global Currency |  | S/4 only — no ECC equivalent |
| `AmountInGlobalCurrency` |  |  |  | `ACDOCA` | `KSL` | `Decimal(34,4)` |  | Amount in Global Currency | GlobalCurrency | S/4 only — no ECC equivalent |
| `FunctionalCurrency` |  |  |  |  |  | `String(5)` |  | Functional Currency |  |  |
| `AmountInFunctionalCurrency` |  |  |  |  |  | `Decimal(34,4)` |  | Amount in Functional Currency | FunctionalCurrency |  |
| `FreeDefinedCurrency1` |  |  |  | `ACDOCA` | `ROCUR` | `String(5)` |  | Freely Defined Currency 1 |  | S/4 only — no ECC equivalent |
| `AmountInFreeDefinedCurrency1` |  |  |  | `ACDOCA` | `OSL` | `Decimal(34,4)` |  | Amount in Freely Defined Currency 1 | FreeDefinedCurrency1 | S/4 only — no ECC equivalent |
| `FreeDefinedCurrency2` |  |  |  | `ACDOCA` | `RVCUR` | `String(5)` |  | Freely Defined Currency 2 |  | S/4 only — no ECC equivalent |
| `AmountInFreeDefinedCurrency2` |  |  |  | `ACDOCA` | `VSL` | `Decimal(34,4)` |  | Amount in Freely Defined Currency 2 | FreeDefinedCurrency2 | S/4 only — no ECC equivalent |
| `FreeDefinedCurrency3` |  |  |  |  |  | `String(5)` |  | Freely Defined Currency 3 |  | S/4 only — no ECC equivalent |
| `AmountInFreeDefinedCurrency3` |  |  |  |  |  | `Decimal(34,4)` |  | Amount in Freely Defined Currency 3 | FreeDefinedCurrency3 | S/4 only — no ECC equivalent |
| `FreeDefinedCurrency4` |  |  |  |  |  | `String(5)` |  | Freely Defined Currency 4 |  |  |
| `AmountInFreeDefinedCurrency4` |  |  |  |  |  | `Decimal(34,4)` |  | Amount in Freely Defined Currency 4 | FreeDefinedCurrency4 |  |
| `FreeDefinedCurrency5` |  |  |  |  |  | `String(5)` |  | Freely Defined Currency 5 |  |  |
| `AmountInFreeDefinedCurrency5` |  |  |  |  |  | `Decimal(34,4)` |  | Amount in Freely Defined Currency 5 | FreeDefinedCurrency5 |  |
| `FreeDefinedCurrency6` |  |  |  |  |  | `String(5)` |  | Freely Defined Currency 6 |  |  |
| `AmountInFreeDefinedCurrency6` |  |  |  |  |  | `Decimal(34,4)` |  | Amount in Freely Defined Currency 6 | FreeDefinedCurrency6 |  |
| `FreeDefinedCurrency7` |  |  |  |  |  | `String(5)` |  | Freely Defined Currency 7 |  |  |
| `AmountInFreeDefinedCurrency7` |  |  |  |  |  | `Decimal(34,4)` |  | Amount in Freely Defined Currency 7 | FreeDefinedCurrency7 |  |
| `FreeDefinedCurrency8` |  |  |  |  |  | `String(5)` |  | Freely Defined Currency 8 |  |  |
| `AmountInFreeDefinedCurrency8` |  |  |  |  |  | `Decimal(34,4)` |  | Amount in Freely Defined Currency 8 | FreeDefinedCurrency8 |  |
| `FixedAmountInGlobalCrcy` |  |  |  |  |  | `Decimal(34,4)` |  | Fixed Amount in Global Currency | GlobalCurrency |  |
| `GrpValnFixedAmtInGlobCrcy` |  |  |  |  |  | `Decimal(34,4)` |  | Group Val. Fixed Amount in Global Cur. | GlobalCurrency |  |
| `PrftCtrValnFxdAmtInGlobCrcy` |  |  |  |  |  | `Decimal(34,4)` |  | PC Val. Fixed Amount in Global Currency | GlobalCurrency |  |
| `FixedAmountInCoCodeCrcy` |  |  |  |  |  | `Decimal(34,4)` |  | Fixed Amount in Company Currency | CompanyCodeCurrency |  |
| `FixedAmountInTransCrcy` |  |  |  |  |  | `Decimal(34,4)` |  | Fixed Amount in Transaction Currency | TransactionCurrency |  |
| `TotalPriceVarcInGlobalCrcy` |  |  |  |  |  | `Decimal(34,4)` |  | Total Price Variance in Global Currency | GlobalCurrency |  |
| `GrpValnTotPrcVarcInGlobCrcy` |  |  |  |  |  | `Decimal(34,4)` |  | GV Total Price Var. in Global Currency | GlobalCurrency |  |
| `PrftCtrValnTotPrcVarcInGlbCrcy` |  |  |  |  |  | `Decimal(34,4)` |  | PC Val. Total Price Var. in Global Cur. | GlobalCurrency |  |
| `FixedPriceVarcInGlobalCrcy` |  |  |  |  |  | `Decimal(34,4)` |  | Fixed Price Variance in Global Currency | GlobalCurrency |  |
| `GrpValnFixedPrcVarcInGlobCrcy` |  |  |  |  |  | `Decimal(34,4)` |  | GV Fixed Price Var. in Global Currency | GlobalCurrency |  |
| `PrftCtrValnFxdPrcVarcInGlbCrcy` |  |  |  |  |  | `Decimal(34,4)` |  | PC Val. Fixed Price Var. in Global Cur. | GlobalCurrency |  |
| `ControllingObjectCurrency` |  |  |  |  |  | `String(5)` |  | CO Object Currency |  |  |
| `AmountInObjectCurrency` |  |  |  |  |  | `Decimal(34,4)` |  | Amount in Object Currency | ControllingObjectCurrency |  |
| `GrantCurrency` |  |  |  |  |  | `String(5)` |  | Grant Currency |  |  |
| `AmountInGrantCurrency` |  |  |  |  |  | `Decimal(34,4)` |  | Amount in Grant Crcy | GrantCurrency |  |
| `BaseUnit` |  | `BSEG` | `MEINS` | `ACDOCA` | `RUNIT` | `String(3)` |  | Base Unit of Measure |  |  |
| `Quantity` |  | `BSEG` | `MENGE` | `ACDOCA` | `MSL` | `Decimal(23,3)` |  | Quantity | BaseUnit |  |
| `FixedQuantity` |  |  |  |  |  | `Decimal(23,3)` |  | Fixed Quantity | BaseUnit |  |
| `CostSourceUnit` |  |  |  |  |  | `String(3)` |  | Cost Source Unit |  |  |
| `ValuationQuantity` |  |  |  |  |  | `Decimal(23,3)` |  | Valuation Quantity | CostSourceUnit |  |
| `ValuationFixedQuantity` |  |  |  |  |  | `Decimal(23,3)` |  | Valuation Fixed Quantity | CostSourceUnit |  |
| `ReferenceQuantityUnit` |  |  |  |  |  | `String(3)` |  | Reference Qty UoM |  |  |
| `ReferenceQuantity` |  |  |  |  |  | `Decimal(23,3)` |  | Reference quantity | ReferenceQuantityUnit |  |
| `AdditionalQuantity1Unit` |  |  |  |  |  | `String(3)` |  | Additional Quantity 1 Unit |  |  |
| `AdditionalQuantity1` |  |  |  |  |  | `Decimal(23,3)` |  | Additional Quantity 1 | AdditionalQuantity1Unit |  |
| `AdditionalQuantity2Unit` |  |  |  |  |  | `String(3)` |  | Additional Quantity 2 Unit |  |  |
| `AdditionalQuantity2` |  |  |  |  |  | `Decimal(23,3)` |  | Additional Quantity 2 | AdditionalQuantity2Unit |  |
| `AdditionalQuantity3Unit` |  |  |  |  |  | `String(3)` |  | Additional Quantity 3 Unit |  |  |
| `AdditionalQuantity3` |  |  |  |  |  | `Decimal(23,3)` |  | Additional Quantity 3 | AdditionalQuantity3Unit |  |
| `IncmpltSummableValnQtyUnt` |  |  |  |  |  | `String(3)` |  | Incomplete Sum. Valuation Quantity Unit |  |  |
| `IncmpltSummableValnQty` |  |  |  |  |  | `Decimal(23,3)` |  | Incomplete Summable Valuation Quantity | IncmpltSummableValnQtyUnt |  |
| `IncmpltSummableValnFxdQty` |  |  |  |  |  | `Decimal(23,3)` |  | Incomplete Sum. Valuation Fix Quantity | IncmpltSummableValnQtyUnt |  |
| `DebitCreditCode` |  | `BSEG` | `SHKZG` | `ACDOCA` | `DRCRK` | `String(1)` |  | Debit/Credit Code |  |  |
| `FiscalPeriod` |  | `BKPF` | `MONAT` | `ACDOCA` | `POPER` | `String(3)` |  | Fiscal Period |  | ECC MONAT unpadded '3'; S/4 ACDOCA.POPER zero-padded '003' |
| `FiscalYearVariant` |  |  |  |  |  | `String(2)` |  | Fiscal Year Variant |  |  |
| `FiscalYearPeriod` |  |  |  |  |  | `String(7)` |  | Fiscal Year Period |  |  |
| `PostingDate` |  | `BKPF` | `BUDAT` | `ACDOCA` | `BUDAT` | `Date` |  | Posting Date |  |  |
| `DocumentDate` |  | `BKPF` | `BLDAT` | `ACDOCA` | `BLDAT` | `Date` |  | Journal Entry Date |  |  |
| `AccountingDocumentType` |  | `BKPF` | `BLART` | `ACDOCA` | `BLART` | `String(2)` |  | Journal Entry Type |  |  |
| `AccountingDocumentItem` |  | `BSEG` | `BUZEI` | `ACDOCA` | `BUZEI` | `String(3)` |  | Posting View Item |  |  |
| `AssignmentReference` |  | `BSEG` | `ZUONR` | `ACDOCA` | `ZUONR` | `String(18)` |  | Assignment Reference |  |  |
| `AccountingDocumentCategory` |  |  |  |  |  | `String(1)` |  | Journal Entry Category |  |  |
| `JournalEntryItemCategory` |  |  |  |  |  | `String(5)` |  | Journal Entry Item Category |  |  |
| `PostingKey` |  | `BSEG` | `BSCHL` | `ACDOCA` | `BSCHL` | `String(2)` |  | Posting Key |  |  |
| `TransactionTypeDetermination` |  |  |  |  |  | `String(3)` |  | Transaction Key |  |  |
| `SubLedgerAcctLineItemType` |  |  |  |  |  | `String(5)` |  | SLA Line Item Type |  |  |
| `AccountingDocCreatedByUser` |  |  |  |  |  | `String(12)` |  | Journal Entry Created By |  |  |
| `LastChangeDateTime` |  |  |  |  |  | `DateTime` |  | Last Change Date Time |  |  |
| `CreationDateTime` |  |  |  |  |  | `DateTime` |  | Creation Date Time |  |  |
| `CreationDate` |  |  |  |  |  | `Date` |  | Creation Date |  |  |
| `EliminationProfitCenter` |  |  |  |  |  | `String(10)` |  | Elimination Profit Center |  |  |
| `OriginObjectType` |  |  |  |  |  | `String(2)` |  | Origin Object Type |  |  |
| `GLAccountType` |  |  |  |  |  | `String(1)` |  | G/L Account Type |  |  |
| `AlternativeGLAccount` |  |  |  |  |  | `String(10)` |  | Alternative G/L Account |  |  |
| `CountryChartOfAccounts` |  |  |  |  |  | `String(4)` |  | Alternative Chart of Accounts |  |  |
| `ItemIsSplit` |  |  |  |  |  | `Boolean` |  | Itm chngd by Doc Spl |  |  |
| `ConsolidationUnit` |  |  |  |  |  | `String(18)` |  | Consolidation Unit |  |  |
| `PartnerConsolidationUnit` |  |  |  |  |  | `String(18)` |  | Partner Consolidation Unit |  |  |
| `Company` |  |  |  |  |  | `String(6)` |  | Company |  |  |
| `ConsolidationChartOfAccounts` |  |  |  |  |  | `String(2)` |  | Consolidation Chart of Accounts |  |  |
| `CnsldtnFinancialStatementItem` |  |  |  |  |  | `String(10)` |  | Consolidation Financial Statement Item |  |  |
| `CnsldtnSubitemCategory` |  |  |  |  |  | `String(3)` |  | Consolidation Subitem Category |  |  |
| `CnsldtnSubitem` |  |  |  |  |  | `String(10)` |  | Consolidation Subitem |  |  |
| `InvoiceReference` |  | `BSEG` | `REBZG` | `ACDOCA` | `REBZG` | `String(10)` |  | Invoice Reference |  |  |
| `InvoiceReferenceFiscalYear` |  | `BSEG` | `REBZJ` | `ACDOCA` | `REBZJ` | `String(4)` |  | Invoice Reference Fiscal Year |  |  |
| `FollowOnDocumentType` |  |  |  |  |  | `String(1)` |  | Follow-On Document Type |  |  |
| `InvoiceItemReference` |  |  |  |  |  | `String(3)` |  | Invoice Item Reference |  |  |
| `ReferencePurchaseOrderCategory` |  |  |  |  |  | `String(3)` |  | Reference Purchase Order Category |  |  |
| `PurchasingDocument` |  | `BSEG` | `EBELN` | `ACDOCA` | `EBELN` | `String(10)` |  | Purchasing Document |  |  |
| `PurchasingDocumentItem` |  | `BSEG` | `EBELP` | `ACDOCA` | `EBELP` | `String(5)` |  | Purchasing Doc. Item |  |  |
| `AccountAssignmentNumber` |  |  |  |  |  | `String(2)` |  | Account Assignment Number |  |  |
| `DocumentItemText` |  | `BSEG` | `SGTXT` | `ACDOCA` | `SGTXT` | `String(50)` |  | Item Text |  |  |
| `SalesDocument` |  | `BSEG` | `VBELN` | `ACDOCA` | `KDAUF` | `String(10)` |  | Sales Document |  |  |
| `SalesDocumentItem` |  |  |  |  |  | `String(6)` |  | Sales Document Item |  |  |
| `Product` |  |  |  |  |  | `String(40)` |  | Product |  |  |
| `Plant` |  | `BSEG` | `WERKS` | `ACDOCA` | `WERKS` | `String(4)` |  | Plant |  |  |
| `Supplier` |  | `BSEG` | `LIFNR` | `ACDOCA` | `LIFNR` | `String(10)` |  | Supplier |  |  |
| `Customer` |  | `BSEG` | `KUNNR` | `ACDOCA` | `KUNNR` | `String(10)` |  | Customer |  |  |
| `ServicesRenderedDate` |  |  |  |  |  | `Date` |  | Serv. Rendered Date |  |  |
| `PerformancePeriodStartDate` |  |  |  |  |  | `Date` |  | Per. of Perf. Start |  |  |
| `PerformancePeriodEndDate` |  |  |  |  |  | `Date` |  | Per. of Perf. End |  |  |
| `ConditionContract` |  |  |  |  |  | `String(10)` |  | Condition Contract |  |  |
| `ExchangeRateDate` |  |  |  |  |  | `Date` |  | Translation Date |  |  |
| `ComponentBreakdown` |  |  |  |  |  | `String(16)` |  | Component Breakdown |  |  |
| `CompBreakdownScaleNumerator` |  |  |  |  |  | `Decimal(23,3)` |  | Component Breakdown Scale Numerator |  |  |
| `FinancialAccountType` |  |  |  |  |  | `String(1)` |  | Account Type |  |  |
| `SpecialGLCode` |  |  |  |  |  | `String(1)` |  | Special G/L |  |  |
| `TaxCode` |  | `BSEG` | `MWSKZ` | `ACDOCA` | `MWSKZ` | `String(2)` |  | Tax Code |  |  |
| `TaxCountry` |  |  |  |  |  | `String(3)` |  | Tax Ctry/Reg. |  |  |
| `HouseBank` |  |  |  |  |  | `String(5)` |  | House Bank |  |  |
| `HouseBankAccount` |  |  |  |  |  | `String(5)` |  | House Bank Account |  |  |
| `IsOpenItemManaged` |  |  |  |  |  | `Boolean` |  | Open Item Management |  |  |
| `ClearingDate` |  | `BSEG` | `AUGDT` | `ACDOCA` | `AUGDT` | `Date` |  | Clearing Date |  |  |
| `ClearingDocFiscalYear` |  |  |  |  |  | `String(4)` |  | Fiscal Year of Clearing JE (Depr.) |  |  |
| `ClearingAccountingDocument` |  | `BSEG` | `AUGBL` | `ACDOCA` | `AUGBL` | `String(10)` |  | Clearing Journal Entry (Deprecated) |  |  |
| `ClearingJournalEntryFiscalYear` |  |  |  |  |  | `String(4)` |  | Fiscal Year of Clearing Journal Entry |  |  |
| `ClearingJournalEntry` |  |  |  |  |  | `String(10)` |  | Clearing Journal Entry |  |  |
| `ValueDate` |  |  |  |  |  | `Date` |  | Value date |  |  |
| `GeneralLedgerAgingScope` |  |  |  |  |  | `String(10)` |  | General Ledger Aging Scope |  |  |
| `GeneralLedgerAgingIncrement` |  |  |  |  |  | `String(15)` |  | General Ledger Aging Increment |  |  |
| `AssetDepreciationArea` |  |  |  |  |  | `String(2)` |  | Depreciation Area |  |  |
| `MasterFixedAsset` |  | `BSEG` | `ANLN1` | `ACDOCA` | `ANLN1` | `String(12)` |  | Fixed Asset |  |  |
| `FixedAsset` |  | `BSEG` | `ANLN2` | `ACDOCA` | `ANLN2` | `String(4)` |  | Asset Subnumber |  |  |
| `AssetValueDate` |  |  |  |  |  | `Date` |  | Asset Value Date |  |  |
| `AssetTransactionType` |  |  |  |  |  | `String(3)` |  | Asset Transaction Type |  |  |
| `AssetAcctTransClassfctn` |  |  |  |  |  | `String(2)` |  | Trans. Type Category |  |  |
| `DepreciationFiscalPeriod` |  |  |  |  |  | `String(3)` |  | Depreciation Fiscal Period |  |  |
| `GroupMasterFixedAsset` |  |  |  |  |  | `String(12)` |  | Group Asset |  |  |
| `GroupFixedAsset` |  |  |  |  |  | `String(4)` |  | Group Asset Subnmbr |  |  |
| `AssetClass` |  |  |  |  |  | `String(8)` |  | Asset Class |  |  |
| `PartnerMasterFixedAsset` |  |  |  |  |  | `String(12)` |  | Partner Master Fixed Asset |  |  |
| `PartnerFixedAsset` |  |  |  |  |  | `String(4)` |  | Partner Fixed Asset |  |  |
| `CostEstimate` |  |  |  |  |  | `String(12)` |  | Cost Estimate |  |  |
| `InventorySpecialStockValnType` |  |  |  |  |  | `String(1)` |  | Inventory Special Stock Valuation Type |  |  |
| `IsSupplierStockValuation` |  |  |  |  |  | `Boolean` |  | Is Supplier Stock Valuation |  |  |
| `InventorySpecialStockType` |  |  |  |  |  | `String(1)` |  | Inventory Special Stock Type |  |  |
| `InventorySpclStkSalesDocument` |  |  |  |  |  | `String(10)` |  | Inventory Special Stock Sales Document |  |  |
| `InventorySpclStkSalesDocItm` |  |  |  |  |  | `String(6)` |  | Inventory Spcl Stock Sales Document Item |  |  |
| `InvtrySpclStockWBSElmntIntID` |  |  |  |  |  | `String(8)` |  | Inv. Special Stock WBS Element Int. ID |  |  |
| `InventorySpclStockWBSElement` |  |  |  |  |  | `String(24)` |  | Inventory WBS Element |  |  |
| `InventorySpecialStockSupplier` |  |  |  |  |  | `String(10)` |  | Inventory Special Stock Supplier |  |  |
| `InventoryValuationType` |  |  |  |  |  | `String(10)` |  | Inventory Valuation Type |  |  |
| `ValuationArea` |  |  |  |  |  | `String(4)` |  | Valuation Area |  |  |
| `MaterialLedgerProcessType` |  |  |  |  |  | `String(4)` |  | Material Ledger Process Type |  |  |
| `MaterialLedgerCategory` |  |  |  |  |  | `String(2)` |  | Material Ledger Category |  |  |
| `SlsPriceAmountInCoCodeCrcy` |  |  |  |  |  | `Decimal(34,4)` |  | Sales Price Amount in Company Code Crcy | CompanyCodeCurrency |  |
| `ProductPriceControl` |  |  |  |  |  | `String(1)` |  | Product Price Control |  |  |
| `ProcurementAlternative` |  |  |  |  |  | `String(12)` |  | Procurement Alternative |  |  |
| `ProductionProcess` |  |  |  |  |  | `String(12)` |  | Production Process |  |  |
| `SenderCompanyCode` |  |  |  |  |  | `String(4)` |  | Company Code in Sender System |  |  |
| `SenderGLAccount` |  |  |  |  |  | `String(10)` |  | Sender G/L Account |  |  |
| `SenderAccountAssignment` |  |  |  |  |  | `String(30)` |  | Sender Account Assignment |  |  |
| `SenderAccountAssignmentType` |  |  |  |  |  | `String(2)` |  | Sender Account Assignment Type |  |  |
| `ControllingObject` |  |  |  |  |  | `String(22)` |  | Controlling Object |  |  |
| `ControllingKeySubNumber` |  |  |  |  |  | `String(14)` |  | CO subkey |  |  |
| `CostOriginGroup` |  |  |  |  |  | `String(4)` |  | Origin Group |  |  |
| `OriginSenderObject` |  |  |  |  |  | `String(22)` |  | Origin Sender Object |  |  |
| `ControllingDebitCreditCode` |  |  |  |  |  | `String(1)` |  | Controlling Debit Credit Code |  |  |
| `OriginCtrlgDebitCreditCode` |  |  |  |  |  | `String(1)` |  | Dr/Cr Ind. (Origin) |  |  |
| `ControllingObjectDebitType` |  |  |  |  |  | `String(1)` |  | Controlling Object Debit Type |  |  |
| `QuantityIsIncomplete` |  |  |  |  |  | `Boolean` |  | Qty Is Incomplete |  |  |
| `OffsettingAccount` |  |  |  |  |  | `String(10)` |  | Offsetting Account |  |  |
| `OffsettingAccountType` |  |  |  |  |  | `String(1)` |  | Offsetting Account Type |  |  |
| `OffsettingChartOfAccounts` |  |  |  |  |  | `String(4)` |  | Offsetting Chart of Accounts |  |  |
| `LineItemIsCompleted` |  |  |  |  |  | `Boolean` |  | Line Item is Completed |  |  |
| `PersonnelNumber` |  |  |  |  |  | `String(8)` |  | Personnel Number |  |  |
| `ProfitabilitySegment` |  |  |  |  |  | `String(10)` |  | Profitability Segment |  |  |
| `ControllingObjectClass` |  |  |  |  |  | `String(2)` |  | Controlling Object Class |  |  |
| `PartnerCompanyCode` |  |  |  |  |  | `String(4)` |  | Partner Company Code |  |  |
| `PartnerControllingObjectClass` |  |  |  |  |  | `String(2)` |  | Partner Controlling Object Class |  |  |
| `OriginProfitCenter` |  |  |  |  |  | `String(10)` |  | Origin Profit Center |  |  |
| `OriginOrder` |  |  |  |  |  | `String(12)` |  | Origin Order |  |  |
| `OriginCostCtrActivityType` |  |  |  |  |  | `String(6)` |  | Origin Cost Center Activity Type |  |  |
| `OriginCostCenter` |  |  |  |  |  | `String(10)` |  | Origin Cost Center |  |  |
| `OriginProduct` |  |  |  |  |  | `String(40)` |  | Origin Product |  |  |
| `VarianceOriginGLAccount` |  |  |  |  |  | `String(10)` |  | Origin G/L Account of a Variance |  |  |
| `AccountAssignment` |  |  |  |  |  | `String(30)` |  | Account Assignment |  |  |
| `AccountAssignmentType` |  |  |  |  |  | `String(2)` |  | Account Assignment Type |  |  |
| `CostCtrActivityType` |  |  |  |  |  | `String(6)` |  | Activity Type |  |  |
| `OrderID` |  | `BSEG` | `AUFNR` | `ACDOCA` |  | `String(12)` |  | Order ID |  |  |
| `OrderCategory` |  |  |  |  |  | `String(2)` |  | Order category |  |  |
| `WBSElementInternalID` |  |  |  |  |  | `String(8)` |  | WBS Element Internal ID |  |  |
| `WBSElement` |  | `BSEG` | `PS_PSP_PNR` | `ACDOCA` |  | `String(24)` |  | WBS Element |  |  |
| `PartnerWBSElementInternalID` |  |  |  |  |  | `String(8)` |  | Partner WBS Element Internal ID |  |  |
| `PartnerWBSElement` |  |  |  |  |  | `String(24)` |  | Partner WBS Element |  |  |
| `ProjectInternalID` |  |  |  |  |  | `String(8)` |  | Project Internal ID |  |  |
| `Project` |  |  |  |  |  | `String(24)` |  | Project |  |  |
| `PartnerProjectInternalID` |  |  |  |  |  | `String(8)` |  | Partner Project Internal ID |  |  |
| `PartnerProject` |  |  |  |  |  | `String(24)` |  | Partner Project |  |  |
| `OperatingConcern` |  |  |  |  |  | `String(4)` |  | Operating concern |  |  |
| `ProjectNetwork` |  |  |  |  |  | `String(12)` |  | Network |  |  |
| `RelatedNetworkActivity` |  |  |  |  |  | `String(4)` |  | Related Network Activity |  |  |
| `BusinessProcess` |  |  |  |  |  | `String(12)` |  | Business Process |  |  |
| `CostObject` |  |  |  |  |  | `String(12)` |  | Cost Object |  |  |
| `BillableControl` |  |  |  |  |  | `String(2)` |  | Billable Control |  |  |
| `CostAnalysisResource` |  |  |  |  |  | `String(10)` |  | Cost Analysis Resource |  |  |
| `CustomerServiceNotification` |  |  |  |  |  | `String(12)` |  | Customer Service Notification |  |  |
| `ServiceDocumentType` |  |  |  |  |  | `String(4)` |  | Service Doc. Type |  |  |
| `ServiceDocument` |  |  |  |  |  | `String(10)` |  | Service Document |  |  |
| `ServiceDocumentItem` |  |  |  |  |  | `String(6)` |  | Service Doc. Item |  |  |
| `PartnerServiceDocumentType` |  |  |  |  |  | `String(4)` |  | Partner Service Document Type |  |  |
| `PartnerServiceDocument` |  |  |  |  |  | `String(10)` |  | Partner Service Document |  |  |
| `PartnerServiceDocumentItem` |  |  |  |  |  | `String(6)` |  | Partner Service Document Item |  |  |
| `ServiceContractType` |  |  |  |  |  | `String(4)` |  | Serv. Contract Type |  |  |
| `ServiceContract` |  |  |  |  |  | `String(10)` |  | Service Contract |  |  |
| `ServiceContractItem` |  |  |  |  |  | `String(6)` |  | Srv Contract Item |  |  |
| `BusinessSolutionOrder` |  |  |  |  |  | `String(10)` |  | Solution Order |  |  |
| `BusinessSolutionOrderItem` |  |  |  |  |  | `String(6)` |  | Solution Order Item |  |  |
| `ProviderContract` |  |  |  |  |  | `String(20)` |  | Provider Contract |  |  |
| `ProviderContractItem` |  |  |  |  |  | `String(6)` |  | Provider Contract Item |  |  |
| `RevenueAccountingContract` |  |  |  |  |  | `String(14)` |  | Revenue Accounting Contract |  |  |
| `PerformanceObligation` |  |  |  |  |  | `String(16)` |  | Performance Obligation |  |  |
| `TimeSheetOvertimeCategory` |  |  |  |  |  | `String(4)` |  | Overtime Category |  |  |
| `PartnerAccountAssignment` |  |  |  |  |  | `String(30)` |  | Partner Account Assignment |  |  |
| `PartnerAccountAssignmentType` |  |  |  |  |  | `String(2)` |  | Partner Account Assignment Type |  |  |
| `StstclAccountAssignmentType1` |  |  |  |  |  | `String(2)` |  | Statistical Account Assignment Type 1 |  |  |
| `StstclAccountAssignmentType2` |  |  |  |  |  | `String(2)` |  | Statistical Account Assignment Type 2 |  |  |
| `StstclAccountAssignmentType3` |  |  |  |  |  | `String(2)` |  | Statistical Account Assignment Type 3 |  |  |
| `WorkPackage` |  |  |  |  |  | `String(50)` |  | Plan Item |  |  |
| `WorkItem` |  |  |  |  |  | `String(10)` |  | Work Item ID |  |  |
| `PartnerCostCtrActivityType` |  |  |  |  |  | `String(6)` |  | Partner Cost Center Activity Type |  |  |
| `PartnerOrder` |  |  |  |  |  | `String(12)` |  | Partner Order |  |  |
| `PartnerOrderCategory` |  |  |  |  |  | `String(2)` |  | Partner Order Cat. |  |  |
| `PartnerSalesDocument` |  |  |  |  |  | `String(10)` |  | Partner Sales Doc. |  |  |
| `PartnerSalesDocumentItem` |  |  |  |  |  | `String(6)` |  | Partner Sales Document Item |  |  |
| `PartnerProjectNetwork` |  |  |  |  |  | `String(12)` |  | Partner Project Network |  |  |
| `PartnerProjectNetworkActivity` |  |  |  |  |  | `String(4)` |  | Partner Project Network Activity |  |  |
| `PartnerBusinessProcess` |  |  |  |  |  | `String(12)` |  | Partner Business Process |  |  |
| `PartnerCostObject` |  |  |  |  |  | `String(12)` |  | Partner Cost Object |  |  |
| `ControllingDocumentItem` |  |  |  |  |  | `String(3)` |  | Controlling Doc Item |  |  |
| `VarianceOriginGroup` |  |  |  |  |  | `String(4)` |  | Varc. Origin Group |  |  |
| `BillingDocumentType` |  |  |  |  |  | `String(4)` |  | Billing Type |  |  |
| `SalesOrganization` |  |  |  |  |  | `String(4)` |  | Sales Organization |  |  |
| `DistributionChannel` |  |  |  |  |  | `String(2)` |  | Distribution Channel |  |  |
| `OrganizationDivision` |  |  |  |  |  | `String(2)` |  | Division |  |  |
| `SoldProduct` |  |  |  |  |  | `String(40)` |  | Product Sold |  |  |
| `SoldProductGroup` |  |  |  |  |  | `String(9)` |  | Product Sold Group |  |  |
| `CustomerGroup` |  |  |  |  |  | `String(2)` |  | Customer Group |  |  |
| `CustomerSupplierCountry` |  |  |  |  |  | `String(3)` |  | Customer or Supplier Country/Region |  |  |
| `CustomerSupplierIndustry` |  |  |  |  |  | `String(4)` |  | Customer Supplier Industry |  |  |
| `SalesDistrict` |  |  |  |  |  | `String(6)` |  | Sales District |  |  |
| `BillToParty` |  |  |  |  |  | `String(10)` |  | Bill-to Party |  |  |
| `ShipToParty` |  |  |  |  |  | `String(10)` |  | Ship-to Party |  |  |
| `CustomerSupplierCorporateGroup` |  |  |  |  |  | `String(10)` |  | Customer Supplier Corporate Group |  |  |
| `CashLedgerCompanyCode` |  |  |  |  |  | `String(4)` |  | Cash Origin CoCode |  |  |
| `CashLedgerAccount` |  |  |  |  |  | `String(10)` |  | Cash Origin Account |  |  |
| `FinancialManagementArea` |  |  |  |  |  | `String(4)` |  | FM Area |  |  |
| `CommitmentItem` |  |  |  |  |  | `String(24)` |  | Commitment Item |  |  |
| `FundsCenter` |  |  |  |  |  | `String(16)` |  | Funds Center |  |  |
| `FundedProgram` |  |  |  |  |  | `String(24)` |  | Funded Program |  |  |
| `Fund` |  |  |  |  |  | `String(10)` |  | Fund |  |  |
| `GrantID` |  |  |  |  |  | `String(20)` |  | Grant |  |  |
| `BudgetPeriod` |  |  |  |  |  | `String(10)` |  | Budget Period |  |  |
| `PartnerFund` |  |  |  |  |  | `String(10)` |  | Partner Fund |  |  |
| `PartnerGrant` |  |  |  |  |  | `String(20)` |  | Partner Grant |  |  |
| `PartnerBudgetPeriod` |  |  |  |  |  | `String(10)` |  | Partner Budget Period |  |  |
| `PubSecBudgetAccount` |  |  |  |  |  | `String(10)` |  | Budget Account |  |  |
| `PubSecBudgetAccountCoCode` |  |  |  |  |  | `String(4)` |  | Company Code for Budget Account |  |  |
| `PubSecBudgetCnsmpnDate` |  |  |  |  |  | `Date` |  | Budget Consumption Date |  |  |
| `PubSecBudgetCnsmpnFsclPeriod` |  |  |  |  |  | `String(3)` |  | Posting Period for Budget Consumption |  |  |
| `PubSecBudgetCnsmpnFsclYear` |  |  |  |  |  | `String(4)` |  | Year of Budget Consumption |  |  |
| `PubSecBudgetIsRelevant` |  |  |  |  |  | `Boolean` |  | Budget-Relevant |  |  |
| `PubSecBudgetCnsmpnType` |  |  |  |  |  | `String(2)` |  | Budget Consumption Type |  |  |
| `PubSecBudgetCnsmpnAmtType` |  |  |  |  |  | `String(4)` |  | Amount Type for Budget Consumption |  |  |
| `SponsoredProgram` |  |  |  |  |  | `String(20)` |  | Sponsored Program |  |  |
| `SponsoredClass` |  |  |  |  |  | `String(20)` |  | Sponsored Class |  |  |
| `GteeMBudgetValidityNumber` |  |  |  |  |  | `String(3)` |  | Bdgt Validty No. |  |  |
| `EarmarkedFundsDocument` |  |  |  |  |  | `String(10)` |  | Earmarked Funds Document |  |  |
| `EarmarkedFundsDocumentItem` |  |  |  |  |  | `String(3)` |  | Earmarked Funds Document Item |  |  |
| `FinancialServicesProductGroup` |  |  |  |  |  | `String(10)` |  | Financial Services Product Group |  |  |
| `FinancialServicesBranch` |  |  |  |  |  | `String(10)` |  | Financial Services Branch |  |  |
| `FinancialDataSource` |  |  |  |  |  | `String(10)` |  | Financial Data Source |  |  |
| `JointVenture` |  |  |  |  |  | `String(6)` |  | Joint venture |  |  |
| `JointVentureEquityGroup` |  |  |  |  |  | `String(3)` |  | Joint Venture Equity Group |  |  |
| `JointVentureCostRecoveryCode` |  |  |  |  |  | `String(2)` |  | Joint Venture Cost Recovery Code |  |  |
| `JointVenturePartner` |  |  |  |  |  | `String(10)` |  | Joint Venture Partner |  |  |
| `JointVentureBillingType` |  |  |  |  |  | `String(2)` |  | Joint Venture Billing Type |  |  |
| `JointVentureEquityType` |  |  |  |  |  | `String(3)` |  | Joint Venture Equity Type |  |  |
| `JointVentureProductionDate` |  |  |  |  |  | `Date` |  | Joint Venture Production Date |  |  |
| `JointVentureBillingDate` |  |  |  |  |  | `Date` |  | Joint Venture Billing Date |  |  |
| `JointVentureOperationalDate` |  |  |  |  |  | `Date` |  | Joint Venture Operational Date |  |  |
| `CutbackRun` |  |  |  |  |  | `Timestamp` |  | Cutback Run |  |  |
| `JointVentureAccountingActivity` |  |  |  |  |  | `String(2)` |  | Joint Venture Accounting Activity |  |  |
| `PartnerVenture` |  |  |  |  |  | `String(6)` |  | PartnerVenture |  |  |
| `PartnerEquityGroup` |  |  |  |  |  | `String(3)` |  | Partner Equity Group |  |  |
| `SenderCostRecoveryCode` |  |  |  |  |  | `String(2)` |  | Sender Cost Recovery Code |  |  |
| `CutbackAccount` |  |  |  |  |  | `String(10)` |  | Cutback Account |  |  |
| `CutbackCostObject` |  |  |  |  |  | `String(22)` |  | Cutback Cost Object |  |  |
| `REBusinessEntity` |  |  |  |  |  | `String(8)` |  | RE Business Entity |  |  |
| `RealEstateBuilding` |  |  |  |  |  | `String(8)` |  | Real Estate Building |  |  |
| `RealEstateProperty` |  |  |  |  |  | `String(8)` |  | Real Estate Property |  |  |
| `RERentalObject` |  |  |  |  |  | `String(8)` |  | RE Rental Object |  |  |
| `RealEstateContract` |  |  |  |  |  | `String(13)` |  | Real Estate Contract |  |  |
| `REServiceChargeKey` |  |  |  |  |  | `String(4)` |  | RE Service Charge Key |  |  |
| `RESettlementUnitID` |  |  |  |  |  | `String(5)` |  | RE Settlement Unit |  |  |
| `SettlementReferenceDate` |  |  |  |  |  | `Date` |  | Settlement Reference Date |  |  |
| `REPartnerBusinessEntity` |  |  |  |  |  | `String(8)` |  | RE Partner Business Entity |  |  |
| `RealEstatePartnerBuilding` |  |  |  |  |  | `String(8)` |  | Real Estate Partner Building |  |  |
| `RealEstatePartnerProperty` |  |  |  |  |  | `String(8)` |  | Real Estate Partner Property |  |  |
| `REPartnerRentalObject` |  |  |  |  |  | `String(8)` |  | RE Partner Rental Object |  |  |
| `RealEstatePartnerContract` |  |  |  |  |  | `String(13)` |  | Real Estate Partner Contract |  |  |
| `REPartnerServiceChargeKey` |  |  |  |  |  | `String(4)` |  | RE Partner Service Charge Key |  |  |
| `REPartnerSettlementUnitID` |  |  |  |  |  | `String(5)` |  | RE Partner Settlement Unit |  |  |
| `PartnerSettlementReferenceDate` |  |  |  |  |  | `Date` |  | Ptnr. Reference Date |  |  |
| `AccrualObjectType` |  |  |  |  |  | `String(4)` |  | Accrual Object Type |  |  |
| `AccrualObjectLogicalSystem` |  |  |  |  |  | `String(10)` |  | Logical Syst. AcrObj |  |  |
| `AccrualObject` |  |  |  |  |  | `String(32)` |  | Accrual Object |  |  |
| `AccrualSubobject` |  |  |  |  |  | `String(32)` |  | Accrual Subobject |  |  |
| `AccrualItemType` |  |  |  |  |  | `String(11)` |  | Accrual Item Type |  |  |
| `AccrualReferenceObject` |  |  |  |  |  | `String(32)` |  | Accrual Reference Object |  |  |
| `AccrualValueDate` |  |  |  |  |  | `Date` |  | Accrual Value Date |  |  |
| `FinancialValuationObjectType` |  |  |  |  |  | `String(4)` |  | Financial Valuation Object Type |  |  |
| `FinancialValuationObject` |  |  |  |  |  | `String(32)` |  | Financial Valuation Object |  |  |
| `FinancialValuationSubobject` |  |  |  |  |  | `String(32)` |  | Financial Valuation Subobject |  |  |
| `NetDueDate` |  |  |  |  |  | `Date` |  | Net Due Date |  |  |
| `CreditRiskClass` |  |  |  |  |  | `String(3)` |  | Credit Risk Class |  |  |
| `WorkCenterInternalID` |  |  |  |  |  | `String(8)` |  | Object ID |  |  |
| `OrderOperation` |  |  |  |  |  | `String(4)` |  | Order Operation |  |  |
| `OrderItem` |  |  |  |  |  | `String(4)` |  | Order item number |  |  |
| `PartnerOrderItem` |  |  |  |  |  | `String(4)` |  | Partner Order item |  |  |
| `OrderSuboperation` |  |  |  |  |  | `String(4)` |  | Order Suboperation |  |  |
| `Equipment` |  |  |  |  |  | `String(18)` |  | Equipment |  |  |
| `FunctionalLocation` |  |  |  |  |  | `String(30)` |  | Functional Location |  |  |
| `Assembly` |  |  |  |  |  | `String(40)` |  | Assembly |  |  |
| `MaintenanceActivityType` |  |  |  |  |  | `String(3)` |  | MaintActivityType |  |  |
| `MaintenanceOrderPlanningCode` |  |  |  |  |  | `String(1)` |  | Order planning ind. |  |  |
| `MaintPriorityType` |  |  |  |  |  | `String(2)` |  | Priority Type |  |  |
| `MaintPriority` |  |  |  |  |  | `String(1)` |  | Priority |  |  |
| `SuperiorOrder` |  |  |  |  |  | `String(12)` |  | Superior Order |  |  |
| `ProductGroup` |  |  |  |  |  | `String(9)` |  | Product Group |  |  |
| `MaintenanceOrderIsPlanned` |  |  |  |  |  | `Boolean` |  | Planned Parts/Work |  |  |
| `OriginOrderOperation` |  |  |  |  |  | `String(4)` |  | Origin Order Operation |  |  |
| `JrnlEntryItemMigrationSource` |  |  |  |  |  | `String(1)` |  | Journal Entry Item Migration Source |  |  |
| `USFedCommitmentString` |  |  |  |  |  | `String(62)` |  | Commitment string |  |  |
| `USFedBudgetaryLedgerStatus` |  |  |  |  |  | `String(5)` |  | BL Status |  |  |
| `USFedFiscalYearBlank` |  |  |  |  |  | `String(4)` |  | FMA Fiscal Year |  |  |
| `USFedObjectClass` |  |  |  |  |  | `String(24)` |  | Obj Class US Fed |  |  |
| `USFedStandardGLAccount` |  |  |  |  |  | `String(6)` |  | SGL account |  |  |
| `USFedAgencyLocationCode` |  |  |  |  |  | `String(8)` |  | Agency Location Code |  |  |
| `USFedApplOfSecdrySrceFunds` |  |  |  |  |  | `String(16)` |  | Application of Funds |  |  |
| `USFedFundType` |  |  |  |  |  | `String(6)` |  | Fund Type |  |  |
| `USFedPaymentOffice` |  |  |  |  |  | `String(5)` |  | Payment Office |  |  |
| `USFedAgency` |  |  |  |  |  | `String(3)` |  | Agency Identifier |  |  |
| `USFedMainAccount` |  |  |  |  |  | `String(4)` |  | Main Account |  |  |
| `USFedSubAccount` |  |  |  |  |  | `String(3)` |  | Sub account |  |  |
| `USFedBeginPerdOfAvailability` |  |  |  |  |  | `String(4)` |  | Begin Prd of Avail |  |  |
| `USFedEndPerdOfAvaily` |  |  |  |  |  | `String(4)` |  | Ending Prd of Avail |  |  |
| `USFedAvailabilityType` |  |  |  |  |  | `String(1)` |  | Avail Type Code |  |  |
| `USFedBusEventTypeCode` |  |  |  |  |  | `String(10)` |  | Business Evt Typ Cd |  |  |
| `USFedSubLevelPrefix` |  |  |  |  |  | `String(2)` |  | Sublevel Prefix |  |  |
| `USFedAuthorityType` |  |  |  |  |  | `String(1)` |  | Authority Type |  |  |
| `USFedApportionmentCategory` |  |  |  |  |  | `String(1)` |  | Apportionment Cat |  |  |
| `USFedApprtmtCatDetailPgmCode` |  |  |  |  |  | `String(4)` |  | Category B Detail |  |  |
| `USFedYearOfBdgtAuthorityCode` |  |  |  |  |  | `String(4)` |  | Yr of Budget Auth |  |  |
| `USFedAvailabilityTimeType` |  |  |  |  |  | `String(1)` |  | Availability Time |  |  |
| `USFedPriorYearAdjmtCode` |  |  |  |  |  | `String(1)` |  | Prior Year Adj. Cd |  |  |
| `USFedBudgetEnforcementActCat` |  |  |  |  |  | `String(1)` |  | BEA Category |  |  |
| `USFedReductionType` |  |  |  |  |  | `String(3)` |  | Reduction Type |  |  |
| `USFedBorrowingSource` |  |  |  |  |  | `String(1)` |  | Borrowing Source |  |  |
| `USFedRptgYearForCohort` |  |  |  |  |  | `String(4)` |  | Year Cohort |  |  |
| `USFedAllocTransfAgencyID` |  |  |  |  |  | `String(3)` |  | Alloc Transfr Agency |  |  |
| `USFedReimbursable` |  |  |  |  |  | `String(1)` |  | Reimbursable |  |  |
| `USFedBudgetImpact` |  |  |  |  |  | `String(1)` |  | Budget Impact |  |  |
| `USFedDisasterEmergencyFundCode` |  |  |  |  |  | `String(3)` |  | Disastr Emer Fnd Cde |  |  |
| `USFedPgmReportingCat` |  |  |  |  |  | `String(3)` |  | Prog.Rpt.Category |  |  |
| `USFedCustodialIndicator` |  |  |  |  |  | `String(1)` |  | Custodial indicator |  |  |
| `USFedPostingSequenceNumber` |  |  |  |  |  | `String(10)` |  | Sequence Nbr |  |  |
| `USFedExchangeIndicator` |  |  |  |  |  | `String(1)` |  | Exchange Indicator |  |  |
| `USFedFederalNonFederalCode` |  |  |  |  |  | `String(1)` |  | Federal/Nonfederal |  |  |
| `USFedTradingPartnerAgency` |  |  |  |  |  | `String(3)` |  | Agency ID (TP) |  |  |
| `USFedTrdgPartMainAccount` |  |  |  |  |  | `String(4)` |  | Main Account (TP) |  |  |
| `USFedTrdgPartSubAccount` |  |  |  |  |  | `String(3)` |  | Subaccount (TP) |  |  |
| `USFedTrdgPartBeginPerdOfAvaily` |  |  |  |  |  | `String(4)` |  | Begin Prd Avail (TP) |  |  |
| `USFedTrdgPartEndPerdOfAvaily` |  |  |  |  |  | `String(4)` |  | End Prd Avail (TP) |  |  |
| `USFedAllocTransfAgencyTrdgPart` |  |  |  |  |  | `String(3)` |  | AllcTrnsfrAgncy (TP) |  |  |
| `USFedTrdgPartAvailabilityType` |  |  |  |  |  | `String(1)` |  | Avail Type Code (TP) |  |  |
| `USFedTrdgPartBusEventTypeCode` |  |  |  |  |  | `String(10)` |  | BusinessEvtTypCd(TP) |  |  |
| `USFedTrdgPartSubLevelPrefix` |  |  |  |  |  | `String(2)` |  | Sublevel Prefix (TP) |  |  |
| `USFedPgmActivityReportingKey` |  |  |  |  |  | `String(15)` |  | Prog Act Rep Key |  |  |
| `GeneralLedgerAccountLineItemOID` |  |  |  |  |  | `String(128)` |  |  |  |  |


## Entity: `GeneralLedgerAccountText`

- **ABAP CDS Name:** `I_GLAccountTextRawData`
- **Label:** General Ledger Account - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** SKAT

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `ChartOfAccounts` |  |  |  |  |  | `String(4)` | Y | Chart of Accounts |  |  |
| `GLAccount` |  |  |  |  |  | `String(10)` | Y | G/L Account |  |  |
| `Language` |  |  |  |  |  | `String(2)` | Y | Language Key |  |  |
| `GLAccountName` |  |  |  |  |  | `String(20)` |  | G/L Account Name |  |  |
| `GLAccountLongName` |  |  |  |  |  | `String(50)` |  | G/L Account Long Name |  |  |
| `LastChangeDateTime` |  |  |  |  |  | `DateTime` |  | Time Stamp |  |  |


## Entity: `GeneralLedgerAccountTypeText`

- **ABAP CDS Name:** `I_GLAccountTypeText`
- **Label:** G/L Account Type - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `GLAccountType` |  |  |  |  |  | `String(10)` | Y | Lower Value |  | S/4 only entity |
| `Language` |  |  |  |  |  | `String(2)` | Y | Lang. |  | S/4 only entity |
| `GLAccountTypeName` |  |  |  |  |  | `String(60)` |  | Short Description |  | S/4 only entity |
| `DomainValue` |  |  |  |  |  | `String(10)` |  | Lower Value |  | S/4 only entity |


## Entity: `OperatingGeneralLedgerAccount`

- **ABAP CDS Name:** `I_GLAccountInCompanyCode`
- **Label:** General Ledger Account in Company Code
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** SKA1, SKB1

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `GLAccount` |  |  |  |  |  | `String(10)` | Y | G/L Account |  |  |
| `CompanyCode` |  |  |  |  |  | `String(4)` | Y | Company Code |  |  |
| `AuthorizationGroup` |  |  |  |  |  | `String(4)` |  | Authorization |  |  |
| `AccountingClerk` |  |  |  |  |  | `String(2)` |  | Clerk Abbrev. |  |  |
| `LastInterestCalcRunDate` |  |  |  |  |  | `Date` |  | Last Int. Calc. |  |  |
| `CreationDate` |  |  |  |  |  | `Date` |  | Created On |  |  |
| `CreatedByUser` |  |  |  |  |  | `String(12)` |  | Created By |  |  |
| `LastChangeDateTime` |  |  |  |  |  | `DateTime` |  | Time Stamp |  |  |
| `PlanningLevel` |  |  |  |  |  | `String(2)` |  | Planning Level |  |  |
| `HouseBank` |  |  |  |  |  | `String(5)` |  | House Bank |  |  |
| `HouseBankAccount` |  |  |  |  |  | `String(5)` |  | Account ID |  |  |
| `ExchRateDifferencesAccountDetn` |  |  |  |  |  | `String(4)` |  | E/R Diff. Key |  |  |
| `ReconciliationAccountType` |  |  |  |  |  | `String(1)` |  | Reconcil. ID |  |  |
| `TaxCategory` |  |  |  |  |  | `String(2)` |  | Tax Category |  |  |
| `InterestCalculationCode` |  |  |  |  |  | `String(2)` |  | Interest Indicator |  |  |
| `GLAccountCurrency` |  |  |  |  |  | `String(5)` |  | Account Currency |  |  |
| `ReconciliationAcctIsChangeable` |  |  |  |  |  | `Boolean` |  | Rec.Act Ready |  |  |
| `IsManagedExternally` |  |  |  |  |  | `Boolean` |  | Is Managed Ext. |  |  |
| `IsAutomaticallyPosted` |  |  |  |  |  | `Boolean` |  | Auto. Posting |  |  |
| `LineItemDisplayIsEnabled` |  |  |  |  |  | `Boolean` |  | Line Items |  |  |
| `SupplementIsAllowed` |  |  |  |  |  | `Boolean` |  | Supplement |  |  |
| `IsOpenItemManaged` |  |  |  |  |  | `Boolean` |  | OI Management |  |  |
| `InterestCalculationDate` |  |  |  |  |  | `Date` |  | Last Key Date |  |  |
| `IntrstCalcFrequencyInMonths` |  |  |  |  |  | `String(2)` |  | Int.Calc.Freq. |  |  |
| `AcctgDocItmDisplaySequenceRule` |  |  |  |  |  | `String(3)` |  | Sort key |  |  |
| `AlternativeGLAccount` |  |  |  |  |  | `String(10)` |  | Alternative G/L Account |  |  |
| `JointVentureRecoveryCode` |  |  |  |  |  | `String(2)` |  | Recovery Indicator |  |  |
| `CommitmentItem` |  |  |  |  |  | `String(14)` |  | Commitment item |  |  |
| `CommitmentItemShortID` |  |  |  |  |  | `String(14)` |  | Commitment Item Short ID |  |  |
| `TaxCodeIsRequired` |  |  |  |  |  | `Boolean` |  | Pstg w/o tax allowed |  |  |
| `BalanceHasLocalCurrency` |  |  |  |  |  | `Boolean` |  | Balances in LC |  |  |
| `ValuationGroup` |  |  |  |  |  | `String(10)` |  | Valuation Group |  |  |
| `APARToleranceGroup` |  |  |  |  |  | `String(4)` |  | Tolerance Group |  |  |
| `AccountIsBlockedForPosting` |  |  |  |  |  | `Boolean` |  | Posting Block |  |  |
| `AccountIsMarkedForDeletion` |  |  |  |  |  | `Boolean` |  | Deletion Flag |  |  |
| `ClearingIsLedgerGroupSpecific` |  |  |  |  |  | `Boolean` |  | OI Mgmt by LedgerGrp |  |  |
| `CashPlanningGroup` |  |  |  |  |  | `String(10)` |  | Planning Group |  |  |
| `IsCashFlowAccount` |  |  |  |  |  | `Boolean` |  | Rel.Cash Flow |  |  |
| `GLAcctInflationKey` |  |  |  |  |  | `String(8)` |  | Inflation key |  |  |
| `FieldStatusGroup` |  |  |  |  |  | `String(4)` |  | Field status group |  |  |
| `MultiCurrencyAccountingCode` |  |  |  |  |  | `String(5)` |  | MCA Key |  |  |
| `IsExtendedOpenItemManaged` |  |  |  |  |  | `Boolean` |  | Extended OI Mgmt |  |  |


## Entity: `SemanticTag`

- **ABAP CDS Name:** `I_SemanticTag`
- **Label:** Semantic Tag
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `SemanticTag` |  |  |  |  |  | `String(10)` | Y | Semantic Tag |  | S/4 only entity |
| `ParentSemanticTag` |  |  |  |  |  | `String(10)` |  | Parent Semantic Tag |  | S/4 only entity |
| `SemanticTagGroup` |  |  |  |  |  | `String(4)` |  | Semantic Tag Group |  | S/4 only entity |


## Entity: `SemanticTagFunctionalArea`

- **ABAP CDS Name:** `I_SemTagFuncArea`
- **Label:** Functional Area with Semantic Tag
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `GLAccountHierarchy` |  |  |  |  |  | `String(42)` | Y | FSV |  | S/4 only entity |
| `HierarchyNode` |  |  |  |  |  | `String(50)` | Y | Node |  | S/4 only entity |
| `SemanticTag` |  |  |  |  |  | `String(10)` | Y | Semantic Tag |  | S/4 only entity |
| `ValidityEndDate` |  |  |  |  |  | `Date` | Y | Valid To |  | S/4 only entity |
| `ValidityStartDate` |  |  |  |  |  | `Date` | Y | Valid From |  | S/4 only entity |
| `FunctionalArea` |  |  |  |  |  | `String(16)` | Y | Functional Area |  | S/4 only entity |


## Entity: `SemanticTagGeneralLedger`

- **ABAP CDS Name:** `I_SemTagGLAccount`
- **Label:** G/L Account with Semantic Tag
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `GLAccountHierarchy` |  |  |  |  |  | `String(42)` | Y | FSV |  | S/4 only entity |
| `HierarchyNode` |  |  |  |  |  | `String(50)` | Y | Node |  | S/4 only entity |
| `SemanticTag` |  |  |  |  |  | `String(10)` | Y | Semantic Tag |  | S/4 only entity |
| `ValidityEndDate` |  |  |  |  |  | `Date` | Y | Valid To |  | S/4 only entity |
| `ValidityStartDate` |  |  |  |  |  | `Date` | Y | Valid From |  | S/4 only entity |
| `ChartOfAccounts` |  |  |  |  |  | `String(4)` | Y | Chart of Accounts |  | S/4 only entity |
| `GLAccount` |  |  |  |  |  | `String(10)` | Y | G/L Account |  | S/4 only entity |
| `FunctionalAreaIsUsed` |  |  |  |  |  | `Boolean` |  | Functional Area |  | S/4 only entity |
| `IsFunctionalAreaPermitted` |  |  |  |  |  | `Boolean` |  | Fun.Area Perm. |  | S/4 only entity |


## Entity: `SemanticTagLeafNode`

- **ABAP CDS Name:** `I_SemanticTagLeafNode`
- **Label:** Hierarchy Leaf Node with Semantic Tag
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `GLAccountHierarchy` |  |  |  |  |  | `String(42)` | Y | Hierarchy ID |  | S/4 only entity |
| `HierarchyNode` |  |  |  |  |  | `String(50)` | Y | Node |  | S/4 only entity |
| `ValidityEndDate` |  |  |  |  |  | `Date` | Y | Valid To |  | S/4 only entity |
| `SemanticTag` |  |  |  |  |  | `String(10)` | Y | Semantic Tag |  | S/4 only entity |
| `ValidityStartDate` |  |  |  |  |  | `Date` |  | Valid From |  | S/4 only entity |
| `ChartOfAccounts` |  |  |  |  |  | `String(4)` |  | Chart of Accounts |  | S/4 only entity |
| `GLAccount` |  |  |  |  |  | `String(10)` |  | G/L Account |  | S/4 only entity |
| `FunctionalArea` |  |  |  |  |  | `String(16)` |  | Functional Area |  | S/4 only entity |


## Entity: `SemanticTagText`

- **ABAP CDS Name:** `I_SemanticTagText`
- **Label:** Semantic Tag - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Language` |  |  |  |  |  | `String(2)` | Y | Language Key |  | S/4 only entity |
| `SemanticTag` |  |  |  |  |  | `String(10)` | Y | Semantic Tag |  | S/4 only entity |
| `SemanticTagName` |  |  |  |  |  | `String(20)` |  | Semantic Tag Name |  | S/4 only entity |
