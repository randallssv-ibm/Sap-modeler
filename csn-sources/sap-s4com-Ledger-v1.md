# Ledger

> Source file: `sap-s4com-Ledger-v1.json`


## Entity: `Ledger`

- **ABAP CDS Name:** `I_Ledger`
- **Label:** Ledger
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** T881

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Ledger` |  | `T881` | `RLDNR` |  |  | `String(2)` | Y | Ledger |  |  |
| `IsLeadingLedger` |  | `T881` | `XLOAD` |  |  | `Boolean` |  | Leading Ledger |  |  |
| `LedgerApplication` |  |  |  |  |  | `String(2)` |  | Application |  |  |
| `LedgerSubApplication` |  |  |  |  |  | `String(3)` |  | Subapplication |  |  |
| `AccountingValuationView` |  |  |  |  |  | `String(1)` |  | Valuation View |  |  |
| `LedgerType` |  |  |  |  |  | `String(1)` |  | Ledger Type |  |  |
| `ExtensionLedgerType` |  |  |  |  |  | `String(1)` |  | Extn. Ledger Type |  |  |
| `ReferenceLedger` |  |  |  |  |  | `String(2)` |  | Fallback Ledger |  |  |
| `TechnicalLedger` |  |  |  |  |  | `String(2)` |  | Technical Ledger |  |  |


## Entity: `LedgerCompanyCodeCurrencyRoles`

- **ABAP CDS Name:** `I_LedgerCompanyCodeCrcyRoles`
- **Label:** Currency Roles for Ledger
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** T881

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Ledger` |  |  |  |  |  | `String(2)` | Y | Ledger |  |  |
| `CompanyCode` |  |  |  |  |  | `String(4)` | Y | Company Code |  |  |
| `FiscalYearVariant` |  |  |  |  |  | `String(2)` |  | Fiscal Year Variant |  |  |
| `CompanyCodeCurrencyRole` |  |  |  |  |  | `String(2)` |  | Company Code Currency Role |  |  |
| `GlobalCurrencyRole` |  |  |  |  |  | `String(2)` |  | Global Currency Role |  |  |
| `FreeDefinedCurrency1Role` |  |  |  |  |  | `String(2)` |  | Freely Defined Currency 1 Role |  |  |
| `FreeDefinedCurrency2Role` |  |  |  |  |  | `String(2)` |  | Freely Defined Currency 2 Role |  |  |
| `FreeDefinedCurrency3Role` |  |  |  |  |  | `String(2)` |  | Freely Defined Currency 3 Role |  |  |
| `FreeDefinedCurrency4Role` |  |  |  |  |  | `String(2)` |  | Freely Defined Currency 4 Role |  |  |
| `FreeDefinedCurrency5Role` |  |  |  |  |  | `String(2)` |  | Freely Defined Currency 5 Role |  |  |
| `FreeDefinedCurrency6Role` |  |  |  |  |  | `String(2)` |  | Freely Defined Currency 6 Role |  |  |
| `FreeDefinedCurrency7Role` |  |  |  |  |  | `String(2)` |  | Freely Defined Currency 7 Role |  |  |
| `FreeDefinedCurrency8Role` |  |  |  |  |  | `String(2)` |  | Freely Defined Currency 8 Role |  |  |
| `AccountingPrinciple` |  |  |  |  |  | `String(4)` |  | Accounting Principle |  |  |
| `FunctionalCurrencyRole` |  |  |  |  |  | `String(2)` |  | Functional Currency Role |  |  |
| `AdditionalCurrency1Field` |  |  |  |  |  | `String(4)` |  | Additional Currency 1 Field |  |  |
| `AdditionalCurrency2Field` |  |  |  |  |  | `String(4)` |  | Additional Currency 2 Field |  |  |


## Entity: `LedgerSourceLedger`

- **ABAP CDS Name:** `I_LedgerSourceLedger`
- **Label:** Mapping between Ledger and Source Ledger
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** T882

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Ledger` |  |  |  |  |  | `String(2)` | Y | Ledger |  |  |
| `SourceLedger` |  |  |  |  |  | `String(2)` | Y | Source Ledger |  | S/4 only — no ECC equivalent; Filter ACDOCA.RLDNR='0L' for leading ledger |


## Entity: `LedgerText`

- **ABAP CDS Name:** `I_LedgerText`
- **Label:** Ledger - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** T881T

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Ledger` |  |  |  |  |  | `String(2)` | Y | Ledger |  |  |
| `Language` |  |  |  |  |  | `String(2)` | Y | Language Key |  |  |
| `LedgerName` |  |  |  |  |  | `String(30)` |  | Ledger Name |  |  |
