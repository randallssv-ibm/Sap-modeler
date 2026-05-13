# FinancialTransaction

> Source file: `sap-s4com-FinancialTransaction-v1.json`


## Entity: `FXFixingReferenceText`

- **ABAP Name:** `I_FXFixingReferenceText`
- **Label:** Foreign Exchange Fixing Reference - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Language` | `SPRAS` | `SPRAS` |  | `String(2)` | Y | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `ForeignExchangeFixingReference` | `FTR_FIXING_REF_ID` | `FTR_FIXING_REF_ID` |  | `String(30)` | Y | Fixing Reference ID |  | _FixingReference | S/4 only entity — no ECC CDC mapping |
| `FXFixingReferenceName` | `FTR_FIXING_REF_ID_TEXT` | `FTR_FIXING_REF_ID_TEXT` |  | `String(40)` |  | Fixing Ref. Desc. |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `FinInstrActivityCategoryText`

- **ABAP Name:** `I_FinInstrActivityCategoryText`
- **Label:** Fin Instrument Activity Category - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Language` | `SPRAS` | `SPRAS` |  | `String(2)` | Y | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `FinancialInstrProductCategory` | `TB_SANLF` | `TB_SANLF` |  | `String(3)` | Y | Product Category |  | _ProductCategory | S/4 only entity — no ECC CDC mapping |
| `FinInstrTransactionCategory` | `TB_SFGTYP` | `TB_SFGTYP` |  | `String(3)` | Y | Transaction Category |  | _TransactionCategory | S/4 only entity — no ECC CDC mapping |
| `FinancialInstrActivityCategory` | `TB_SFGZUTY` | `TB_SFGZUTY` |  | `String(2)` | Y | Activity Category |  | _ActivityCategory | S/4 only entity — no ECC CDC mapping |
| `FinInstrActivityCategoryName` | `TB_XTTEXT` | `TB_XTTEXT` |  | `String(30)` |  | Activity Cat. Name |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `FinInstrProductTypeSupplement`

- **ABAP Name:** `I_FinInstrProdTypeSuplmnt`
- **Label:** Product Type Supplements
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `FinancialInstrumentProductType` | `VVSART` | `VVSART` |  | `String(3)` | Y | Product Type |  |  | S/4 only entity — no ECC CDC mapping |
| `TreasurySettlementType` | `TI_SETTLFL` | `TI_SETTLFL` |  | `String(1)` |  | Settlement |  |  | S/4 only entity — no ECC CDC mapping |
| `OptionExerciseType` | `SOPTAUS` | `SOPTAUS` |  | `String(1)` |  | Exercise Type |  |  | S/4 only entity — no ECC CDC mapping |
| `TradeFinanceCategory` | `FTR_TF_CAT` | `FTR_TF_CAT` |  | `String(1)` |  | Trade Finance Cat. |  |  | S/4 only entity — no ECC CDC mapping |
| `OptionUnderlyingProductType` | `OPTION_UNDERLYING_PRODUCT_TYPE` | `OPTION_UNDERLYING_PRODUCT_TYPE` |  | `String(3)` |  | UL Product Type |  |  | S/4 only entity — no ECC CDC mapping |
| `OptionUndrlgTransactionType` | `TB_USFHAAR` | `TB_USFHAAR` |  | `String(3)` |  | Underly.Trans.Type |  |  | S/4 only entity — no ECC CDC mapping |
| `IntrstRateSwapIsCrossCurrency` | `TI_JWSWAP` | `TI_JWSWAP` |  | `Boolean` |  | Currency Swap |  |  | S/4 only entity — no ECC CDC mapping |
| `ProductTypeCashFlowCalculation` | `TB_CASH_FLOW_CALC` | `TB_CASH_FLOW_CALC` |  | `String(2)` |  | CF Calculation |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `FinInstrProductTypeText`

- **ABAP Name:** `I_FinancialInstrProdTypeText`
- **Label:** Product Type - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Language` | `SPRAS` | `SPRAS` |  | `String(2)` | Y | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `FinancialInstrumentProductType` | `VVSART` | `VVSART` |  | `String(3)` | Y | Product Type |  | _FinancialInstrProductType | S/4 only entity — no ECC CDC mapping |
| `FinancialInstrProdTypeName` | `FTR_GEN_PRODUCT_TYPE_NAME` | `FTR_GEN_PRODUCT_TYPE_NAME` |  | `String(30)` |  | Product Type Name |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `FinInstrTransCategoryText`

- **ABAP Name:** `I_FinInstrTransCatText`
- **Label:** Transaction Category - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Language` | `SPRAS` | `SPRAS` |  | `String(2)` | Y | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `FinancialInstrProductCategory` | `TB_SANLF` | `TB_SANLF` |  | `String(3)` | Y | Product Category |  | _FinancialInstrProdCat | S/4 only entity — no ECC CDC mapping |
| `FinInstrTransactionCategory` | `TB_SFGTYP` | `TB_SFGTYP` |  | `String(3)` | Y | Transaction Category |  |  | S/4 only entity — no ECC CDC mapping |
| `FinInstrTransCategoryName` | `TB_FTEXT` | `TB_FTEXT` |  | `String(30)` |  | Trans. Category Name |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `FinInstrTransactionCategory`

- **ABAP Name:** `I_FinInstrTransCat`
- **Label:** Transaction Category
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `FinancialInstrProductCategory` | `TB_SANLF` | `TB_SANLF` |  | `String(3)` | Y | Product Category |  | _FinancialInstrProdCat | S/4 only entity — no ECC CDC mapping |
| `FinInstrTransactionCategory` | `TB_SFGTYP` | `TB_SFGTYP` |  | `String(3)` | Y | Transaction Category |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `FinInstrTransactionTypeText`

