# GeneralLedgerAccount

> Source file: `sap-s4com-GeneralLedgerAccount-v1.json`


## Entity: `ChartOfAccounts`

- **ABAP Name:** `I_ChartOfAccounts`
- **Label:** Chart Of Accounts
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `ChartOfAccounts` | `ChartOfAccounts` | `String(4)` | Y | Chart of Accounts |  |  | S/4 only entity (no ECC CDC mapping) |
| `CorporateGroupChartOfAccounts` | `CorporateGroupChartOfAccounts` | `String(4)` |  | Group Chart of Accts |  |  | S/4 only entity (no ECC CDC mapping) |
| `ChartOfAcctsIsBlocked` | `ChartOfAcctsIsBlocked` | `Boolean` |  | Blocked |  |  | S/4 only entity (no ECC CDC mapping) |
| `MaintenanceLanguage` | `MaintenanceLanguage` | `String(2)` |  | Maint.Language |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `ChartOfAccountsText`

- **ABAP Name:** `I_ChartOfAccountsText`
- **Label:** Chart Of Accounts - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `ChartOfAccounts` | `ChartOfAccounts` | `String(4)` | Y | Chart of Accounts |  | _ChartOfAccounts | S/4 only entity (no ECC CDC mapping) |
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `ChartOfAccountsName` | `ChartOfAccountsName` | `String(50)` |  | Chart of Accounts Description |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `FinancialStatementHierNode`

- **ABAP Name:** `I_FinancialStatementHierNode`
- **Label:** Financial Statement Hierarchy Node
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `FinancialStatementHierarchy` | `FinancialStatementHierarchy` | `String(42)` | Y | Hierarchy ID |  | _Hierarchy | S/4 only entity (no ECC CDC mapping) |
| `HierarchyNode` | `HierarchyNode` | `String(50)` | Y | Node |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityEndDate` | `ValidityEndDate` | `Date` | Y | Valid To |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityStartDate` | `ValidityStartDate` | `Date` |  | Validity Start Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `ParentNode` | `ParentNode` | `String(50)` |  | Par. Node |  |  | S/4 only entity (no ECC CDC mapping) |
| `HierarchyVersion` | `HierarchyVersion` | `String(15)` |  | Version |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinancialStatementLeafItem` | `FinancialStatementLeafItem` | `String(50)` |  | Node |  |  | S/4 only entity (no ECC CDC mapping) |
| `SequenceNumber` | `SequenceNumber` | `String(56)` |  |  |  |  | S/4 only entity (no ECC CDC mapping) |
| `SignIsInverted` | `SignIsInverted` | `Boolean` |  | Attribute Value |  |  | S/4 only entity (no ECC CDC mapping) |
| `ChartOfAccounts` | `ChartOfAccounts` | `String(12)` |  | Node Class |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinancialStatementNodeType` | `FinancialStatementNodeType` | `String(1)` |  | Node Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinStmntNodeFormattedID` | `FinStmntNodeFormattedID` | `String(32)` |  | Node for Extraction |  |  | S/4 only entity (no ECC CDC mapping) |
| `HierarchyNodeVal` | `HierarchyNodeVal` | `String(40)` |  | Value |  |  | S/4 only entity (no ECC CDC mapping) |
| `HierarchyNodeSequence` | `HierarchyNodeSequence` | `String(6)` |  | Sequence Number |  |  | S/4 only entity (no ECC CDC mapping) |
| `HierarchyLevel` | `HierarchyLevel` | `String(6)` |  | Hierarchy Level |  |  | S/4 only entity (no ECC CDC mapping) |
| `DebitCreditCode` | `DebitCreditCode` | `String(1)` |  | Balance |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `FinancialStatementHierNodeText`

- **ABAP Name:** `I_FinancialStatementHierNodeT`
- **Label:** Financial Statement Hierarchy Node - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `FinancialStatementHierarchy` | `FinancialStatementHierarchy` | `String(42)` | Y | Hierarchy ID |  | _Hierarchy | S/4 only entity (no ECC CDC mapping) |
| `HierarchyNode` | `HierarchyNode` | `String(50)` | Y | Node |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityEndDate` | `ValidityEndDate` | `Date` | Y | Valid To |  |  | S/4 only entity (no ECC CDC mapping) |
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `HierarchyNodeText` | `HierarchyNodeText` | `String(50)` |  | Description |  |  | S/4 only entity (no ECC CDC mapping) |
| `HierarchyNodeShortText` | `HierarchyNodeShortText` | `String(20)` |  |  |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityStartDate` | `ValidityStartDate` | `Date` |  | Valid From |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinStmntNodeFormattedID` | `FinStmntNodeFormattedID` | `String(32)` |  | Node for Extraction |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `FinancialStatementHierText`

- **ABAP Name:** `I_FinancialStatementHierT`
- **Label:** Financial Statement Hierarchy - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `FinancialStatementHierarchy` | `FinancialStatementHierarchy` | `String(42)` | Y | Hierarchy ID |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityEndDate` | `ValidityEndDate` | `Date` | Y | Valid To |  |  | S/4 only entity (no ECC CDC mapping) |
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityStartDate` | `ValidityStartDate` | `Date` |  | Valid From |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinancialStmntHierarchyName` | `FinancialStmntHierarchyName` | `String(50)` |  | Financial Statement Description |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `FinancialStatementHierarchy`

- **ABAP Name:** `I_FinancialStatementHier`
- **Label:** Financial Statement Hierarchy
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `FinancialStatementHierarchy` | `FinancialStatementHierarchy` | `String(42)` | Y | Hierarchy ID |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityEndDate` | `ValidityEndDate` | `Date` | Y | Validity End Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityStartDate` | `ValidityStartDate` | `Date` |  | Validity Start Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `HierarchyType` | `HierarchyType` | `String(4)` |  | Hierarchy Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `LastChangedByUser` | `LastChangedByUser` | `String(12)` |  | Last Changed By |  |  | S/4 only entity (no ECC CDC mapping) |
| `LastChangeTime` | `LastChangeTime` | `DateTime` |  | Updated At |  |  | S/4 only entity (no ECC CDC mapping) |
| `LastChangeDateTime` | `LastChangeDateTime` | `DateTime` |  | Updated At |  |  | S/4 only entity (no ECC CDC mapping) |
| `ChartOfAccounts` | `ChartOfAccounts` | `String(80)` |  | Char80 |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinancialStatementAssetsItem` | `FinancialStatementAssetsItem` | `String(80)` |  | Char80 |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinStatementLiabilitiesItem` | `FinStatementLiabilitiesItem` | `String(80)` |  | Char80 |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinancialStatementNetLossItem` | `FinancialStatementNetLossItem` | `String(80)` |  | Char80 |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinStatementNetProfitItem` | `FinStatementNetProfitItem` | `String(80)` |  | Char80 |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinStatementProfitAndLossItem` | `FinStatementProfitAndLossItem` | `String(80)` |  | Char80 |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinancialStatementOrphansItem` | `FinancialStatementOrphansItem` | `String(80)` |  | Char80 |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinancialStatementNotesItem` | `FinancialStatementNotesItem` | `String(80)` |  | Char80 |  |  | S/4 only entity (no ECC CDC mapping) |
| `GroupChartOfAccountIsUsed` | `GroupChartOfAccountIsUsed` | `Boolean` |  | Char80 |  |  | S/4 only entity (no ECC CDC mapping) |
| `FunctionalAreaIsUsed` | `FunctionalAreaIsUsed` | `Boolean` |  | Char80 |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `GLAccountHierNodeBySemanticTag`

- **ABAP Name:** `I_GLAccountHierNodeBySemTag`
- **Label:** GLAccount Hierarchy Node By Semantic Tag
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `GLAccountHierarchy` | `GLAccountHierarchy` | `String(42)` | Y | Hierarchy ID |  | _Hierarchy | S/4 only entity (no ECC CDC mapping) |
| `HierarchyNode` | `HierarchyNode` | `String(50)` | Y | Node |  |  | S/4 only entity (no ECC CDC mapping) |
| `SemanticTag` | `SemanticTag` | `String(10)` | Y | Semantic Tag |  | _SemanticTag | S/4 only entity (no ECC CDC mapping) |
| `HierarchyNodeType` | `HierarchyNodeType` | `String(30)` |  | Field Name |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `GLAccountHierarchyNode`

- **ABAP Name:** `I_GLAccountHierarchyNode`
- **Label:** G/L Account Hierarchy Node
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `GLAccountHierarchy` | `GLAccountHierarchy` | `String(42)` | Y | G/L Account Hierarchy |  | _Hierarchy | S/4 only entity (no ECC CDC mapping) |
| `HierarchyNode` | `HierarchyNode` | `String(50)` | Y | Node |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityEndDate` | `ValidityEndDate` | `Date` | Y | Validity End Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `ParentNode` | `ParentNode` | `String(50)` |  | Par. Node |  |  | S/4 only entity (no ECC CDC mapping) |
| `HierarchyVersion` | `HierarchyVersion` | `String(15)` |  | Version |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityStartDate` | `ValidityStartDate` | `Date` |  | Validity Start Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `ChartOfAccounts` | `ChartOfAccounts` | `String(4)` |  | Chart of Accounts |  | _ChartOfAccounts | S/4 only entity (no ECC CDC mapping) |
| `GLAccount` | `GLAccount` | `String(10)` |  | G/L Account |  | _GLAccountInChartOfAccounts | S/4 only entity (no ECC CDC mapping) |
| `SequenceNumber` | `SequenceNumber` | `String(56)` |  |  |  |  | S/4 only entity (no ECC CDC mapping) |
| `HierarchyNodeSequence` | `HierarchyNodeSequence` | `String(6)` |  | Sequence Number |  |  | S/4 only entity (no ECC CDC mapping) |
| `HierarchyNodeLevel` | `HierarchyNodeLevel` | `String(6)` |  | Hierarchy Level |  |  | S/4 only entity (no ECC CDC mapping) |
| `NodeType` | `NodeType` | `String(1)` |  | Node Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `SignIsInverted` | `SignIsInverted` | `Boolean` |  | Attribute Value |  |  | S/4 only entity (no ECC CDC mapping) |
| `HierarchyNodeVal` | `HierarchyNodeVal` | `String(40)` |  | Value |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `GLAccountHierarchyNodeText`

- **ABAP Name:** `I_GLAccountHierarchyNodeT`
- **Label:** G/L Account Hierarchy Node - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `GLAccountHierarchy` | `GLAccountHierarchy` | `String(42)` | Y | G/L Account Hierarchy |  | _Hierarchy | S/4 only entity (no ECC CDC mapping) |
| `HierarchyNode` | `HierarchyNode` | `String(50)` | Y | Node |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityEndDate` | `ValidityEndDate` | `Date` | Y | Valid To |  |  | S/4 only entity (no ECC CDC mapping) |
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `HierarchyNodeText` | `HierarchyNodeText` | `String(50)` |  | Description |  |  | S/4 only entity (no ECC CDC mapping) |
| `HierarchyNodeShortText` | `HierarchyNodeShortText` | `String(20)` |  |  |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityStartDate` | `ValidityStartDate` | `Date` |  | Valid From |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `GLAccountHierarchyText`

- **ABAP Name:** `I_GLAccountHierarchyText`
- **Label:** G/L Account Hierarchy - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `GLAccountHierarchy` | `GLAccountHierarchy` | `String(42)` | Y | G/L Account Hierarchy |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityEndDate` | `ValidityEndDate` | `Date` | Y | Valid To |  |  | S/4 only entity (no ECC CDC mapping) |
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityStartDate` | `ValidityStartDate` | `Date` |  | Valid From |  |  | S/4 only entity (no ECC CDC mapping) |
| `GLAccountHierarchyName` | `GLAccountHierarchyName` | `String(50)` |  | Description |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `GLAccountTypeFlowType`

- **ABAP Name:** `I_GLAccountTypeFlowType`
- **Label:** Flow Type for G/L Account Type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `GLAccountTypeFlowType` | `GLAccountTypeFlowType` | `String(12)` | Y | GLAcct Type FlowType |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `GeneralLedgerAccount`

