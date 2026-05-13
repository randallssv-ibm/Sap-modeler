# JournalEntryItemCodes

> Source file: `sap-s4com-JournalEntryItemCodes-v1.json`


## Entity: `AssetAcctTransClassification`

- **ABAP CDS Name:** `I_MovementCategory`
- **Label:** Movement Category
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `AssetAcctTransClassfctn` | `FAA_MOVCAT` |  |  |  |  | `String(2)` | Y | Trans. Type Category |  | S/4 only entity |


## Entity: `ControllingDebitCreditCode`

- **ABAP CDS Name:** `I_ControllingDebitCreditCode`
- **Label:** Controlling Debit Credit Code
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `ControllingDebitCreditCode` | `FINS_CO_BELKZ` |  |  |  |  | `String(1)` | Y | Dr/Cr indicator  CO |  | S/4 only entity |
| `DomainValue` |  |  |  |  |  | `String(1)` |  |  |  | S/4 only entity |
| `DomainValue_2` | `DOMVALUE_L` |  |  |  |  | `String(10)` |  | Lower Value |  | S/4 only entity |


## Entity: `ControllingDebitCreditCodeText`

- **ABAP CDS Name:** `I_ControllingDebitCreditCodeT`
- **Label:** Debit Credit Code in Controlling - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `ControllingDebitCreditCode` |  |  |  |  |  | `String(1)` | Y |  |  | S/4 only entity |
| `Language` | `SPRAS` |  |  |  |  | `String(2)` | Y | Language Key |  | S/4 only entity |
| `ControllingDebitCreditCodeName` | `VAL_TEXT` |  |  |  |  | `String(60)` |  | Short Description |  | S/4 only entity |


## Entity: `DebitCreditCode`

- **ABAP CDS Name:** `I_DebitCreditCode`
- **Label:** Debit Credit Code
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `DebitCreditCode` | `FIS_SHKZG` |  |  |  |  | `String(1)` | Y | Debit/Credit Code |  | S/4 only entity |


## Entity: `DebitCreditCodeText`

