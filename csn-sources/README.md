# SAP S/4HANA Cloud — CSN Data Product Reference

Parsed from official SAP CSN JSON files. English labels only. One markdown file per data product.

Each field row shows: CDS field name · ABAP data element (from JSON) · ECC table/field · S/4 ACDOCA table/field · type · key · label · currency/UOM ref · FK association · ECC/S4 diff flag.

---

## Naming Conventions

| Layer | Convention | Example |
|---|---|---|
| **ECC ABAP tables** | Uppercase, 4–6 chars, no prefix | `BKPF`, `BSEG`, `CSKS`, `SKA1` |
| **ECC ABAP fields** | Uppercase, 4–10 chars | `BUKRS`, `GJAHR`, `HKONT`, `SHKZG` |
| **S/4 ACDOCA fields** | Uppercase, often R-prefixed for renamed keys | `RBUKRS`, `RACCT`, `RCNTR`, `DRCRK` |
| **CDS entity names** | PascalCase, prefixed `I_` in ABAP | `I_JournalEntry`, `I_CostCenter` |
| **CDS field names** | PascalCase | `CompanyCode`, `GLAccount`, `DebitCreditCode` |
| **ABAP data elements** | Uppercase with namespace prefix in S/4 | `FIS_BUKRS`, `FARP_BELNR_D`, `BKTXT` (no prefix = same as ECC) |

**Key rename: ECC → ACDOCA**

| ECC Field | ECC Table | ACDOCA Field | Note |
|---|---|---|---|
| `BUKRS` | BKPF / BSEG | `RBUKRS` | R-prefix = "reference company code" |
| `HKONT` | BSEG | `RACCT` | Account number |
| `KOSTL` | BSEG | `RCNTR` | Cost center |
| `SHKZG` | BSEG | `DRCRK` | Debit/Credit indicator |
| `DMBTR` | BSEG | `HSL` | Amount in company code currency |
| `WRBTR` | BSEG | `WSL` | Amount in transaction currency |
| `WAERS` | BKPF | `RWCUR` | Transaction currency key |
| `MONAT` | BKPF | `POPER` | Fiscal period (ECC unpadded; ACDOCA zero-padded `003`) |
| `BUZEI` | BSEG | `DOCLN` | Line item (3 chars in BSEG → 6 chars in ACDOCA) |
| _(none)_ | — | `KSL` / `RKCUR` | Global currency amount/key — S/4 only |

---

## ECC / S4 Diff Flags

| Flag | Meaning |
|---|---|
| `S/4 only — no ECC equivalent` | Field (e.g. `SourceLedger`, `AmountInGlobalCurrency`) does not exist in ECC |
| `S/4 only entity` | Entity has no ECC CDC mapping — native S/4 object |
| `ECC MONAT unpadded '3'; S/4 ACDOCA.POPER zero-padded '003'` | Fiscal period format difference — pad in ECC Bronze |
| `Filter ACDOCA.RLDNR='0L' for leading ledger` | S/4 multi-ledger; ECC is single-ledger |
| `ECC: not in BSEG — derive via FX join; S/4: native in ACDOCA.KSL/RKCUR` | Global currency gap |

---

## Data Products

