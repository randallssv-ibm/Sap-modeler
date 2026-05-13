# JournalEntryItemCodes

> Source file: `sap-s4com-JournalEntryItemCodes-v1.json`


## Entity: `AssetAcctTransClassification`

- **ABAP Name:** `I_MovementCategory`
- **Label:** Movement Category
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `AssetAcctTransClassfctn` |  |  | `String(2)` | Y | Trans. Type Category |  |  | S/4 only entity |


## Entity: `ControllingDebitCreditCode`

- **ABAP Name:** `I_ControllingDebitCreditCode`
- **Label:** Controlling Debit Credit Code
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `ControllingDebitCreditCode` |  |  | `String(1)` | Y | Dr/Cr indicator  CO |  |  | S/4 only entity |
| `DomainValue` |  |  | `String(1)` |  |  |  |  | S/4 only entity |
| `DomainValue_2` |  |  | `String(10)` |  | Lower Value |  |  | S/4 only entity |


## Entity: `ControllingDebitCreditCodeText`

- **ABAP Name:** `I_ControllingDebitCreditCodeT`
- **Label:** Debit Credit Code in Controlling - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `ControllingDebitCreditCode` |  |  | `String(1)` | Y |  |  |  | S/4 only entity |
| `Language` |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity |
| `ControllingDebitCreditCodeName` |  |  | `String(60)` |  | Short Description |  |  | S/4 only entity |


## Entity: `DebitCreditCode`

- **ABAP Name:** `I_DebitCreditCode`
- **Label:** Debit Credit Code
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `DebitCreditCode` |  |  | `String(1)` | Y | Debit/Credit Code |  |  | S/4 only entity |


## Entity: `DebitCreditCodeText`

- **ABAP Name:** `I_DebitCreditCodeText`
- **Label:** Debit Credit Code - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `Language` |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity |
| `DebitCreditCode` |  |  | `String(1)` | Y | Debit/Credit Code |  |  | S/4 only entity |
| `DebitCreditCodeName` |  |  | `String(60)` |  | D/C Code Name |  |  | S/4 only entity |


## Entity: `FinancialAccountType`

- **ABAP Name:** `I_FinancialAccountType`
- **Label:** Financial Account Type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `FinancialAccountType` |  |  | `String(1)` | Y | Account Type |  |  | S/4 only entity |
| `DomainValue` |  |  | `String(10)` |  | Lower Value |  |  | S/4 only entity |


## Entity: `FinancialAccountTypeText`

- **ABAP Name:** `I_FinancialAccountTypeText`
- **Label:** Financial Account Type - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `FinancialAccountType` |  |  | `String(1)` | Y | Account Type |  |  | S/4 only entity |
| `Language` |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity |
| `FinancialAccountTypeName` |  |  | `String(60)` |  | Fin. Acc. Type Name |  |  | S/4 only entity |
| `DomainValue` |  |  | `String(10)` |  | Lower Value |  |  | S/4 only entity |


## Entity: `GeneralLedgerRecordType`

- **ABAP Name:** `I_GLRecordType`
- **Label:** General Ledger Record Type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `GLRecordType` |  |  | `String(1)` | Y | Record Type |  |  | S/4 only entity |


## Entity: `JournalEntryItemObsoleteReason`

- **ABAP Name:** `I_JrnlEntryItemObsoleteRsn`
- **Label:** Obsolete Reason of Journal Entry Item
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `JrnlEntryItemObsoleteReason` |  |  | `String(1)` | Y | Obsolete Reason |  |  | S/4 only entity |
| `DomainValue` |  |  | `String(10)` |  | Lower Value |  |  | S/4 only entity |


## Entity: `JrnlEntryItemObsltRsnText`

- **ABAP Name:** `I_JrnlEntryItemObsltRsnT`
- **Label:** Obsolete Reason of Entry Item - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `JrnlEntryItemObsoleteReason` |  |  | `String(1)` | Y | Obsolete Reason |  |  | S/4 only entity |
| `Language` |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity |
| `DomainValue` |  |  | `String(10)` |  | Lower Value |  |  | S/4 only entity |
| `JrnlEntryItemObsoleteRsnName` |  |  | `String(60)` |  | Fin. Acc. Type Name |  |  | S/4 only entity |


## Entity: `MovementCategoryText`

- **ABAP Name:** `I_MovementCategoryText`
- **Label:** Movement Category - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `AssetAcctTransClassfctn` |  |  | `String(2)` | Y | Trans. Type Category |  |  | S/4 only entity |
| `Language` |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity |
| `AssetAcctTransClassfctnName` |  |  | `String(50)` |  | Trans.Type Cat. Text |  |  | S/4 only entity |


## Entity: `PostingKey`

