# JournalEntryItemCodes

> Source file: `sap-s4com-JournalEntryItemCodes-v1.json`


## Entity: `AssetAcctTransClassification`

- **ABAP Name:** `I_MovementCategory`
- **Label:** Movement Category
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `AssetAcctTransClassfctn` | `FAA_MOVCAT` | `FAA_MOVCAT` |  | `String(2)` | Y | Trans. Type Category |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `ControllingDebitCreditCode`

- **ABAP Name:** `I_ControllingDebitCreditCode`
- **Label:** Controlling Debit Credit Code
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `ControllingDebitCreditCode` | `FINS_CO_BELKZ` | `CO_BELKZ` |  | `String(1)` | Y | Dr/Cr indicator  CO |  |  | S/4 only entity — no ECC CDC mapping |
| `DomainValue` |  |  |  | `String(1)` |  |  |  |  | S/4 only entity — no ECC CDC mapping |
| `DomainValue_2` | `DOMVALUE_L` | `DOMVALUE_L` |  | `String(10)` |  | Lower Value |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `ControllingDebitCreditCodeText`

- **ABAP Name:** `I_ControllingDebitCreditCodeT`
- **Label:** Debit Credit Code in Controlling - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `ControllingDebitCreditCode` |  |  |  | `String(1)` | Y |  |  |  | S/4 only entity — no ECC CDC mapping |
| `Language` | `SPRAS` | `SPRAS` |  | `String(2)` | Y | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `ControllingDebitCreditCodeName` | `VAL_TEXT` | `VAL_TEXT` |  | `String(60)` |  | Short Description |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `DebitCreditCode`

- **ABAP Name:** `I_DebitCreditCode`
- **Label:** Debit Credit Code
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `DebitCreditCode` | `FIS_SHKZG` | `SHKZG` |  | `String(1)` | Y | Debit/Credit Code |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `DebitCreditCodeText`

