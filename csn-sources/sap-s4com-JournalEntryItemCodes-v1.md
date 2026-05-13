# JournalEntryItemCodes

> Source file: `sap-s4com-JournalEntryItemCodes-v1.json`


## Entity: `AssetAcctTransClassification`

- **ABAP Name:** `I_MovementCategory`
- **Label:** Movement Category
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `AssetAcctTransClassfctn` | `AssetAcctTransClassfctn` | `String(2)` | Y | Trans. Type Category |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `ControllingDebitCreditCode`

- **ABAP Name:** `I_ControllingDebitCreditCode`
- **Label:** Controlling Debit Credit Code
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `ControllingDebitCreditCode` | `ControllingDebitCreditCode` | `String(1)` | Y | Dr/Cr indicator  CO |  |  | S/4 only entity (no ECC CDC mapping) |
| `DomainValue` | `DomainValue` | `String(1)` |  |  |  |  | S/4 only entity (no ECC CDC mapping) |
| `DomainValue_2` | `DomainValue_2` | `String(10)` |  | Lower Value |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `ControllingDebitCreditCodeText`

- **ABAP Name:** `I_ControllingDebitCreditCodeT`
- **Label:** Debit Credit Code in Controlling - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `ControllingDebitCreditCode` | `ControllingDebitCreditCode` | `String(1)` | Y |  |  |  | S/4 only entity (no ECC CDC mapping) |
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `ControllingDebitCreditCodeName` | `ControllingDebitCreditCodeName` | `String(60)` |  | Short Description |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `DebitCreditCode`

- **ABAP Name:** `I_DebitCreditCode`
- **Label:** Debit Credit Code
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `DebitCreditCode` | `DebitCreditCode` | `String(1)` | Y | Debit/Credit Code |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `DebitCreditCodeText`

- **ABAP Name:** `I_DebitCreditCodeText`
- **Label:** Debit Credit Code - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `DebitCreditCode` | `DebitCreditCode` | `String(1)` | Y | Debit/Credit Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `DebitCreditCodeName` | `DebitCreditCodeName` | `String(60)` |  | D/C Code Name |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `FinancialAccountType`

- **ABAP Name:** `I_FinancialAccountType`
- **Label:** Financial Account Type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `FinancialAccountType` | `FinancialAccountType` | `String(1)` | Y | Account Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `DomainValue` | `DomainValue` | `String(10)` |  | Lower Value |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `FinancialAccountTypeText`