- **ABAP Name:** `I_FinancialInstrTransTypeText`
- **Label:** Transaction Type - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Language` | `SPRAS` | `SPRAS` |  | `String(2)` | Y | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `FinancialInstrumentProductType` | `VVSART` | `VVSART` |  | `String(3)` | Y | Product Type |  | _Financialinstrproducttype | S/4 only entity — no ECC CDC mapping |
| `FinancialInstrTransactionType` | `FTR_GEN_TRANSACTION_TYPE` | `FTR_GEN_TRANSACTION_TYPE` |  | `String(3)` | Y | Transaction Type |  | _FinancialInstrTransType | S/4 only entity — no ECC CDC mapping |
| `FinancialInstrTransTypeName` | `FTR_GEN_TRANSACTION_TYPE_NAME` | `FTR_GEN_TRANSACTION_TYPE_NAME` |  | `String(30)` |  | Trans. Type Name |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `FinInstrumentActivityCategory`

- **ABAP Name:** `I_FinInstrActivityCategory`
- **Label:** Financial Instrument Activity Category
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `FinancialInstrProductCategory` | `TB_SANLF` | `TB_SANLF` |  | `String(3)` | Y | Product Category |  | _ProductCategory | S/4 only entity — no ECC CDC mapping |
| `FinInstrTransactionCategory` | `TB_SFGTYP` | `TB_SFGTYP` |  | `String(3)` | Y | Transaction Category |  | _TransactionCategory | S/4 only entity — no ECC CDC mapping |
| `FinancialInstrActivityCategory` | `TB_SFGZUTY` | `TB_SFGZUTY` |  | `String(2)` | Y | Activity Category |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransGenActivityCategory` | `FTR_GEN_ACTIVITY_CATEGORY` | `FTR_GEN_ACTIVITY_CATEGORY` |  | `String(3)` |  | General Activity Category |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `FinTransNoticePeriodUnit`

- **ABAP Name:** `I_FinTransNoticePeriodUnit`
- **Label:** Financial Transaction Notice Period Unit
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `FinTransNoticePeriodUnit` | `TB_SKUEND` | `TB_SKUEND` |  | `String(1)` | Y | Unit |  |  | S/4 only entity — no ECC CDC mapping |
| `DomainValue` | `DOMVALUE_L` | `DOMVALUE_L` |  | `String(10)` |  | Lower Value |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `FinTransNoticePeriodUnitText`

- **ABAP Name:** `I_FinTransNoticePeriodUnitText`
- **Label:** Fin Trans Notice Period Unit - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Language` | `SPRAS` | `SPRAS` |  | `String(2)` | Y | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransNoticePeriodUnit` | `TB_SKUEND` | `TB_SKUEND` |  | `String(1)` | Y | Unit |  | _NoticePeriodUnit | S/4 only entity — no ECC CDC mapping |
| `DomainValue` | `DOMVALUE_L` | `DOMVALUE_L` |  | `String(10)` |  | Lower Value |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransNoticePeriodUnitName` | `TB_SKUEND_NAME` | `TB_SKUEND_NAME` |  | `String(60)` |  | NoticePer. Unit Name |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `FinTransOptionExerciseType`

- **ABAP Name:** `I_OptionExerciseType`
- **Label:** Option exercise type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `OptionExerciseType` | `SOPTAUS` | `SOPTAUS` |  | `String(1)` | Y | Exercise Type |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `FinTransOptionExerciseTypeText`

- **ABAP Name:** `I_OptionExerciseTypeText`
- **Label:** Option exercise type - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `OptionExerciseType` | `SOPTAUS` | `SOPTAUS` |  | `String(1)` | Y | Exercise Type |  |  | S/4 only entity — no ECC CDC mapping |
| `Language` | `DDLANGUAGE` | `DDLANGUAGE` |  | `String(2)` | Y | Lang. |  |  | S/4 only entity — no ECC CDC mapping |
| `OptionExerciseTypeName` | `OPTION_EXERCISE_TYPE_NAME` | `OPTION_EXERCISE_TYPE_NAME` |  | `String(60)` |  | Option Exercise Type |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `FinTransOptionSettlementType`

- **ABAP Name:** `I_OptionSettlementType`
- **Label:** Option settlement type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `OptionSettlementType` | `OPTION_SETTLEMENT_TYPE` | `OPTION_SETTLEMENT_TYPE` |  | `String(1)` | Y | Settlement Type |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `FinTransOptnSettlementTypeText`

- **ABAP Name:** `I_OptionSettlementTypeText`
- **Label:** Option settlement type - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `OptionSettlementType` | `OPTION_SETTLEMENT_TYPE` | `OPTION_SETTLEMENT_TYPE` |  | `String(1)` | Y | Settlement Type |  |  | S/4 only entity — no ECC CDC mapping |
| `Language` | `DDLANGUAGE` | `DDLANGUAGE` |  | `String(2)` | Y | Lang. |  |  | S/4 only entity — no ECC CDC mapping |
| `OptionSettlementTypeName` | `OPTION_SETTLEMENT_TYPE_NAME` | `OPTION_SETTLEMENT_TYPE_NAME` |  | `String(60)` |  | Option Settlemt Type |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `FinTransOptnUndrlgAllocation`

- **ABAP Name:** `I_FinTransOptnUndrlgAllocation`
- **Label:** Fin Trans Option Underlying Allocation
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `FinTransOptionNumber` | `TI_RGATT` | `TI_RGATT` |  | `String(13)` | Y | Class |  |  | S/4 only entity — no ECC CDC mapping |
| `OptionUnderlyingTransaction` | `OPTION_UNDERLYING_TRANSACTION` | `OPTION_UNDERLYING_TRANSACTION` |  | `String(13)` | Y | Transaction |  |  | S/4 only entity — no ECC CDC mapping |
| `FinancialTransactionFromExer` | `TB_VRFHA` | `TB_VRFHA` |  | `String(13)` |  | Exercise Transaction |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `FinTransReleaseStatus`

- **ABAP Name:** `I_FinTransReleaseStatus`
- **Label:** Financial Transaction Release Status
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `FinTransReleaseStatus` | `TB_FRGZUST` | `TB_FRGZUST` |  | `String(1)` | Y | Release Status |  |  | S/4 only entity — no ECC CDC mapping |
| `DomainValue` | `DOMVALUE_L` | `DOMVALUE_L` |  | `String(10)` |  | Lower Value |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `FinTransReleaseStatusText`

- **ABAP Name:** `I_FinTransReleaseStatusText`
- **Label:** Fin Transaction Release Status - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Language` | `SPRAS` | `SPRAS` |  | `String(2)` | Y | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransReleaseStatus` | `TB_FRGZUST` | `TB_FRGZUST` |  | `String(1)` | Y | Release Status |  | _ReleaseStatus | S/4 only entity — no ECC CDC mapping |
| `DomainValue` | `DOMVALUE_L` | `DOMVALUE_L` |  | `String(10)` |  | Lower Value |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransReleaseStatusName` | `TB_FRGZUST_NAME` | `TB_FRGZUST_NAME` |  | `String(60)` |  | Release Status Name |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `FinTransUnderlyingFlow`

