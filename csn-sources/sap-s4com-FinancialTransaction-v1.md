# FinancialTransaction

> Source file: `sap-s4com-FinancialTransaction-v1.json`


## Entity: `FXFixingReferenceText`

- **ABAP CDS Name:** `I_FXFixingReferenceText`
- **Label:** Foreign Exchange Fixing Reference - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** VTBFXFR

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Language` | `SPRAS` |  |  |  |  | `String(2)` | Y | Language Key |  |  |
| `ForeignExchangeFixingReference` | `FTR_FIXING_REF_ID` |  |  |  |  | `String(30)` | Y | Fixing Reference ID |  |  |
| `FXFixingReferenceName` | `FTR_FIXING_REF_ID_TEXT` |  |  |  |  | `String(40)` |  | Fixing Ref. Desc. |  |  |


## Entity: `FinInstrActivityCategoryText`

- **ABAP CDS Name:** `I_FinInstrActivityCategoryText`
- **Label:** Fin Instrument Activity Category - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Language` | `SPRAS` |  |  |  |  | `String(2)` | Y | Language Key |  | S/4 only entity |
| `FinancialInstrProductCategory` | `TB_SANLF` |  |  |  |  | `String(3)` | Y | Product Category |  | S/4 only entity |
| `FinInstrTransactionCategory` | `TB_SFGTYP` |  |  |  |  | `String(3)` | Y | Transaction Category |  | S/4 only entity |
| `FinancialInstrActivityCategory` | `TB_SFGZUTY` |  |  |  |  | `String(2)` | Y | Activity Category |  | S/4 only entity |
| `FinInstrActivityCategoryName` | `TB_XTTEXT` |  |  |  |  | `String(30)` |  | Activity Cat. Name |  | S/4 only entity |


## Entity: `FinInstrProductTypeSupplement`

- **ABAP CDS Name:** `I_FinInstrProdTypeSuplmnt`
- **Label:** Product Type Supplements
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `FinancialInstrumentProductType` | `VVSART` |  |  |  |  | `String(3)` | Y | Product Type |  | S/4 only entity |
| `TreasurySettlementType` | `TI_SETTLFL` |  |  |  |  | `String(1)` |  | Settlement |  | S/4 only entity |
| `OptionExerciseType` | `SOPTAUS` |  |  |  |  | `String(1)` |  | Exercise Type |  | S/4 only entity |
| `TradeFinanceCategory` | `FTR_TF_CAT` |  |  |  |  | `String(1)` |  | Trade Finance Cat. |  | S/4 only entity |
| `OptionUnderlyingProductType` | `OPTION_UNDERLYING_PRODUCT_TYPE` |  |  |  |  | `String(3)` |  | UL Product Type |  | S/4 only entity |
| `OptionUndrlgTransactionType` | `TB_USFHAAR` |  |  |  |  | `String(3)` |  | Underly.Trans.Type |  | S/4 only entity |
| `IntrstRateSwapIsCrossCurrency` | `TI_JWSWAP` |  |  |  |  | `Boolean` |  | Currency Swap |  | S/4 only entity |
| `ProductTypeCashFlowCalculation` | `TB_CASH_FLOW_CALC` |  |  |  |  | `String(2)` |  | CF Calculation |  | S/4 only entity |


## Entity: `FinInstrProductTypeText`

- **ABAP CDS Name:** `I_FinancialInstrProdTypeText`
- **Label:** Product Type - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Language` | `SPRAS` |  |  |  |  | `String(2)` | Y | Language Key |  | S/4 only entity |
| `FinancialInstrumentProductType` | `VVSART` |  |  |  |  | `String(3)` | Y | Product Type |  | S/4 only entity |
| `FinancialInstrProdTypeName` | `FTR_GEN_PRODUCT_TYPE_NAME` |  |  |  |  | `String(30)` |  | Product Type Name |  | S/4 only entity |


## Entity: `FinInstrTransCategoryText`

- **ABAP CDS Name:** `I_FinInstrTransCatText`
- **Label:** Transaction Category - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Language` | `SPRAS` |  |  |  |  | `String(2)` | Y | Language Key |  | S/4 only entity |
| `FinancialInstrProductCategory` | `TB_SANLF` |  |  |  |  | `String(3)` | Y | Product Category |  | S/4 only entity |
| `FinInstrTransactionCategory` | `TB_SFGTYP` |  |  |  |  | `String(3)` | Y | Transaction Category |  | S/4 only entity |
| `FinInstrTransCategoryName` | `TB_FTEXT` |  |  |  |  | `String(30)` |  | Trans. Category Name |  | S/4 only entity |


## Entity: `FinInstrTransactionCategory`

- **ABAP CDS Name:** `I_FinInstrTransCat`
- **Label:** Transaction Category
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `FinancialInstrProductCategory` | `TB_SANLF` |  |  |  |  | `String(3)` | Y | Product Category |  | S/4 only entity |
| `FinInstrTransactionCategory` | `TB_SFGTYP` |  |  |  |  | `String(3)` | Y | Transaction Category |  | S/4 only entity |


## Entity: `FinInstrTransactionTypeText`