- **ABAP Name:** `I_GLAccountInChartOfAccounts`
- **Label:** G/L Account In Chart Of Accounts
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `ChartOfAccounts` | `ChartOfAccounts` | `String(4)` | Y | Chart of Accounts |  | _ChartOfAccounts | S/4 only entity (no ECC CDC mapping) |
| `GLAccount` | `GLAccount` | `String(10)` | Y | G/L Account |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsBalanceSheetAccount` | `IsBalanceSheetAccount` | `Boolean` |  | Balance sheet acct |  |  | S/4 only entity (no ECC CDC mapping) |
| `GLAccountGroup` | `GLAccountGroup` | `String(4)` |  | Account Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `CorporateGroupChartOfAccounts` | `CorporateGroupChartOfAccounts` | `String(4)` |  | Group Chart of Accts |  | _CorporateGroupChartOfAccounts | S/4 only entity (no ECC CDC mapping) |
| `CorporateGroupAccount` | `CorporateGroupAccount` | `String(10)` |  | Group Account Number |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProfitLossAccountType` | `ProfitLossAccountType` | `String(2)` |  | P&L state. acct |  |  | S/4 only entity (no ECC CDC mapping) |
| `SampleGLAccount` | `SampleGLAccount` | `String(10)` |  | Sample Account |  |  | S/4 only entity (no ECC CDC mapping) |
| `AccountIsMarkedForDeletion` | `AccountIsMarkedForDeletion` | `Boolean` |  | Deletion Flag |  |  | S/4 only entity (no ECC CDC mapping) |
| `AccountIsBlockedForCreation` | `AccountIsBlockedForCreation` | `Boolean` |  | Creation Block |  |  | S/4 only entity (no ECC CDC mapping) |
| `AccountIsBlockedForPosting` | `AccountIsBlockedForPosting` | `Boolean` |  | Posting Block |  |  | S/4 only entity (no ECC CDC mapping) |
| `AccountIsBlockedForPlanning` | `AccountIsBlockedForPlanning` | `Boolean` |  | Planning Block |  |  | S/4 only entity (no ECC CDC mapping) |
| `PartnerCompany` | `PartnerCompany` | `String(6)` |  | Trading Partner No. |  |  | S/4 only entity (no ECC CDC mapping) |
| `FunctionalArea` | `FunctionalArea` | `String(16)` |  | Functional Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `CreationDate` | `CreationDate` | `Date` |  | Created On |  |  | S/4 only entity (no ECC CDC mapping) |
| `CreatedByUser` | `CreatedByUser` | `String(12)` |  | Created By |  |  | S/4 only entity (no ECC CDC mapping) |
| `LastChangeDateTime` | `LastChangeDateTime` | `DateTime` |  | Time Stamp |  |  | S/4 only entity (no ECC CDC mapping) |
| `GLAccountType` | `GLAccountType` | `String(1)` |  | G/L Account Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `GLAccountSubtype` | `GLAccountSubtype` | `String(1)` |  | G/L Account Subtype |  |  | S/4 only entity (no ECC CDC mapping) |
| `GLAccountExternal` | `GLAccountExternal` | `String(10)` |  | G/L Acct External ID |  |  | S/4 only entity (no ECC CDC mapping) |
| `BankReconciliationAccount` | `BankReconciliationAccount` | `String(10)` |  | Reconciliation Acct |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsProfitLossAccount` | `IsProfitLossAccount` | `Boolean` |  | Profit Loss Account |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `GeneralLedgerAccountFlowType`

- **ABAP Name:** `I_GLAccountFlowType`
- **Label:** GLAccount Flow Type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `GLAccountFlowType` | `GLAccountFlowType` | `String(10)` | Y | G/L Acct. Flow Type |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `GeneralLedgerAccountHierarchy`

- **ABAP Name:** `I_GLAccountHierarchy`
- **Label:** General Ledger Account Hierarchy
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `GLAccountHierarchy` | `GLAccountHierarchy` | `String(42)` | Y | G/L Account Hierarchy |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityEndDate` | `ValidityEndDate` | `Date` | Y | Valid To |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityStartDate` | `ValidityStartDate` | `Date` |  | Valid From |  |  | S/4 only entity (no ECC CDC mapping) |
| `HierarchyType` | `HierarchyType` | `String(4)` |  | Hierarchy Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `LastChangedByUser` | `LastChangedByUser` | `String(12)` |  | Last Changed By |  |  | S/4 only entity (no ECC CDC mapping) |
| `LastChangeTime` | `LastChangeTime` | `DateTime` |  | Updated At |  |  | S/4 only entity (no ECC CDC mapping) |
| `LastChangeDateTime` | `LastChangeDateTime` | `DateTime` |  | Updated At |  |  | S/4 only entity (no ECC CDC mapping) |
| `HierarchyShortID` | `HierarchyShortID` | `String(20)` |  | Hierarchy ID |  |  | S/4 only entity (no ECC CDC mapping) |
| `FunctionalAreaIsUsed` | `FunctionalAreaIsUsed` | `Boolean` |  | Functional Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `SemanticTagIsUsed` | `SemanticTagIsUsed` | `Boolean` |  | Sem. Tag Assigned |  |  | S/4 only entity (no ECC CDC mapping) |
| `ChartOfAccounts` | `ChartOfAccounts` | `String(4)` |  | Chart of Accounts |  | _ChartOfAccounts | S/4 only entity (no ECC CDC mapping) |


## Entity: `GeneralLedgerAccountLineItem`

- **ABAP Name:** `I_GLAccountLineItemRawData`
- **Label:** Raw Data of G/L Account Line Item
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `SourceLedger` | `SourceLedger` | `String(2)` | Y | Source Ledger |  |  | S/4 only — no ECC equivalent; S/4 only entity (no ECC CDC mapping); S/4 only — use filter SourceLedger='0L' for leading ledger |
| `CompanyCode` | `CompanyCode` | `String(4)` | Y | Company Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `FiscalYear` | `FiscalYear` | `String(4)` | Y | Fiscal Year |  |  | S/4 only entity (no ECC CDC mapping) |
| `AccountingDocument` | `AccountingDocument` | `String(10)` | Y | Journal Entry |  |  | S/4 only entity (no ECC CDC mapping) |
| `LedgerGLLineItem` | `LedgerGLLineItem` | `String(6)` | Y | Journal Entry Item |  |  | S/4 only entity (no ECC CDC mapping) |
| `LedgerFiscalYear` | `LedgerFiscalYear` | `String(4)` |  | Fiscal Year of Ledger |  |  | S/4 only — no ECC equivalent; S/4 only entity (no ECC CDC mapping) |
| `GLRecordType` | `GLRecordType` | `String(1)` |  | Record Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `JrnlEntrAltvFYConsecutiveID` | `JrnlEntrAltvFYConsecutiveID` | `String(10)` |  | Shifted Fiscal Year Consecutive ID |  |  | S/4 only entity (no ECC CDC mapping) |
| `ChartOfAccounts` | `ChartOfAccounts` | `String(4)` |  | Chart of Accounts |  | _ChartOfAccounts | S/4 only entity (no ECC CDC mapping) |
| `ControllingArea` | `ControllingArea` | `String(4)` |  | Controlling Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinancialTransactionType` | `FinancialTransactionType` | `String(3)` |  | Financial Transaction Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `GLBusinessTransactionType` | `GLBusinessTransactionType` | `String(4)` |  | Transaction Type for General Ledger |  |  | S/4 only entity (no ECC CDC mapping) |
| `BusinessTransactionCategory` | `BusinessTransactionCategory` | `String(4)` |  | Business Transaction Category |  |  | S/4 only entity (no ECC CDC mapping) |
| `BusinessTransactionType` | `BusinessTransactionType` | `String(4)` |  | Business Transaction Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinancialClosingStep` | `FinancialClosingStep` | `String(3)` |  | Financial Closing Step |  |  | S/4 only entity (no ECC CDC mapping) |
| `ControllingBusTransacType` | `ControllingBusTransacType` | `String(4)` |  | Business Transaction |  |  | S/4 only entity (no ECC CDC mapping) |
| `ReferenceDocumentType` | `ReferenceDocumentType` | `String(5)` |  | Reference Document Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `LogicalSystem` | `LogicalSystem` | `String(10)` |  | Logical System |  |  | S/4 only entity (no ECC CDC mapping) |
| `ReferenceDocumentContext` | `ReferenceDocumentContext` | `String(10)` |  | Reference Document Context |  |  | S/4 only entity (no ECC CDC mapping) |
| `ReferenceDocument` | `ReferenceDocument` | `String(10)` |  | Reference Document |  |  | S/4 only entity (no ECC CDC mapping) |
| `ReferenceDocumentItem` | `ReferenceDocumentItem` | `String(6)` |  | Reference Document Item |  |  | S/4 only entity (no ECC CDC mapping) |
| `ReferenceDocumentItemGroup` | `ReferenceDocumentItemGroup` | `String(6)` |  | Reference Document Item Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `TransactionSubitem` | `TransactionSubitem` | `String(6)` |  | Sub Transaction |  |  | S/4 only entity (no ECC CDC mapping) |
| `AccountingNotificationUUID` | `AccountingNotificationUUID` | `UUID` |  | Accounting Notification UUID |  |  | S/4 only entity (no ECC CDC mapping) |
| `OffsettingLedgerGLLineItem` | `OffsettingLedgerGLLineItem` | `String(6)` |  | G/L Offsetting Entry Line Item |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsReversal` | `IsReversal` | `Boolean` |  | Is Reversing |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsReversed` | `IsReversed` | `Boolean` |  | Is Reversed |  |  | S/4 only entity (no ECC CDC mapping) |
| `ReversalReferenceDocumentType` | `ReversalReferenceDocumentType` | `String(5)` |  | Reversal Reference Document Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `ReversalReferenceDocumentCntxt` | `ReversalReferenceDocumentCntxt` | `String(10)` |  | Reversal Reference Document Context |  |  | S/4 only entity (no ECC CDC mapping) |
| `ReversalReferenceDocument` | `ReversalReferenceDocument` | `String(10)` |  | Reversal Reference Document |  |  | S/4 only entity (no ECC CDC mapping) |
| `ReversalTransactionSubitem` | `ReversalTransactionSubitem` | `String(6)` |  | Reversal Transaction Sub Item |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsSettlement` | `IsSettlement` | `Boolean` |  | Is Settling |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsSettled` | `IsSettled` | `Boolean` |  | Is Settled |  |  | S/4 only entity (no ECC CDC mapping) |
| `PredecessorReferenceDocType` | `PredecessorReferenceDocType` | `String(5)` |  | Predecessor Reference Document Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `PredecessorReferenceDocCntxt` | `PredecessorReferenceDocCntxt` | `String(10)` |  | Predecessor Reference Document Context |  |  | S/4 only entity (no ECC CDC mapping) |
| `PredecessorReferenceDocument` | `PredecessorReferenceDocument` | `String(10)` |  | Predecessor Reference Document |  |  | S/4 only entity (no ECC CDC mapping) |
| `PredecessorReferenceDocItem` | `PredecessorReferenceDocItem` | `String(6)` |  | Predecessor Reference Document Item |  |  | S/4 only entity (no ECC CDC mapping) |
| `PrdcssrJournalEntryCompanyCode` | `PrdcssrJournalEntryCompanyCode` | `String(4)` |  | Predecessor Journal Entry Company Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `PrdcssrJournalEntryFiscalYear` | `PrdcssrJournalEntryFiscalYear` | `String(4)` |  | Predecessor Journal Entry Fiscal Year |  |  | S/4 only entity (no ECC CDC mapping) |
| `PredecessorJournalEntry` | `PredecessorJournalEntry` | `String(10)` |  | Predecessor Journal Entry |  |  | S/4 only entity (no ECC CDC mapping) |
| `PredecessorJournalEntryItem` | `PredecessorJournalEntryItem` | `String(6)` |  | Predecessor Journal Entry Item |  |  | S/4 only entity (no ECC CDC mapping) |
| `SourceReferenceDocumentType` | `SourceReferenceDocumentType` | `String(5)` |  | Source Reference Document Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `SourceLogicalSystem` | `SourceLogicalSystem` | `String(10)` |  | Source Logical System |  |  | S/4 only entity (no ECC CDC mapping) |
| `SourceReferenceDocumentCntxt` | `SourceReferenceDocumentCntxt` | `String(10)` |  | Source Reference Document Context |  |  | S/4 only entity (no ECC CDC mapping) |
| `SourceReferenceDocument` | `SourceReferenceDocument` | `String(10)` |  | Source Reference Document |  |  | S/4 only entity (no ECC CDC mapping) |
| `SourceReferenceDocumentItem` | `SourceReferenceDocumentItem` | `String(6)` |  | Source Reference Document Item |  |  | S/4 only entity (no ECC CDC mapping) |
| `SourceReferenceDocSubitem` | `SourceReferenceDocSubitem` | `String(6)` |  | Source Reference Document Subitem |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsCommitment` | `IsCommitment` | `Boolean` |  | Is Commitment |  |  | S/4 only entity (no ECC CDC mapping) |
| `JrnlEntryItemObsoleteReason` | `JrnlEntryItemObsoleteReason` | `String(1)` |  | Obsolete Reason |  |  | S/4 only entity (no ECC CDC mapping) |
| `JournalEntryIsSecondaryEntry` | `JournalEntryIsSecondaryEntry` | `Boolean` |  | Is Secondary Journal Entry |  |  | S/4 only entity (no ECC CDC mapping) |
| `JrnlPeriodEndClosingRunLogUUID` | `JrnlPeriodEndClosingRunLogUUID` | `UUID` |  | Closing Run UUID |  |  | S/4 only entity (no ECC CDC mapping) |
| `OrganizationalChange` | `OrganizationalChange` | `String(10)` |  | Organizational Change |  |  | S/4 only entity (no ECC CDC mapping) |
| `GLAccount` | `GLAccount` | `String(10)` |  | G/L Account |  | _GLAccountInChartOfAccounts | S/4 only entity (no ECC CDC mapping) |
| `CostCenter` | `CostCenter` | `String(10)` |  | Cost Center |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProfitCenter` | `ProfitCenter` | `String(10)` |  | Profit Center |  |  | S/4 only entity (no ECC CDC mapping) |
| `FunctionalArea` | `FunctionalArea` | `String(16)` |  | Functional Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `BusinessArea` | `BusinessArea` | `String(4)` |  | Business Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `Segment` | `Segment` | `String(10)` |  | Segment |  |  | S/4 only entity (no ECC CDC mapping) |
| `PartnerCostCenter` | `PartnerCostCenter` | `String(10)` |  | Partner Cost Center |  |  | S/4 only entity (no ECC CDC mapping) |
| `PartnerProfitCenter` | `PartnerProfitCenter` | `String(10)` |  | Partner Profit Center |  |  | S/4 only entity (no ECC CDC mapping) |
| `PartnerFunctionalArea` | `PartnerFunctionalArea` | `String(16)` |  | Partner Func. Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `PartnerBusinessArea` | `PartnerBusinessArea` | `String(4)` |  | Partner Bus. Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `PartnerCompany` | `PartnerCompany` | `String(6)` |  | Trading Partner |  |  | S/4 only entity (no ECC CDC mapping) |
| `PartnerSegment` | `PartnerSegment` | `String(10)` |  | Partner Segment |  |  | S/4 only entity (no ECC CDC mapping) |
| `BalanceTransactionCurrency` | `BalanceTransactionCurrency` | `String(5)` |  | Balance Transaction Currency |  |  | S/4 only entity (no ECC CDC mapping) |
| `AmountInBalanceTransacCrcy` | `AmountInBalanceTransacCrcy` | `Decimal(34,4)` |  | Amount in Balance Transaction Currency | BalanceTransactionCurrency |  | S/4 only entity (no ECC CDC mapping) |
| `TransactionCurrency` | `TransactionCurrency` | `String(5)` |  | Transaction Currency |  |  | S/4 only entity (no ECC CDC mapping) |
| `AmountInTransactionCurrency` | `AmountInTransactionCurrency` | `Decimal(34,4)` |  | Amount in Transaction Currency | TransactionCurrency |  | S/4 only entity (no ECC CDC mapping) |
| `CompanyCodeCurrency` | `CompanyCodeCurrency` | `String(5)` |  | Company Code Currency |  |  | S/4 only entity (no ECC CDC mapping) |
| `AmountInCompanyCodeCurrency` | `AmountInCompanyCodeCurrency` | `Decimal(34,4)` |  | Amount in Company Code Currency | CompanyCodeCurrency |  | S/4 only entity (no ECC CDC mapping) |
| `GlobalCurrency` | `GlobalCurrency` | `String(5)` |  | Global Currency |  |  | S/4 only — no ECC equivalent; S/4 only entity (no ECC CDC mapping); S/4 only — ECC BSEG lacks global currency |
| `AmountInGlobalCurrency` | `AmountInGlobalCurrency` | `Decimal(34,4)` |  | Amount in Global Currency | GlobalCurrency |  | S/4 only — no ECC equivalent; S/4 only entity (no ECC CDC mapping); S/4 only — ECC BSEG lacks global currency |
| `FunctionalCurrency` | `FunctionalCurrency` | `String(5)` |  | Functional Currency |  |  | S/4 only entity (no ECC CDC mapping) |
| `AmountInFunctionalCurrency` | `AmountInFunctionalCurrency` | `Decimal(34,4)` |  | Amount in Functional Currency | FunctionalCurrency |  | S/4 only entity (no ECC CDC mapping) |
| `FreeDefinedCurrency1` | `FreeDefinedCurrency1` | `String(5)` |  | Freely Defined Currency 1 |  |  | S/4 only — no ECC equivalent; S/4 only entity (no ECC CDC mapping) |
| `AmountInFreeDefinedCurrency1` | `AmountInFreeDefinedCurrency1` | `Decimal(34,4)` |  | Amount in Freely Defined Currency 1 | FreeDefinedCurrency1 |  | S/4 only — no ECC equivalent; S/4 only entity (no ECC CDC mapping) |
| `FreeDefinedCurrency2` | `FreeDefinedCurrency2` | `String(5)` |  | Freely Defined Currency 2 |  |  | S/4 only — no ECC equivalent; S/4 only entity (no ECC CDC mapping) |
| `AmountInFreeDefinedCurrency2` | `AmountInFreeDefinedCurrency2` | `Decimal(34,4)` |  | Amount in Freely Defined Currency 2 | FreeDefinedCurrency2 |  | S/4 only — no ECC equivalent; S/4 only entity (no ECC CDC mapping) |
| `FreeDefinedCurrency3` | `FreeDefinedCurrency3` | `String(5)` |  | Freely Defined Currency 3 |  |  | S/4 only — no ECC equivalent; S/4 only entity (no ECC CDC mapping) |
| `AmountInFreeDefinedCurrency3` | `AmountInFreeDefinedCurrency3` | `Decimal(34,4)` |  | Amount in Freely Defined Currency 3 | FreeDefinedCurrency3 |  | S/4 only — no ECC equivalent; S/4 only entity (no ECC CDC mapping) |
| `FreeDefinedCurrency4` | `FreeDefinedCurrency4` | `String(5)` |  | Freely Defined Currency 4 |  |  | S/4 only entity (no ECC CDC mapping) |
| `AmountInFreeDefinedCurrency4` | `AmountInFreeDefinedCurrency4` | `Decimal(34,4)` |  | Amount in Freely Defined Currency 4 | FreeDefinedCurrency4 |  | S/4 only entity (no ECC CDC mapping) |
| `FreeDefinedCurrency5` | `FreeDefinedCurrency5` | `String(5)` |  | Freely Defined Currency 5 |  |  | S/4 only entity (no ECC CDC mapping) |
| `AmountInFreeDefinedCurrency5` | `AmountInFreeDefinedCurrency5` | `Decimal(34,4)` |  | Amount in Freely Defined Currency 5 | FreeDefinedCurrency5 |  | S/4 only entity (no ECC CDC mapping) |
| `FreeDefinedCurrency6` | `FreeDefinedCurrency6` | `String(5)` |  | Freely Defined Currency 6 |  |  | S/4 only entity (no ECC CDC mapping) |
| `AmountInFreeDefinedCurrency6` | `AmountInFreeDefinedCurrency6` | `Decimal(34,4)` |  | Amount in Freely Defined Currency 6 | FreeDefinedCurrency6 |  | S/4 only entity (no ECC CDC mapping) |
| `FreeDefinedCurrency7` | `FreeDefinedCurrency7` | `String(5)` |  | Freely Defined Currency 7 |  |  | S/4 only entity (no ECC CDC mapping) |
| `AmountInFreeDefinedCurrency7` | `AmountInFreeDefinedCurrency7` | `Decimal(34,4)` |  | Amount in Freely Defined Currency 7 | FreeDefinedCurrency7 |  | S/4 only entity (no ECC CDC mapping) |
| `FreeDefinedCurrency8` | `FreeDefinedCurrency8` | `String(5)` |  | Freely Defined Currency 8 |  |  | S/4 only entity (no ECC CDC mapping) |
| `AmountInFreeDefinedCurrency8` | `AmountInFreeDefinedCurrency8` | `Decimal(34,4)` |  | Amount in Freely Defined Currency 8 | FreeDefinedCurrency8 |  | S/4 only entity (no ECC CDC mapping) |
| `FixedAmountInGlobalCrcy` | `FixedAmountInGlobalCrcy` | `Decimal(34,4)` |  | Fixed Amount in Global Currency | GlobalCurrency |  | S/4 only entity (no ECC CDC mapping); S/4 only — ECC BSEG lacks global currency |
| `GrpValnFixedAmtInGlobCrcy` | `GrpValnFixedAmtInGlobCrcy` | `Decimal(34,4)` |  | Group Val. Fixed Amount in Global Cur. | GlobalCurrency |  | S/4 only entity (no ECC CDC mapping) |
| `PrftCtrValnFxdAmtInGlobCrcy` | `PrftCtrValnFxdAmtInGlobCrcy` | `Decimal(34,4)` |  | PC Val. Fixed Amount in Global Currency | GlobalCurrency |  | S/4 only entity (no ECC CDC mapping) |
| `FixedAmountInCoCodeCrcy` | `FixedAmountInCoCodeCrcy` | `Decimal(34,4)` |  | Fixed Amount in Company Currency | CompanyCodeCurrency |  | S/4 only entity (no ECC CDC mapping) |
| `FixedAmountInTransCrcy` | `FixedAmountInTransCrcy` | `Decimal(34,4)` |  | Fixed Amount in Transaction Currency | TransactionCurrency |  | S/4 only entity (no ECC CDC mapping) |
| `TotalPriceVarcInGlobalCrcy` | `TotalPriceVarcInGlobalCrcy` | `Decimal(34,4)` |  | Total Price Variance in Global Currency | GlobalCurrency |  | S/4 only entity (no ECC CDC mapping) |
| `GrpValnTotPrcVarcInGlobCrcy` | `GrpValnTotPrcVarcInGlobCrcy` | `Decimal(34,4)` |  | GV Total Price Var. in Global Currency | GlobalCurrency |  | S/4 only entity (no ECC CDC mapping) |
| `PrftCtrValnTotPrcVarcInGlbCrcy` | `PrftCtrValnTotPrcVarcInGlbCrcy` | `Decimal(34,4)` |  | PC Val. Total Price Var. in Global Cur. | GlobalCurrency |  | S/4 only entity (no ECC CDC mapping) |
| `FixedPriceVarcInGlobalCrcy` | `FixedPriceVarcInGlobalCrcy` | `Decimal(34,4)` |  | Fixed Price Variance in Global Currency | GlobalCurrency |  | S/4 only entity (no ECC CDC mapping) |
| `GrpValnFixedPrcVarcInGlobCrcy` | `GrpValnFixedPrcVarcInGlobCrcy` | `Decimal(34,4)` |  | GV Fixed Price Var. in Global Currency | GlobalCurrency |  | S/4 only entity (no ECC CDC mapping) |
| `PrftCtrValnFxdPrcVarcInGlbCrcy` | `PrftCtrValnFxdPrcVarcInGlbCrcy` | `Decimal(34,4)` |  | PC Val. Fixed Price Var. in Global Cur. | GlobalCurrency |  | S/4 only entity (no ECC CDC mapping) |
| `ControllingObjectCurrency` | `ControllingObjectCurrency` | `String(5)` |  | CO Object Currency |  |  | S/4 only entity (no ECC CDC mapping) |
| `AmountInObjectCurrency` | `AmountInObjectCurrency` | `Decimal(34,4)` |  | Amount in Object Currency | ControllingObjectCurrency |  | S/4 only entity (no ECC CDC mapping) |
| `GrantCurrency` | `GrantCurrency` | `String(5)` |  | Grant Currency |  |  | S/4 only entity (no ECC CDC mapping) |
| `AmountInGrantCurrency` | `AmountInGrantCurrency` | `Decimal(34,4)` |  | Amount in Grant Crcy | GrantCurrency |  | S/4 only entity (no ECC CDC mapping) |
| `BaseUnit` | `BaseUnit` | `String(3)` |  | Base Unit of Measure |  |  | S/4 only entity (no ECC CDC mapping) |
| `Quantity` | `Quantity` | `Decimal(23,3)` |  | Quantity | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `FixedQuantity` | `FixedQuantity` | `Decimal(23,3)` |  | Fixed Quantity | BaseUnit |  | S/4 only entity (no ECC CDC mapping) |
| `CostSourceUnit` | `CostSourceUnit` | `String(3)` |  | Cost Source Unit |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValuationQuantity` | `ValuationQuantity` | `Decimal(23,3)` |  | Valuation Quantity | CostSourceUnit |  | S/4 only entity (no ECC CDC mapping) |
| `ValuationFixedQuantity` | `ValuationFixedQuantity` | `Decimal(23,3)` |  | Valuation Fixed Quantity | CostSourceUnit |  | S/4 only entity (no ECC CDC mapping) |
| `ReferenceQuantityUnit` | `ReferenceQuantityUnit` | `String(3)` |  | Reference Qty UoM |  |  | S/4 only entity (no ECC CDC mapping) |
| `ReferenceQuantity` | `ReferenceQuantity` | `Decimal(23,3)` |  | Reference quantity | ReferenceQuantityUnit |  | S/4 only entity (no ECC CDC mapping) |
| `AdditionalQuantity1Unit` | `AdditionalQuantity1Unit` | `String(3)` |  | Additional Quantity 1 Unit |  |  | S/4 only entity (no ECC CDC mapping) |
| `AdditionalQuantity1` | `AdditionalQuantity1` | `Decimal(23,3)` |  | Additional Quantity 1 | AdditionalQuantity1Unit |  | S/4 only entity (no ECC CDC mapping) |
| `AdditionalQuantity2Unit` | `AdditionalQuantity2Unit` | `String(3)` |  | Additional Quantity 2 Unit |  |  | S/4 only entity (no ECC CDC mapping) |
| `AdditionalQuantity2` | `AdditionalQuantity2` | `Decimal(23,3)` |  | Additional Quantity 2 | AdditionalQuantity2Unit |  | S/4 only entity (no ECC CDC mapping) |
| `AdditionalQuantity3Unit` | `AdditionalQuantity3Unit` | `String(3)` |  | Additional Quantity 3 Unit |  |  | S/4 only entity (no ECC CDC mapping) |
| `AdditionalQuantity3` | `AdditionalQuantity3` | `Decimal(23,3)` |  | Additional Quantity 3 | AdditionalQuantity3Unit |  | S/4 only entity (no ECC CDC mapping) |
| `IncmpltSummableValnQtyUnt` | `IncmpltSummableValnQtyUnt` | `String(3)` |  | Incomplete Sum. Valuation Quantity Unit |  |  | S/4 only entity (no ECC CDC mapping) |
| `IncmpltSummableValnQty` | `IncmpltSummableValnQty` | `Decimal(23,3)` |  | Incomplete Summable Valuation Quantity | IncmpltSummableValnQtyUnt |  | S/4 only entity (no ECC CDC mapping) |
| `IncmpltSummableValnFxdQty` | `IncmpltSummableValnFxdQty` | `Decimal(23,3)` |  | Incomplete Sum. Valuation Fix Quantity | IncmpltSummableValnQtyUnt |  | S/4 only entity (no ECC CDC mapping) |
| `DebitCreditCode` | `DebitCreditCode` | `String(1)` |  | Debit/Credit Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `FiscalPeriod` | `FiscalPeriod` | `String(3)` |  | Fiscal Period |  |  | S/4 only entity (no ECC CDC mapping); ECC: BKPF.MONAT (unpadded '3'); S/4: zero-padded '003' |
| `FiscalYearVariant` | `FiscalYearVariant` | `String(2)` |  | Fiscal Year Variant |  |  | S/4 only entity (no ECC CDC mapping) |
| `FiscalYearPeriod` | `FiscalYearPeriod` | `String(7)` |  | Fiscal Year Period |  |  | S/4 only entity (no ECC CDC mapping) |
| `PostingDate` | `PostingDate` | `Date` |  | Posting Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `DocumentDate` | `DocumentDate` | `Date` |  | Journal Entry Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `AccountingDocumentType` | `AccountingDocumentType` | `String(2)` |  | Journal Entry Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `AccountingDocumentItem` | `AccountingDocumentItem` | `String(3)` |  | Posting View Item |  |  | S/4 only entity (no ECC CDC mapping) |
| `AssignmentReference` | `AssignmentReference` | `String(18)` |  | Assignment Reference |  |  | S/4 only entity (no ECC CDC mapping) |
| `AccountingDocumentCategory` | `AccountingDocumentCategory` | `String(1)` |  | Journal Entry Category |  |  | S/4 only entity (no ECC CDC mapping) |
| `JournalEntryItemCategory` | `JournalEntryItemCategory` | `String(5)` |  | Journal Entry Item Category |  |  | S/4 only entity (no ECC CDC mapping) |
| `PostingKey` | `PostingKey` | `String(2)` |  | Posting Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `TransactionTypeDetermination` | `TransactionTypeDetermination` | `String(3)` |  | Transaction Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `SubLedgerAcctLineItemType` | `SubLedgerAcctLineItemType` | `String(5)` |  | SLA Line Item Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `AccountingDocCreatedByUser` | `AccountingDocCreatedByUser` | `String(12)` |  | Journal Entry Created By |  |  | S/4 only entity (no ECC CDC mapping) |
| `LastChangeDateTime` | `LastChangeDateTime` | `DateTime` |  | Last Change Date Time |  |  | S/4 only entity (no ECC CDC mapping) |
| `CreationDateTime` | `CreationDateTime` | `DateTime` |  | Creation Date Time |  |  | S/4 only entity (no ECC CDC mapping) |
| `CreationDate` | `CreationDate` | `Date` |  | Creation Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `EliminationProfitCenter` | `EliminationProfitCenter` | `String(10)` |  | Elimination Profit Center |  |  | S/4 only entity (no ECC CDC mapping) |
| `OriginObjectType` | `OriginObjectType` | `String(2)` |  | Origin Object Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `GLAccountType` | `GLAccountType` | `String(1)` |  | G/L Account Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `AlternativeGLAccount` | `AlternativeGLAccount` | `String(10)` |  | Alternative G/L Account |  | _AlternativeGLAccount | S/4 only entity (no ECC CDC mapping) |
| `CountryChartOfAccounts` | `CountryChartOfAccounts` | `String(4)` |  | Alternative Chart of Accounts |  | _CountryChartOfAccounts | S/4 only entity (no ECC CDC mapping) |
| `ItemIsSplit` | `ItemIsSplit` | `Boolean` |  | Itm chngd by Doc Spl |  |  | S/4 only entity (no ECC CDC mapping) |
| `ConsolidationUnit` | `ConsolidationUnit` | `String(18)` |  | Consolidation Unit |  |  | S/4 only entity (no ECC CDC mapping) |
| `PartnerConsolidationUnit` | `PartnerConsolidationUnit` | `String(18)` |  | Partner Consolidation Unit |  |  | S/4 only entity (no ECC CDC mapping) |
| `Company` | `Company` | `String(6)` |  | Company |  |  | S/4 only entity (no ECC CDC mapping) |
| `ConsolidationChartOfAccounts` | `ConsolidationChartOfAccounts` | `String(2)` |  | Consolidation Chart of Accounts |  |  | S/4 only entity (no ECC CDC mapping) |
| `CnsldtnFinancialStatementItem` | `CnsldtnFinancialStatementItem` | `String(10)` |  | Consolidation Financial Statement Item |  |  | S/4 only entity (no ECC CDC mapping) |
| `CnsldtnSubitemCategory` | `CnsldtnSubitemCategory` | `String(3)` |  | Consolidation Subitem Category |  |  | S/4 only entity (no ECC CDC mapping) |
| `CnsldtnSubitem` | `CnsldtnSubitem` | `String(10)` |  | Consolidation Subitem |  |  | S/4 only entity (no ECC CDC mapping) |
| `InvoiceReference` | `InvoiceReference` | `String(10)` |  | Invoice Reference |  |  | S/4 only entity (no ECC CDC mapping) |
| `InvoiceReferenceFiscalYear` | `InvoiceReferenceFiscalYear` | `String(4)` |  | Invoice Reference Fiscal Year |  |  | S/4 only entity (no ECC CDC mapping) |
| `FollowOnDocumentType` | `FollowOnDocumentType` | `String(1)` |  | Follow-On Document Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `InvoiceItemReference` | `InvoiceItemReference` | `String(3)` |  | Invoice Item Reference |  |  | S/4 only entity (no ECC CDC mapping) |
| `ReferencePurchaseOrderCategory` | `ReferencePurchaseOrderCategory` | `String(3)` |  | Reference Purchase Order Category |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchasingDocument` | `PurchasingDocument` | `String(10)` |  | Purchasing Document |  |  | S/4 only entity (no ECC CDC mapping) |
| `PurchasingDocumentItem` | `PurchasingDocumentItem` | `String(5)` |  | Purchasing Doc. Item |  |  | S/4 only entity (no ECC CDC mapping) |
| `AccountAssignmentNumber` | `AccountAssignmentNumber` | `String(2)` |  | Account Assignment Number |  |  | S/4 only entity (no ECC CDC mapping) |
| `DocumentItemText` | `DocumentItemText` | `String(50)` |  | Item Text |  |  | S/4 only entity (no ECC CDC mapping) |
| `SalesDocument` | `SalesDocument` | `String(10)` |  | Sales Document |  |  | S/4 only entity (no ECC CDC mapping) |
| `SalesDocumentItem` | `SalesDocumentItem` | `String(6)` |  | Sales Document Item |  |  | S/4 only entity (no ECC CDC mapping) |
| `Product` | `Product` | `String(40)` |  | Product |  |  | S/4 only entity (no ECC CDC mapping) |
| `Plant` | `Plant` | `String(4)` |  | Plant |  |  | S/4 only entity (no ECC CDC mapping) |
| `Supplier` | `Supplier` | `String(10)` |  | Supplier |  |  | S/4 only entity (no ECC CDC mapping) |
| `Customer` | `Customer` | `String(10)` |  | Customer |  |  | S/4 only entity (no ECC CDC mapping) |
| `ServicesRenderedDate` | `ServicesRenderedDate` | `Date` |  | Serv. Rendered Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `PerformancePeriodStartDate` | `PerformancePeriodStartDate` | `Date` |  | Per. of Perf. Start |  |  | S/4 only entity (no ECC CDC mapping) |
| `PerformancePeriodEndDate` | `PerformancePeriodEndDate` | `Date` |  | Per. of Perf. End |  |  | S/4 only entity (no ECC CDC mapping) |
| `ConditionContract` | `ConditionContract` | `String(10)` |  | Condition Contract |  |  | S/4 only entity (no ECC CDC mapping) |
| `ExchangeRateDate` | `ExchangeRateDate` | `Date` |  | Translation Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `ComponentBreakdown` | `ComponentBreakdown` | `String(16)` |  | Component Breakdown |  |  | S/4 only entity (no ECC CDC mapping) |
| `CompBreakdownScaleNumerator` | `CompBreakdownScaleNumerator` | `Decimal(23,3)` |  | Component Breakdown Scale Numerator |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinancialAccountType` | `FinancialAccountType` | `String(1)` |  | Account Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `SpecialGLCode` | `SpecialGLCode` | `String(1)` |  | Special G/L |  |  | S/4 only entity (no ECC CDC mapping) |
| `TaxCode` | `TaxCode` | `String(2)` |  | Tax Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `TaxCountry` | `TaxCountry` | `String(3)` |  | Tax Ctry/Reg. |  |  | S/4 only entity (no ECC CDC mapping) |
| `HouseBank` | `HouseBank` | `String(5)` |  | House Bank |  |  | S/4 only entity (no ECC CDC mapping) |
| `HouseBankAccount` | `HouseBankAccount` | `String(5)` |  | House Bank Account |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsOpenItemManaged` | `IsOpenItemManaged` | `Boolean` |  | Open Item Management |  |  | S/4 only entity (no ECC CDC mapping) |
| `ClearingDate` | `ClearingDate` | `Date` |  | Clearing Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `ClearingDocFiscalYear` | `ClearingDocFiscalYear` | `String(4)` |  | Fiscal Year of Clearing JE (Depr.) |  |  | S/4 only entity (no ECC CDC mapping) |
| `ClearingAccountingDocument` | `ClearingAccountingDocument` | `String(10)` |  | Clearing Journal Entry (Deprecated) |  |  | S/4 only entity (no ECC CDC mapping) |
| `ClearingJournalEntryFiscalYear` | `ClearingJournalEntryFiscalYear` | `String(4)` |  | Fiscal Year of Clearing Journal Entry |  |  | S/4 only entity (no ECC CDC mapping) |
| `ClearingJournalEntry` | `ClearingJournalEntry` | `String(10)` |  | Clearing Journal Entry |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValueDate` | `ValueDate` | `Date` |  | Value date |  |  | S/4 only entity (no ECC CDC mapping) |
| `GeneralLedgerAgingScope` | `GeneralLedgerAgingScope` | `String(10)` |  | General Ledger Aging Scope |  |  | S/4 only entity (no ECC CDC mapping) |
| `GeneralLedgerAgingIncrement` | `GeneralLedgerAgingIncrement` | `String(15)` |  | General Ledger Aging Increment |  |  | S/4 only entity (no ECC CDC mapping) |
| `AssetDepreciationArea` | `AssetDepreciationArea` | `String(2)` |  | Depreciation Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `MasterFixedAsset` | `MasterFixedAsset` | `String(12)` |  | Fixed Asset |  |  | S/4 only entity (no ECC CDC mapping) |
| `FixedAsset` | `FixedAsset` | `String(4)` |  | Asset Subnumber |  |  | S/4 only entity (no ECC CDC mapping) |
| `AssetValueDate` | `AssetValueDate` | `Date` |  | Asset Value Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `AssetTransactionType` | `AssetTransactionType` | `String(3)` |  | Asset Transaction Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `AssetAcctTransClassfctn` | `AssetAcctTransClassfctn` | `String(2)` |  | Trans. Type Category |  |  | S/4 only entity (no ECC CDC mapping) |
| `DepreciationFiscalPeriod` | `DepreciationFiscalPeriod` | `String(3)` |  | Depreciation Fiscal Period |  |  | S/4 only entity (no ECC CDC mapping) |
| `GroupMasterFixedAsset` | `GroupMasterFixedAsset` | `String(12)` |  | Group Asset |  |  | S/4 only entity (no ECC CDC mapping) |
| `GroupFixedAsset` | `GroupFixedAsset` | `String(4)` |  | Group Asset Subnmbr |  |  | S/4 only entity (no ECC CDC mapping) |
| `AssetClass` | `AssetClass` | `String(8)` |  | Asset Class |  |  | S/4 only entity (no ECC CDC mapping) |
| `PartnerMasterFixedAsset` | `PartnerMasterFixedAsset` | `String(12)` |  | Partner Master Fixed Asset |  |  | S/4 only entity (no ECC CDC mapping) |
| `PartnerFixedAsset` | `PartnerFixedAsset` | `String(4)` |  | Partner Fixed Asset |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostEstimate` | `CostEstimate` | `String(12)` |  | Cost Estimate |  |  | S/4 only entity (no ECC CDC mapping) |
| `InventorySpecialStockValnType` | `InventorySpecialStockValnType` | `String(1)` |  | Inventory Special Stock Valuation Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsSupplierStockValuation` | `IsSupplierStockValuation` | `Boolean` |  | Is Supplier Stock Valuation |  |  | S/4 only entity (no ECC CDC mapping) |
| `InventorySpecialStockType` | `InventorySpecialStockType` | `String(1)` |  | Inventory Special Stock Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `InventorySpclStkSalesDocument` | `InventorySpclStkSalesDocument` | `String(10)` |  | Inventory Special Stock Sales Document |  |  | S/4 only entity (no ECC CDC mapping) |
| `InventorySpclStkSalesDocItm` | `InventorySpclStkSalesDocItm` | `String(6)` |  | Inventory Spcl Stock Sales Document Item |  |  | S/4 only entity (no ECC CDC mapping) |
| `InvtrySpclStockWBSElmntIntID` | `InvtrySpclStockWBSElmntIntID` | `String(8)` |  | Inv. Special Stock WBS Element Int. ID |  |  | S/4 only entity (no ECC CDC mapping) |
| `InventorySpclStockWBSElement` | `InventorySpclStockWBSElement` | `String(24)` |  | Inventory WBS Element |  |  | S/4 only entity (no ECC CDC mapping) |
| `InventorySpecialStockSupplier` | `InventorySpecialStockSupplier` | `String(10)` |  | Inventory Special Stock Supplier |  |  | S/4 only entity (no ECC CDC mapping) |
| `InventoryValuationType` | `InventoryValuationType` | `String(10)` |  | Inventory Valuation Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValuationArea` | `ValuationArea` | `String(4)` |  | Valuation Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `MaterialLedgerProcessType` | `MaterialLedgerProcessType` | `String(4)` |  | Material Ledger Process Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `MaterialLedgerCategory` | `MaterialLedgerCategory` | `String(2)` |  | Material Ledger Category |  |  | S/4 only entity (no ECC CDC mapping) |
| `SlsPriceAmountInCoCodeCrcy` | `SlsPriceAmountInCoCodeCrcy` | `Decimal(34,4)` |  | Sales Price Amount in Company Code Crcy | CompanyCodeCurrency |  | S/4 only entity (no ECC CDC mapping) |
| `ProductPriceControl` | `ProductPriceControl` | `String(1)` |  | Product Price Control |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProcurementAlternative` | `ProcurementAlternative` | `String(12)` |  | Procurement Alternative |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductionProcess` | `ProductionProcess` | `String(12)` |  | Production Process |  |  | S/4 only entity (no ECC CDC mapping) |
| `SenderCompanyCode` | `SenderCompanyCode` | `String(4)` |  | Company Code in Sender System |  |  | S/4 only entity (no ECC CDC mapping) |
| `SenderGLAccount` | `SenderGLAccount` | `String(10)` |  | Sender G/L Account |  |  | S/4 only entity (no ECC CDC mapping) |
| `SenderAccountAssignment` | `SenderAccountAssignment` | `String(30)` |  | Sender Account Assignment |  |  | S/4 only entity (no ECC CDC mapping) |
| `SenderAccountAssignmentType` | `SenderAccountAssignmentType` | `String(2)` |  | Sender Account Assignment Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `ControllingObject` | `ControllingObject` | `String(22)` |  | Controlling Object |  |  | S/4 only entity (no ECC CDC mapping) |
| `ControllingKeySubNumber` | `ControllingKeySubNumber` | `String(14)` |  | CO subkey |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostOriginGroup` | `CostOriginGroup` | `String(4)` |  | Origin Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `OriginSenderObject` | `OriginSenderObject` | `String(22)` |  | Origin Sender Object |  |  | S/4 only entity (no ECC CDC mapping) |
| `ControllingDebitCreditCode` | `ControllingDebitCreditCode` | `String(1)` |  | Controlling Debit Credit Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `OriginCtrlgDebitCreditCode` | `OriginCtrlgDebitCreditCode` | `String(1)` |  | Dr/Cr Ind. (Origin) |  |  | S/4 only entity (no ECC CDC mapping) |
| `ControllingObjectDebitType` | `ControllingObjectDebitType` | `String(1)` |  | Controlling Object Debit Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `QuantityIsIncomplete` | `QuantityIsIncomplete` | `Boolean` |  | Qty Is Incomplete |  |  | S/4 only entity (no ECC CDC mapping) |
| `OffsettingAccount` | `OffsettingAccount` | `String(10)` |  | Offsetting Account |  |  | S/4 only entity (no ECC CDC mapping) |
| `OffsettingAccountType` | `OffsettingAccountType` | `String(1)` |  | Offsetting Account Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `OffsettingChartOfAccounts` | `OffsettingChartOfAccounts` | `String(4)` |  | Offsetting Chart of Accounts |  | _OffsettingChartOfAccounts | S/4 only entity (no ECC CDC mapping) |
| `LineItemIsCompleted` | `LineItemIsCompleted` | `Boolean` |  | Line Item is Completed |  |  | S/4 only entity (no ECC CDC mapping) |
| `PersonnelNumber` | `PersonnelNumber` | `String(8)` |  | Personnel Number |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProfitabilitySegment` | `ProfitabilitySegment` | `String(10)` |  | Profitability Segment |  |  | S/4 only entity (no ECC CDC mapping) |
| `ControllingObjectClass` | `ControllingObjectClass` | `String(2)` |  | Controlling Object Class |  |  | S/4 only entity (no ECC CDC mapping) |
| `PartnerCompanyCode` | `PartnerCompanyCode` | `String(4)` |  | Partner Company Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `PartnerControllingObjectClass` | `PartnerControllingObjectClass` | `String(2)` |  | Partner Controlling Object Class |  |  | S/4 only entity (no ECC CDC mapping) |
| `OriginProfitCenter` | `OriginProfitCenter` | `String(10)` |  | Origin Profit Center |  |  | S/4 only entity (no ECC CDC mapping) |
| `OriginOrder` | `OriginOrder` | `String(12)` |  | Origin Order |  |  | S/4 only entity (no ECC CDC mapping) |
| `OriginCostCtrActivityType` | `OriginCostCtrActivityType` | `String(6)` |  | Origin Cost Center Activity Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `OriginCostCenter` | `OriginCostCenter` | `String(10)` |  | Origin Cost Center |  |  | S/4 only entity (no ECC CDC mapping) |
| `OriginProduct` | `OriginProduct` | `String(40)` |  | Origin Product |  |  | S/4 only entity (no ECC CDC mapping) |
| `VarianceOriginGLAccount` | `VarianceOriginGLAccount` | `String(10)` |  | Origin G/L Account of a Variance |  |  | S/4 only entity (no ECC CDC mapping) |
| `AccountAssignment` | `AccountAssignment` | `String(30)` |  | Account Assignment |  |  | S/4 only entity (no ECC CDC mapping) |
| `AccountAssignmentType` | `AccountAssignmentType` | `String(2)` |  | Account Assignment Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCtrActivityType` | `CostCtrActivityType` | `String(6)` |  | Activity Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `OrderID` | `OrderID` | `String(12)` |  | Order ID |  |  | S/4 only entity (no ECC CDC mapping) |
| `OrderCategory` | `OrderCategory` | `String(2)` |  | Order category |  |  | S/4 only entity (no ECC CDC mapping) |
| `WBSElementInternalID` | `WBSElementInternalID` | `String(8)` |  | WBS Element Internal ID |  |  | S/4 only entity (no ECC CDC mapping) |
| `WBSElement` | `WBSElement` | `String(24)` |  | WBS Element |  |  | S/4 only entity (no ECC CDC mapping) |
| `PartnerWBSElementInternalID` | `PartnerWBSElementInternalID` | `String(8)` |  | Partner WBS Element Internal ID |  |  | S/4 only entity (no ECC CDC mapping) |
| `PartnerWBSElement` | `PartnerWBSElement` | `String(24)` |  | Partner WBS Element |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProjectInternalID` | `ProjectInternalID` | `String(8)` |  | Project Internal ID |  |  | S/4 only entity (no ECC CDC mapping) |
| `Project` | `Project` | `String(24)` |  | Project |  |  | S/4 only entity (no ECC CDC mapping) |
| `PartnerProjectInternalID` | `PartnerProjectInternalID` | `String(8)` |  | Partner Project Internal ID |  |  | S/4 only entity (no ECC CDC mapping) |
| `PartnerProject` | `PartnerProject` | `String(24)` |  | Partner Project |  |  | S/4 only entity (no ECC CDC mapping) |
| `OperatingConcern` | `OperatingConcern` | `String(4)` |  | Operating concern |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProjectNetwork` | `ProjectNetwork` | `String(12)` |  | Network |  |  | S/4 only entity (no ECC CDC mapping) |
| `RelatedNetworkActivity` | `RelatedNetworkActivity` | `String(4)` |  | Related Network Activity |  |  | S/4 only entity (no ECC CDC mapping) |
| `BusinessProcess` | `BusinessProcess` | `String(12)` |  | Business Process |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostObject` | `CostObject` | `String(12)` |  | Cost Object |  |  | S/4 only entity (no ECC CDC mapping) |
| `BillableControl` | `BillableControl` | `String(2)` |  | Billable Control |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostAnalysisResource` | `CostAnalysisResource` | `String(10)` |  | Cost Analysis Resource |  |  | S/4 only entity (no ECC CDC mapping) |
| `CustomerServiceNotification` | `CustomerServiceNotification` | `String(12)` |  | Customer Service Notification |  |  | S/4 only entity (no ECC CDC mapping) |
| `ServiceDocumentType` | `ServiceDocumentType` | `String(4)` |  | Service Doc. Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `ServiceDocument` | `ServiceDocument` | `String(10)` |  | Service Document |  |  | S/4 only entity (no ECC CDC mapping) |
| `ServiceDocumentItem` | `ServiceDocumentItem` | `String(6)` |  | Service Doc. Item |  |  | S/4 only entity (no ECC CDC mapping) |
| `PartnerServiceDocumentType` | `PartnerServiceDocumentType` | `String(4)` |  | Partner Service Document Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `PartnerServiceDocument` | `PartnerServiceDocument` | `String(10)` |  | Partner Service Document |  |  | S/4 only entity (no ECC CDC mapping) |
| `PartnerServiceDocumentItem` | `PartnerServiceDocumentItem` | `String(6)` |  | Partner Service Document Item |  |  | S/4 only entity (no ECC CDC mapping) |
| `ServiceContractType` | `ServiceContractType` | `String(4)` |  | Serv. Contract Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `ServiceContract` | `ServiceContract` | `String(10)` |  | Service Contract |  |  | S/4 only entity (no ECC CDC mapping) |
| `ServiceContractItem` | `ServiceContractItem` | `String(6)` |  | Srv Contract Item |  |  | S/4 only entity (no ECC CDC mapping) |
| `BusinessSolutionOrder` | `BusinessSolutionOrder` | `String(10)` |  | Solution Order |  |  | S/4 only entity (no ECC CDC mapping) |
| `BusinessSolutionOrderItem` | `BusinessSolutionOrderItem` | `String(6)` |  | Solution Order Item |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProviderContract` | `ProviderContract` | `String(20)` |  | Provider Contract |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProviderContractItem` | `ProviderContractItem` | `String(6)` |  | Provider Contract Item |  |  | S/4 only entity (no ECC CDC mapping) |
| `RevenueAccountingContract` | `RevenueAccountingContract` | `String(14)` |  | Revenue Accounting Contract |  |  | S/4 only entity (no ECC CDC mapping) |
| `PerformanceObligation` | `PerformanceObligation` | `String(16)` |  | Performance Obligation |  |  | S/4 only entity (no ECC CDC mapping) |
| `TimeSheetOvertimeCategory` | `TimeSheetOvertimeCategory` | `String(4)` |  | Overtime Category |  |  | S/4 only entity (no ECC CDC mapping) |
| `PartnerAccountAssignment` | `PartnerAccountAssignment` | `String(30)` |  | Partner Account Assignment |  |  | S/4 only entity (no ECC CDC mapping) |
| `PartnerAccountAssignmentType` | `PartnerAccountAssignmentType` | `String(2)` |  | Partner Account Assignment Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `StstclAccountAssignmentType1` | `StstclAccountAssignmentType1` | `String(2)` |  | Statistical Account Assignment Type 1 |  |  | S/4 only entity (no ECC CDC mapping) |
| `StstclAccountAssignmentType2` | `StstclAccountAssignmentType2` | `String(2)` |  | Statistical Account Assignment Type 2 |  |  | S/4 only entity (no ECC CDC mapping) |
| `StstclAccountAssignmentType3` | `StstclAccountAssignmentType3` | `String(2)` |  | Statistical Account Assignment Type 3 |  |  | S/4 only entity (no ECC CDC mapping) |
| `WorkPackage` | `WorkPackage` | `String(50)` |  | Plan Item |  |  | S/4 only entity (no ECC CDC mapping) |
| `WorkItem` | `WorkItem` | `String(10)` |  | Work Item ID |  |  | S/4 only entity (no ECC CDC mapping) |
| `PartnerCostCtrActivityType` | `PartnerCostCtrActivityType` | `String(6)` |  | Partner Cost Center Activity Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `PartnerOrder` | `PartnerOrder` | `String(12)` |  | Partner Order |  |  | S/4 only entity (no ECC CDC mapping) |
| `PartnerOrderCategory` | `PartnerOrderCategory` | `String(2)` |  | Partner Order Cat. |  |  | S/4 only entity (no ECC CDC mapping) |
| `PartnerSalesDocument` | `PartnerSalesDocument` | `String(10)` |  | Partner Sales Doc. |  |  | S/4 only entity (no ECC CDC mapping) |
| `PartnerSalesDocumentItem` | `PartnerSalesDocumentItem` | `String(6)` |  | Partner Sales Document Item |  |  | S/4 only entity (no ECC CDC mapping) |
| `PartnerProjectNetwork` | `PartnerProjectNetwork` | `String(12)` |  | Partner Project Network |  |  | S/4 only entity (no ECC CDC mapping) |
| `PartnerProjectNetworkActivity` | `PartnerProjectNetworkActivity` | `String(4)` |  | Partner Project Network Activity |  |  | S/4 only entity (no ECC CDC mapping) |
| `PartnerBusinessProcess` | `PartnerBusinessProcess` | `String(12)` |  | Partner Business Process |  |  | S/4 only entity (no ECC CDC mapping) |
| `PartnerCostObject` | `PartnerCostObject` | `String(12)` |  | Partner Cost Object |  |  | S/4 only entity (no ECC CDC mapping) |
| `ControllingDocumentItem` | `ControllingDocumentItem` | `String(3)` |  | Controlling Doc Item |  |  | S/4 only entity (no ECC CDC mapping) |
| `VarianceOriginGroup` | `VarianceOriginGroup` | `String(4)` |  | Varc. Origin Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `BillingDocumentType` | `BillingDocumentType` | `String(4)` |  | Billing Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `SalesOrganization` | `SalesOrganization` | `String(4)` |  | Sales Organization |  |  | S/4 only entity (no ECC CDC mapping) |
| `DistributionChannel` | `DistributionChannel` | `String(2)` |  | Distribution Channel |  |  | S/4 only entity (no ECC CDC mapping) |
| `OrganizationDivision` | `OrganizationDivision` | `String(2)` |  | Division |  |  | S/4 only entity (no ECC CDC mapping) |
| `SoldProduct` | `SoldProduct` | `String(40)` |  | Product Sold |  |  | S/4 only entity (no ECC CDC mapping) |
| `SoldProductGroup` | `SoldProductGroup` | `String(9)` |  | Product Sold Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `CustomerGroup` | `CustomerGroup` | `String(2)` |  | Customer Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `CustomerSupplierCountry` | `CustomerSupplierCountry` | `String(3)` |  | Customer or Supplier Country/Region |  |  | S/4 only entity (no ECC CDC mapping) |
| `CustomerSupplierIndustry` | `CustomerSupplierIndustry` | `String(4)` |  | Customer Supplier Industry |  |  | S/4 only entity (no ECC CDC mapping) |
| `SalesDistrict` | `SalesDistrict` | `String(6)` |  | Sales District |  |  | S/4 only entity (no ECC CDC mapping) |
| `BillToParty` | `BillToParty` | `String(10)` |  | Bill-to Party |  |  | S/4 only entity (no ECC CDC mapping) |
| `ShipToParty` | `ShipToParty` | `String(10)` |  | Ship-to Party |  |  | S/4 only entity (no ECC CDC mapping) |
| `CustomerSupplierCorporateGroup` | `CustomerSupplierCorporateGroup` | `String(10)` |  | Customer Supplier Corporate Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `CashLedgerCompanyCode` | `CashLedgerCompanyCode` | `String(4)` |  | Cash Origin CoCode |  |  | S/4 only entity (no ECC CDC mapping) |
| `CashLedgerAccount` | `CashLedgerAccount` | `String(10)` |  | Cash Origin Account |  | _CashLedgerAccount | S/4 only entity (no ECC CDC mapping) |
| `FinancialManagementArea` | `FinancialManagementArea` | `String(4)` |  | FM Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `CommitmentItem` | `CommitmentItem` | `String(24)` |  | Commitment Item |  |  | S/4 only entity (no ECC CDC mapping) |
| `FundsCenter` | `FundsCenter` | `String(16)` |  | Funds Center |  |  | S/4 only entity (no ECC CDC mapping) |
| `FundedProgram` | `FundedProgram` | `String(24)` |  | Funded Program |  |  | S/4 only entity (no ECC CDC mapping) |
| `Fund` | `Fund` | `String(10)` |  | Fund |  |  | S/4 only entity (no ECC CDC mapping) |
| `GrantID` | `GrantID` | `String(20)` |  | Grant |  |  | S/4 only entity (no ECC CDC mapping) |
| `BudgetPeriod` | `BudgetPeriod` | `String(10)` |  | Budget Period |  |  | S/4 only entity (no ECC CDC mapping) |
| `PartnerFund` | `PartnerFund` | `String(10)` |  | Partner Fund |  |  | S/4 only entity (no ECC CDC mapping) |
| `PartnerGrant` | `PartnerGrant` | `String(20)` |  | Partner Grant |  |  | S/4 only entity (no ECC CDC mapping) |
| `PartnerBudgetPeriod` | `PartnerBudgetPeriod` | `String(10)` |  | Partner Budget Period |  |  | S/4 only entity (no ECC CDC mapping) |
| `PubSecBudgetAccount` | `PubSecBudgetAccount` | `String(10)` |  | Budget Account |  |  | S/4 only entity (no ECC CDC mapping) |
| `PubSecBudgetAccountCoCode` | `PubSecBudgetAccountCoCode` | `String(4)` |  | Company Code for Budget Account |  |  | S/4 only entity (no ECC CDC mapping) |
| `PubSecBudgetCnsmpnDate` | `PubSecBudgetCnsmpnDate` | `Date` |  | Budget Consumption Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `PubSecBudgetCnsmpnFsclPeriod` | `PubSecBudgetCnsmpnFsclPeriod` | `String(3)` |  | Posting Period for Budget Consumption |  |  | S/4 only entity (no ECC CDC mapping) |
| `PubSecBudgetCnsmpnFsclYear` | `PubSecBudgetCnsmpnFsclYear` | `String(4)` |  | Year of Budget Consumption |  |  | S/4 only entity (no ECC CDC mapping) |
| `PubSecBudgetIsRelevant` | `PubSecBudgetIsRelevant` | `Boolean` |  | Budget-Relevant |  |  | S/4 only entity (no ECC CDC mapping) |
| `PubSecBudgetCnsmpnType` | `PubSecBudgetCnsmpnType` | `String(2)` |  | Budget Consumption Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `PubSecBudgetCnsmpnAmtType` | `PubSecBudgetCnsmpnAmtType` | `String(4)` |  | Amount Type for Budget Consumption |  |  | S/4 only entity (no ECC CDC mapping) |
| `SponsoredProgram` | `SponsoredProgram` | `String(20)` |  | Sponsored Program |  |  | S/4 only entity (no ECC CDC mapping) |
| `SponsoredClass` | `SponsoredClass` | `String(20)` |  | Sponsored Class |  |  | S/4 only entity (no ECC CDC mapping) |
| `GteeMBudgetValidityNumber` | `GteeMBudgetValidityNumber` | `String(3)` |  | Bdgt Validty No. |  |  | S/4 only entity (no ECC CDC mapping) |
| `EarmarkedFundsDocument` | `EarmarkedFundsDocument` | `String(10)` |  | Earmarked Funds Document |  |  | S/4 only entity (no ECC CDC mapping) |
| `EarmarkedFundsDocumentItem` | `EarmarkedFundsDocumentItem` | `String(3)` |  | Earmarked Funds Document Item |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinancialServicesProductGroup` | `FinancialServicesProductGroup` | `String(10)` |  | Financial Services Product Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinancialServicesBranch` | `FinancialServicesBranch` | `String(10)` |  | Financial Services Branch |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinancialDataSource` | `FinancialDataSource` | `String(10)` |  | Financial Data Source |  |  | S/4 only entity (no ECC CDC mapping) |
| `JointVenture` | `JointVenture` | `String(6)` |  | Joint venture |  |  | S/4 only entity (no ECC CDC mapping) |
| `JointVentureEquityGroup` | `JointVentureEquityGroup` | `String(3)` |  | Joint Venture Equity Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `JointVentureCostRecoveryCode` | `JointVentureCostRecoveryCode` | `String(2)` |  | Joint Venture Cost Recovery Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `JointVenturePartner` | `JointVenturePartner` | `String(10)` |  | Joint Venture Partner |  |  | S/4 only entity (no ECC CDC mapping) |
| `JointVentureBillingType` | `JointVentureBillingType` | `String(2)` |  | Joint Venture Billing Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `JointVentureEquityType` | `JointVentureEquityType` | `String(3)` |  | Joint Venture Equity Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `JointVentureProductionDate` | `JointVentureProductionDate` | `Date` |  | Joint Venture Production Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `JointVentureBillingDate` | `JointVentureBillingDate` | `Date` |  | Joint Venture Billing Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `JointVentureOperationalDate` | `JointVentureOperationalDate` | `Date` |  | Joint Venture Operational Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `CutbackRun` | `CutbackRun` | `Timestamp` |  | Cutback Run |  |  | S/4 only entity (no ECC CDC mapping) |
| `JointVentureAccountingActivity` | `JointVentureAccountingActivity` | `String(2)` |  | Joint Venture Accounting Activity |  |  | S/4 only entity (no ECC CDC mapping) |
| `PartnerVenture` | `PartnerVenture` | `String(6)` |  | PartnerVenture |  |  | S/4 only entity (no ECC CDC mapping) |
| `PartnerEquityGroup` | `PartnerEquityGroup` | `String(3)` |  | Partner Equity Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `SenderCostRecoveryCode` | `SenderCostRecoveryCode` | `String(2)` |  | Sender Cost Recovery Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `CutbackAccount` | `CutbackAccount` | `String(10)` |  | Cutback Account |  |  | S/4 only entity (no ECC CDC mapping) |
| `CutbackCostObject` | `CutbackCostObject` | `String(22)` |  | Cutback Cost Object |  |  | S/4 only entity (no ECC CDC mapping) |
| `REBusinessEntity` | `REBusinessEntity` | `String(8)` |  | RE Business Entity |  |  | S/4 only entity (no ECC CDC mapping) |
| `RealEstateBuilding` | `RealEstateBuilding` | `String(8)` |  | Real Estate Building |  |  | S/4 only entity (no ECC CDC mapping) |
| `RealEstateProperty` | `RealEstateProperty` | `String(8)` |  | Real Estate Property |  |  | S/4 only entity (no ECC CDC mapping) |
| `RERentalObject` | `RERentalObject` | `String(8)` |  | RE Rental Object |  |  | S/4 only entity (no ECC CDC mapping) |
| `RealEstateContract` | `RealEstateContract` | `String(13)` |  | Real Estate Contract |  |  | S/4 only entity (no ECC CDC mapping) |
| `REServiceChargeKey` | `REServiceChargeKey` | `String(4)` |  | RE Service Charge Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `RESettlementUnitID` | `RESettlementUnitID` | `String(5)` |  | RE Settlement Unit |  |  | S/4 only entity (no ECC CDC mapping) |
| `SettlementReferenceDate` | `SettlementReferenceDate` | `Date` |  | Settlement Reference Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `REPartnerBusinessEntity` | `REPartnerBusinessEntity` | `String(8)` |  | RE Partner Business Entity |  |  | S/4 only entity (no ECC CDC mapping) |
| `RealEstatePartnerBuilding` | `RealEstatePartnerBuilding` | `String(8)` |  | Real Estate Partner Building |  |  | S/4 only entity (no ECC CDC mapping) |
| `RealEstatePartnerProperty` | `RealEstatePartnerProperty` | `String(8)` |  | Real Estate Partner Property |  |  | S/4 only entity (no ECC CDC mapping) |
| `REPartnerRentalObject` | `REPartnerRentalObject` | `String(8)` |  | RE Partner Rental Object |  |  | S/4 only entity (no ECC CDC mapping) |
| `RealEstatePartnerContract` | `RealEstatePartnerContract` | `String(13)` |  | Real Estate Partner Contract |  |  | S/4 only entity (no ECC CDC mapping) |
| `REPartnerServiceChargeKey` | `REPartnerServiceChargeKey` | `String(4)` |  | RE Partner Service Charge Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `REPartnerSettlementUnitID` | `REPartnerSettlementUnitID` | `String(5)` |  | RE Partner Settlement Unit |  |  | S/4 only entity (no ECC CDC mapping) |
| `PartnerSettlementReferenceDate` | `PartnerSettlementReferenceDate` | `Date` |  | Ptnr. Reference Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `AccrualObjectType` | `AccrualObjectType` | `String(4)` |  | Accrual Object Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `AccrualObjectLogicalSystem` | `AccrualObjectLogicalSystem` | `String(10)` |  | Logical Syst. AcrObj |  |  | S/4 only entity (no ECC CDC mapping) |
| `AccrualObject` | `AccrualObject` | `String(32)` |  | Accrual Object |  |  | S/4 only entity (no ECC CDC mapping) |
| `AccrualSubobject` | `AccrualSubobject` | `String(32)` |  | Accrual Subobject |  |  | S/4 only entity (no ECC CDC mapping) |
| `AccrualItemType` | `AccrualItemType` | `String(11)` |  | Accrual Item Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `AccrualReferenceObject` | `AccrualReferenceObject` | `String(32)` |  | Accrual Reference Object |  |  | S/4 only entity (no ECC CDC mapping) |
| `AccrualValueDate` | `AccrualValueDate` | `Date` |  | Accrual Value Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinancialValuationObjectType` | `FinancialValuationObjectType` | `String(4)` |  | Financial Valuation Object Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinancialValuationObject` | `FinancialValuationObject` | `String(32)` |  | Financial Valuation Object |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinancialValuationSubobject` | `FinancialValuationSubobject` | `String(32)` |  | Financial Valuation Subobject |  |  | S/4 only entity (no ECC CDC mapping) |
| `NetDueDate` | `NetDueDate` | `Date` |  | Net Due Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `CreditRiskClass` | `CreditRiskClass` | `String(3)` |  | Credit Risk Class |  |  | S/4 only entity (no ECC CDC mapping) |
| `WorkCenterInternalID` | `WorkCenterInternalID` | `String(8)` |  | Object ID |  |  | S/4 only entity (no ECC CDC mapping) |
| `OrderOperation` | `OrderOperation` | `String(4)` |  | Order Operation |  |  | S/4 only entity (no ECC CDC mapping) |
| `OrderItem` | `OrderItem` | `String(4)` |  | Order item number |  |  | S/4 only entity (no ECC CDC mapping) |
| `PartnerOrderItem` | `PartnerOrderItem` | `String(4)` |  | Partner Order item |  |  | S/4 only entity (no ECC CDC mapping) |
| `OrderSuboperation` | `OrderSuboperation` | `String(4)` |  | Order Suboperation |  |  | S/4 only entity (no ECC CDC mapping) |
| `Equipment` | `Equipment` | `String(18)` |  | Equipment |  |  | S/4 only entity (no ECC CDC mapping) |
| `FunctionalLocation` | `FunctionalLocation` | `String(30)` |  | Functional Location |  |  | S/4 only entity (no ECC CDC mapping) |
| `Assembly` | `Assembly` | `String(40)` |  | Assembly |  |  | S/4 only entity (no ECC CDC mapping) |
| `MaintenanceActivityType` | `MaintenanceActivityType` | `String(3)` |  | MaintActivityType |  |  | S/4 only entity (no ECC CDC mapping) |
| `MaintenanceOrderPlanningCode` | `MaintenanceOrderPlanningCode` | `String(1)` |  | Order planning ind. |  |  | S/4 only entity (no ECC CDC mapping) |
| `MaintPriorityType` | `MaintPriorityType` | `String(2)` |  | Priority Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `MaintPriority` | `MaintPriority` | `String(1)` |  | Priority |  |  | S/4 only entity (no ECC CDC mapping) |
| `SuperiorOrder` | `SuperiorOrder` | `String(12)` |  | Superior Order |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductGroup` | `ProductGroup` | `String(9)` |  | Product Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `MaintenanceOrderIsPlanned` | `MaintenanceOrderIsPlanned` | `Boolean` |  | Planned Parts/Work |  |  | S/4 only entity (no ECC CDC mapping) |
| `OriginOrderOperation` | `OriginOrderOperation` | `String(4)` |  | Origin Order Operation |  |  | S/4 only entity (no ECC CDC mapping) |
| `JrnlEntryItemMigrationSource` | `JrnlEntryItemMigrationSource` | `String(1)` |  | Journal Entry Item Migration Source |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedCommitmentString` | `USFedCommitmentString` | `String(62)` |  | Commitment string |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedBudgetaryLedgerStatus` | `USFedBudgetaryLedgerStatus` | `String(5)` |  | BL Status |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedFiscalYearBlank` | `USFedFiscalYearBlank` | `String(4)` |  | FMA Fiscal Year |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedObjectClass` | `USFedObjectClass` | `String(24)` |  | Obj Class US Fed |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedStandardGLAccount` | `USFedStandardGLAccount` | `String(6)` |  | SGL account |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedAgencyLocationCode` | `USFedAgencyLocationCode` | `String(8)` |  | Agency Location Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedApplOfSecdrySrceFunds` | `USFedApplOfSecdrySrceFunds` | `String(16)` |  | Application of Funds |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedFundType` | `USFedFundType` | `String(6)` |  | Fund Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedPaymentOffice` | `USFedPaymentOffice` | `String(5)` |  | Payment Office |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedAgency` | `USFedAgency` | `String(3)` |  | Agency Identifier |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedMainAccount` | `USFedMainAccount` | `String(4)` |  | Main Account |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedSubAccount` | `USFedSubAccount` | `String(3)` |  | Sub account |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedBeginPerdOfAvailability` | `USFedBeginPerdOfAvailability` | `String(4)` |  | Begin Prd of Avail |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedEndPerdOfAvaily` | `USFedEndPerdOfAvaily` | `String(4)` |  | Ending Prd of Avail |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedAvailabilityType` | `USFedAvailabilityType` | `String(1)` |  | Avail Type Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedBusEventTypeCode` | `USFedBusEventTypeCode` | `String(10)` |  | Business Evt Typ Cd |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedSubLevelPrefix` | `USFedSubLevelPrefix` | `String(2)` |  | Sublevel Prefix |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedAuthorityType` | `USFedAuthorityType` | `String(1)` |  | Authority Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedApportionmentCategory` | `USFedApportionmentCategory` | `String(1)` |  | Apportionment Cat |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedApprtmtCatDetailPgmCode` | `USFedApprtmtCatDetailPgmCode` | `String(4)` |  | Category B Detail |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedYearOfBdgtAuthorityCode` | `USFedYearOfBdgtAuthorityCode` | `String(4)` |  | Yr of Budget Auth |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedAvailabilityTimeType` | `USFedAvailabilityTimeType` | `String(1)` |  | Availability Time |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedPriorYearAdjmtCode` | `USFedPriorYearAdjmtCode` | `String(1)` |  | Prior Year Adj. Cd |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedBudgetEnforcementActCat` | `USFedBudgetEnforcementActCat` | `String(1)` |  | BEA Category |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedReductionType` | `USFedReductionType` | `String(3)` |  | Reduction Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedBorrowingSource` | `USFedBorrowingSource` | `String(1)` |  | Borrowing Source |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedRptgYearForCohort` | `USFedRptgYearForCohort` | `String(4)` |  | Year Cohort |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedAllocTransfAgencyID` | `USFedAllocTransfAgencyID` | `String(3)` |  | Alloc Transfr Agency |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedReimbursable` | `USFedReimbursable` | `String(1)` |  | Reimbursable |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedBudgetImpact` | `USFedBudgetImpact` | `String(1)` |  | Budget Impact |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedDisasterEmergencyFundCode` | `USFedDisasterEmergencyFundCode` | `String(3)` |  | Disastr Emer Fnd Cde |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedPgmReportingCat` | `USFedPgmReportingCat` | `String(3)` |  | Prog.Rpt.Category |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedCustodialIndicator` | `USFedCustodialIndicator` | `String(1)` |  | Custodial indicator |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedPostingSequenceNumber` | `USFedPostingSequenceNumber` | `String(10)` |  | Sequence Nbr |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedExchangeIndicator` | `USFedExchangeIndicator` | `String(1)` |  | Exchange Indicator |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedFederalNonFederalCode` | `USFedFederalNonFederalCode` | `String(1)` |  | Federal/Nonfederal |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedTradingPartnerAgency` | `USFedTradingPartnerAgency` | `String(3)` |  | Agency ID (TP) |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedTrdgPartMainAccount` | `USFedTrdgPartMainAccount` | `String(4)` |  | Main Account (TP) |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedTrdgPartSubAccount` | `USFedTrdgPartSubAccount` | `String(3)` |  | Subaccount (TP) |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedTrdgPartBeginPerdOfAvaily` | `USFedTrdgPartBeginPerdOfAvaily` | `String(4)` |  | Begin Prd Avail (TP) |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedTrdgPartEndPerdOfAvaily` | `USFedTrdgPartEndPerdOfAvaily` | `String(4)` |  | End Prd Avail (TP) |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedAllocTransfAgencyTrdgPart` | `USFedAllocTransfAgencyTrdgPart` | `String(3)` |  | AllcTrnsfrAgncy (TP) |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedTrdgPartAvailabilityType` | `USFedTrdgPartAvailabilityType` | `String(1)` |  | Avail Type Code (TP) |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedTrdgPartBusEventTypeCode` | `USFedTrdgPartBusEventTypeCode` | `String(10)` |  | BusinessEvtTypCd(TP) |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedTrdgPartSubLevelPrefix` | `USFedTrdgPartSubLevelPrefix` | `String(2)` |  | Sublevel Prefix (TP) |  |  | S/4 only entity (no ECC CDC mapping) |
| `USFedPgmActivityReportingKey` | `USFedPgmActivityReportingKey` | `String(15)` |  | Prog Act Rep Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `GeneralLedgerAccountLineItemOID` | `GeneralLedgerAccountLineItemOID` | `String(128)` |  |  |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `GeneralLedgerAccountText`