- **ABAP Name:** `I_FinTransUnderlyingFlow`
- **Label:** Fin Transaction Underlying Flow
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `OptionUnderlyingTransaction` | `OPTION_UNDERLYING_TRANSACTION` | `OPTION_UNDERLYING_TRANSACTION` |  | `String(13)` | Y | Transaction |  |  | S/4 only entity — no ECC CDC mapping |
| `FinancialInstrumentActivity` | `TB_RFHAZU` | `TB_RFHAZU` |  | `String(5)` | Y | Activity |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransFlowCreationDate` | `TB_CRDAT` | `TB_CRDAT` |  | `Date` | Y | Entered On |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransFlowCreationTime` | `FTR_FLOW_CREATION_TIME` | `FTR_FLOW_CREATION_TIME` |  | `String(6)` | Y | Entry Time |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransFlowNumber` | `TB_RFHAZB` | `TB_RFHAZB` |  | `String(4)` | Y | Flow |  |  | S/4 only entity — no ECC CDC mapping |
| `CreatedByUser` | `TB_CRUSER` | `TB_CRUSER` |  | `String(12)` |  | Entered By |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransCreationDate` | `FTR_CREATION_DATE` | `FTR_CREATION_DATE` |  | `Date` |  | Created On |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransCreationTime` | `TB_TCRTIM` | `TB_TCRTIM` |  | `String(6)` |  | Entry Time |  |  | S/4 only entity — no ECC CDC mapping |
| `LastChangedByUser` | `TB_UPUSER` | `TB_UPUSER` |  | `String(12)` |  | Last Changed By |  |  | S/4 only entity — no ECC CDC mapping |
| `LastChangeDate` | `TB_DUPDAT` | `TB_DUPDAT` |  | `Date` |  | Changed On |  |  | S/4 only entity — no ECC CDC mapping |
| `FinInstrumentLastChangedTime` | `TB_TUPTIM` | `TB_TUPTIM` |  | `String(6)` |  | Time Changed |  |  | S/4 only entity — no ECC CDC mapping |
| `TreasuryContractType` | `RANTYP` | `RANTYP` |  | `String(1)` |  | Contract Type |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransFlowType` | `TB_SFHAZBA` | `TB_SFHAZBA` |  | `String(4)` |  | Flow Type |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransFlowCategory` | `FTR_FLOW_CATEGORY` | `FTR_FLOW_CATEGORY` |  | `String(2)` |  | Flow Category |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransFlowPaytAmtDirection` | `FTR_FLOW_PAYMENT_AMT_DIRECTION` | `FTR_FLOW_PAYMENT_AMT_DIRECTION` |  | `String(1)` |  | Direction |  |  | S/4 only entity — no ECC CDC mapping |
| `FinancialTransactionDirection` | `TB_RKONDGR` | `TB_RKONDGR` |  | `String(1)` |  | Direction |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransFlowSource` | `TB_SHERK` | `TB_SHERK` |  | `String(4)` |  | Source |  |  | S/4 only entity — no ECC CDC mapping |
| `PayerPayee` | `TB_RPZAHL_NEW` | `TB_RPZAHL_NEW` |  | `String(10)` |  | Payer/Payee |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransFlowPaymentDate` | `FTR_FLOW_PAYMENT_DATE` | `FTR_FLOW_PAYMENT_DATE` |  | `Date` |  | Payment Date |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransFlowPaytAmt` | `FTR_FLOW_PAYMENT_AMOUNT` | `FTR_FLOW_PAYMENT_AMOUNT` |  | `Decimal(34,4)` |  | Payment Amnt in PyC | FinTransFlowPaytAmtCrcy |  | S/4 only entity — no ECC CDC mapping |
| `FinTransFlowPaytAmtCrcy` | `TB_WZBETR` | `TB_WZBETR` |  | `String(5)` |  | Payment Currency |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransFlowInLoclCrcyPaytAmt` | `TB_HWBETR` | `TB_HWBETR` |  | `Decimal(34,4)` |  | Pmnt Amnt in LCurr | FinTransFlowPaytAmtCrcy |  | S/4 only entity — no ECC CDC mapping |
| `FinTransFlowLoclCrcyCnvrsnRate` | `FTR_FLOW_LOCL_CRCY_CNVRSN_RATE` | `FTR_FLOW_LOCL_CRCY_CNVRSN_RATE` |  | `Decimal(9,5)` |  | Crcy Cnvrsn Rate |  |  | S/4 only entity — no ECC CDC mapping |
| `CalculationDate` | `DVALUT` | `DVALUT` |  | `Date` |  | Calculation Date |  |  | S/4 only entity — no ECC CDC mapping |
| `CalculationPeriodStartDate` | `DBERVON` | `DBERVON` |  | `Date` |  | Calculation From |  |  | S/4 only entity — no ECC CDC mapping |
| `CalculationPeriodEndDate` | `DBERBIS` | `DBERBIS` |  | `Date` |  | Calculation To |  |  | S/4 only entity — no ECC CDC mapping |
| `CalcPeriodEndDateIsInclusive` | `VVSINCLBIS` | `VVSINCLBIS` |  | `String(1)` |  | Inclusive End Date |  |  | S/4 only entity — no ECC CDC mapping |
| `CalcPeriodStartDateIsExclusive` | `VVSEXCLVON` | `VVSEXCLVON` |  | `String(1)` |  | Exclusive Start Date |  |  | S/4 only entity — no ECC CDC mapping |
| `CalcPeriodEndDateIsMonthEnd` |  |  |  | `Boolean` |  | Month-End End Date |  |  | S/4 only entity — no ECC CDC mapping |
| `CalcPeriodStartDateIsMonthEnd` |  |  |  | `Boolean` |  | Month-End Start Date |  |  | S/4 only entity — no ECC CDC mapping |
| `NumberOfCalculationDays` | `VVATAGE` | `VVATAGE` |  | `String(6)` |  | Number of Days |  |  | S/4 only entity — no ECC CDC mapping |
| `NrOfBaseDaysPerCalcPeriod` | `ABASTAGE` | `ABASTAGE` |  | `String(6)` |  | No. of base days |  |  | S/4 only entity — no ECC CDC mapping |
| `InterestCalculationMethod` | `SZBMETH` | `SZBMETH` |  | `String(1)` |  | Int. Calc. Method |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransFlowCalcBaseAmount` | `BBASIS` | `BBASIS` |  | `Decimal(34,4)` |  | Base Amount | FinTransFlowCalcBaseAmountCrcy |  | S/4 only entity — no ECC CDC mapping |
| `FinTransFlowCalcBaseAmountCrcy` | `TB_WBASIS` | `TB_WBASIS` |  | `String(5)` |  | Calculatn Basis Crcy |  |  | S/4 only entity — no ECC CDC mapping |
| `IntrstCalcMethFactoryCalendar` | `TFMSKALIDWT` | `TFMSKALIDWT` |  | `String(2)` |  | Interest Calendar |  |  | S/4 only entity — no ECC CDC mapping |
| `InterestBaseDaysMethod` | `VVSTGBASIS` | `VVSTGBASIS` |  | `String(1)` |  | Base Days Method |  |  | S/4 only entity — no ECC CDC mapping |
| `InterestCalculationType` | `TFMSINTCALC` | `TFMSINTCALC` |  | `String(1)` |  | Int. Calc. Type |  |  | S/4 only entity — no ECC CDC mapping |
| `ConditionPercentageRate` | `PKOND` | `PKOND` |  | `Decimal(10,7)` |  | Percentage Rate |  |  | S/4 only entity — no ECC CDC mapping |
| `FinCndnPctgRateFixingDate` | `VVDPKOND` | `VVDPKOND` |  | `Date` |  | PercFixingDte |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransFlowIntrstRateFixDate` | `TB_DZFEST` | `TB_DZFEST` |  | `Date` |  | Int.Rate Fixing Date |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransPositionValueDate` | `TB_DBESTAND` | `TB_DBESTAND` |  | `Date` |  | Position Value Date |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransFlowPositionAmount` | `FTR_POSITION_AMOUNT` | `FTR_POSITION_AMOUNT` |  | `Decimal(34,4)` |  | PositionAmount | FinTransFlwPosAmtCrcy |  | S/4 only entity — no ECC CDC mapping |
| `FinTransFlwPosAmtCrcy` | `TB_WBBETR` | `TB_WBBETR` |  | `String(5)` |  | Position Currency |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransFlowNomAmt` | `FTR_FLOW_NORMINAL_AMOUNT` | `FTR_FLOW_NORMINAL_AMOUNT` |  | `Decimal(34,4)` |  | Nominal Amount | FinTransFlowNomAmtCrcy |  | S/4 only entity — no ECC CDC mapping |
| `FinTransFlowNomAmtCrcy` | `FTR_FLOW_NORMINAL_AMOUNT_CRCY` | `FTR_FLOW_NORMINAL_AMOUNT_CRCY` |  | `String(5)` |  | Nominal Amount Currency |  |  | S/4 only entity — no ECC CDC mapping |
| `MarketValueInQtanCurrency` | `TB_BEBETR` | `TB_BEBETR` |  | `Decimal(34,4)` |  | Mkt Val. in QC | QuotationCurrency |  | S/4 only entity — no ECC CDC mapping |
| `QuotationCurrency` | `TB_WEBETR` | `TB_WEBETR` |  | `String(5)` |  | Price Currency |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransTradedNumberOfUnits` | `FTR_FINTRANS_UNITS_L` | `FTR_FINTRANS_UNITS_L` |  | `Decimal(24,14)` |  | Number of Units |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransTrdPriceCrcyUnitRate` | `FTR_PRICE` | `FTR_PRICE` |  | `Decimal(23,14)` |  | Price (Unit-Quoted) |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransTradedPriceCrcyUnit` | `FTR_TRADED_PRICE_CURRENCY_UNIT` | `FTR_TRADED_PRICE_CURRENCY_UNIT` |  | `String(5)` |  | Currency Unit |  |  | S/4 only entity — no ECC CDC mapping |
| `SecurityExchange` | `VVRHANDPL` | `VVRHANDPL` |  | `String(10)` |  | Exchange |  |  | S/4 only entity — no ECC CDC mapping |
| `FinConditionItem` | `TB_KOND` | `TB_KOND` |  | `String(4)` |  | Condition |  |  | S/4 only entity — no ECC CDC mapping |
| `ConditionItemValidityStartDate` | `DGUEL_KP` | `DGUEL_KP` |  | `Date` |  | Item Effective From |  |  | S/4 only entity — no ECC CDC mapping |
| `FinConditionSubItem` | `NSTUFE` | `NSTUFE` |  | `String(2)` |  | Level Number |  |  | S/4 only entity — no ECC CDC mapping |
| `InterestConditionType` | `SKOART` | `SKOART` |  | `String(4)` |  | Condition Type |  |  | S/4 only entity — no ECC CDC mapping |
| `FinInstrConditionLogicGroup` | `FTR_INSTR_CNDN_LOGIC_GROUP` | `FTR_INSTR_CNDN_LOGIC_GROUP` |  | `String(4)` |  | Condition Group |  |  | S/4 only entity — no ECC CDC mapping |
| `FinCndnCrsRefcdAccmlnCndnGrp` | `TB_SUM_RKOND` | `TB_SUM_RKOND` |  | `String(4)` |  | Accum. Cond.Grp |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransFlwReltdAccumulatingID` | `TB_SUM_ID_SOURCE` | `TB_SUM_ID_SOURCE` |  | `String(40)` |  | Rel.AccumFlowID |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransFlowAccumulatingFlowID` | `TB_SUM_ID_SUM` | `TB_SUM_ID_SUM` |  | `String(40)` |  | Accum. Flow ID |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransTradedPricePercent` | `FTR_PRICE_PERCENT` | `FTR_PRICE_PERCENT` |  | `Decimal(23,14)` |  | Price (%) |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `FinancialInstrTransactionType`

- **ABAP Name:** `I_FinancialInstrTransType`
- **Label:** Transaction Type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `FinancialInstrTransactionType` | `FTR_GEN_TRANSACTION_TYPE` | `FTR_GEN_TRANSACTION_TYPE` |  | `String(3)` | Y | Transaction Type |  |  | S/4 only entity — no ECC CDC mapping |
| `FinancialInstrumentProductType` | `VVSART` | `VVSART` |  | `String(3)` | Y | Product Type |  | _FinancialInstrProductType | S/4 only entity — no ECC CDC mapping |
| `FinInstrTransactionCategory` | `TB_SFGTYP` | `TB_SFGTYP` |  | `String(3)` |  | Transaction Category |  |  | S/4 only entity — no ECC CDC mapping |
| `TreasuryContractType` | `RANTYP` | `RANTYP` |  | `String(1)` |  | Contract Type |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `FinancialInstrumentProductType`

- **ABAP Name:** `I_FinancialinstrProductType`
- **Label:** Product Type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `FinancialInstrumentProductType` | `VVSART` | `VVSART` |  | `String(3)` | Y | Product Type |  |  | S/4 only entity — no ECC CDC mapping |
| `TreasuryContractType` | `RANTYP` | `RANTYP` |  | `String(1)` |  | Contract Type |  |  | S/4 only entity — no ECC CDC mapping |
| `FinancialInstrProductCategory` | `SANLF` | `SANLF` |  | `String(3)` |  | Product Category |  |  | S/4 only entity — no ECC CDC mapping |
| `FinCndnTypeAllocCndnGroup` | `SKOGRP` | `SKOGRP` |  | `String(3)` |  | Condition Group |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `FinancialInstrumentStatus`

- **ABAP Name:** `I_FinInstrumentStatus`
- **Label:** Financial Instrument Status
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `FinancialInstrumentStatus` | `TB_SAKTIV` | `TB_SAKTIV` |  | `String(1)` | Y | Active Status |  |  | S/4 only entity — no ECC CDC mapping |
| `DomainValue` | `DOMVALUE_L` | `DOMVALUE_L` |  | `String(10)` |  | Lower Value |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `FinancialInstrumentStatusText`

- **ABAP Name:** `I_FinInstrumentStatusText`
- **Label:** Financial Instrument Status - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Language` | `SPRAS` | `SPRAS` |  | `String(2)` | Y | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `FinancialInstrumentStatus` | `TB_SAKTIV` | `TB_SAKTIV` |  | `String(1)` | Y | Active Status |  | _Status | S/4 only entity — no ECC CDC mapping |
| `DomainValue` | `DOMVALUE_L` | `DOMVALUE_L` |  | `String(10)` |  | Lower Value |  |  | S/4 only entity — no ECC CDC mapping |
| `FinancialInstrumentStatusName` | `TB_SAKTIV_NAME` | `TB_SAKTIV_NAME` |  | `String(60)` |  | Active Status Name |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `FinancialTransaction`