- **ABAP CDS Name:** `I_FinancialInstrTransTypeText`
- **Label:** Transaction Type - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Language` | `SPRAS` |  |  |  |  | `String(2)` | Y | Language Key |  | S/4 only entity |
| `FinancialInstrumentProductType` | `VVSART` |  |  |  |  | `String(3)` | Y | Product Type |  | S/4 only entity |
| `FinancialInstrTransactionType` | `FTR_GEN_TRANSACTION_TYPE` |  |  |  |  | `String(3)` | Y | Transaction Type |  | S/4 only entity |
| `FinancialInstrTransTypeName` | `FTR_GEN_TRANSACTION_TYPE_NAME` |  |  |  |  | `String(30)` |  | Trans. Type Name |  | S/4 only entity |


## Entity: `FinInstrumentActivityCategory`

- **ABAP CDS Name:** `I_FinInstrActivityCategory`
- **Label:** Financial Instrument Activity Category
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `FinancialInstrProductCategory` | `TB_SANLF` |  |  |  |  | `String(3)` | Y | Product Category |  | S/4 only entity |
| `FinInstrTransactionCategory` | `TB_SFGTYP` |  |  |  |  | `String(3)` | Y | Transaction Category |  | S/4 only entity |
| `FinancialInstrActivityCategory` | `TB_SFGZUTY` |  |  |  |  | `String(2)` | Y | Activity Category |  | S/4 only entity |
| `FinTransGenActivityCategory` | `FTR_GEN_ACTIVITY_CATEGORY` |  |  |  |  | `String(3)` |  | General Activity Category |  | S/4 only entity |


## Entity: `FinTransNoticePeriodUnit`

- **ABAP CDS Name:** `I_FinTransNoticePeriodUnit`
- **Label:** Financial Transaction Notice Period Unit
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `FinTransNoticePeriodUnit` | `TB_SKUEND` |  |  |  |  | `String(1)` | Y | Unit |  | S/4 only entity |
| `DomainValue` | `DOMVALUE_L` |  |  |  |  | `String(10)` |  | Lower Value |  | S/4 only entity |


## Entity: `FinTransNoticePeriodUnitText`

- **ABAP CDS Name:** `I_FinTransNoticePeriodUnitText`
- **Label:** Fin Trans Notice Period Unit - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Language` | `SPRAS` |  |  |  |  | `String(2)` | Y | Language Key |  | S/4 only entity |
| `FinTransNoticePeriodUnit` | `TB_SKUEND` |  |  |  |  | `String(1)` | Y | Unit |  | S/4 only entity |
| `DomainValue` | `DOMVALUE_L` |  |  |  |  | `String(10)` |  | Lower Value |  | S/4 only entity |
| `FinTransNoticePeriodUnitName` | `TB_SKUEND_NAME` |  |  |  |  | `String(60)` |  | NoticePer. Unit Name |  | S/4 only entity |


## Entity: `FinTransOptionExerciseType`

- **ABAP CDS Name:** `I_OptionExerciseType`
- **Label:** Option exercise type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `OptionExerciseType` | `SOPTAUS` |  |  |  |  | `String(1)` | Y | Exercise Type |  | S/4 only entity |


## Entity: `FinTransOptionExerciseTypeText`

- **ABAP CDS Name:** `I_OptionExerciseTypeText`
- **Label:** Option exercise type - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `OptionExerciseType` | `SOPTAUS` |  |  |  |  | `String(1)` | Y | Exercise Type |  | S/4 only entity |
| `Language` | `DDLANGUAGE` |  |  |  |  | `String(2)` | Y | Lang. |  | S/4 only entity |
| `OptionExerciseTypeName` | `OPTION_EXERCISE_TYPE_NAME` |  |  |  |  | `String(60)` |  | Option Exercise Type |  | S/4 only entity |


## Entity: `FinTransOptionSettlementType`

- **ABAP CDS Name:** `I_OptionSettlementType`
- **Label:** Option settlement type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `OptionSettlementType` | `OPTION_SETTLEMENT_TYPE` |  |  |  |  | `String(1)` | Y | Settlement Type |  | S/4 only entity |


## Entity: `FinTransOptnSettlementTypeText`

- **ABAP CDS Name:** `I_OptionSettlementTypeText`
- **Label:** Option settlement type - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `OptionSettlementType` | `OPTION_SETTLEMENT_TYPE` |  |  |  |  | `String(1)` | Y | Settlement Type |  | S/4 only entity |
| `Language` | `DDLANGUAGE` |  |  |  |  | `String(2)` | Y | Lang. |  | S/4 only entity |
| `OptionSettlementTypeName` | `OPTION_SETTLEMENT_TYPE_NAME` |  |  |  |  | `String(60)` |  | Option Settlemt Type |  | S/4 only entity |


## Entity: `FinTransOptnUndrlgAllocation`

- **ABAP CDS Name:** `I_FinTransOptnUndrlgAllocation`
- **Label:** Fin Trans Option Underlying Allocation
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `FinTransOptionNumber` | `TI_RGATT` |  |  |  |  | `String(13)` | Y | Class |  | S/4 only entity |
| `OptionUnderlyingTransaction` | `OPTION_UNDERLYING_TRANSACTION` |  |  |  |  | `String(13)` | Y | Transaction |  | S/4 only entity |
| `FinancialTransactionFromExer` | `TB_VRFHA` |  |  |  |  | `String(13)` |  | Exercise Transaction |  | S/4 only entity |


## Entity: `FinTransReleaseStatus`

- **ABAP CDS Name:** `I_FinTransReleaseStatus`
- **Label:** Financial Transaction Release Status
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `FinTransReleaseStatus` | `TB_FRGZUST` |  |  |  |  | `String(1)` | Y | Release Status |  | S/4 only entity |
| `DomainValue` | `DOMVALUE_L` |  |  |  |  | `String(10)` |  | Lower Value |  | S/4 only entity |


## Entity: `FinTransReleaseStatusText`

