# CashFlow

> Source file: `sap-s4com-CashFlow-v1.json`


## Entity: `CashFlow`

- **ABAP CDS Name:** `I_CashLiquidityActualFlow`
- **Label:** Cash Liquidity Actual Flow for WCI
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `CashFlowID` |  |  |  |  |  | `String(16)` | Y | Flow ID |  | S/4 only entity |
| `CshFlwValdtyStrtDteTmeVal` |  |  |  |  |  | `Decimal(21,7)` | Y | FQM Flow Valid From |  | S/4 only entity |
| `CompanyCode` |  |  |  |  |  | `String(4)` |  | Company Code |  | S/4 only entity |
| `TransactionDate` |  |  |  |  |  | `Date` |  | Transaction Date |  | S/4 only entity |
| `PostingDate` |  |  |  |  |  | `Date` |  | Posting Date |  | S/4 only entity |
| `TransactionCurrency` |  |  |  |  |  | `String(5)` |  | Currency |  | S/4 only entity |
| `AmountInTransactionCurrency` |  |  |  |  |  | `Decimal(34,4)` |  | Amount | TransactionCurrency | S/4 only entity |
| `CompanyCodeCurrency` |  |  |  |  |  | `String(5)` |  | Currency |  | S/4 only entity |
| `AmountInCompanyCodeCurrency` |  |  |  |  |  | `Decimal(34,4)` |  | Amount in Company Code Currency | CompanyCodeCurrency | S/4 only entity |
| `GlobalCurrency` |  |  |  |  |  | `String(5)` |  | Global Currency |  | S/4 only — no ECC equivalent |
| `AmountInGlobalCurrency` |  |  |  |  |  | `Decimal(34,4)` |  | Amount in Global Currency | GlobalCurrency | S/4 only — no ECC equivalent |
| `BankAccountInternalID` |  |  |  |  |  | `String(10)` |  | Technical ID |  | S/4 only entity |
| `Bank` |  |  |  |  |  | `String(15)` |  | Bank Key |  | S/4 only entity |
| `BankCountry` |  |  |  |  |  | `String(3)` |  | Bank Ctry/Rgn. Key |  | S/4 only entity |
| `BankName` |  |  |  |  |  | `String(60)` |  | Bank Name |  | S/4 only entity |
| `CashFlowOID` |  |  |  |  |  | `String(128)` |  |  |  | S/4 only entity |


## Entity: `CashFlowForecast`

- **ABAP CDS Name:** `I_CashLiquidityForecastFlow`
- **Label:** Cash Liquidity Forecast Flow for WCI
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `CashFlowID` |  |  |  |  |  | `String(16)` | Y | Flow ID |  | S/4 only entity |
| `CshFlwValdtyStrtDteTmeVal` |  |  |  |  |  | `Decimal(21,7)` | Y | FQM Flow Valid From |  | S/4 only entity |
| `CompanyCode` |  |  |  |  |  | `String(4)` |  | Company Code |  | S/4 only entity |
| `TransactionDate` |  |  |  |  |  | `Date` |  | Transaction Date |  | S/4 only entity |
| `PostingDate` |  |  |  |  |  | `Date` |  | Posting Date |  | S/4 only entity |
| `TransactionCurrency` |  |  |  |  |  | `String(5)` |  | Currency |  | S/4 only entity |
| `AmountInTransactionCurrency` |  |  |  |  |  | `Decimal(34,4)` |  | Amount | TransactionCurrency | S/4 only entity |
| `CompanyCodeCurrency` |  |  |  |  |  | `String(5)` |  | Currency |  | S/4 only entity |
| `AmountInCompanyCodeCurrency` |  |  |  |  |  | `Decimal(34,4)` |  | Amount in Company Code Currency | CompanyCodeCurrency | S/4 only entity |
| `GlobalCurrency` |  |  |  |  |  | `String(5)` |  | Global Currency |  | S/4 only — no ECC equivalent |
| `AmountInGlobalCurrency` |  |  |  |  |  | `Decimal(34,4)` |  | Amount in Global Currency | GlobalCurrency | S/4 only — no ECC equivalent |
| `BankAccountInternalID` |  |  |  |  |  | `String(10)` |  | Technical ID |  | S/4 only entity |
| `CashFlowOID` |  |  |  |  |  | `String(128)` |  |  |  | S/4 only entity |