- **ABAP Name:** `I_FinancialTransactionDEX`
- **Label:** Financial Transaction
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `CompanyCode` | `BUKRS` | `BUKRS` |  | `String(4)` | Y | Company Code |  |  | S/4 only entity — no ECC CDC mapping |
| `FinancialTransaction` | `TB_RFHA` | `TB_RFHA` |  | `String(13)` | Y | Transaction |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransCreationDate` | `FTR_CREATION_DATE` | `FTR_CREATION_DATE` |  | `Date` |  | Created On |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransCreationTime` | `TB_TCRTIM` | `TB_TCRTIM` |  | `String(6)` |  | Entry Time |  |  | S/4 only entity — no ECC CDC mapping |
| `LastChangeDate` | `TB_DUPDAT` | `TB_DUPDAT` |  | `Date` |  | Changed On |  |  | S/4 only entity — no ECC CDC mapping |
| `FinInstrumentLastChangedTime` | `TB_TUPTIM` | `TB_TUPTIM` |  | `String(6)` |  | Time Changed |  |  | S/4 only entity — no ECC CDC mapping |
| `TreasuryContractType` | `RANTYP` | `RANTYP` |  | `String(1)` |  | Contract Type |  | _ContractType | S/4 only entity — no ECC CDC mapping |
| `FinancialInstrProductCategory` | `FTR_GEN_FIN_INSTR_PROD_CATEG` | `FTR_GEN_FIN_INSTR_PROD_CATEG` |  | `String(3)` |  | Product Category |  | _FinancialInstrProdCat | S/4 only entity — no ECC CDC mapping |
| `FinancialInstrumentProductType` | `VVSART` | `VVSART` |  | `String(3)` |  | Product Type |  | _FinancialInstrProdType | S/4 only entity — no ECC CDC mapping |
| `FinInstrTransactionCategory` | `TB_SFGTYP` | `TB_SFGTYP` |  | `String(3)` |  | Transaction Category |  | _FinInstrTransCat | S/4 only entity — no ECC CDC mapping |
| `FinancialInstrTransactionType` | `FTR_GEN_TRANSACTION_TYPE` | `FTR_GEN_TRANSACTION_TYPE` |  | `String(3)` |  | Transaction Type |  | _FinancialInstrTransType | S/4 only entity — no ECC CDC mapping |
| `TermStartDate` | `TB_DBLFZ` | `TB_DBLFZ` |  | `Date` |  | Term Start |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransNoticePeriod` | `TB_AKUEND` | `TB_AKUEND` |  | `String(3)` |  | Period of Notice |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransNoticePeriodUnit` | `TB_SKUEND` | `TB_SKUEND` |  | `String(1)` |  | Unit |  | _NoticePeriodUnit | S/4 only entity — no ECC CDC mapping |
| `FinTransFactoryCalendar1` | `SKALID` | `SKALID` |  | `String(2)` |  | Calendar |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransFactoryCalendar2` | `SKALID` | `SKALID` |  | `String(2)` |  | Calendar |  |  | S/4 only entity — no ECC CDC mapping |
| `Counterparty` | `RKONTRAH_NEW` | `RKONTRAH_NEW` |  | `String(10)` |  | Counterparty |  |  | S/4 only entity — no ECC CDC mapping |
| `FinancialInstrumentGuarantor` | `TB_RGARANT_NEW` | `TB_RGARANT_NEW` |  | `String(10)` |  | Guarantor |  |  | S/4 only entity — no ECC CDC mapping |
| `Portfolio` | `RPORTB` | `RPORTB` |  | `String(10)` |  | Portfolio |  | _Portfolio | S/4 only entity — no ECC CDC mapping |
| `TreasuryFinanceProject` | `TB_TFPROJ` | `TB_TFPROJ` |  | `String(13)` |  | Finance Project |  |  | S/4 only entity — no ECC CDC mapping |
| `FinancialInstrumentAssignment` | `FTR_GEN_FIN_INSTR_ASSIGNMENT` | `FTR_GEN_FIN_INSTR_ASSIGNMENT` |  | `String(18)` |  | Free Assignment |  |  | S/4 only entity — no ECC CDC mapping |
| `FinancialInstrumentReference` | `FTR_GEN_FIN_INSTR_INTERNAL_REF` | `FTR_GEN_FIN_INSTR_INTERNAL_REF` |  | `String(16)` |  | Free Internal Ref. |  |  | S/4 only entity — no ECC CDC mapping |
| `FinancialInstrCharacteristic` | `FTR_GEN_FIN_INSTR_CHAR` | `FTR_GEN_FIN_INSTR_CHAR` |  | `String(25)` |  | Free Charact. |  |  | S/4 only entity — no ECC CDC mapping |
| `ControllingArea` | `KOKRS` | `KOKRS` |  | `String(4)` |  | Controlling Area |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCenter` | `KOSTL` | `KOSTL` |  | `String(10)` |  | Cost Center |  |  | S/4 only entity — no ECC CDC mapping |
| `HedgingClassification` | `TOE_HEDGING_CLASSIFICATION` | `TOE_HEDGING_CLASSIFICATION` |  | `String(5)` |  | Hedging Classificatn |  |  | S/4 only entity — no ECC CDC mapping |
| `HedgeRequestIdentifier` | `HEDGE_REQUEST_IDENTIFIER` | `HEDGE_REQUEST_IDENTIFIER` |  | `String(13)` |  | Hedge Request ID |  |  | S/4 only entity — no ECC CDC mapping |
| `ProfitCenter` | `PRCTR` | `PRCTR` |  | `String(10)` |  | Profit Center |  |  | S/4 only entity — no ECC CDC mapping |
| `WBSElementInternalID` | `PS_S4_PSPNR` | `PS_S4_PSPNR` |  | `String(8)` |  | WBS Internal ID |  |  | S/4 only entity — no ECC CDC mapping |
| `TreasuryFacilityCompanyCode` | `TB_FACILITYBUKRS` | `TB_FACILITYBUKRS` |  | `String(4)` |  | CoCd of Facility |  |  | S/4 only entity — no ECC CDC mapping |
| `TreasuryFacility` | `TB_FACILITYNR` | `TB_FACILITYNR` |  | `String(13)` |  | Facility |  |  | S/4 only entity — no ECC CDC mapping |
| `FinancialInstrumentStatus` | `TB_SAKTIV` | `TB_SAKTIV` |  | `String(1)` |  | Active Status |  | _Status | S/4 only entity — no ECC CDC mapping |
| `FinTransReleaseStatus` | `TB_FRGZUST` | `TB_FRGZUST` |  | `String(1)` |  | Release Status |  | _ReleaseStatus | S/4 only entity — no ECC CDC mapping |
| `TransactionCurrency` | `TB_WGSCHFT` | `TB_WGSCHFT` |  | `String(5)` |  | Transaction Currency |  |  | S/4 only entity — no ECC CDC mapping |
| `FinInstrumentOutgoingCurrency` | `TB_WGSCHF1` | `TB_WGSCHF1` |  | `String(5)` |  | Outgoing Currency |  |  | S/4 only entity — no ECC CDC mapping |
| `FinInstrumentIncomingCurrency` | `TB_WGSCHF2` | `TB_WGSCHF2` |  | `String(5)` |  | Incoming Currency |  |  | S/4 only entity — no ECC CDC mapping |
| `TradedCurrency` | `FTR_TRADED_CURR` | `FTR_TRADED_CURR` |  | `String(5)` |  | Traded Currency |  |  | S/4 only entity — no ECC CDC mapping |
| `SecurityClass` | `FTR_GEN_SECURITY_CLASS` | `FTR_GEN_SECURITY_CLASS` |  | `String(13)` |  | Security Class |  |  | S/4 only entity — no ECC CDC mapping |
| `ClassificationOfFinInstr` | `FTR_CFI_CODE` | `FTR_CFI_CODE` |  | `String(6)` |  | CFI Code |  |  | S/4 only entity — no ECC CDC mapping |
| `SecurityAccount` | `FTR_GEN_SECURITY_ACCOUNT` | `FTR_GEN_SECURITY_ACCOUNT` |  | `String(10)` |  | Securities Account |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransIsRiskMitigating` | `FTR_THRESHOLD_RISK_MITIGATING` | `FTR_THRESHOLD_RISK_MITIGATING` |  | `Boolean` |  | Risk Mitigation |  |  | S/4 only entity — no ECC CDC mapping |
| `FinInstrLastActiveActivity` | `FTR_GEN_FIN_INSTR_LAST_ACT_ACT` | `FTR_GEN_FIN_INSTR_LAST_ACT_ACT` |  | `String(5)` |  | Last Active Activity |  |  | S/4 only entity — no ECC CDC mapping |
| `TrsyTradedAmountBuySellCode` | `TTM_FX_BUY_SELL` | `TTM_FX_BUY_SELL` |  | `String(1)` |  | Buy/Sell |  |  | S/4 only entity — no ECC CDC mapping |
| `Segment` | `FB_SEGMENT` | `FB_SEGMENT` |  | `String(10)` |  | Segment |  |  | S/4 only entity — no ECC CDC mapping |
| `OnBehalfOfCompany` | `TRBA_BEHALF_OF_COMPANY` | `TRBA_BEHALF_OF_COMPANY` |  | `String(4)` |  | On Behalf of CoCode |  |  | S/4 only entity — no ECC CDC mapping |
| `MarketIdentifierCode` | `TBA_MIC` | `TBA_MIC` |  | `String(4)` |  | MIC |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransRoundingCategory` | `TB_SRNDNG` | `TB_SRNDNG` |  | `String(1)` |  | Round |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransGeneralValuationClass` | `TPM_COM_VAL_CLASS` | `TPM_COM_VAL_CLASS` |  | `String(4)` |  | Gen. Valn Class |  |  | S/4 only entity — no ECC CDC mapping |
| `Fund` | `FM_FUND` | `FM_FUND` |  | `String(10)` |  | Fund |  |  | S/4 only entity — no ECC CDC mapping |
| `GrantID` | `GM_GRANT_NBR` | `GM_GRANT_NBR` |  | `String(20)` |  | Grant |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransAuthorizationGroup` | `TBEGRU` | `TBEGRU` |  | `String(4)` |  | Authorization Group |  |  | S/4 only entity — no ECC CDC mapping |
| `BusinessPlace` | `BUPLA` | `BUPLA` |  | `String(4)` |  | Business Place |  |  | S/4 only entity — no ECC CDC mapping |
| `FunctionalArea` | `FKBER` | `FKBER` |  | `String(16)` |  | Functional Area |  |  | S/4 only entity — no ECC CDC mapping |
| `TrsyPosCustomDiffntnTerm1` | `TPM_CUST_DIFF_TERM_VALUE` | `TPM_CUST_DIFF_TERM_VALUE` |  | `String(20)` |  | Cust.Diff.Term Val. |  |  | S/4 only entity — no ECC CDC mapping |
| `TrsyPosCustomDiffntnTerm2` | `TPM_CUST_DIFF_TERM_VALUE` | `TPM_CUST_DIFF_TERM_VALUE` |  | `String(20)` |  | Cust.Diff.Term Val. |  |  | S/4 only entity — no ECC CDC mapping |
| `TrsyPosCustomDiffntnTerm3` | `TPM_CUST_DIFF_TERM_VALUE` | `TPM_CUST_DIFF_TERM_VALUE` |  | `String(20)` |  | Cust.Diff.Term Val. |  |  | S/4 only entity — no ECC CDC mapping |
| `TrsyPosCustomDiffntnTerm4` | `TPM_CUST_DIFF_TERM_VALUE` | `TPM_CUST_DIFF_TERM_VALUE` |  | `String(20)` |  | Cust.Diff.Term Val. |  |  | S/4 only entity — no ECC CDC mapping |
| `TrsyPosCustomDiffntnTerm5` | `TPM_CUST_DIFF_TERM_VALUE` | `TPM_CUST_DIFF_TERM_VALUE` |  | `String(20)` |  | Cust.Diff.Term Val. |  |  | S/4 only entity — no ECC CDC mapping |
| `UniqueProductIdentifier` | `FTR_UPI` | `FTR_UPI` |  | `String(12)` |  | Unique Product ID |  |  | S/4 only entity — no ECC CDC mapping |
| `InternationalSecuritiesIdnNmbr` | `RANL_ISIN` | `RANL_ISIN` |  | `String(12)` |  | Security ID (ISIN) |  |  | S/4 only entity — no ECC CDC mapping |
| `ReportTrackingNumber` | `FTR_RTN` | `FTR_RTN` |  | `String(52)` |  | Report Tracking No. |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransOptionNumber` | `TI_RGATT` | `TI_RGATT` |  | `String(13)` |  | Class |  |  | S/4 only entity — no ECC CDC mapping |
| `FinancialInstrActivityCategory` | `TB_SFGZUTY` | `TB_SFGZUTY` |  | `String(2)` |  | Activity Category |  | _ActivityCategory | S/4 only entity — no ECC CDC mapping |
| `TermEndDate` | `TB_DELFZ` | `TB_DELFZ` |  | `Date` |  | Term End |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransTermCategory` | `FTR_TERM_CATEGORY` | `FTR_TERM_CATEGORY` |  | `String(1)` |  | Term Category |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransTermStartEndInclusive` | `FTR_TERM_START_END_INCLUSIVE` | `FTR_TERM_START_END_INCLUSIVE` |  | `String(1)` |  | Term Start and End Inclusive |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransNoticeDate` | `TB_NOTICE_DATE` | `TB_NOTICE_DATE` |  | `Date` |  | Notice Date |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransActyConclusionDate` | `FTR_ACTY_CONCLUSION_DTE` | `FTR_ACTY_CONCLUSION_DTE` |  | `Date` |  | Conclusion Date |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransActyConclusionTime` | `TB_TVTRAB` | `TB_TVTRAB` |  | `String(6)` |  | Contract.Concl.Time |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransActyConclusionTimeZone` | `TB_ZVTRAB` | `TB_ZVTRAB` |  | `String(6)` |  | Time Zone Contr.Date |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransRolloverDate` | `TB_DBLFZ` | `TB_DBLFZ` |  | `Date` |  | Term Start |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransExerciseDate` | `TB_DELFZ` | `TB_DELFZ` |  | `Date` |  | Term End |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransOrderValidityEndDate` | `TB_LIMITDA` | `TB_LIMITDA` |  | `Date` |  | Limit Date |  |  | S/4 only entity — no ECC CDC mapping |
| `FinTransFixingDate` | `TB_DFIX` | `TB_DFIX` |  | `Date` |  | Fixing Date |  |  | S/4 only entity — no ECC CDC mapping |
| `ForeignExchangeFixingReference` | `FTR_FIXING_REF_ID` | `FTR_FIXING_REF_ID` |  | `String(30)` |  | Fixing Reference ID |  | _FixingReference | S/4 only entity — no ECC CDC mapping |
| `Trader` | `RDEALER` | `RDEALER` |  | `String(12)` |  | Trader |  |  | S/4 only entity — no ECC CDC mapping |
| `FinancialInstrContactPerson` | `TB_GSPPART` | `TB_GSPPART` |  | `String(19)` |  | Contact Person |  |  | S/4 only entity — no ECC CDC mapping |
| `FinInstrExternalReference` | `TB_NORDEXT` | `TB_NORDEXT` |  | `String(16)` |  | External Reference |  |  | S/4 only entity — no ECC CDC mapping |
| `TreasuryReversalReason` | `SSTOGRD` | `SSTOGRD` |  | `String(2)` |  | Reason for Reversal |  | _ReversalReason | S/4 only entity — no ECC CDC mapping |
| `LeadingCurrency` | `TB_WLWAERS` | `TB_WLWAERS` |  | `String(5)` |  | Leading Currency |  |  | S/4 only entity — no ECC CDC mapping |
| `FollowingCurrency` | `TB_WFWAERS` | `TB_WFWAERS` |  | `String(5)` |  | Following Currency |  |  | S/4 only entity — no ECC CDC mapping |
| `ExchangeRate` | `TB_KKURS` | `TB_KKURS` |  | `Decimal(13,9)` |  | Transaction Rate |  |  | S/4 only entity — no ECC CDC mapping |
| `SpotExchangeRate` | `TB_KKASSA` | `TB_KKASSA` |  | `Decimal(13,9)` |  | Spot Rate |  |  | S/4 only entity — no ECC CDC mapping |
| `SwapExchangeRate` | `TB_KSWAP` | `TB_KSWAP` |  | `Decimal(13,9)` |  | Swap Rate |  |  | S/4 only entity — no ECC CDC mapping |
| `LiquidityEffectValue` | `TX_KWLIQ` | `TX_KWLIQ` |  | `Decimal(13,9)` |  | Liquidity Effect |  |  | S/4 only entity — no ECC CDC mapping |
| `CurrencyPair` | `FTR_CURR_PAIR` | `FTR_CURR_PAIR` |  | `String(20)` |  | Currency Pair |  |  | S/4 only entity — no ECC CDC mapping |
| `EffectiveInterestRate` | `TB_PYIELD` | `TB_PYIELD` |  | `Decimal(10,7)` |  | Effect.Interest Rate |  |  | S/4 only entity — no ECC CDC mapping |
| `EffectiveInterestMethod` | `SEFFMETH` | `SEFFMETH` |  | `String(1)` |  | Effect. Int. Method |  |  | S/4 only entity — no ECC CDC mapping |
| `LetterOfCredit` | `FTR_LC_NUMBER` | `FTR_LC_NUMBER` |  | `String(16)` |  | Letter of Credit No. |  |  | S/4 only entity — no ECC CDC mapping |
| `TreasuryApplicant` | `FTR_APPLICANT` | `FTR_APPLICANT` |  | `String(10)` |  | Applicant |  |  | S/4 only entity — no ECC CDC mapping |
| `TreasuryBeneficiary` | `FTR_BENEFICIARY` | `FTR_BENEFICIARY` |  | `String(10)` |  | Beneficiary |  |  | S/4 only entity — no ECC CDC mapping |
| `TrsyMnllyEnteredBnfcyName` | `FTR_MAN_BENE_NAME` | `FTR_MAN_BENE_NAME` |  | `String(25)` |  | Benefic. Name (Man.) |  |  | S/4 only entity — no ECC CDC mapping |
| `TrsyMnllyEnteredApplcntName` | `FTR_MAN_APPL_NAME` | `FTR_MAN_APPL_NAME` |  | `String(25)` |  | ApplicantName (Man.) |  |  | S/4 only entity — no ECC CDC mapping |
| `TreasuryAdvisingBank` | `FTR_ADVISING_BANK` | `FTR_ADVISING_BANK` |  | `String(10)` |  | Advising Bank |  |  | S/4 only entity — no ECC CDC mapping |
| `TreasuryIssuingBank` | `FTR_ISSUE_BANK` | `FTR_ISSUE_BANK` |  | `String(10)` |  | Issuing Bank |  |  | S/4 only entity — no ECC CDC mapping |
| `BankGuaranteeNumber` | `FTR_BG_NUMBER` | `FTR_BG_NUMBER` |  | `String(16)` |  | Bank Guarantee No. |  |  | S/4 only entity — no ECC CDC mapping |
| `BankGuaranteeType` | `FTR_BG_TYPE` | `FTR_BG_TYPE` |  | `String(4)` |  | Bank Guarantee Type |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `ForeignExchangeFixingReference`