- **ABAP CDS Name:** `I_FinTransReleaseStatusText`
- **Label:** Fin Transaction Release Status - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Language` | `SPRAS` |  |  |  |  | `String(2)` | Y | Language Key |  | S/4 only entity |
| `FinTransReleaseStatus` | `TB_FRGZUST` |  |  |  |  | `String(1)` | Y | Release Status |  | S/4 only entity |
| `DomainValue` | `DOMVALUE_L` |  |  |  |  | `String(10)` |  | Lower Value |  | S/4 only entity |
| `FinTransReleaseStatusName` | `TB_FRGZUST_NAME` |  |  |  |  | `String(60)` |  | Release Status Name |  | S/4 only entity |


## Entity: `FinTransUnderlyingFlow`

- **ABAP CDS Name:** `I_FinTransUnderlyingFlow`
- **Label:** Fin Transaction Underlying Flow
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `OptionUnderlyingTransaction` | `OPTION_UNDERLYING_TRANSACTION` |  |  |  |  | `String(13)` | Y | Transaction |  | S/4 only entity |
| `FinancialInstrumentActivity` | `TB_RFHAZU` |  |  |  |  | `String(5)` | Y | Activity |  | S/4 only entity |
| `FinTransFlowCreationDate` | `TB_CRDAT` |  |  |  |  | `Date` | Y | Entered On |  | S/4 only entity |
| `FinTransFlowCreationTime` | `FTR_FLOW_CREATION_TIME` |  |  |  |  | `String(6)` | Y | Entry Time |  | S/4 only entity |
| `FinTransFlowNumber` | `TB_RFHAZB` |  |  |  |  | `String(4)` | Y | Flow |  | S/4 only entity |
| `CreatedByUser` | `TB_CRUSER` |  |  |  |  | `String(12)` |  | Entered By |  | S/4 only entity |
| `FinTransCreationDate` | `FTR_CREATION_DATE` |  |  |  |  | `Date` |  | Created On |  | S/4 only entity |
| `FinTransCreationTime` | `TB_TCRTIM` |  |  |  |  | `String(6)` |  | Entry Time |  | S/4 only entity |
| `LastChangedByUser` | `TB_UPUSER` |  |  |  |  | `String(12)` |  | Last Changed By |  | S/4 only entity |
| `LastChangeDate` | `TB_DUPDAT` |  |  |  |  | `Date` |  | Changed On |  | S/4 only entity |
| `FinInstrumentLastChangedTime` | `TB_TUPTIM` |  |  |  |  | `String(6)` |  | Time Changed |  | S/4 only entity |
| `TreasuryContractType` | `RANTYP` |  |  |  |  | `String(1)` |  | Contract Type |  | S/4 only entity |
| `FinTransFlowType` | `TB_SFHAZBA` |  |  |  |  | `String(4)` |  | Flow Type |  | S/4 only entity |
| `FinTransFlowCategory` | `FTR_FLOW_CATEGORY` |  |  |  |  | `String(2)` |  | Flow Category |  | S/4 only entity |
| `FinTransFlowPaytAmtDirection` | `FTR_FLOW_PAYMENT_AMT_DIRECTION` |  |  |  |  | `String(1)` |  | Direction |  | S/4 only entity |
| `FinancialTransactionDirection` | `TB_RKONDGR` |  |  |  |  | `String(1)` |  | Direction |  | S/4 only entity |
| `FinTransFlowSource` | `TB_SHERK` |  |  |  |  | `String(4)` |  | Source |  | S/4 only entity |
| `PayerPayee` | `TB_RPZAHL_NEW` |  |  |  |  | `String(10)` |  | Payer/Payee |  | S/4 only entity |
| `FinTransFlowPaymentDate` | `FTR_FLOW_PAYMENT_DATE` |  |  |  |  | `Date` |  | Payment Date |  | S/4 only entity |
| `FinTransFlowPaytAmt` | `FTR_FLOW_PAYMENT_AMOUNT` |  |  |  |  | `Decimal(34,4)` |  | Payment Amnt in PyC | FinTransFlowPaytAmtCrcy | S/4 only entity |
| `FinTransFlowPaytAmtCrcy` | `TB_WZBETR` |  |  |  |  | `String(5)` |  | Payment Currency |  | S/4 only entity |
| `FinTransFlowInLoclCrcyPaytAmt` | `TB_HWBETR` |  |  |  |  | `Decimal(34,4)` |  | Pmnt Amnt in LCurr | FinTransFlowPaytAmtCrcy | S/4 only entity |
| `FinTransFlowLoclCrcyCnvrsnRate` | `FTR_FLOW_LOCL_CRCY_CNVRSN_RATE` |  |  |  |  | `Decimal(9,5)` |  | Crcy Cnvrsn Rate |  | S/4 only entity |
| `CalculationDate` | `DVALUT` |  |  |  |  | `Date` |  | Calculation Date |  | S/4 only entity |
| `CalculationPeriodStartDate` | `DBERVON` |  |  |  |  | `Date` |  | Calculation From |  | S/4 only entity |
| `CalculationPeriodEndDate` | `DBERBIS` |  |  |  |  | `Date` |  | Calculation To |  | S/4 only entity |
| `CalcPeriodEndDateIsInclusive` | `VVSINCLBIS` |  |  |  |  | `String(1)` |  | Inclusive End Date |  | S/4 only entity |
| `CalcPeriodStartDateIsExclusive` | `VVSEXCLVON` |  |  |  |  | `String(1)` |  | Exclusive Start Date |  | S/4 only entity |
| `CalcPeriodEndDateIsMonthEnd` |  |  |  |  |  | `Boolean` |  | Month-End End Date |  | S/4 only entity |
| `CalcPeriodStartDateIsMonthEnd` |  |  |  |  |  | `Boolean` |  | Month-End Start Date |  | S/4 only entity |
| `NumberOfCalculationDays` | `VVATAGE` |  |  |  |  | `String(6)` |  | Number of Days |  | S/4 only entity |
| `NrOfBaseDaysPerCalcPeriod` | `ABASTAGE` |  |  |  |  | `String(6)` |  | No. of base days |  | S/4 only entity |
| `InterestCalculationMethod` | `SZBMETH` |  |  |  |  | `String(1)` |  | Int. Calc. Method |  | S/4 only entity |
| `FinTransFlowCalcBaseAmount` | `BBASIS` |  |  |  |  | `Decimal(34,4)` |  | Base Amount | FinTransFlowCalcBaseAmountCrcy | S/4 only entity |
| `FinTransFlowCalcBaseAmountCrcy` | `TB_WBASIS` |  |  |  |  | `String(5)` |  | Calculatn Basis Crcy |  | S/4 only entity |
| `IntrstCalcMethFactoryCalendar` | `TFMSKALIDWT` |  |  |  |  | `String(2)` |  | Interest Calendar |  | S/4 only entity |
| `InterestBaseDaysMethod` | `VVSTGBASIS` |  |  |  |  | `String(1)` |  | Base Days Method |  | S/4 only entity |
| `InterestCalculationType` | `TFMSINTCALC` |  |  |  |  | `String(1)` |  | Int. Calc. Type |  | S/4 only entity |
| `ConditionPercentageRate` | `PKOND` |  |  |  |  | `Decimal(10,7)` |  | Percentage Rate |  | S/4 only entity |
| `FinCndnPctgRateFixingDate` | `VVDPKOND` |  |  |  |  | `Date` |  | PercFixingDte |  | S/4 only entity |
| `FinTransFlowIntrstRateFixDate` | `TB_DZFEST` |  |  |  |  | `Date` |  | Int.Rate Fixing Date |  | S/4 only entity |
| `FinTransPositionValueDate` | `TB_DBESTAND` |  |  |  |  | `Date` |  | Position Value Date |  | S/4 only entity |
| `FinTransFlowPositionAmount` | `FTR_POSITION_AMOUNT` |  |  |  |  | `Decimal(34,4)` |  | PositionAmount | FinTransFlwPosAmtCrcy | S/4 only entity |
| `FinTransFlwPosAmtCrcy` | `TB_WBBETR` |  |  |  |  | `String(5)` |  | Position Currency |  | S/4 only entity |
| `FinTransFlowNomAmt` | `FTR_FLOW_NORMINAL_AMOUNT` |  |  |  |  | `Decimal(34,4)` |  | Nominal Amount | FinTransFlowNomAmtCrcy | S/4 only entity |
| `FinTransFlowNomAmtCrcy` | `FTR_FLOW_NORMINAL_AMOUNT_CRCY` |  |  |  |  | `String(5)` |  | Nominal Amount Currency |  | S/4 only entity |
| `MarketValueInQtanCurrency` | `TB_BEBETR` |  |  |  |  | `Decimal(34,4)` |  | Mkt Val. in QC | QuotationCurrency | S/4 only entity |
| `QuotationCurrency` | `TB_WEBETR` |  |  |  |  | `String(5)` |  | Price Currency |  | S/4 only entity |
| `FinTransTradedNumberOfUnits` | `FTR_FINTRANS_UNITS_L` |  |  |  |  | `Decimal(24,14)` |  | Number of Units |  | S/4 only entity |
| `FinTransTrdPriceCrcyUnitRate` | `FTR_PRICE` |  |  |  |  | `Decimal(23,14)` |  | Price (Unit-Quoted) |  | S/4 only entity |
| `FinTransTradedPriceCrcyUnit` | `FTR_TRADED_PRICE_CURRENCY_UNIT` |  |  |  |  | `String(5)` |  | Currency Unit |  | S/4 only entity |
| `SecurityExchange` | `VVRHANDPL` |  |  |  |  | `String(10)` |  | Exchange |  | S/4 only entity |
| `FinConditionItem` | `TB_KOND` |  |  |  |  | `String(4)` |  | Condition |  | S/4 only entity |
| `ConditionItemValidityStartDate` | `DGUEL_KP` |  |  |  |  | `Date` |  | Item Effective From |  | S/4 only entity |
| `FinConditionSubItem` | `NSTUFE` |  |  |  |  | `String(2)` |  | Level Number |  | S/4 only entity |
| `InterestConditionType` | `SKOART` |  |  |  |  | `String(4)` |  | Condition Type |  | S/4 only entity |
| `FinInstrConditionLogicGroup` | `FTR_INSTR_CNDN_LOGIC_GROUP` |  |  |  |  | `String(4)` |  | Condition Group |  | S/4 only entity |
| `FinCndnCrsRefcdAccmlnCndnGrp` | `TB_SUM_RKOND` |  |  |  |  | `String(4)` |  | Accum. Cond.Grp |  | S/4 only entity |
| `FinTransFlwReltdAccumulatingID` | `TB_SUM_ID_SOURCE` |  |  |  |  | `String(40)` |  | Rel.AccumFlowID |  | S/4 only entity |
| `FinTransFlowAccumulatingFlowID` | `TB_SUM_ID_SUM` |  |  |  |  | `String(40)` |  | Accum. Flow ID |  | S/4 only entity |
| `FinTransTradedPricePercent` | `FTR_PRICE_PERCENT` |  |  |  |  | `Decimal(23,14)` |  | Price (%) |  | S/4 only entity |


## Entity: `FinancialInstrTransactionType`

- **ABAP CDS Name:** `I_FinancialInstrTransType`
- **Label:** Transaction Type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `FinancialInstrTransactionType` | `FTR_GEN_TRANSACTION_TYPE` |  |  |  |  | `String(3)` | Y | Transaction Type |  | S/4 only entity |
| `FinancialInstrumentProductType` | `VVSART` |  |  |  |  | `String(3)` | Y | Product Type |  | S/4 only entity |
| `FinInstrTransactionCategory` | `TB_SFGTYP` |  |  |  |  | `String(3)` |  | Transaction Category |  | S/4 only entity |
| `TreasuryContractType` | `RANTYP` |  |  |  |  | `String(1)` |  | Contract Type |  | S/4 only entity |


## Entity: `FinancialInstrumentProductType`

- **ABAP CDS Name:** `I_FinancialinstrProductType`
- **Label:** Product Type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `FinancialInstrumentProductType` | `VVSART` |  |  |  |  | `String(3)` | Y | Product Type |  | S/4 only entity |
| `TreasuryContractType` | `RANTYP` |  |  |  |  | `String(1)` |  | Contract Type |  | S/4 only entity |
| `FinancialInstrProductCategory` | `SANLF` |  |  |  |  | `String(3)` |  | Product Category |  | S/4 only entity |
| `FinCndnTypeAllocCndnGroup` | `SKOGRP` |  |  |  |  | `String(3)` |  | Condition Group |  | S/4 only entity |


## Entity: `FinancialInstrumentStatus`

- **ABAP CDS Name:** `I_FinInstrumentStatus`
- **Label:** Financial Instrument Status
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `FinancialInstrumentStatus` | `TB_SAKTIV` |  |  |  |  | `String(1)` | Y | Active Status |  | S/4 only entity |
| `DomainValue` | `DOMVALUE_L` |  |  |  |  | `String(10)` |  | Lower Value |  | S/4 only entity |


## Entity: `FinancialInstrumentStatusText`

- **ABAP CDS Name:** `I_FinInstrumentStatusText`
- **Label:** Financial Instrument Status - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Language` | `SPRAS` |  |  |  |  | `String(2)` | Y | Language Key |  | S/4 only entity |
| `FinancialInstrumentStatus` | `TB_SAKTIV` |  |  |  |  | `String(1)` | Y | Active Status |  | S/4 only entity |
| `DomainValue` | `DOMVALUE_L` |  |  |  |  | `String(10)` |  | Lower Value |  | S/4 only entity |
| `FinancialInstrumentStatusName` | `TB_SAKTIV_NAME` |  |  |  |  | `String(60)` |  | Active Status Name |  | S/4 only entity |