- **ABAP Name:** `I_GLAccountTextRawData`
- **Label:** General Ledger Account - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `ChartOfAccounts` | `ChartOfAccounts` | `String(4)` | Y | Chart of Accounts |  | _ChartOfAccounts | S/4 only entity (no ECC CDC mapping) |
| `GLAccount` | `GLAccount` | `String(10)` | Y | G/L Account |  |  | S/4 only entity (no ECC CDC mapping) |
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `GLAccountName` | `GLAccountName` | `String(20)` |  | G/L Account Name |  |  | S/4 only entity (no ECC CDC mapping) |
| `GLAccountLongName` | `GLAccountLongName` | `String(50)` |  | G/L Account Long Name |  |  | S/4 only entity (no ECC CDC mapping) |
| `LastChangeDateTime` | `LastChangeDateTime` | `DateTime` |  | Time Stamp |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `GeneralLedgerAccountTypeText`

- **ABAP Name:** `I_GLAccountTypeText`
- **Label:** G/L Account Type - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `GLAccountType` | `GLAccountType` | `String(10)` | Y | Lower Value |  |  | S/4 only entity (no ECC CDC mapping) |
| `Language` | `Language` | `String(2)` | Y | Lang. |  |  | S/4 only entity (no ECC CDC mapping) |
| `GLAccountTypeName` | `GLAccountTypeName` | `String(60)` |  | Short Description |  |  | S/4 only entity (no ECC CDC mapping) |
| `DomainValue` | `DomainValue` | `String(10)` |  | Lower Value |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `OperatingGeneralLedgerAccount`