- **ABAP Name:** `I_FXFixingReference`
- **Label:** Foreign Exchange Fixing Reference
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `ForeignExchangeFixingReference` | `FTR_FIXING_REF_ID` | `FTR_FIXING_REF_ID` |  | `String(30)` | Y | Fixing Reference ID |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `TradeFinanceCategory`

- **ABAP Name:** `I_TradeFinanceCategory`
- **Label:** Trade Finance Category
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `TradeFinanceCategory` | `FTR_TF_CAT` | `FTR_TF_CAT` |  | `String(1)` | Y | Trade Finance Cat. |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `TradeFinanceCategoryText`

- **ABAP Name:** `I_TradeFinanceCategoryText`
- **Label:** Trade Finance Category - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `TradeFinanceCategory` | `FTR_TF_CAT` | `FTR_TF_CAT` |  | `String(1)` | Y | Trade Finance Cat. |  |  | S/4 only entity — no ECC CDC mapping |
| `Language` | `DDLANGUAGE` | `DDLANGUAGE` |  | `String(2)` | Y | Lang. |  |  | S/4 only entity — no ECC CDC mapping |
| `TradeFinanceCategoryName` | `TRADE_FINANCE_CATEGORY_NAME` | `TRADE_FINANCE_CATEGORY_NAME` |  | `String(60)` |  | Category Name |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `TreasuryContractType`