- **ABAP Name:** `I_FinancialAccountTypeText`
- **Label:** Financial Account Type - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `FinancialAccountType` | `FinancialAccountType` | `String(1)` | Y | Account Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinancialAccountTypeName` | `FinancialAccountTypeName` | `String(60)` |  | Fin. Acc. Type Name |  |  | S/4 only entity (no ECC CDC mapping) |
| `DomainValue` | `DomainValue` | `String(10)` |  | Lower Value |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `GeneralLedgerRecordType`

- **ABAP Name:** `I_GLRecordType`
- **Label:** General Ledger Record Type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `GLRecordType` | `GLRecordType` | `String(1)` | Y | Record Type |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `JournalEntryItemObsoleteReason`

- **ABAP Name:** `I_JrnlEntryItemObsoleteRsn`
- **Label:** Obsolete Reason of Journal Entry Item
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `JrnlEntryItemObsoleteReason` | `JrnlEntryItemObsoleteReason` | `String(1)` | Y | Obsolete Reason |  |  | S/4 only entity (no ECC CDC mapping) |
| `DomainValue` | `DomainValue` | `String(10)` |  | Lower Value |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `JrnlEntryItemObsltRsnText`

- **ABAP Name:** `I_JrnlEntryItemObsltRsnT`
- **Label:** Obsolete Reason of Entry Item - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `JrnlEntryItemObsoleteReason` | `JrnlEntryItemObsoleteReason` | `String(1)` | Y | Obsolete Reason |  |  | S/4 only entity (no ECC CDC mapping) |
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `DomainValue` | `DomainValue` | `String(10)` |  | Lower Value |  |  | S/4 only entity (no ECC CDC mapping) |
| `JrnlEntryItemObsoleteRsnName` | `JrnlEntryItemObsoleteRsnName` | `String(60)` |  | Fin. Acc. Type Name |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `MovementCategoryText`

- **ABAP Name:** `I_MovementCategoryText`
- **Label:** Movement Category - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `AssetAcctTransClassfctn` | `AssetAcctTransClassfctn` | `String(2)` | Y | Trans. Type Category |  |  | S/4 only entity (no ECC CDC mapping) |
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `AssetAcctTransClassfctnName` | `AssetAcctTransClassfctnName` | `String(50)` |  | Trans.Type Cat. Text |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `PostingKey`

- **ABAP Name:** `I_PostingKey`
- **Label:** Posting Key
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `PostingKey` | `PostingKey` | `String(2)` | Y | Posting Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `DebitCreditCode` | `DebitCreditCode` | `String(1)` |  | Debit/Credit Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinancialAccountType` | `FinancialAccountType` | `String(1)` |  | Account Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsSalesRelated` | `IsSalesRelated` | `Boolean` |  | Sales-Related Item |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsUsedInPaymentTransaction` | `IsUsedInPaymentTransaction` | `Boolean` |  | Payment Transaction |  |  | S/4 only entity (no ECC CDC mapping) |
| `ReversalPostingKey` | `ReversalPostingKey` | `String(2)` |  | Reversal Posting Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsSpecialGLTransaction` | `IsSpecialGLTransaction` | `Boolean` |  | Special G/L |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `PostingKeyText`

- **ABAP Name:** `I_PostingKeyText`
- **Label:** Posting Key - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `PostingKey` | `PostingKey` | `String(2)` | Y | Posting Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `PostingKeyName` | `PostingKeyName` | `String(20)` |  | Posting Key Name |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `PostingKeyWithSpecialGLCode`

- **ABAP Name:** `I_PostingKeyWithSpecialGLCode`
- **Label:** Posting Key with Special General Ledger Code
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `PostingKey` | `PostingKey` | `String(2)` | Y | Posting Key |  | _PostingKey | S/4 only entity (no ECC CDC mapping) |
| `SpecialGLCode` | `SpecialGLCode` | `String(1)` | Y | Special G/L |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `PostingKeyWithSpecialGLCodeText`

- **ABAP Name:** `I_PostingKeyWthSpclGLCodeTxt`
- **Label:** Posting Key With Special General Leder Code - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `PostingKey` | `PostingKey` | `String(2)` | Y | Posting Key |  | _PostingKey | S/4 only entity (no ECC CDC mapping) |
| `SpecialGLCode` | `SpecialGLCode` | `String(1)` | Y | Special G/L |  | _SpecialGLCode | S/4 only entity (no ECC CDC mapping) |
| `FinancialAccountType` | `FinancialAccountType` | `String(1)` |  | Account Type |  | _FinancialAccountType | S/4 only entity (no ECC CDC mapping) |
| `PostingKeyName` | `PostingKeyName` | `String(20)` |  | Posting Key Name |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `SpecialGeneralLedgerCode`

- **ABAP Name:** `I_SpecialGLCode`
- **Label:** Special General Ledger Code
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `SpecialGLCode` | `SpecialGLCode` | `String(1)` | Y | Special G/L Ind. |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinancialAccountType` | `FinancialAccountType` | `String(1)` | Y | Account Type |  | _FinancialAccountType | S/4 only entity (no ECC CDC mapping) |
| `SpecialGLTransactionType` | `SpecialGLTransactionType` | `String(1)` |  | Sp. G/L Trans.Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `CreditLimitIsChecked` | `CreditLimitIsChecked` | `Boolean` |  | Rel.to Credit Limit |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsNotedItmWithoutBalUpdt` | `IsNotedItmWithoutBalUpdt` | `Boolean` |  | Noted Items |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `SpecialGeneralLedgerCodeText`

- **ABAP Name:** `I_SpecialGLCodeText`
- **Label:** Special General Ledger Code - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `FinancialAccountType` | `FinancialAccountType` | `String(1)` | Y | Account Type |  | _FinancialAccountType | S/4 only entity (no ECC CDC mapping) |
| `SpecialGLCode` | `SpecialGLCode` | `String(1)` | Y | Special G/L Ind. |  |  | S/4 only entity (no ECC CDC mapping) |
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `SpecialGLCodeName` | `SpecialGLCodeName` | `String(7)` |  | Name |  |  | S/4 only entity (no ECC CDC mapping) |
| `SpecialGLCodeLongName` | `SpecialGLCodeLongName` | `String(30)` |  | Description |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `SubledgerAccountLineItemType`

- **ABAP Name:** `I_SubLedgerAccLineItemType`
- **Label:** SubLedger Account LineItem Type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `SubLedgerAcctLineItemType` | `SubLedgerAcctLineItemType` | `String(5)` | Y | SLA Line Item Type |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `SubledgerAccountLineItemTypeText`

- **ABAP Name:** `I_SubLedgerAccLineItemTypeT`
- **Label:** Subledger Account Line Item Type - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `SubLedgerAcctLineItemType` | `SubLedgerAcctLineItemType` | `String(5)` | Y | SLA Line Item Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `SubLedgerAcctLineItemTypeName` | `SubLedgerAcctLineItemTypeName` | `String(70)` |  | Subl. LIt. Type Text |  |  | S/4 only entity (no ECC CDC mapping) |