- **ABAP Name:** `I_GLAccountInCompanyCode`
- **Label:** General Ledger Account in Company Code
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `GLAccount` | `GLAccount` | `String(10)` | Y | G/L Account |  |  | S/4 only entity (no ECC CDC mapping) |
| `CompanyCode` | `CompanyCode` | `String(4)` | Y | Company Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `AuthorizationGroup` | `AuthorizationGroup` | `String(4)` |  | Authorization |  |  | S/4 only entity (no ECC CDC mapping) |
| `AccountingClerk` | `AccountingClerk` | `String(2)` |  | Clerk Abbrev. |  |  | S/4 only entity (no ECC CDC mapping) |
| `LastInterestCalcRunDate` | `LastInterestCalcRunDate` | `Date` |  | Last Int. Calc. |  |  | S/4 only entity (no ECC CDC mapping) |
| `CreationDate` | `CreationDate` | `Date` |  | Created On |  |  | S/4 only entity (no ECC CDC mapping) |
| `CreatedByUser` | `CreatedByUser` | `String(12)` |  | Created By |  |  | S/4 only entity (no ECC CDC mapping) |
| `LastChangeDateTime` | `LastChangeDateTime` | `DateTime` |  | Time Stamp |  |  | S/4 only entity (no ECC CDC mapping) |
| `PlanningLevel` | `PlanningLevel` | `String(2)` |  | Planning Level |  |  | S/4 only entity (no ECC CDC mapping) |
| `HouseBank` | `HouseBank` | `String(5)` |  | House Bank |  |  | S/4 only entity (no ECC CDC mapping) |
| `HouseBankAccount` | `HouseBankAccount` | `String(5)` |  | Account ID |  |  | S/4 only entity (no ECC CDC mapping) |
| `ExchRateDifferencesAccountDetn` | `ExchRateDifferencesAccountDetn` | `String(4)` |  | E/R Diff. Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `ReconciliationAccountType` | `ReconciliationAccountType` | `String(1)` |  | Reconcil. ID |  |  | S/4 only entity (no ECC CDC mapping) |
| `TaxCategory` | `TaxCategory` | `String(2)` |  | Tax Category |  |  | S/4 only entity (no ECC CDC mapping) |
| `InterestCalculationCode` | `InterestCalculationCode` | `String(2)` |  | Interest Indicator |  |  | S/4 only entity (no ECC CDC mapping) |
| `GLAccountCurrency` | `GLAccountCurrency` | `String(5)` |  | Account Currency |  |  | S/4 only entity (no ECC CDC mapping) |
| `ReconciliationAcctIsChangeable` | `ReconciliationAcctIsChangeable` | `Boolean` |  | Rec.Act Ready |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsManagedExternally` | `IsManagedExternally` | `Boolean` |  | Is Managed Ext. |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsAutomaticallyPosted` | `IsAutomaticallyPosted` | `Boolean` |  | Auto. Posting |  |  | S/4 only entity (no ECC CDC mapping) |
| `LineItemDisplayIsEnabled` | `LineItemDisplayIsEnabled` | `Boolean` |  | Line Items |  |  | S/4 only entity (no ECC CDC mapping) |
| `SupplementIsAllowed` | `SupplementIsAllowed` | `Boolean` |  | Supplement |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsOpenItemManaged` | `IsOpenItemManaged` | `Boolean` |  | OI Management |  |  | S/4 only entity (no ECC CDC mapping) |
| `InterestCalculationDate` | `InterestCalculationDate` | `Date` |  | Last Key Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `IntrstCalcFrequencyInMonths` | `IntrstCalcFrequencyInMonths` | `String(2)` |  | Int.Calc.Freq. |  |  | S/4 only entity (no ECC CDC mapping) |
| `AcctgDocItmDisplaySequenceRule` | `AcctgDocItmDisplaySequenceRule` | `String(3)` |  | Sort key |  |  | S/4 only entity (no ECC CDC mapping) |
| `AlternativeGLAccount` | `AlternativeGLAccount` | `String(10)` |  | Alternative G/L Account |  |  | S/4 only entity (no ECC CDC mapping) |
| `JointVentureRecoveryCode` | `JointVentureRecoveryCode` | `String(2)` |  | Recovery Indicator |  |  | S/4 only entity (no ECC CDC mapping) |
| `CommitmentItem` | `CommitmentItem` | `String(14)` |  | Commitment item |  |  | S/4 only entity (no ECC CDC mapping) |
| `CommitmentItemShortID` | `CommitmentItemShortID` | `String(14)` |  | Commitment Item Short ID |  |  | S/4 only entity (no ECC CDC mapping) |
| `TaxCodeIsRequired` | `TaxCodeIsRequired` | `Boolean` |  | Pstg w/o tax allowed |  |  | S/4 only entity (no ECC CDC mapping) |
| `BalanceHasLocalCurrency` | `BalanceHasLocalCurrency` | `Boolean` |  | Balances in LC |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValuationGroup` | `ValuationGroup` | `String(10)` |  | Valuation Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `APARToleranceGroup` | `APARToleranceGroup` | `String(4)` |  | Tolerance Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `AccountIsBlockedForPosting` | `AccountIsBlockedForPosting` | `Boolean` |  | Posting Block |  |  | S/4 only entity (no ECC CDC mapping) |
| `AccountIsMarkedForDeletion` | `AccountIsMarkedForDeletion` | `Boolean` |  | Deletion Flag |  |  | S/4 only entity (no ECC CDC mapping) |
| `ClearingIsLedgerGroupSpecific` | `ClearingIsLedgerGroupSpecific` | `Boolean` |  | OI Mgmt by LedgerGrp |  |  | S/4 only entity (no ECC CDC mapping) |
| `CashPlanningGroup` | `CashPlanningGroup` | `String(10)` |  | Planning Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsCashFlowAccount` | `IsCashFlowAccount` | `Boolean` |  | Rel.Cash Flow |  |  | S/4 only entity (no ECC CDC mapping) |
| `GLAcctInflationKey` | `GLAcctInflationKey` | `String(8)` |  | Inflation key |  |  | S/4 only entity (no ECC CDC mapping) |
| `FieldStatusGroup` | `FieldStatusGroup` | `String(4)` |  | Field status group |  |  | S/4 only entity (no ECC CDC mapping) |
| `MultiCurrencyAccountingCode` | `MultiCurrencyAccountingCode` | `String(5)` |  | MCA Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsExtendedOpenItemManaged` | `IsExtendedOpenItemManaged` | `Boolean` |  | Extended OI Mgmt |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `SemanticTag`

