# Ledger

> Source file: `sap-s4com-Ledger-v1.json`


## Entity: `Ledger`

- **ABAP Name:** `I_Ledger`
- **Label:** Ledger
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Ledger` | `Ledger` | `String(2)` | Y | Ledger |  |  | S/4 only — no ECC equivalent; S/4 only entity (no ECC CDC mapping) |
| `IsLeadingLedger` | `IsLeadingLedger` | `Boolean` |  | Leading Ledger |  |  | S/4 only entity (no ECC CDC mapping) |
| `LedgerApplication` | `LedgerApplication` | `String(2)` |  | Application |  |  | S/4 only entity (no ECC CDC mapping) |
| `LedgerSubApplication` | `LedgerSubApplication` | `String(3)` |  | Subapplication |  |  | S/4 only entity (no ECC CDC mapping) |
| `AccountingValuationView` | `AccountingValuationView` | `String(1)` |  | Valuation View |  |  | S/4 only entity (no ECC CDC mapping) |
| `LedgerType` | `LedgerType` | `String(1)` |  | Ledger Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `ExtensionLedgerType` | `ExtensionLedgerType` | `String(1)` |  | Extn. Ledger Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `ReferenceLedger` | `ReferenceLedger` | `String(2)` |  | Fallback Ledger |  |  | S/4 only entity (no ECC CDC mapping) |
| `TechnicalLedger` | `TechnicalLedger` | `String(2)` |  | Technical Ledger |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `LedgerCompanyCodeCurrencyRoles`

- **ABAP Name:** `I_LedgerCompanyCodeCrcyRoles`
- **Label:** Currency Roles for Ledger
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Ledger` | `Ledger` | `String(2)` | Y | Ledger |  | _Ledger | S/4 only — no ECC equivalent; S/4 only entity (no ECC CDC mapping) |
| `CompanyCode` | `CompanyCode` | `String(4)` | Y | Company Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `FiscalYearVariant` | `FiscalYearVariant` | `String(2)` |  | Fiscal Year Variant |  |  | S/4 only entity (no ECC CDC mapping) |
| `CompanyCodeCurrencyRole` | `CompanyCodeCurrencyRole` | `String(2)` |  | Company Code Currency Role |  |  | S/4 only entity (no ECC CDC mapping) |
| `GlobalCurrencyRole` | `GlobalCurrencyRole` | `String(2)` |  | Global Currency Role |  |  | S/4 only entity (no ECC CDC mapping); S/4 only — ECC BSEG lacks global currency |
| `FreeDefinedCurrency1Role` | `FreeDefinedCurrency1Role` | `String(2)` |  | Freely Defined Currency 1 Role |  |  | S/4 only entity (no ECC CDC mapping) |
| `FreeDefinedCurrency2Role` | `FreeDefinedCurrency2Role` | `String(2)` |  | Freely Defined Currency 2 Role |  |  | S/4 only entity (no ECC CDC mapping) |
| `FreeDefinedCurrency3Role` | `FreeDefinedCurrency3Role` | `String(2)` |  | Freely Defined Currency 3 Role |  |  | S/4 only entity (no ECC CDC mapping) |
| `FreeDefinedCurrency4Role` | `FreeDefinedCurrency4Role` | `String(2)` |  | Freely Defined Currency 4 Role |  |  | S/4 only entity (no ECC CDC mapping) |
| `FreeDefinedCurrency5Role` | `FreeDefinedCurrency5Role` | `String(2)` |  | Freely Defined Currency 5 Role |  |  | S/4 only entity (no ECC CDC mapping) |
| `FreeDefinedCurrency6Role` | `FreeDefinedCurrency6Role` | `String(2)` |  | Freely Defined Currency 6 Role |  |  | S/4 only entity (no ECC CDC mapping) |
| `FreeDefinedCurrency7Role` | `FreeDefinedCurrency7Role` | `String(2)` |  | Freely Defined Currency 7 Role |  |  | S/4 only entity (no ECC CDC mapping) |
| `FreeDefinedCurrency8Role` | `FreeDefinedCurrency8Role` | `String(2)` |  | Freely Defined Currency 8 Role |  |  | S/4 only entity (no ECC CDC mapping) |
| `AccountingPrinciple` | `AccountingPrinciple` | `String(4)` |  | Accounting Principle |  |  | S/4 only entity (no ECC CDC mapping) |
| `FunctionalCurrencyRole` | `FunctionalCurrencyRole` | `String(2)` |  | Functional Currency Role |  |  | S/4 only entity (no ECC CDC mapping) |
| `AdditionalCurrency1Field` | `AdditionalCurrency1Field` | `String(4)` |  | Additional Currency 1 Field |  |  | S/4 only entity (no ECC CDC mapping) |
| `AdditionalCurrency2Field` | `AdditionalCurrency2Field` | `String(4)` |  | Additional Currency 2 Field |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `LedgerSourceLedger`

- **ABAP Name:** `I_LedgerSourceLedger`
- **Label:** Mapping between Ledger and Source Ledger
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Ledger` | `Ledger` | `String(2)` | Y | Ledger |  | _Ledger | S/4 only — no ECC equivalent; S/4 only entity (no ECC CDC mapping) |
| `SourceLedger` | `SourceLedger` | `String(2)` | Y | Source Ledger |  |  | S/4 only — no ECC equivalent; S/4 only entity (no ECC CDC mapping); S/4 only — use filter SourceLedger='0L' for leading ledger |


## Entity: `LedgerText`

- **ABAP Name:** `I_LedgerText`
- **Label:** Ledger - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Ledger` | `Ledger` | `String(2)` | Y | Ledger |  |  | S/4 only — no ECC equivalent; S/4 only entity (no ECC CDC mapping) |
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `LedgerName` | `LedgerName` | `String(30)` |  | Ledger Name |  |  | S/4 only entity (no ECC CDC mapping) |