## Entity: `FinancialTransaction`

- **ABAP CDS Name:** `I_FinancialTransactionDEX`
- **Label:** Financial Transaction
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** VTBFHA, VTBFHAZU

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `CompanyCode` | `BUKRS` |  |  |  |  | `String(4)` | Y | Company Code |  |  |
| `FinancialTransaction` | `TB_RFHA` |  |  |  |  | `String(13)` | Y | Transaction |  |  |
| `FinTransCreationDate` | `FTR_CREATION_DATE` |  |  |  |  | `Date` |  | Created On |  |  |
| `FinTransCreationTime` | `TB_TCRTIM` |  |  |  |  | `String(6)` |  | Entry Time |  |  |
| `LastChangeDate` | `TB_DUPDAT` |  |  |  |  | `Date` |  | Changed On |  |  |
| `FinInstrumentLastChangedTime` | `TB_TUPTIM` |  |  |  |  | `String(6)` |  | Time Changed |  |  |
| `TreasuryContractType` | `RANTYP` |  |  |  |  | `String(1)` |  | Contract Type |  |  |
| `FinancialInstrProductCategory` | `FTR_GEN_FIN_INSTR_PROD_CATEG` |  |  |  |  | `String(3)` |  | Product Category |  |  |
| `FinancialInstrumentProductType` | `VVSART` |  |  |  |  | `String(3)` |  | Product Type |  |  |
| `FinInstrTransactionCategory` | `TB_SFGTYP` |  |  |  |  | `String(3)` |  | Transaction Category |  |  |
| `FinancialInstrTransactionType` | `FTR_GEN_TRANSACTION_TYPE` |  |  |  |  | `String(3)` |  | Transaction Type |  |  |
| `TermStartDate` | `TB_DBLFZ` |  |  |  |  | `Date` |  | Term Start |  |  |
| `FinTransNoticePeriod` | `TB_AKUEND` |  |  |  |  | `String(3)` |  | Period of Notice |  |  |
| `FinTransNoticePeriodUnit` | `TB_SKUEND` |  |  |  |  | `String(1)` |  | Unit |  |  |
| `FinTransFactoryCalendar1` | `SKALID` |  |  |  |  | `String(2)` |  | Calendar |  |  |
| `FinTransFactoryCalendar2` | `SKALID` |  |  |  |  | `String(2)` |  | Calendar |  |  |
| `Counterparty` | `RKONTRAH_NEW` |  |  |  |  | `String(10)` |  | Counterparty |  |  |
| `FinancialInstrumentGuarantor` | `TB_RGARANT_NEW` |  |  |  |  | `String(10)` |  | Guarantor |  |  |
| `Portfolio` | `RPORTB` |  |  |  |  | `String(10)` |  | Portfolio |  |  |
| `TreasuryFinanceProject` | `TB_TFPROJ` |  |  |  |  | `String(13)` |  | Finance Project |  |  |
| `FinancialInstrumentAssignment` | `FTR_GEN_FIN_INSTR_ASSIGNMENT` |  |  |  |  | `String(18)` |  | Free Assignment |  |  |
| `FinancialInstrumentReference` | `FTR_GEN_FIN_INSTR_INTERNAL_REF` |  |  |  |  | `String(16)` |  | Free Internal Ref. |  |  |
| `FinancialInstrCharacteristic` | `FTR_GEN_FIN_INSTR_CHAR` |  |  |  |  | `String(25)` |  | Free Charact. |  |  |
| `ControllingArea` | `KOKRS` |  |  |  |  | `String(4)` |  | Controlling Area |  |  |
| `CostCenter` | `KOSTL` |  |  |  |  | `String(10)` |  | Cost Center |  |  |
| `HedgingClassification` | `TOE_HEDGING_CLASSIFICATION` |  |  |  |  | `String(5)` |  | Hedging Classificatn |  |  |
| `HedgeRequestIdentifier` | `HEDGE_REQUEST_IDENTIFIER` |  |  |  |  | `String(13)` |  | Hedge Request ID |  |  |
| `ProfitCenter` | `PRCTR` |  |  |  |  | `String(10)` |  | Profit Center |  |  |
| `WBSElementInternalID` | `PS_S4_PSPNR` |  |  |  |  | `String(8)` |  | WBS Internal ID |  |  |
| `TreasuryFacilityCompanyCode` | `TB_FACILITYBUKRS` |  |  |  |  | `String(4)` |  | CoCd of Facility |  |  |
| `TreasuryFacility` | `TB_FACILITYNR` |  |  |  |  | `String(13)` |  | Facility |  |  |
| `FinancialInstrumentStatus` | `TB_SAKTIV` |  |  |  |  | `String(1)` |  | Active Status |  |  |
| `FinTransReleaseStatus` | `TB_FRGZUST` |  |  |  |  | `String(1)` |  | Release Status |  |  |
| `TransactionCurrency` | `TB_WGSCHFT` |  |  |  |  | `String(5)` |  | Transaction Currency |  |  |
| `FinInstrumentOutgoingCurrency` | `TB_WGSCHF1` |  |  |  |  | `String(5)` |  | Outgoing Currency |  |  |
| `FinInstrumentIncomingCurrency` | `TB_WGSCHF2` |  |  |  |  | `String(5)` |  | Incoming Currency |  |  |
| `TradedCurrency` | `FTR_TRADED_CURR` |  |  |  |  | `String(5)` |  | Traded Currency |  |  |
| `SecurityClass` | `FTR_GEN_SECURITY_CLASS` |  |  |  |  | `String(13)` |  | Security Class |  |  |
| `ClassificationOfFinInstr` | `FTR_CFI_CODE` |  |  |  |  | `String(6)` |  | CFI Code |  |  |
| `SecurityAccount` | `FTR_GEN_SECURITY_ACCOUNT` |  |  |  |  | `String(10)` |  | Securities Account |  |  |
| `FinTransIsRiskMitigating` | `FTR_THRESHOLD_RISK_MITIGATING` |  |  |  |  | `Boolean` |  | Risk Mitigation |  |  |
| `FinInstrLastActiveActivity` | `FTR_GEN_FIN_INSTR_LAST_ACT_ACT` |  |  |  |  | `String(5)` |  | Last Active Activity |  |  |
| `TrsyTradedAmountBuySellCode` | `TTM_FX_BUY_SELL` |  |  |  |  | `String(1)` |  | Buy/Sell |  |  |
| `Segment` | `FB_SEGMENT` |  |  |  |  | `String(10)` |  | Segment |  |  |
| `OnBehalfOfCompany` | `TRBA_BEHALF_OF_COMPANY` |  |  |  |  | `String(4)` |  | On Behalf of CoCode |  |  |
| `MarketIdentifierCode` | `TBA_MIC` |  |  |  |  | `String(4)` |  | MIC |  |  |
| `FinTransRoundingCategory` | `TB_SRNDNG` |  |  |  |  | `String(1)` |  | Round |  |  |
| `FinTransGeneralValuationClass` | `TPM_COM_VAL_CLASS` |  |  |  |  | `String(4)` |  | Gen. Valn Class |  |  |
| `Fund` | `FM_FUND` |  |  |  |  | `String(10)` |  | Fund |  |  |
| `GrantID` | `GM_GRANT_NBR` |  |  |  |  | `String(20)` |  | Grant |  |  |
| `FinTransAuthorizationGroup` | `TBEGRU` |  |  |  |  | `String(4)` |  | Authorization Group |  |  |
| `BusinessPlace` | `BUPLA` |  |  |  |  | `String(4)` |  | Business Place |  |  |
| `FunctionalArea` | `FKBER` |  |  |  |  | `String(16)` |  | Functional Area |  |  |
| `TrsyPosCustomDiffntnTerm1` | `TPM_CUST_DIFF_TERM_VALUE` |  |  |  |  | `String(20)` |  | Cust.Diff.Term Val. |  |  |
| `TrsyPosCustomDiffntnTerm2` | `TPM_CUST_DIFF_TERM_VALUE` |  |  |  |  | `String(20)` |  | Cust.Diff.Term Val. |  |  |
| `TrsyPosCustomDiffntnTerm3` | `TPM_CUST_DIFF_TERM_VALUE` |  |  |  |  | `String(20)` |  | Cust.Diff.Term Val. |  |  |
| `TrsyPosCustomDiffntnTerm4` | `TPM_CUST_DIFF_TERM_VALUE` |  |  |  |  | `String(20)` |  | Cust.Diff.Term Val. |  |  |
| `TrsyPosCustomDiffntnTerm5` | `TPM_CUST_DIFF_TERM_VALUE` |  |  |  |  | `String(20)` |  | Cust.Diff.Term Val. |  |  |
| `UniqueProductIdentifier` | `FTR_UPI` |  |  |  |  | `String(12)` |  | Unique Product ID |  |  |
| `InternationalSecuritiesIdnNmbr` | `RANL_ISIN` |  |  |  |  | `String(12)` |  | Security ID (ISIN) |  |  |
| `ReportTrackingNumber` | `FTR_RTN` |  |  |  |  | `String(52)` |  | Report Tracking No. |  |  |
| `FinTransOptionNumber` | `TI_RGATT` |  |  |  |  | `String(13)` |  | Class |  |  |
| `FinancialInstrActivityCategory` | `TB_SFGZUTY` |  |  |  |  | `String(2)` |  | Activity Category |  |  |
| `TermEndDate` | `TB_DELFZ` |  |  |  |  | `Date` |  | Term End |  |  |
| `FinTransTermCategory` | `FTR_TERM_CATEGORY` |  |  |  |  | `String(1)` |  | Term Category |  |  |
| `FinTransTermStartEndInclusive` | `FTR_TERM_START_END_INCLUSIVE` |  |  |  |  | `String(1)` |  | Term Start and End Inclusive |  |  |
| `FinTransNoticeDate` | `TB_NOTICE_DATE` |  |  |  |  | `Date` |  | Notice Date |  |  |
| `FinTransActyConclusionDate` | `FTR_ACTY_CONCLUSION_DTE` |  |  |  |  | `Date` |  | Conclusion Date |  |  |
| `FinTransActyConclusionTime` | `TB_TVTRAB` |  |  |  |  | `String(6)` |  | Contract.Concl.Time |  |  |
| `FinTransActyConclusionTimeZone` | `TB_ZVTRAB` |  |  |  |  | `String(6)` |  | Time Zone Contr.Date |  |  |
| `FinTransRolloverDate` | `TB_DBLFZ` |  |  |  |  | `Date` |  | Term Start |  |  |
| `FinTransExerciseDate` | `TB_DELFZ` |  |  |  |  | `Date` |  | Term End |  |  |
| `FinTransOrderValidityEndDate` | `TB_LIMITDA` |  |  |  |  | `Date` |  | Limit Date |  |  |
| `FinTransFixingDate` | `TB_DFIX` |  |  |  |  | `Date` |  | Fixing Date |  |  |
| `ForeignExchangeFixingReference` | `FTR_FIXING_REF_ID` |  |  |  |  | `String(30)` |  | Fixing Reference ID |  |  |
| `Trader` | `RDEALER` |  |  |  |  | `String(12)` |  | Trader |  |  |
| `FinancialInstrContactPerson` | `TB_GSPPART` |  |  |  |  | `String(19)` |  | Contact Person |  |  |
| `FinInstrExternalReference` | `TB_NORDEXT` |  |  |  |  | `String(16)` |  | External Reference |  |  |
| `TreasuryReversalReason` | `SSTOGRD` |  |  |  |  | `String(2)` |  | Reason for Reversal |  |  |
| `LeadingCurrency` | `TB_WLWAERS` |  |  |  |  | `String(5)` |  | Leading Currency |  |  |
| `FollowingCurrency` | `TB_WFWAERS` |  |  |  |  | `String(5)` |  | Following Currency |  |  |
| `ExchangeRate` | `TB_KKURS` |  |  |  |  | `Decimal(13,9)` |  | Transaction Rate |  |  |
| `SpotExchangeRate` | `TB_KKASSA` |  |  |  |  | `Decimal(13,9)` |  | Spot Rate |  |  |
| `SwapExchangeRate` | `TB_KSWAP` |  |  |  |  | `Decimal(13,9)` |  | Swap Rate |  |  |
| `LiquidityEffectValue` | `TX_KWLIQ` |  |  |  |  | `Decimal(13,9)` |  | Liquidity Effect |  |  |
| `CurrencyPair` | `FTR_CURR_PAIR` |  |  |  |  | `String(20)` |  | Currency Pair |  |  |
| `EffectiveInterestRate` | `TB_PYIELD` |  |  |  |  | `Decimal(10,7)` |  | Effect.Interest Rate |  |  |
| `EffectiveInterestMethod` | `SEFFMETH` |  |  |  |  | `String(1)` |  | Effect. Int. Method |  |  |
| `LetterOfCredit` | `FTR_LC_NUMBER` |  |  |  |  | `String(16)` |  | Letter of Credit No. |  |  |
| `TreasuryApplicant` | `FTR_APPLICANT` |  |  |  |  | `String(10)` |  | Applicant |  |  |
| `TreasuryBeneficiary` | `FTR_BENEFICIARY` |  |  |  |  | `String(10)` |  | Beneficiary |  |  |
| `TrsyMnllyEnteredBnfcyName` | `FTR_MAN_BENE_NAME` |  |  |  |  | `String(25)` |  | Benefic. Name (Man.) |  |  |
| `TrsyMnllyEnteredApplcntName` | `FTR_MAN_APPL_NAME` |  |  |  |  | `String(25)` |  | ApplicantName (Man.) |  |  |
| `TreasuryAdvisingBank` | `FTR_ADVISING_BANK` |  |  |  |  | `String(10)` |  | Advising Bank |  |  |
| `TreasuryIssuingBank` | `FTR_ISSUE_BANK` |  |  |  |  | `String(10)` |  | Issuing Bank |  |  |
| `BankGuaranteeNumber` | `FTR_BG_NUMBER` |  |  |  |  | `String(16)` |  | Bank Guarantee No. |  |  |
| `BankGuaranteeType` | `FTR_BG_TYPE` |  |  |  |  | `String(4)` |  | Bank Guarantee Type |  |  |