- **ABAP Name:** `I_DebitCreditCodeText`
- **Label:** Debit Credit Code - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Language` | `SPRAS` | `SPRAS` |  | `String(2)` | Y | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `DebitCreditCode` | `FIS_SHKZG` | `SHKZG` |  | `String(1)` | Y | Debit/Credit Code |  |  | S/4 only entity — no ECC CDC mapping |
| `DebitCreditCodeName` | `FIS_SHKZG_NAME` | `SHKZG_NAME` |  | `String(60)` |  | D/C Code Name |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `FinancialAccountType`

- **ABAP Name:** `I_FinancialAccountType`
- **Label:** Financial Account Type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `FinancialAccountType` | `FARP_KOART` | `KOART` |  | `String(1)` | Y | Account Type |  |  | S/4 only entity — no ECC CDC mapping |
| `DomainValue` | `DOMVALUE_L` | `DOMVALUE_L` |  | `String(10)` |  | Lower Value |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `FinancialAccountTypeText`

- **ABAP Name:** `I_FinancialAccountTypeText`
- **Label:** Financial Account Type - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `FinancialAccountType` | `FARP_KOART` | `KOART` |  | `String(1)` | Y | Account Type |  |  | S/4 only entity — no ECC CDC mapping |
| `Language` | `SPRAS` | `SPRAS` |  | `String(2)` | Y | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `FinancialAccountTypeName` | `FIS_FIN_ACC_TYPE_NAME` | `FIN_ACC_TYPE_NAME` |  | `String(60)` |  | Fin. Acc. Type Name |  |  | S/4 only entity — no ECC CDC mapping |
| `DomainValue` | `DOMVALUE_L` | `DOMVALUE_L` |  | `String(10)` |  | Lower Value |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `GeneralLedgerRecordType`

- **ABAP Name:** `I_GLRecordType`
- **Label:** General Ledger Record Type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `GLRecordType` | `RRCTY` | `RRCTY` |  | `String(1)` | Y | Record Type |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `JournalEntryItemObsoleteReason`

- **ABAP Name:** `I_JrnlEntryItemObsoleteRsn`
- **Label:** Obsolete Reason of Journal Entry Item
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `JrnlEntryItemObsoleteReason` | `FINS_OBSOLETE_ITEM_REASON` | `OBSOLETE_ITEM_REASON` |  | `String(1)` | Y | Obsolete Reason |  |  | S/4 only entity — no ECC CDC mapping |
| `DomainValue` | `DOMVALUE_L` | `DOMVALUE_L` |  | `String(10)` |  | Lower Value |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `JrnlEntryItemObsltRsnText`

- **ABAP Name:** `I_JrnlEntryItemObsltRsnT`
- **Label:** Obsolete Reason of Entry Item - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `JrnlEntryItemObsoleteReason` | `FINS_OBSOLETE_ITEM_REASON` | `OBSOLETE_ITEM_REASON` |  | `String(1)` | Y | Obsolete Reason |  |  | S/4 only entity — no ECC CDC mapping |
| `Language` | `SPRAS` | `SPRAS` |  | `String(2)` | Y | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `DomainValue` | `DOMVALUE_L` | `DOMVALUE_L` |  | `String(10)` |  | Lower Value |  |  | S/4 only entity — no ECC CDC mapping |
| `JrnlEntryItemObsoleteRsnName` | `FIS_FIN_ACC_TYPE_NAME` | `FIN_ACC_TYPE_NAME` |  | `String(60)` |  | Fin. Acc. Type Name |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `MovementCategoryText`

- **ABAP Name:** `I_MovementCategoryText`
- **Label:** Movement Category - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `AssetAcctTransClassfctn` | `FAA_MOVCAT` | `FAA_MOVCAT` |  | `String(2)` | Y | Trans. Type Category |  |  | S/4 only entity — no ECC CDC mapping |
| `Language` | `LANGU` | `LANGU` |  | `String(2)` | Y | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `AssetAcctTransClassfctnName` | `FAA_MOVCAT_TEXT` | `FAA_MOVCAT_TEXT` |  | `String(50)` |  | Trans.Type Cat. Text |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `PostingKey`

- **ABAP Name:** `I_PostingKey`
- **Label:** Posting Key
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `PostingKey` | `FIS_BSCHL` | `BSCHL` |  | `String(2)` | Y | Posting Key |  |  | S/4 only entity — no ECC CDC mapping |
| `DebitCreditCode` | `FIS_SHKZG` | `SHKZG` |  | `String(1)` |  | Debit/Credit Code |  |  | S/4 only entity — no ECC CDC mapping |
| `FinancialAccountType` | `FARP_KOART` | `KOART` |  | `String(1)` |  | Account Type |  |  | S/4 only entity — no ECC CDC mapping |
| `IsSalesRelated` | `FARP_XUMSW` | `XUMSW` |  | `Boolean` |  | Sales-Related Item |  |  | S/4 only entity — no ECC CDC mapping |
| `IsUsedInPaymentTransaction` | `XZAHL` | `XZAHL` |  | `Boolean` |  | Payment Transaction |  |  | S/4 only entity — no ECC CDC mapping |
| `ReversalPostingKey` | `STBSL` | `STBSL` |  | `String(2)` |  | Reversal Posting Key |  |  | S/4 only entity — no ECC CDC mapping |
| `IsSpecialGLTransaction` | `XSONU` | `XSONU` |  | `Boolean` |  | Special G/L |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `PostingKeyText`

- **ABAP Name:** `I_PostingKeyText`
- **Label:** Posting Key - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Language` | `SPRAS` | `SPRAS` |  | `String(2)` | Y | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `PostingKey` | `FIS_BSCHL` | `BSCHL` |  | `String(2)` | Y | Posting Key |  |  | S/4 only entity — no ECC CDC mapping |
| `PostingKeyName` | `FIS_BSCHL_NAME` | `BSCHL_NAME` |  | `String(20)` |  | Posting Key Name |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `PostingKeyWithSpecialGLCode`

- **ABAP Name:** `I_PostingKeyWithSpecialGLCode`
- **Label:** Posting Key with Special General Ledger Code
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `PostingKey` | `FIS_BSCHL` | `BSCHL` |  | `String(2)` | Y | Posting Key |  | _PostingKey | S/4 only entity — no ECC CDC mapping |
| `SpecialGLCode` | `FAC_UMSKZ` | `UMSKZ` |  | `String(1)` | Y | Special G/L |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `PostingKeyWithSpecialGLCodeText`

