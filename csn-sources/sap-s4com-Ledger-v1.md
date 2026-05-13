# Ledger

> Source file: `sap-s4com-Ledger-v1.json`


## Entity: `Ledger`

- **ABAP Name:** `I_Ledger`
- **Label:** Ledger
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `Ledger` | `T881` | `RLDNR` | `String(2)` | Y | Ledger |  |  | S/4 only — no ECC equivalent |
| `IsLeadingLedger` | `T881` | `XLOAD` | `Boolean` |  | Leading Ledger |  |  |  |
| `LedgerApplication` |  |  | `String(2)` |  | Application |  |  | S/4 only entity |
| `LedgerSubApplication` |  |  | `String(3)` |  | Subapplication |  |  | S/4 only entity |
| `AccountingValuationView` |  |  | `String(1)` |  | Valuation View |  |  | S/4 only entity |
| `LedgerType` | `T881` | `LDGRTYPE` | `String(1)` |  | Ledger Type |  |  |  |
| `ExtensionLedgerType` |  |  | `String(1)` |  | Extn. Ledger Type |  |  | S/4 only entity |
| `ReferenceLedger` |  |  | `String(2)` |  | Fallback Ledger |  |  | S/4 only entity |
| `TechnicalLedger` |  |  | `String(2)` |  | Technical Ledger |  |  | S/4 only entity |


## Entity: `LedgerCompanyCodeCurrencyRoles`

- **ABAP Name:** `I_LedgerCompanyCodeCrcyRoles`
- **Label:** Currency Roles for Ledger
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `Ledger` |  |  | `String(2)` | Y | Ledger |  | _Ledger | S/4 only — no ECC equivalent |
| `CompanyCode` | `T001` | `BUKRS` | `String(4)` | Y | Company Code |  |  |  |
| `FiscalYearVariant` |  |  | `String(2)` |  | Fiscal Year Variant |  |  | S/4 only entity |
| `CompanyCodeCurrencyRole` |  |  | `String(2)` |  | Company Code Currency Role |  |  | S/4 only entity |
| `GlobalCurrencyRole` |  |  | `String(2)` |  | Global Currency Role |  |  | S/4 only entity |
| `FreeDefinedCurrency1Role` |  |  | `String(2)` |  | Freely Defined Currency 1 Role |  |  | S/4 only entity |
| `FreeDefinedCurrency2Role` |  |  | `String(2)` |  | Freely Defined Currency 2 Role |  |  | S/4 only entity |
| `FreeDefinedCurrency3Role` |  |  | `String(2)` |  | Freely Defined Currency 3 Role |  |  | S/4 only entity |
| `FreeDefinedCurrency4Role` |  |  | `String(2)` |  | Freely Defined Currency 4 Role |  |  | S/4 only entity |
| `FreeDefinedCurrency5Role` |  |  | `String(2)` |  | Freely Defined Currency 5 Role |  |  | S/4 only entity |
| `FreeDefinedCurrency6Role` |  |  | `String(2)` |  | Freely Defined Currency 6 Role |  |  | S/4 only entity |
| `FreeDefinedCurrency7Role` |  |  | `String(2)` |  | Freely Defined Currency 7 Role |  |  | S/4 only entity |
| `FreeDefinedCurrency8Role` |  |  | `String(2)` |  | Freely Defined Currency 8 Role |  |  | S/4 only entity |
| `AccountingPrinciple` |  |  | `String(4)` |  | Accounting Principle |  |  | S/4 only entity |
| `FunctionalCurrencyRole` |  |  | `String(2)` |  | Functional Currency Role |  |  | S/4 only entity |
| `AdditionalCurrency1Field` |  |  | `String(4)` |  | Additional Currency 1 Field |  |  | S/4 only entity |
| `AdditionalCurrency2Field` |  |  | `String(4)` |  | Additional Currency 2 Field |  |  | S/4 only entity |


## Entity: `LedgerSourceLedger`

- **ABAP Name:** `I_LedgerSourceLedger`
- **Label:** Mapping between Ledger and Source Ledger
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `Ledger` |  |  | `String(2)` | Y | Ledger |  | _Ledger | S/4 only — no ECC equivalent |
| `SourceLedger` |  |  | `String(2)` | Y | Source Ledger |  |  | S/4 only — no ECC equivalent; Filter SourceLedger='0L' for leading ledger in S/4 |


## Entity: `LedgerText`

- **ABAP Name:** `I_LedgerText`
- **Label:** Ledger - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `Ledger` |  |  | `String(2)` | Y | Ledger |  |  | S/4 only — no ECC equivalent |
| `Language` |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity |
| `LedgerName` |  |  | `String(30)` |  | Ledger Name |  |  | S/4 only entity |
