# CashFlow

> Source file: `sap-s4com-CashFlow-v1.json`


## Entity: `CashFlow`

- **ABAP Name:** `I_CashLiquidityActualFlow`
- **Label:** Cash Liquidity Actual Flow for WCI
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `CashFlowID` |  |  |  | `String(16)` | Y | Flow ID |  |  | S/4 only entity — no ECC CDC mapping |
| `CshFlwValdtyStrtDteTmeVal` |  |  |  | `Decimal(21,7)` | Y | FQM Flow Valid From |  |  | S/4 only entity — no ECC CDC mapping |
| `CompanyCode` |  |  |  | `String(4)` |  | Company Code |  |  | S/4 only entity — no ECC CDC mapping |
| `TransactionDate` |  |  |  | `Date` |  | Transaction Date |  |  | S/4 only entity — no ECC CDC mapping |
| `PostingDate` |  |  |  | `Date` |  | Posting Date |  |  | S/4 only entity — no ECC CDC mapping |
| `TransactionCurrency` |  |  |  | `String(5)` |  | Currency |  |  | S/4 only entity — no ECC CDC mapping |
| `AmountInTransactionCurrency` |  |  |  | `Decimal(34,4)` |  | Amount | TransactionCurrency |  | S/4 only entity — no ECC CDC mapping |
| `CompanyCodeCurrency` |  |  |  | `String(5)` |  | Currency |  |  | S/4 only entity — no ECC CDC mapping |
| `AmountInCompanyCodeCurrency` |  |  |  | `Decimal(34,4)` |  | Amount in Company Code Currency | CompanyCodeCurrency |  | S/4 only entity — no ECC CDC mapping |
| `GlobalCurrency` |  |  |  | `String(5)` |  | Global Currency |  |  | S/4 only — no ECC equivalent |
| `AmountInGlobalCurrency` |  |  |  | `Decimal(34,4)` |  | Amount in Global Currency | GlobalCurrency |  | S/4 only — no ECC equivalent |
| `BankAccountInternalID` |  |  |  | `String(10)` |  | Technical ID |  |  | S/4 only entity — no ECC CDC mapping |
| `Bank` |  |  |  | `String(15)` |  | Bank Key |  |  | S/4 only entity — no ECC CDC mapping |
| `BankCountry` |  |  |  | `String(3)` |  | Bank Ctry/Rgn. Key |  |  | S/4 only entity — no ECC CDC mapping |
| `BankName` |  |  |  | `String(60)` |  | Bank Name |  |  | S/4 only entity — no ECC CDC mapping |
| `CashFlowOID` |  |  |  | `String(128)` |  |  |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `CashFlowForecast`

- **ABAP Name:** `I_CashLiquidityForecastFlow`
- **Label:** Cash Liquidity Forecast Flow for WCI
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `CashFlowID` |  |  |  | `String(16)` | Y | Flow ID |  |  | S/4 only entity — no ECC CDC mapping |
| `CshFlwValdtyStrtDteTmeVal` |  |  |  | `Decimal(21,7)` | Y | FQM Flow Valid From |  |  | S/4 only entity — no ECC CDC mapping |
| `CompanyCode` |  |  |  | `String(4)` |  | Company Code |  |  | S/4 only entity — no ECC CDC mapping |
| `TransactionDate` |  |  |  | `Date` |  | Transaction Date |  |  | S/4 only entity — no ECC CDC mapping |
| `PostingDate` |  |  |  | `Date` |  | Posting Date |  |  | S/4 only entity — no ECC CDC mapping |
| `TransactionCurrency` |  |  |  | `String(5)` |  | Currency |  |  | S/4 only entity — no ECC CDC mapping |
| `AmountInTransactionCurrency` |  |  |  | `Decimal(34,4)` |  | Amount | TransactionCurrency |  | S/4 only entity — no ECC CDC mapping |
| `CompanyCodeCurrency` |  |  |  | `String(5)` |  | Currency |  |  | S/4 only entity — no ECC CDC mapping |
| `AmountInCompanyCodeCurrency` |  |  |  | `Decimal(34,4)` |  | Amount in Company Code Currency | CompanyCodeCurrency |  | S/4 only entity — no ECC CDC mapping |
| `GlobalCurrency` |  |  |  | `String(5)` |  | Global Currency |  |  | S/4 only — no ECC equivalent |
| `AmountInGlobalCurrency` |  |  |  | `Decimal(34,4)` |  | Amount in Global Currency | GlobalCurrency |  | S/4 only — no ECC equivalent |
| `BankAccountInternalID` |  |  |  | `String(10)` |  | Technical ID |  |  | S/4 only entity — no ECC CDC mapping |
| `CashFlowOID` |  |  |  | `String(128)` |  |  |  |  | S/4 only entity — no ECC CDC mapping |