- **ABAP Name:** `I_PostingKey`
- **Label:** Posting Key
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `PostingKey` |  |  | `String(2)` | Y | Posting Key |  |  | S/4 only entity |
| `DebitCreditCode` |  |  | `String(1)` |  | Debit/Credit Code |  |  | S/4 only entity |
| `FinancialAccountType` |  |  | `String(1)` |  | Account Type |  |  | S/4 only entity |
| `IsSalesRelated` |  |  | `Boolean` |  | Sales-Related Item |  |  | S/4 only entity |
| `IsUsedInPaymentTransaction` |  |  | `Boolean` |  | Payment Transaction |  |  | S/4 only entity |
| `ReversalPostingKey` |  |  | `String(2)` |  | Reversal Posting Key |  |  | S/4 only entity |
| `IsSpecialGLTransaction` |  |  | `Boolean` |  | Special G/L |  |  | S/4 only entity |


## Entity: `PostingKeyText`

- **ABAP Name:** `I_PostingKeyText`
- **Label:** Posting Key - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `Language` |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity |
| `PostingKey` |  |  | `String(2)` | Y | Posting Key |  |  | S/4 only entity |
| `PostingKeyName` |  |  | `String(20)` |  | Posting Key Name |  |  | S/4 only entity |


## Entity: `PostingKeyWithSpecialGLCode`

- **ABAP Name:** `I_PostingKeyWithSpecialGLCode`
- **Label:** Posting Key with Special General Ledger Code
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `PostingKey` |  |  | `String(2)` | Y | Posting Key |  | _PostingKey | S/4 only entity |
| `SpecialGLCode` |  |  | `String(1)` | Y | Special G/L |  |  | S/4 only entity |


## Entity: `PostingKeyWithSpecialGLCodeText`

- **ABAP Name:** `I_PostingKeyWthSpclGLCodeTxt`
- **Label:** Posting Key With Special General Leder Code - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `Language` |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity |
| `PostingKey` |  |  | `String(2)` | Y | Posting Key |  | _PostingKey | S/4 only entity |
| `SpecialGLCode` |  |  | `String(1)` | Y | Special G/L |  | _SpecialGLCode | S/4 only entity |
| `FinancialAccountType` |  |  | `String(1)` |  | Account Type |  | _FinancialAccountType | S/4 only entity |
| `PostingKeyName` |  |  | `String(20)` |  | Posting Key Name |  |  | S/4 only entity |


## Entity: `SpecialGeneralLedgerCode`

- **ABAP Name:** `I_SpecialGLCode`
- **Label:** Special General Ledger Code
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `SpecialGLCode` |  |  | `String(1)` | Y | Special G/L Ind. |  |  | S/4 only entity |
| `FinancialAccountType` |  |  | `String(1)` | Y | Account Type |  | _FinancialAccountType | S/4 only entity |
| `SpecialGLTransactionType` |  |  | `String(1)` |  | Sp. G/L Trans.Type |  |  | S/4 only entity |
| `CreditLimitIsChecked` |  |  | `Boolean` |  | Rel.to Credit Limit |  |  | S/4 only entity |
| `IsNotedItmWithoutBalUpdt` |  |  | `Boolean` |  | Noted Items |  |  | S/4 only entity |


## Entity: `SpecialGeneralLedgerCodeText`

- **ABAP Name:** `I_SpecialGLCodeText`
- **Label:** Special General Ledger Code - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `FinancialAccountType` |  |  | `String(1)` | Y | Account Type |  | _FinancialAccountType | S/4 only entity |
| `SpecialGLCode` |  |  | `String(1)` | Y | Special G/L Ind. |  |  | S/4 only entity |
| `Language` |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity |
| `SpecialGLCodeName` |  |  | `String(7)` |  | Name |  |  | S/4 only entity |
| `SpecialGLCodeLongName` |  |  | `String(30)` |  | Description |  |  | S/4 only entity |


## Entity: `SubledgerAccountLineItemType`

- **ABAP Name:** `I_SubLedgerAccLineItemType`
- **Label:** SubLedger Account LineItem Type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `SubLedgerAcctLineItemType` |  |  | `String(5)` | Y | SLA Line Item Type |  |  | S/4 only entity |


## Entity: `SubledgerAccountLineItemTypeText`

- **ABAP Name:** `I_SubLedgerAccLineItemTypeT`
- **Label:** Subledger Account Line Item Type - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `SubLedgerAcctLineItemType` |  |  | `String(5)` | Y | SLA Line Item Type |  |  | S/4 only entity |
| `Language` |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity |
| `SubLedgerAcctLineItemTypeName` |  |  | `String(70)` |  | Subl. LIt. Type Text |  |  | S/4 only entity |