- **ABAP Name:** `I_PostingKeyWthSpclGLCodeTxt`
- **Label:** Posting Key With Special General Leder Code - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Language` | `SPRAS` | `SPRAS` |  | `String(2)` | Y | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `PostingKey` | `FIS_BSCHL` | `BSCHL` |  | `String(2)` | Y | Posting Key |  | _PostingKey | S/4 only entity — no ECC CDC mapping |
| `SpecialGLCode` | `FAC_UMSKZ` | `UMSKZ` |  | `String(1)` | Y | Special G/L |  | _SpecialGLCode | S/4 only entity — no ECC CDC mapping |
| `FinancialAccountType` | `FARP_KOART` | `KOART` |  | `String(1)` |  | Account Type |  | _FinancialAccountType | S/4 only entity — no ECC CDC mapping |
| `PostingKeyName` | `FIS_BSCHL_NAME` | `BSCHL_NAME` |  | `String(20)` |  | Posting Key Name |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `SpecialGeneralLedgerCode`

- **ABAP Name:** `I_SpecialGLCode`
- **Label:** Special General Ledger Code
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `SpecialGLCode` | `UMSKZ` | `UMSKZ` |  | `String(1)` | Y | Special G/L Ind. |  |  | S/4 only entity — no ECC CDC mapping |
| `FinancialAccountType` | `KOART` | `KOART` |  | `String(1)` | Y | Account Type |  | _FinancialAccountType | S/4 only entity — no ECC CDC mapping |
| `SpecialGLTransactionType` | `UMSKS` | `UMSKS` |  | `String(1)` |  | Sp. G/L Trans.Type |  |  | S/4 only entity — no ECC CDC mapping |
| `CreditLimitIsChecked` | `KLIMP_074U` | `KLIMP_074U` |  | `Boolean` |  | Rel.to Credit Limit |  |  | S/4 only entity — no ECC CDC mapping |
| `IsNotedItmWithoutBalUpdt` | `MERKP_074U` | `MERKP_074U` |  | `Boolean` |  | Noted Items |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `SpecialGeneralLedgerCodeText`

- **ABAP Name:** `I_SpecialGLCodeText`
- **Label:** Special General Ledger Code - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `FinancialAccountType` | `KOART` | `KOART` |  | `String(1)` | Y | Account Type |  | _FinancialAccountType | S/4 only entity — no ECC CDC mapping |
| `SpecialGLCode` | `UMSKZ` | `UMSKZ` |  | `String(1)` | Y | Special G/L Ind. |  |  | S/4 only entity — no ECC CDC mapping |
| `Language` | `SPRAS` | `SPRAS` |  | `String(2)` | Y | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `SpecialGLCodeName` | `KTEXT_074T` | `KTEXT_074T` |  | `String(7)` |  | Name |  |  | S/4 only entity — no ECC CDC mapping |
| `SpecialGLCodeLongName` | `LTEXT_074T` | `LTEXT_074T` |  | `String(30)` |  | Description |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `SubledgerAccountLineItemType`

- **ABAP Name:** `I_SubLedgerAccLineItemType`
- **Label:** SubLedger Account LineItem Type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `SubLedgerAcctLineItemType` | `SLALITTYPE` | `SLALITTYPE` |  | `String(5)` | Y | SLA Line Item Type |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `SubledgerAccountLineItemTypeText`

- **ABAP Name:** `I_SubLedgerAccLineItemTypeT`
- **Label:** Subledger Account Line Item Type - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `SubLedgerAcctLineItemType` | `SLALITTYPE` | `SLALITTYPE` |  | `String(5)` | Y | SLA Line Item Type |  |  | S/4 only entity — no ECC CDC mapping |
| `Language` | `LANGU` | `LANGU` |  | `String(2)` | Y | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `SubLedgerAcctLineItemTypeName` | `FIS_SLALITTYPE_DESC` | `SLALITTYPE_DESC` |  | `String(70)` |  | Subl. LIt. Type Text |  |  | S/4 only entity — no ECC CDC mapping |