## Entity: `ForeignExchangeFixingReference`

- **ABAP CDS Name:** `I_FXFixingReference`
- **Label:** Foreign Exchange Fixing Reference
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `ForeignExchangeFixingReference` | `FTR_FIXING_REF_ID` |  |  |  |  | `String(30)` | Y | Fixing Reference ID |  | S/4 only entity |


## Entity: `TradeFinanceCategory`

- **ABAP CDS Name:** `I_TradeFinanceCategory`
- **Label:** Trade Finance Category
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `TradeFinanceCategory` | `FTR_TF_CAT` |  |  |  |  | `String(1)` | Y | Trade Finance Cat. |  | S/4 only entity |


## Entity: `TradeFinanceCategoryText`

- **ABAP CDS Name:** `I_TradeFinanceCategoryText`
- **Label:** Trade Finance Category - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `TradeFinanceCategory` | `FTR_TF_CAT` |  |  |  |  | `String(1)` | Y | Trade Finance Cat. |  | S/4 only entity |
| `Language` | `DDLANGUAGE` |  |  |  |  | `String(2)` | Y | Lang. |  | S/4 only entity |
| `TradeFinanceCategoryName` | `TRADE_FINANCE_CATEGORY_NAME` |  |  |  |  | `String(60)` |  | Category Name |  | S/4 only entity |