| Data Product | Primary Entity | ECC Tables (ABAP) | S/4 Tables |
|---|---|---|---|
| [ARBankStatement](./sap-s4com-ARBankStatement-v1.md) | `ARBankStatement` | FEBKO, FEBEP | S/4 bank statement CDS |
| [BillingDocument](./sap-s4com-BillingDocument-v1.md) | `BillingDocument`, `BillingDocumentItem` | VBRK, VBRP | VBRK, VBRP |
| [CashFlow](./sap-s4com-CashFlow-v1.md) | `CashFlow`, `CashFlowForecast` | _(S/4 only — no ECC equivalent)_ | FQM tables |
| [CnsldtnGLChartOfAccounts](./sap-s4com-CnsldtnGLChartOfAccounts-v1.md) | `CnsldtnGLChartOfAccounts` | GLPCA, GLPCT | S/4 consolidation CDS |
| [CompanyCode](./sap-s4com-CompanyCode-v1.md) | `CompanyCode` | T001 | T001 |
| [ControllingArea](./sap-s4com-ControllingArea-v1.md) | `ControllingArea` | TKA01 | TKA01 |
| [CostCenter](./sap-s4com-CostCenter-v1.md) | `CostCenter`, `CostCenterText`, `CostCenterHierarchyNode` | CSKS, CSKT, SETHEADER, SETNODE, SETLEAF | CSKS, CSKT |
| [CostCenterActivityType](./sap-s4com-CostCenterActivityType-v1.md) | `CostCenterActivityType`, `CostCenterActivityTypeText` | CSLA, CSLT | CSLA, CSLT |
| [CostOriginGroup](./sap-s4com-CostOriginGroup-v1.md) | `CostOriginGroup`, `CostOriginGroupText` | CSKG, CSKGT | CSKG, CSKGT |
| [Customer](./sap-s4com-Customer-v1.md) | `Customer`, `CustomerCompanyCode` | KNA1, KNB1, KNB5, ADRC | KNA1, KNB1, BUT000 |
| [FinancialTransaction](./sap-s4com-FinancialTransaction-v1.md) | `FinancialTransaction` | VTBFHA, VTBFHAZU _(Treasury)_ | S/4 Treasury CDS |
| [FiscalYear](./sap-s4com-FiscalYear-v1.md) | `FiscalYear`, `FiscalYearVariant` | T009, T009B | T009, T009B |
| [FunctionalArea](./sap-s4com-FunctionalArea-v1.md) | `FunctionalArea`, `FunctionalAreaText` | TFKB, TFKBT | TFKB, TFKBT |
| [GeneralLedgerAccount](./sap-s4com-GeneralLedgerAccount-v1.md) | `GeneralLedgerAccount`, `GeneralLedgerAccountLineItem` | SKA1, SKB1, SKAT, BSEG, ACDOCA | SKA1, SKB1, SKAT, ACDOCA |
| [InvoiceList](./sap-s4com-InvoiceList-v1.md) | `InvoiceList`, `InvoiceListItem` | VFRK, VFRP | VFRK, VFRP |
| [JournalEntryCodes](./sap-s4com-JournalEntryCodes-v1.md) | `JournalEntryType`, `BusinessTransactionType` | T003, T003T, TBSL, TBSLT | T003, T003T |
| [JournalEntryHeader](./sap-s4com-JournalEntryHeader-v1.md) | `JournalEntry` | **BKPF** | ACDOCA (header subset) |
| [JournalEntryItemCodes](./sap-s4com-JournalEntryItemCodes-v1.md) | `DebitCreditCode`, `PostingKey`, `SpecialGeneralLedgerCode` | TBSL, TBSLT, T074, T074T | ACDOCA code fields |
| [Ledger](./sap-s4com-Ledger-v1.md) | `Ledger`, `LedgerText` | T881, T881T _(New GL only)_ | T881, T881T |
| [Plant](./sap-s4com-Plant-v1.md) | `Plant` | T001W | T001W |
| [Product](./sap-s4com-Product-v1.md) | `Product`, `ProductPlant`, `ProductDescription` | MARA, MARC, MAKT, MBEW | MARA, MARC, MAKT |
| [ProfitCenter](./sap-s4com-ProfitCenter-v1.md) | `ProfitCenter`, `ProfitCenterText`, `ProfitCenterHierarchyNode` | CEPC, CEPCT, SETHEADER, SETNODE, SETLEAF | CEPC, CEPCT |
| [PurchaseOrder](./sap-s4com-PurchaseOrder-v1.md) | `PurchaseOrder`, `PurchaseOrderItem`, `PurchaseOrderAccountAssignment` | EKKO, EKPO, EKKN | EKKO, EKPO, EKKN |
| [SalesMasterDataConfiguration](./sap-s4com-SalesMasterDataConfiguration-v1.md) | _(SD config code tables)_ | TVAK, TVAP, TVRO, TVCPA | SD config tables |
| [SalesOrder](./sap-s4com-SalesOrder-v1.md) | `SalesOrder`, `SalesOrderItem` | VBAK, VBAP, VBKD, VEDA | VBAK, VBAP |
| [Supplier](./sap-s4com-Supplier-v1.md) | `Supplier`, `SupplierCompanyCode`, `SupplierPurchasingOrganization` | LFA1, LFB1, LFM1, ADRC | LFA1, LFB1, BUT000 |