- **ABAP CDS Name:** `I_DebitCreditCodeText`
- **Label:** Debit Credit Code - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Language` | `SPRAS` |  |  |  |  | `String(2)` | Y | Language Key |  | S/4 only entity |
| `DebitCreditCode` | `FIS_SHKZG` |  |  |  |  | `String(1)` | Y | Debit/Credit Code |  | S/4 only entity |
| `DebitCreditCodeName` | `FIS_SHKZG_NAME` |  |  |  |  | `String(60)` |  | D/C Code Name |  | S/4 only entity |


## Entity: `FinancialAccountType`

- **ABAP CDS Name:** `I_FinancialAccountType`
- **Label:** Financial Account Type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `FinancialAccountType` | `FARP_KOART` |  |  |  |  | `String(1)` | Y | Account Type |  | S/4 only entity |
| `DomainValue` | `DOMVALUE_L` |  |  |  |  | `String(10)` |  | Lower Value |  | S/4 only entity |


## Entity: `FinancialAccountTypeText`

- **ABAP CDS Name:** `I_FinancialAccountTypeText`
- **Label:** Financial Account Type - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `FinancialAccountType` | `FARP_KOART` |  |  |  |  | `String(1)` | Y | Account Type |  | S/4 only entity |
| `Language` | `SPRAS` |  |  |  |  | `String(2)` | Y | Language Key |  | S/4 only entity |
| `FinancialAccountTypeName` | `FIS_FIN_ACC_TYPE_NAME` |  |  |  |  | `String(60)` |  | Fin. Acc. Type Name |  | S/4 only entity |
| `DomainValue` | `DOMVALUE_L` |  |  |  |  | `String(10)` |  | Lower Value |  | S/4 only entity |


## Entity: `GeneralLedgerRecordType`

- **ABAP CDS Name:** `I_GLRecordType`
- **Label:** General Ledger Record Type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `GLRecordType` | `RRCTY` |  |  |  |  | `String(1)` | Y | Record Type |  | S/4 only entity |


## Entity: `JournalEntryItemObsoleteReason`

- **ABAP CDS Name:** `I_JrnlEntryItemObsoleteRsn`
- **Label:** Obsolete Reason of Journal Entry Item
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `JrnlEntryItemObsoleteReason` | `FINS_OBSOLETE_ITEM_REASON` |  |  |  |  | `String(1)` | Y | Obsolete Reason |  | S/4 only entity |
| `DomainValue` | `DOMVALUE_L` |  |  |  |  | `String(10)` |  | Lower Value |  | S/4 only entity |


## Entity: `JrnlEntryItemObsltRsnText`

- **ABAP CDS Name:** `I_JrnlEntryItemObsltRsnT`
- **Label:** Obsolete Reason of Entry Item - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `JrnlEntryItemObsoleteReason` | `FINS_OBSOLETE_ITEM_REASON` |  |  |  |  | `String(1)` | Y | Obsolete Reason |  | S/4 only entity |
| `Language` | `SPRAS` |  |  |  |  | `String(2)` | Y | Language Key |  | S/4 only entity |
| `DomainValue` | `DOMVALUE_L` |  |  |  |  | `String(10)` |  | Lower Value |  | S/4 only entity |
| `JrnlEntryItemObsoleteRsnName` | `FIS_FIN_ACC_TYPE_NAME` |  |  |  |  | `String(60)` |  | Fin. Acc. Type Name |  | S/4 only entity |


## Entity: `MovementCategoryText`

- **ABAP CDS Name:** `I_MovementCategoryText`
- **Label:** Movement Category - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `AssetAcctTransClassfctn` | `FAA_MOVCAT` |  |  |  |  | `String(2)` | Y | Trans. Type Category |  | S/4 only entity |
| `Language` | `LANGU` |  |  |  |  | `String(2)` | Y | Language Key |  | S/4 only entity |
| `AssetAcctTransClassfctnName` | `FAA_MOVCAT_TEXT` |  |  |  |  | `String(50)` |  | Trans.Type Cat. Text |  | S/4 only entity |


## Entity: `PostingKey`

- **ABAP CDS Name:** `I_PostingKey`
- **Label:** Posting Key
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `PostingKey` | `FIS_BSCHL` |  |  |  |  | `String(2)` | Y | Posting Key |  | S/4 only entity |
| `DebitCreditCode` | `FIS_SHKZG` |  |  |  |  | `String(1)` |  | Debit/Credit Code |  | S/4 only entity |
| `FinancialAccountType` | `FARP_KOART` |  |  |  |  | `String(1)` |  | Account Type |  | S/4 only entity |
| `IsSalesRelated` | `FARP_XUMSW` |  |  |  |  | `Boolean` |  | Sales-Related Item |  | S/4 only entity |
| `IsUsedInPaymentTransaction` | `XZAHL` |  |  |  |  | `Boolean` |  | Payment Transaction |  | S/4 only entity |
| `ReversalPostingKey` | `STBSL` |  |  |  |  | `String(2)` |  | Reversal Posting Key |  | S/4 only entity |
| `IsSpecialGLTransaction` | `XSONU` |  |  |  |  | `Boolean` |  | Special G/L |  | S/4 only entity |


## Entity: `PostingKeyText`

- **ABAP CDS Name:** `I_PostingKeyText`
- **Label:** Posting Key - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Language` | `SPRAS` |  |  |  |  | `String(2)` | Y | Language Key |  | S/4 only entity |
| `PostingKey` | `FIS_BSCHL` |  |  |  |  | `String(2)` | Y | Posting Key |  | S/4 only entity |
| `PostingKeyName` | `FIS_BSCHL_NAME` |  |  |  |  | `String(20)` |  | Posting Key Name |  | S/4 only entity |


## Entity: `PostingKeyWithSpecialGLCode`