## Entity: `TreasuryContractType`

- **ABAP CDS Name:** `I_TreasuryContractType`
- **Label:** Treasury Contract Type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `TreasuryContractType` | `RANTYP` |  |  |  |  | `String(1)` | Y | Contract Type |  | S/4 only entity |
| `DomainValue` | `DOMVALUE_L` |  |  |  |  | `String(10)` |  | Lower Value |  | S/4 only entity |


## Entity: `TreasuryContractTypeText`

- **ABAP CDS Name:** `I_TreasuryContractTypeText`
- **Label:** Treasury Contract Type - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Language` | `SPRAS` |  |  |  |  | `String(2)` | Y | Language Key |  | S/4 only entity |
| `TreasuryContractType` | `RANTYP` |  |  |  |  | `String(1)` | Y | Contract Type |  | S/4 only entity |
| `DomainValue` | `DOMVALUE_L` |  |  |  |  | `String(10)` |  | Lower Value |  | S/4 only entity |
| `TreasuryContractTypeName` | `RANTYP_NAME` |  |  |  |  | `String(60)` |  | Contract Type Name |  | S/4 only entity |


## Entity: `TreasuryPortfolio`

- **ABAP CDS Name:** `I_TreasuryPortfolio`
- **Label:** Portfolio
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** VTBFHA

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `CompanyCode` | `BUKRS` |  |  |  |  | `String(4)` | Y | Company Code |  |  |
| `Portfolio` | `RPORTB` |  |  |  |  | `String(10)` | Y | Portfolio |  |  |


## Entity: `TreasuryPortfolioText`

- **ABAP CDS Name:** `I_TreasuryPortfolioText`
- **Label:** Portfolio - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `CompanyCode` | `BUKRS` |  |  |  |  | `String(4)` | Y | Company Code |  | S/4 only entity |
| `Portfolio` | `RPORTB` |  |  |  |  | `String(10)` | Y | Portfolio |  | S/4 only entity |
| `Language` | `SPRAS` |  |  |  |  | `String(2)` | Y | Language Key |  | S/4 only entity |
| `PortfolioName` | `FTR_GEN_PORTFOLIO_NAME` |  |  |  |  | `String(30)` |  | Portfolio Name |  | S/4 only entity |


## Entity: `TreasuryProductCategory`

- **ABAP CDS Name:** `I_FinancialInstrProdCat`
- **Label:** Product Category
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `FinancialInstrProductCategory` | `SANLF` |  |  |  |  | `String(3)` | Y | Product Category |  | S/4 only entity |
| `TreasuryContractType` | `RANTYP` |  |  |  |  | `String(1)` |  | Contract Type |  | S/4 only entity |


## Entity: `TreasuryProductCategoryText`

- **ABAP CDS Name:** `I_FinancialInstrProdCatText`
- **Label:** Product Category - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Language` | `SPRAS` |  |  |  |  | `String(2)` | Y | Language Key |  | S/4 only entity |
| `FinancialInstrProductCategory` | `SANLF` |  |  |  |  | `String(3)` | Y | Product Category |  | S/4 only entity |
| `FinInstrProductCategoryName` | `TEXT30` |  |  |  |  | `String(30)` |  | Text |  | S/4 only entity |


## Entity: `TreasuryReversalReason`

- **ABAP CDS Name:** `I_TreasuryReversalReason`
- **Label:** Treasury Reversal Reason
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `TreasuryReversalReason` | `SSTOGRD` |  |  |  |  | `String(2)` | Y | Reason for Reversal |  | S/4 only entity |


## Entity: `TreasuryReversalReasonText`

- **ABAP CDS Name:** `I_TreasuryReversalReasonText`
- **Label:** Treasury Reversal Reason - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Language` | `SPRAS` |  |  |  |  | `String(2)` | Y | Language Key |  | S/4 only entity |
| `TreasuryReversalReason` | `SSTOGRD` |  |  |  |  | `String(2)` | Y | Reason for Reversal |  | S/4 only entity |
| `TreasuryReversalReasonName` | `XLANGBEZ` |  |  |  |  | `String(60)` |  | Long name |  | S/4 only entity |