- **ABAP Name:** `I_SemanticTag`
- **Label:** Semantic Tag
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `SemanticTag` | `SemanticTag` | `String(10)` | Y | Semantic Tag |  |  | S/4 only entity (no ECC CDC mapping) |
| `ParentSemanticTag` | `ParentSemanticTag` | `String(10)` |  | Parent Semantic Tag |  |  | S/4 only entity (no ECC CDC mapping) |
| `SemanticTagGroup` | `SemanticTagGroup` | `String(4)` |  | Semantic Tag Group |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `SemanticTagFunctionalArea`

- **ABAP Name:** `I_SemTagFuncArea`
- **Label:** Functional Area with Semantic Tag
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `GLAccountHierarchy` | `GLAccountHierarchy` | `String(42)` | Y | FSV |  | _Hierarchy | S/4 only entity (no ECC CDC mapping) |
| `HierarchyNode` | `HierarchyNode` | `String(50)` | Y | Node |  |  | S/4 only entity (no ECC CDC mapping) |
| `SemanticTag` | `SemanticTag` | `String(10)` | Y | Semantic Tag |  | _SemanticTag | S/4 only entity (no ECC CDC mapping) |
| `ValidityEndDate` | `ValidityEndDate` | `Date` | Y | Valid To |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityStartDate` | `ValidityStartDate` | `Date` | Y | Valid From |  |  | S/4 only entity (no ECC CDC mapping) |
| `FunctionalArea` | `FunctionalArea` | `String(16)` | Y | Functional Area |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `SemanticTagGeneralLedger`

- **ABAP Name:** `I_SemTagGLAccount`
- **Label:** G/L Account with Semantic Tag
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `GLAccountHierarchy` | `GLAccountHierarchy` | `String(42)` | Y | FSV |  | _Hierarchy | S/4 only entity (no ECC CDC mapping) |
| `HierarchyNode` | `HierarchyNode` | `String(50)` | Y | Node |  |  | S/4 only entity (no ECC CDC mapping) |
| `SemanticTag` | `SemanticTag` | `String(10)` | Y | Semantic Tag |  | _SemanticTag | S/4 only entity (no ECC CDC mapping) |
| `ValidityEndDate` | `ValidityEndDate` | `Date` | Y | Valid To |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityStartDate` | `ValidityStartDate` | `Date` | Y | Valid From |  |  | S/4 only entity (no ECC CDC mapping) |
| `ChartOfAccounts` | `ChartOfAccounts` | `String(4)` | Y | Chart of Accounts |  | _ChartOfAccounts | S/4 only entity (no ECC CDC mapping) |
| `GLAccount` | `GLAccount` | `String(10)` | Y | G/L Account |  | _GLAccountInChartOfAccounts | S/4 only entity (no ECC CDC mapping) |
| `FunctionalAreaIsUsed` | `FunctionalAreaIsUsed` | `Boolean` |  | Functional Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsFunctionalAreaPermitted` | `IsFunctionalAreaPermitted` | `Boolean` |  | Fun.Area Perm. |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `SemanticTagLeafNode`

- **ABAP Name:** `I_SemanticTagLeafNode`
- **Label:** Hierarchy Leaf Node with Semantic Tag
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `GLAccountHierarchy` | `GLAccountHierarchy` | `String(42)` | Y | Hierarchy ID |  | _Hierarchy | S/4 only entity (no ECC CDC mapping) |
| `HierarchyNode` | `HierarchyNode` | `String(50)` | Y | Node |  | _GLAccountHierarchyNode | S/4 only entity (no ECC CDC mapping) |
| `ValidityEndDate` | `ValidityEndDate` | `Date` | Y | Valid To |  |  | S/4 only entity (no ECC CDC mapping) |
| `SemanticTag` | `SemanticTag` | `String(10)` | Y | Semantic Tag |  | _SemanticTag | S/4 only entity (no ECC CDC mapping) |
| `ValidityStartDate` | `ValidityStartDate` | `Date` |  | Valid From |  |  | S/4 only entity (no ECC CDC mapping) |
| `ChartOfAccounts` | `ChartOfAccounts` | `String(4)` |  | Chart of Accounts |  |  | S/4 only entity (no ECC CDC mapping) |
| `GLAccount` | `GLAccount` | `String(10)` |  | G/L Account |  |  | S/4 only entity (no ECC CDC mapping) |
| `FunctionalArea` | `FunctionalArea` | `String(16)` |  | Functional Area |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `SemanticTagText`

- **ABAP Name:** `I_SemanticTagText`
- **Label:** Semantic Tag - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `SemanticTag` | `SemanticTag` | `String(10)` | Y | Semantic Tag |  |  | S/4 only entity (no ECC CDC mapping) |
| `SemanticTagName` | `SemanticTagName` | `String(20)` |  | Semantic Tag Name |  |  | S/4 only entity (no ECC CDC mapping) |