- **ABAP CDS Name:** `I_PostingKeyWithSpecialGLCode`
- **Label:** Posting Key with Special General Ledger Code
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `PostingKey` | `FIS_BSCHL` |  |  |  |  | `String(2)` | Y | Posting Key |  | S/4 only entity |
| `SpecialGLCode` | `FAC_UMSKZ` |  |  |  |  | `String(1)` | Y | Special G/L |  | S/4 only entity |


## Entity: `PostingKeyWithSpecialGLCodeText`

- **ABAP CDS Name:** `I_PostingKeyWthSpclGLCodeTxt`
- **Label:** Posting Key With Special General Leder Code - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Language` | `SPRAS` |  |  |  |  | `String(2)` | Y | Language Key |  | S/4 only entity |
| `PostingKey` | `FIS_BSCHL` |  |  |  |  | `String(2)` | Y | Posting Key |  | S/4 only entity |
| `SpecialGLCode` | `FAC_UMSKZ` |  |  |  |  | `String(1)` | Y | Special G/L |  | S/4 only entity |
| `FinancialAccountType` | `FARP_KOART` |  |  |  |  | `String(1)` |  | Account Type |  | S/4 only entity |
| `PostingKeyName` | `FIS_BSCHL_NAME` |  |  |  |  | `String(20)` |  | Posting Key Name |  | S/4 only entity |


## Entity: `SpecialGeneralLedgerCode`

- **ABAP CDS Name:** `I_SpecialGLCode`
- **Label:** Special General Ledger Code
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `SpecialGLCode` | `UMSKZ` |  |  |  |  | `String(1)` | Y | Special G/L Ind. |  | S/4 only entity |
| `FinancialAccountType` | `KOART` |  |  |  |  | `String(1)` | Y | Account Type |  | S/4 only entity |
| `SpecialGLTransactionType` | `UMSKS` |  |  |  |  | `String(1)` |  | Sp. G/L Trans.Type |  | S/4 only entity |
| `CreditLimitIsChecked` | `KLIMP_074U` |  |  |  |  | `Boolean` |  | Rel.to Credit Limit |  | S/4 only entity |
| `IsNotedItmWithoutBalUpdt` | `MERKP_074U` |  |  |  |  | `Boolean` |  | Noted Items |  | S/4 only entity |


## Entity: `SpecialGeneralLedgerCodeText`

- **ABAP CDS Name:** `I_SpecialGLCodeText`
- **Label:** Special General Ledger Code - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `FinancialAccountType` | `KOART` |  |  |  |  | `String(1)` | Y | Account Type |  | S/4 only entity |
| `SpecialGLCode` | `UMSKZ` |  |  |  |  | `String(1)` | Y | Special G/L Ind. |  | S/4 only entity |
| `Language` | `SPRAS` |  |  |  |  | `String(2)` | Y | Language Key |  | S/4 only entity |
| `SpecialGLCodeName` | `KTEXT_074T` |  |  |  |  | `String(7)` |  | Name |  | S/4 only entity |
| `SpecialGLCodeLongName` | `LTEXT_074T` |  |  |  |  | `String(30)` |  | Description |  | S/4 only entity |


## Entity: `SubledgerAccountLineItemType`

- **ABAP CDS Name:** `I_SubLedgerAccLineItemType`
- **Label:** SubLedger Account LineItem Type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `SubLedgerAcctLineItemType` | `SLALITTYPE` |  |  |  |  | `String(5)` | Y | SLA Line Item Type |  | S/4 only entity |


## Entity: `SubledgerAccountLineItemTypeText`

- **ABAP CDS Name:** `I_SubLedgerAccLineItemTypeT`
- **Label:** Subledger Account Line Item Type - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `SubLedgerAcctLineItemType` | `SLALITTYPE` |  |  |  |  | `String(5)` | Y | SLA Line Item Type |  | S/4 only entity |
| `Language` | `LANGU` |  |  |  |  | `String(2)` | Y | Language Key |  | S/4 only entity |
| `SubLedgerAcctLineItemTypeName` | `FIS_SLALITTYPE_DESC` |  |  |  |  | `String(70)` |  | Subl. LIt. Type Text |  | S/4 only entity |