- **ABAP Name:** `I_TreasuryContractType`
- **Label:** Treasury Contract Type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `TreasuryContractType` | `RANTYP` | `RANTYP` |  | `String(1)` | Y | Contract Type |  |  | S/4 only entity — no ECC CDC mapping |
| `DomainValue` | `DOMVALUE_L` | `DOMVALUE_L` |  | `String(10)` |  | Lower Value |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `TreasuryContractTypeText`

- **ABAP Name:** `I_TreasuryContractTypeText`
- **Label:** Treasury Contract Type - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Language` | `SPRAS` | `SPRAS` |  | `String(2)` | Y | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `TreasuryContractType` | `RANTYP` | `RANTYP` |  | `String(1)` | Y | Contract Type |  | _ContractType | S/4 only entity — no ECC CDC mapping |
| `DomainValue` | `DOMVALUE_L` | `DOMVALUE_L` |  | `String(10)` |  | Lower Value |  |  | S/4 only entity — no ECC CDC mapping |
| `TreasuryContractTypeName` | `RANTYP_NAME` | `RANTYP_NAME` |  | `String(60)` |  | Contract Type Name |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `TreasuryPortfolio`

- **ABAP Name:** `I_TreasuryPortfolio`
- **Label:** Portfolio
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `CompanyCode` | `BUKRS` | `BUKRS` |  | `String(4)` | Y | Company Code |  |  | S/4 only entity — no ECC CDC mapping |
| `Portfolio` | `RPORTB` | `RPORTB` |  | `String(10)` | Y | Portfolio |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `TreasuryPortfolioText`

- **ABAP Name:** `I_TreasuryPortfolioText`
- **Label:** Portfolio - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `CompanyCode` | `BUKRS` | `BUKRS` |  | `String(4)` | Y | Company Code |  |  | S/4 only entity — no ECC CDC mapping |
| `Portfolio` | `RPORTB` | `RPORTB` |  | `String(10)` | Y | Portfolio |  | _TreasuryPortfolio | S/4 only entity — no ECC CDC mapping |
| `Language` | `SPRAS` | `SPRAS` |  | `String(2)` | Y | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `PortfolioName` | `FTR_GEN_PORTFOLIO_NAME` | `FTR_GEN_PORTFOLIO_NAME` |  | `String(30)` |  | Portfolio Name |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `TreasuryProductCategory`

- **ABAP Name:** `I_FinancialInstrProdCat`
- **Label:** Product Category
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `FinancialInstrProductCategory` | `SANLF` | `SANLF` |  | `String(3)` | Y | Product Category |  |  | S/4 only entity — no ECC CDC mapping |
| `TreasuryContractType` | `RANTYP` | `RANTYP` |  | `String(1)` |  | Contract Type |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `TreasuryProductCategoryText`

- **ABAP Name:** `I_FinancialInstrProdCatText`
- **Label:** Product Category - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Language` | `SPRAS` | `SPRAS` |  | `String(2)` | Y | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `FinancialInstrProductCategory` | `SANLF` | `SANLF` |  | `String(3)` | Y | Product Category |  | _FinancialInstrProdCat | S/4 only entity — no ECC CDC mapping |
| `FinInstrProductCategoryName` | `TEXT30` | `TEXT30` |  | `String(30)` |  | Text |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `TreasuryReversalReason`

- **ABAP Name:** `I_TreasuryReversalReason`
- **Label:** Treasury Reversal Reason
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `TreasuryReversalReason` | `SSTOGRD` | `SSTOGRD` |  | `String(2)` | Y | Reason for Reversal |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `TreasuryReversalReasonText`

- **ABAP Name:** `I_TreasuryReversalReasonText`
- **Label:** Treasury Reversal Reason - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Language` | `SPRAS` | `SPRAS` |  | `String(2)` | Y | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `TreasuryReversalReason` | `SSTOGRD` | `SSTOGRD` |  | `String(2)` | Y | Reason for Reversal |  | _ReversalReason | S/4 only entity — no ECC CDC mapping |
| `TreasuryReversalReasonName` | `XLANGBEZ` | `XLANGBEZ` |  | `String(60)` |  | Long name |  |  | S/4 only entity — no ECC CDC mapping |
