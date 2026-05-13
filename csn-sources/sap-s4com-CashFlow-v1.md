# CashFlow

> Source file: `sap-s4com-CashFlow-v1.json`


## Entity: `CashFlow`

- **ABAP Name:** `I_CashLiquidityActualFlow`
- **Label:** Cash Liquidity Actual Flow for WCI
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `CashFlowID` | `CashFlowID` | `String(16)` | Y | Flow ID |  |  | S/4 only entity (no ECC CDC mapping) |
| `CshFlwValdtyStrtDteTmeVal` | `CshFlwValdtyStrtDteTmeVal` | `Decimal(21,7)` | Y | FQM Flow Valid From |  |  | S/4 only entity (no ECC CDC mapping) |
| `CompanyCode` | `CompanyCode` | `String(4)` |  | Company Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `TransactionDate` | `TransactionDate` | `Date` |  | Transaction Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `PostingDate` | `PostingDate` | `Date` |  | Posting Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `TransactionCurrency` | `TransactionCurrency` | `String(5)` |  | Currency |  |  | S/4 only entity (no ECC CDC mapping) |
| `AmountInTransactionCurrency` | `AmountInTransactionCurrency` | `Decimal(34,4)` |  | Amount | TransactionCurrency |  | S/4 only entity (no ECC CDC mapping) |
| `CompanyCodeCurrency` | `CompanyCodeCurrency` | `String(5)` |  | Currency |  |  | S/4 only entity (no ECC CDC mapping) |
| `AmountInCompanyCodeCurrency` | `AmountInCompanyCodeCurrency` | `Decimal(34,4)` |  | Amount in Company Code Currency | CompanyCodeCurrency |  | S/4 only entity (no ECC CDC mapping) |
| `GlobalCurrency` | `GlobalCurrency` | `String(5)` |  | Global Currency |  |  | S/4 only — no ECC equivalent; S/4 only entity (no ECC CDC mapping); S/4 only — ECC BSEG lacks global currency |
| `AmountInGlobalCurrency` | `AmountInGlobalCurrency` | `Decimal(34,4)` |  | Amount in Global Currency | GlobalCurrency |  | S/4 only — no ECC equivalent; S/4 only entity (no ECC CDC mapping); S/4 only — ECC BSEG lacks global currency |
| `BankAccountInternalID` | `BankAccountInternalID` | `String(10)` |  | Technical ID |  |  | S/4 only entity (no ECC CDC mapping) |
| `Bank` | `Bank` | `String(15)` |  | Bank Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `BankCountry` | `BankCountry` | `String(3)` |  | Bank Ctry/Rgn. Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `BankName` | `BankName` | `String(60)` |  | Bank Name |  |  | S/4 only entity (no ECC CDC mapping) |
| `CashFlowOID` | `CashFlowOID` | `String(128)` |  |  |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `CashFlowForecast`

- **ABAP Name:** `I_CashLiquidityForecastFlow`
- **Label:** Cash Liquidity Forecast Flow for WCI
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `CashFlowID` | `CashFlowID` | `String(16)` | Y | Flow ID |  |  | S/4 only entity (no ECC CDC mapping) |
| `CshFlwValdtyStrtDteTmeVal` | `CshFlwValdtyStrtDteTmeVal` | `Decimal(21,7)` | Y | FQM Flow Valid From |  |  | S/4 only entity (no ECC CDC mapping) |
| `CompanyCode` | `CompanyCode` | `String(4)` |  | Company Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `TransactionDate` | `TransactionDate` | `Date` |  | Transaction Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `PostingDate` | `PostingDate` | `Date` |  | Posting Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `TransactionCurrency` | `TransactionCurrency` | `String(5)` |  | Currency |  |  | S/4 only entity (no ECC CDC mapping) |
| `AmountInTransactionCurrency` | `AmountInTransactionCurrency` | `Decimal(34,4)` |  | Amount | TransactionCurrency |  | S/4 only entity (no ECC CDC mapping) |
| `CompanyCodeCurrency` | `CompanyCodeCurrency` | `String(5)` |  | Currency |  |  | S/4 only entity (no ECC CDC mapping) |
| `AmountInCompanyCodeCurrency` | `AmountInCompanyCodeCurrency` | `Decimal(34,4)` |  | Amount in Company Code Currency | CompanyCodeCurrency |  | S/4 only entity (no ECC CDC mapping) |
| `GlobalCurrency` | `GlobalCurrency` | `String(5)` |  | Global Currency |  |  | S/4 only — no ECC equivalent; S/4 only entity (no ECC CDC mapping); S/4 only — ECC BSEG lacks global currency |
| `AmountInGlobalCurrency` | `AmountInGlobalCurrency` | `Decimal(34,4)` |  | Amount in Global Currency | GlobalCurrency |  | S/4 only — no ECC equivalent; S/4 only entity (no ECC CDC mapping); S/4 only — ECC BSEG lacks global currency |
| `BankAccountInternalID` | `BankAccountInternalID` | `String(10)` |  | Technical ID |  |  | S/4 only entity (no ECC CDC mapping) |
| `CashFlowOID` | `CashFlowOID` | `String(128)` |  |  |  |  | S/4 only entity (no ECC CDC mapping) |
