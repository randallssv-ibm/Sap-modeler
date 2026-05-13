# FinancialTransaction

> Source file: `sap-s4com-FinancialTransaction-v1.json`


## Entity: `FXFixingReferenceText`

- **ABAP Name:** `I_FXFixingReferenceText`
- **Label:** Foreign Exchange Fixing Reference - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `Language` |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity |
| `ForeignExchangeFixingReference` |  |  | `String(30)` | Y | Fixing Reference ID |  | _FixingReference | S/4 only entity |
| `FXFixingReferenceName` |  |  | `String(40)` |  | Fixing Ref. Desc. |  |  | S/4 only entity |


## Entity: `FinInstrActivityCategoryText`

- **ABAP Name:** `I_FinInstrActivityCategoryText`
- **Label:** Fin Instrument Activity Category - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `Language` |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity |
| `FinancialInstrProductCategory` |  |  | `String(3)` | Y | Product Category |  | _ProductCategory | S/4 only entity |
| `FinInstrTransactionCategory` |  |  | `String(3)` | Y | Transaction Category |  | _TransactionCategory | S/4 only entity |
| `FinancialInstrActivityCategory` |  |  | `String(2)` | Y | Activity Category |  | _ActivityCategory | S/4 only entity |
| `FinInstrActivityCategoryName` |  |  | `String(30)` |  | Activity Cat. Name |  |  | S/4 only entity |


## Entity: `FinInstrProductTypeSupplement`

- **ABAP Name:** `I_FinInstrProdTypeSuplmnt`
- **Label:** Product Type Supplements
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `FinancialInstrumentProductType` |  |  | `String(3)` | Y | Product Type |  |  | S/4 only entity |
| `TreasurySettlementType` |  |  | `String(1)` |  | Settlement |  |  | S/4 only entity |
| `OptionExerciseType` |  |  | `String(1)` |  | Exercise Type |  |  | S/4 only entity |
| `TradeFinanceCategory` |  |  | `String(1)` |  | Trade Finance Cat. |  |  | S/4 only entity |
| `OptionUnderlyingProductType` |  |  | `String(3)` |  | UL Product Type |  |  | S/4 only entity |
| `OptionUndrlgTransactionType` |  |  | `String(3)` |  | Underly.Trans.Type |  |  | S/4 only entity |
| `IntrstRateSwapIsCrossCurrency` |  |  | `Boolean` |  | Currency Swap |  |  | S/4 only entity |
| `ProductTypeCashFlowCalculation` |  |  | `String(2)` |  | CF Calculation |  |  | S/4 only entity |


## Entity: `FinInstrProductTypeText`

- **ABAP Name:** `I_FinancialInstrProdTypeText`
- **Label:** Product Type - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `Language` |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity |
| `FinancialInstrumentProductType` |  |  | `String(3)` | Y | Product Type |  | _FinancialInstrProductType | S/4 only entity |
| `FinancialInstrProdTypeName` |  |  | `String(30)` |  | Product Type Name |  |  | S/4 only entity |


## Entity: `FinInstrTransCategoryText`

- **ABAP Name:** `I_FinInstrTransCatText`
- **Label:** Transaction Category - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `Language` |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity |
| `FinancialInstrProductCategory` |  |  | `String(3)` | Y | Product Category |  | _FinancialInstrProdCat | S/4 only entity |
| `FinInstrTransactionCategory` |  |  | `String(3)` | Y | Transaction Category |  |  | S/4 only entity |
| `FinInstrTransCategoryName` |  |  | `String(30)` |  | Trans. Category Name |  |  | S/4 only entity |


## Entity: `FinInstrTransactionCategory`

- **ABAP Name:** `I_FinInstrTransCat`
- **Label:** Transaction Category
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `FinancialInstrProductCategory` |  |  | `String(3)` | Y | Product Category |  | _FinancialInstrProdCat | S/4 only entity |
| `FinInstrTransactionCategory` |  |  | `String(3)` | Y | Transaction Category |  |  | S/4 only entity |


## Entity: `FinInstrTransactionTypeText`

- **ABAP Name:** `I_FinancialInstrTransTypeText`
- **Label:** Transaction Type - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `Language` |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity |
| `FinancialInstrumentProductType` |  |  | `String(3)` | Y | Product Type |  | _Financialinstrproducttype | S/4 only entity |
| `FinancialInstrTransactionType` |  |  | `String(3)` | Y | Transaction Type |  | _FinancialInstrTransType | S/4 only entity |
| `FinancialInstrTransTypeName` |  |  | `String(30)` |  | Trans. Type Name |  |  | S/4 only entity |


## Entity: `FinInstrumentActivityCategory`

- **ABAP Name:** `I_FinInstrActivityCategory`
- **Label:** Financial Instrument Activity Category
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `FinancialInstrProductCategory` |  |  | `String(3)` | Y | Product Category |  | _ProductCategory | S/4 only entity |
| `FinInstrTransactionCategory` |  |  | `String(3)` | Y | Transaction Category |  | _TransactionCategory | S/4 only entity |
| `FinancialInstrActivityCategory` |  |  | `String(2)` | Y | Activity Category |  |  | S/4 only entity |
| `FinTransGenActivityCategory` |  |  | `String(3)` |  | General Activity Category |  |  | S/4 only entity |


## Entity: `FinTransNoticePeriodUnit`

- **ABAP Name:** `I_FinTransNoticePeriodUnit`
- **Label:** Financial Transaction Notice Period Unit
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `FinTransNoticePeriodUnit` |  |  | `String(1)` | Y | Unit |  |  | S/4 only entity |
| `DomainValue` |  |  | `String(10)` |  | Lower Value |  |  | S/4 only entity |


## Entity: `FinTransNoticePeriodUnitText`

- **ABAP Name:** `I_FinTransNoticePeriodUnitText`
- **Label:** Fin Trans Notice Period Unit - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `Language` |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity |
| `FinTransNoticePeriodUnit` |  |  | `String(1)` | Y | Unit |  | _NoticePeriodUnit | S/4 only entity |
| `DomainValue` |  |  | `String(10)` |  | Lower Value |  |  | S/4 only entity |
| `FinTransNoticePeriodUnitName` |  |  | `String(60)` |  | NoticePer. Unit Name |  |  | S/4 only entity |


## Entity: `FinTransOptionExerciseType`

- **ABAP Name:** `I_OptionExerciseType`
- **Label:** Option exercise type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `OptionExerciseType` |  |  | `String(1)` | Y | Exercise Type |  |  | S/4 only entity |


## Entity: `FinTransOptionExerciseTypeText`

- **ABAP Name:** `I_OptionExerciseTypeText`
- **Label:** Option exercise type - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `OptionExerciseType` |  |  | `String(1)` | Y | Exercise Type |  |  | S/4 only entity |
| `Language` |  |  | `String(2)` | Y | Lang. |  |  | S/4 only entity |
| `OptionExerciseTypeName` |  |  | `String(60)` |  | Option Exercise Type |  |  | S/4 only entity |


## Entity: `FinTransOptionSettlementType`

- **ABAP Name:** `I_OptionSettlementType`
- **Label:** Option settlement type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `OptionSettlementType` |  |  | `String(1)` | Y | Settlement Type |  |  | S/4 only entity |


## Entity: `FinTransOptnSettlementTypeText`

- **ABAP Name:** `I_OptionSettlementTypeText`
- **Label:** Option settlement type - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `OptionSettlementType` |  |  | `String(1)` | Y | Settlement Type |  |  | S/4 only entity |
| `Language` |  |  | `String(2)` | Y | Lang. |  |  | S/4 only entity |
| `OptionSettlementTypeName` |  |  | `String(60)` |  | Option Settlemt Type |  |  | S/4 only entity |


## Entity: `FinTransOptnUndrlgAllocation`

- **ABAP Name:** `I_FinTransOptnUndrlgAllocation`
- **Label:** Fin Trans Option Underlying Allocation
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `FinTransOptionNumber` |  |  | `String(13)` | Y | Class |  |  | S/4 only entity |
| `OptionUnderlyingTransaction` |  |  | `String(13)` | Y | Transaction |  |  | S/4 only entity |
| `FinancialTransactionFromExer` |  |  | `String(13)` |  | Exercise Transaction |  |  | S/4 only entity |


## Entity: `FinTransReleaseStatus`

- **ABAP Name:** `I_FinTransReleaseStatus`
- **Label:** Financial Transaction Release Status
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `FinTransReleaseStatus` |  |  | `String(1)` | Y | Release Status |  |  | S/4 only entity |
| `DomainValue` |  |  | `String(10)` |  | Lower Value |  |  | S/4 only entity |


## Entity: `FinTransReleaseStatusText`

- **ABAP Name:** `I_FinTransReleaseStatusText`
- **Label:** Fin Transaction Release Status - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `Language` |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity |
| `FinTransReleaseStatus` |  |  | `String(1)` | Y | Release Status |  | _ReleaseStatus | S/4 only entity |
| `DomainValue` |  |  | `String(10)` |  | Lower Value |  |  | S/4 only entity |
| `FinTransReleaseStatusName` |  |  | `String(60)` |  | Release Status Name |  |  | S/4 only entity |


## Entity: `FinTransUnderlyingFlow`

- **ABAP Name:** `I_FinTransUnderlyingFlow`
- **Label:** Fin Transaction Underlying Flow
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `OptionUnderlyingTransaction` |  |  | `String(13)` | Y | Transaction |  |  | S/4 only entity |
| `FinancialInstrumentActivity` |  |  | `String(5)` | Y | Activity |  |  | S/4 only entity |
| `FinTransFlowCreationDate` |  |  | `Date` | Y | Entered On |  |  | S/4 only entity |
| `FinTransFlowCreationTime` |  |  | `String(6)` | Y | Entry Time |  |  | S/4 only entity |
| `FinTransFlowNumber` |  |  | `String(4)` | Y | Flow |  |  | S/4 only entity |
| `CreatedByUser` |  |  | `String(12)` |  | Entered By |  |  | S/4 only entity |
| `FinTransCreationDate` |  |  | `Date` |  | Created On |  |  | S/4 only entity |
| `FinTransCreationTime` |  |  | `String(6)` |  | Entry Time |  |  | S/4 only entity |
| `LastChangedByUser` |  |  | `String(12)` |  | Last Changed By |  |  | S/4 only entity |
| `LastChangeDate` |  |  | `Date` |  | Changed On |  |  | S/4 only entity |
| `FinInstrumentLastChangedTime` |  |  | `String(6)` |  | Time Changed |  |  | S/4 only entity |
| `TreasuryContractType` |  |  | `String(1)` |  | Contract Type |  |  | S/4 only entity |
| `FinTransFlowType` |  |  | `String(4)` |  | Flow Type |  |  | S/4 only entity |
| `FinTransFlowCategory` |  |  | `String(2)` |  | Flow Category |  |  | S/4 only entity |
| `FinTransFlowPaytAmtDirection` |  |  | `String(1)` |  | Direction |  |  | S/4 only entity |
| `FinancialTransactionDirection` |  |  | `String(1)` |  | Direction |  |  | S/4 only entity |
| `FinTransFlowSource` |  |  | `String(4)` |  | Source |  |  | S/4 only entity |
| `PayerPayee` |  |  | `String(10)` |  | Payer/Payee |  |  | S/4 only entity |
| `FinTransFlowPaymentDate` |  |  | `Date` |  | Payment Date |  |  | S/4 only entity |
| `FinTransFlowPaytAmt` |  |  | `Decimal(34,4)` |  | Payment Amnt in PyC | FinTransFlowPaytAmtCrcy |  | S/4 only entity |
| `FinTransFlowPaytAmtCrcy` |  |  | `String(5)` |  | Payment Currency |  |  | S/4 only entity |
| `FinTransFlowInLoclCrcyPaytAmt` |  |  | `Decimal(34,4)` |  | Pmnt Amnt in LCurr | FinTransFlowPaytAmtCrcy |  | S/4 only entity |
| `FinTransFlowLoclCrcyCnvrsnRate` |  |  | `Decimal(9,5)` |  | Crcy Cnvrsn Rate |  |  | S/4 only entity |
| `CalculationDate` |  |  | `Date` |  | Calculation Date |  |  | S/4 only entity |
| `CalculationPeriodStartDate` |  |  | `Date` |  | Calculation From |  |  | S/4 only entity |
| `CalculationPeriodEndDate` |  |  | `Date` |  | Calculation To |  |  | S/4 only entity |
| `CalcPeriodEndDateIsInclusive` |  |  | `String(1)` |  | Inclusive End Date |  |  | S/4 only entity |
| `CalcPeriodStartDateIsExclusive` |  |  | `String(1)` |  | Exclusive Start Date |  |  | S/4 only entity |
| `CalcPeriodEndDateIsMonthEnd` |  |  | `Boolean` |  | Month-End End Date |  |  | S/4 only entity |
| `CalcPeriodStartDateIsMonthEnd` |  |  | `Boolean` |  | Month-End Start Date |  |  | S/4 only entity |
| `NumberOfCalculationDays` |  |  | `String(6)` |  | Number of Days |  |  | S/4 only entity |
| `NrOfBaseDaysPerCalcPeriod` |  |  | `String(6)` |  | No. of base days |  |  | S/4 only entity |
| `InterestCalculationMethod` |  |  | `String(1)` |  | Int. Calc. Method |  |  | S/4 only entity |
| `FinTransFlowCalcBaseAmount` |  |  | `Decimal(34,4)` |  | Base Amount | FinTransFlowCalcBaseAmountCrcy |  | S/4 only entity |
| `FinTransFlowCalcBaseAmountCrcy` |  |  | `String(5)` |  | Calculatn Basis Crcy |  |  | S/4 only entity |
| `IntrstCalcMethFactoryCalendar` |  |  | `String(2)` |  | Interest Calendar |  |  | S/4 only entity |
| `InterestBaseDaysMethod` |  |  | `String(1)` |  | Base Days Method |  |  | S/4 only entity |
| `InterestCalculationType` |  |  | `String(1)` |  | Int. Calc. Type |  |  | S/4 only entity |
| `ConditionPercentageRate` |  |  | `Decimal(10,7)` |  | Percentage Rate |  |  | S/4 only entity |
| `FinCndnPctgRateFixingDate` |  |  | `Date` |  | PercFixingDte |  |  | S/4 only entity |
| `FinTransFlowIntrstRateFixDate` |  |  | `Date` |  | Int.Rate Fixing Date |  |  | S/4 only entity |
| `FinTransPositionValueDate` |  |  | `Date` |  | Position Value Date |  |  | S/4 only entity |
| `FinTransFlowPositionAmount` |  |  | `Decimal(34,4)` |  | PositionAmount | FinTransFlwPosAmtCrcy |  | S/4 only entity |
| `FinTransFlwPosAmtCrcy` |  |  | `String(5)` |  | Position Currency |  |  | S/4 only entity |
| `FinTransFlowNomAmt` |  |  | `Decimal(34,4)` |  | Nominal Amount | FinTransFlowNomAmtCrcy |  | S/4 only entity |
| `FinTransFlowNomAmtCrcy` |  |  | `String(5)` |  | Nominal Amount Currency |  |  | S/4 only entity |
| `MarketValueInQtanCurrency` |  |  | `Decimal(34,4)` |  | Mkt Val. in QC | QuotationCurrency |  | S/4 only entity |
| `QuotationCurrency` |  |  | `String(5)` |  | Price Currency |  |  | S/4 only entity |
| `FinTransTradedNumberOfUnits` |  |  | `Decimal(24,14)` |  | Number of Units |  |  | S/4 only entity |
| `FinTransTrdPriceCrcyUnitRate` |  |  | `Decimal(23,14)` |  | Price (Unit-Quoted) |  |  | S/4 only entity |
| `FinTransTradedPriceCrcyUnit` |  |  | `String(5)` |  | Currency Unit |  |  | S/4 only entity |
| `SecurityExchange` |  |  | `String(10)` |  | Exchange |  |  | S/4 only entity |
| `FinConditionItem` |  |  | `String(4)` |  | Condition |  |  | S/4 only entity |
| `ConditionItemValidityStartDate` |  |  | `Date` |  | Item Effective From |  |  | S/4 only entity |
| `FinConditionSubItem` |  |  | `String(2)` |  | Level Number |  |  | S/4 only entity |
| `InterestConditionType` |  |  | `String(4)` |  | Condition Type |  |  | S/4 only entity |
| `FinInstrConditionLogicGroup` |  |  | `String(4)` |  | Condition Group |  |  | S/4 only entity |
| `FinCndnCrsRefcdAccmlnCndnGrp` |  |  | `String(4)` |  | Accum. Cond.Grp |  |  | S/4 only entity |
| `FinTransFlwReltdAccumulatingID` |  |  | `String(40)` |  | Rel.AccumFlowID |  |  | S/4 only entity |
| `FinTransFlowAccumulatingFlowID` |  |  | `String(40)` |  | Accum. Flow ID |  |  | S/4 only entity |
| `FinTransTradedPricePercent` |  |  | `Decimal(23,14)` |  | Price (%) |  |  | S/4 only entity |


## Entity: `FinancialInstrTransactionType`

- **ABAP Name:** `I_FinancialInstrTransType`
- **Label:** Transaction Type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `FinancialInstrTransactionType` |  |  | `String(3)` | Y | Transaction Type |  |  | S/4 only entity |
| `FinancialInstrumentProductType` |  |  | `String(3)` | Y | Product Type |  | _FinancialInstrProductType | S/4 only entity |
| `FinInstrTransactionCategory` |  |  | `String(3)` |  | Transaction Category |  |  | S/4 only entity |
| `TreasuryContractType` |  |  | `String(1)` |  | Contract Type |  |  | S/4 only entity |


## Entity: `FinancialInstrumentProductType`

- **ABAP Name:** `I_FinancialinstrProductType`
- **Label:** Product Type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `FinancialInstrumentProductType` |  |  | `String(3)` | Y | Product Type |  |  | S/4 only entity |
| `TreasuryContractType` |  |  | `String(1)` |  | Contract Type |  |  | S/4 only entity |
| `FinancialInstrProductCategory` |  |  | `String(3)` |  | Product Category |  |  | S/4 only entity |
| `FinCndnTypeAllocCndnGroup` |  |  | `String(3)` |  | Condition Group |  |  | S/4 only entity |


## Entity: `FinancialInstrumentStatus`

- **ABAP Name:** `I_FinInstrumentStatus`
- **Label:** Financial Instrument Status
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `FinancialInstrumentStatus` |  |  | `String(1)` | Y | Active Status |  |  | S/4 only entity |
| `DomainValue` |  |  | `String(10)` |  | Lower Value |  |  | S/4 only entity |


## Entity: `FinancialInstrumentStatusText`

- **ABAP Name:** `I_FinInstrumentStatusText`
- **Label:** Financial Instrument Status - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `Language` |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity |
| `FinancialInstrumentStatus` |  |  | `String(1)` | Y | Active Status |  | _Status | S/4 only entity |
| `DomainValue` |  |  | `String(10)` |  | Lower Value |  |  | S/4 only entity |
| `FinancialInstrumentStatusName` |  |  | `String(60)` |  | Active Status Name |  |  | S/4 only entity |


## Entity: `FinancialTransaction`

- **ABAP Name:** `I_FinancialTransactionDEX`
- **Label:** Financial Transaction
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `CompanyCode` | `T001` | `BUKRS` | `String(4)` | Y | Company Code |  |  |  |
| `FinancialTransaction` |  |  | `String(13)` | Y | Transaction |  |  | S/4 only entity |
| `FinTransCreationDate` |  |  | `Date` |  | Created On |  |  | S/4 only entity |
| `FinTransCreationTime` |  |  | `String(6)` |  | Entry Time |  |  | S/4 only entity |
| `LastChangeDate` |  |  | `Date` |  | Changed On |  |  | S/4 only entity |
| `FinInstrumentLastChangedTime` |  |  | `String(6)` |  | Time Changed |  |  | S/4 only entity |
| `TreasuryContractType` |  |  | `String(1)` |  | Contract Type |  | _ContractType | S/4 only entity |
| `FinancialInstrProductCategory` |  |  | `String(3)` |  | Product Category |  | _FinancialInstrProdCat | S/4 only entity |
| `FinancialInstrumentProductType` |  |  | `String(3)` |  | Product Type |  | _FinancialInstrProdType | S/4 only entity |
| `FinInstrTransactionCategory` |  |  | `String(3)` |  | Transaction Category |  | _FinInstrTransCat | S/4 only entity |
| `FinancialInstrTransactionType` |  |  | `String(3)` |  | Transaction Type |  | _FinancialInstrTransType | S/4 only entity |
| `TermStartDate` |  |  | `Date` |  | Term Start |  |  | S/4 only entity |
| `FinTransNoticePeriod` |  |  | `String(3)` |  | Period of Notice |  |  | S/4 only entity |
| `FinTransNoticePeriodUnit` |  |  | `String(1)` |  | Unit |  | _NoticePeriodUnit | S/4 only entity |
| `FinTransFactoryCalendar1` |  |  | `String(2)` |  | Calendar |  |  | S/4 only entity |
| `FinTransFactoryCalendar2` |  |  | `String(2)` |  | Calendar |  |  | S/4 only entity |
| `Counterparty` |  |  | `String(10)` |  | Counterparty |  |  | S/4 only entity |
| `FinancialInstrumentGuarantor` |  |  | `String(10)` |  | Guarantor |  |  | S/4 only entity |
| `Portfolio` |  |  | `String(10)` |  | Portfolio |  | _Portfolio | S/4 only entity |
| `TreasuryFinanceProject` |  |  | `String(13)` |  | Finance Project |  |  | S/4 only entity |
| `FinancialInstrumentAssignment` |  |  | `String(18)` |  | Free Assignment |  |  | S/4 only entity |
| `FinancialInstrumentReference` |  |  | `String(16)` |  | Free Internal Ref. |  |  | S/4 only entity |
| `FinancialInstrCharacteristic` |  |  | `String(25)` |  | Free Charact. |  |  | S/4 only entity |
| `ControllingArea` | `TKA01` | `KOKRS` | `String(4)` |  | Controlling Area |  |  |  |
| `CostCenter` |  |  | `String(10)` |  | Cost Center |  |  | S/4 only entity |
| `HedgingClassification` |  |  | `String(5)` |  | Hedging Classificatn |  |  | S/4 only entity |
| `HedgeRequestIdentifier` |  |  | `String(13)` |  | Hedge Request ID |  |  | S/4 only entity |
| `ProfitCenter` |  |  | `String(10)` |  | Profit Center |  |  | S/4 only entity |
| `WBSElementInternalID` |  |  | `String(8)` |  | WBS Internal ID |  |  | S/4 only entity |
| `TreasuryFacilityCompanyCode` |  |  | `String(4)` |  | CoCd of Facility |  |  | S/4 only entity |
| `TreasuryFacility` |  |  | `String(13)` |  | Facility |  |  | S/4 only entity |
| `FinancialInstrumentStatus` |  |  | `String(1)` |  | Active Status |  | _Status | S/4 only entity |
| `FinTransReleaseStatus` |  |  | `String(1)` |  | Release Status |  | _ReleaseStatus | S/4 only entity |
| `TransactionCurrency` |  |  | `String(5)` |  | Transaction Currency |  |  | S/4 only entity |
| `FinInstrumentOutgoingCurrency` |  |  | `String(5)` |  | Outgoing Currency |  |  | S/4 only entity |
| `FinInstrumentIncomingCurrency` |  |  | `String(5)` |  | Incoming Currency |  |  | S/4 only entity |
| `TradedCurrency` |  |  | `String(5)` |  | Traded Currency |  |  | S/4 only entity |
| `SecurityClass` |  |  | `String(13)` |  | Security Class |  |  | S/4 only entity |
| `ClassificationOfFinInstr` |  |  | `String(6)` |  | CFI Code |  |  | S/4 only entity |
| `SecurityAccount` |  |  | `String(10)` |  | Securities Account |  |  | S/4 only entity |
| `FinTransIsRiskMitigating` |  |  | `Boolean` |  | Risk Mitigation |  |  | S/4 only entity |
| `FinInstrLastActiveActivity` |  |  | `String(5)` |  | Last Active Activity |  |  | S/4 only entity |
| `TrsyTradedAmountBuySellCode` |  |  | `String(1)` |  | Buy/Sell |  |  | S/4 only entity |
| `Segment` |  |  | `String(10)` |  | Segment |  |  | S/4 only entity |
| `OnBehalfOfCompany` |  |  | `String(4)` |  | On Behalf of CoCode |  |  | S/4 only entity |
| `MarketIdentifierCode` |  |  | `String(4)` |  | MIC |  |  | S/4 only entity |
| `FinTransRoundingCategory` |  |  | `String(1)` |  | Round |  |  | S/4 only entity |
| `FinTransGeneralValuationClass` |  |  | `String(4)` |  | Gen. Valn Class |  |  | S/4 only entity |
| `Fund` |  |  | `String(10)` |  | Fund |  |  | S/4 only entity |
| `GrantID` |  |  | `String(20)` |  | Grant |  |  | S/4 only entity |
| `FinTransAuthorizationGroup` |  |  | `String(4)` |  | Authorization Group |  |  | S/4 only entity |
| `BusinessPlace` |  |  | `String(4)` |  | Business Place |  |  | S/4 only entity |
| `FunctionalArea` |  |  | `String(16)` |  | Functional Area |  |  | S/4 only entity |
| `TrsyPosCustomDiffntnTerm1` |  |  | `String(20)` |  | Cust.Diff.Term Val. |  |  | S/4 only entity |
| `TrsyPosCustomDiffntnTerm2` |  |  | `String(20)` |  | Cust.Diff.Term Val. |  |  | S/4 only entity |
| `TrsyPosCustomDiffntnTerm3` |  |  | `String(20)` |  | Cust.Diff.Term Val. |  |  | S/4 only entity |
| `TrsyPosCustomDiffntnTerm4` |  |  | `String(20)` |  | Cust.Diff.Term Val. |  |  | S/4 only entity |
| `TrsyPosCustomDiffntnTerm5` |  |  | `String(20)` |  | Cust.Diff.Term Val. |  |  | S/4 only entity |
| `UniqueProductIdentifier` |  |  | `String(12)` |  | Unique Product ID |  |  | S/4 only entity |
| `InternationalSecuritiesIdnNmbr` |  |  | `String(12)` |  | Security ID (ISIN) |  |  | S/4 only entity |
| `ReportTrackingNumber` |  |  | `String(52)` |  | Report Tracking No. |  |  | S/4 only entity |
| `FinTransOptionNumber` |  |  | `String(13)` |  | Class |  |  | S/4 only entity |
| `FinancialInstrActivityCategory` |  |  | `String(2)` |  | Activity Category |  | _ActivityCategory | S/4 only entity |
| `TermEndDate` |  |  | `Date` |  | Term End |  |  | S/4 only entity |
| `FinTransTermCategory` |  |  | `String(1)` |  | Term Category |  |  | S/4 only entity |
| `FinTransTermStartEndInclusive` |  |  | `String(1)` |  | Term Start and End Inclusive |  |  | S/4 only entity |
| `FinTransNoticeDate` |  |  | `Date` |  | Notice Date |  |  | S/4 only entity |
| `FinTransActyConclusionDate` |  |  | `Date` |  | Conclusion Date |  |  | S/4 only entity |
| `FinTransActyConclusionTime` |  |  | `String(6)` |  | Contract.Concl.Time |  |  | S/4 only entity |
| `FinTransActyConclusionTimeZone` |  |  | `String(6)` |  | Time Zone Contr.Date |  |  | S/4 only entity |
| `FinTransRolloverDate` |  |  | `Date` |  | Term Start |  |  | S/4 only entity |
| `FinTransExerciseDate` |  |  | `Date` |  | Term End |  |  | S/4 only entity |
| `FinTransOrderValidityEndDate` |  |  | `Date` |  | Limit Date |  |  | S/4 only entity |
| `FinTransFixingDate` |  |  | `Date` |  | Fixing Date |  |  | S/4 only entity |
| `ForeignExchangeFixingReference` |  |  | `String(30)` |  | Fixing Reference ID |  | _FixingReference | S/4 only entity |
| `Trader` |  |  | `String(12)` |  | Trader |  |  | S/4 only entity |
| `FinancialInstrContactPerson` |  |  | `String(19)` |  | Contact Person |  |  | S/4 only entity |
| `FinInstrExternalReference` |  |  | `String(16)` |  | External Reference |  |  | S/4 only entity |
| `TreasuryReversalReason` |  |  | `String(2)` |  | Reason for Reversal |  | _ReversalReason | S/4 only entity |
| `LeadingCurrency` |  |  | `String(5)` |  | Leading Currency |  |  | S/4 only entity |
| `FollowingCurrency` |  |  | `String(5)` |  | Following Currency |  |  | S/4 only entity |
| `ExchangeRate` |  |  | `Decimal(13,9)` |  | Transaction Rate |  |  | S/4 only entity |
| `SpotExchangeRate` |  |  | `Decimal(13,9)` |  | Spot Rate |  |  | S/4 only entity |
| `SwapExchangeRate` |  |  | `Decimal(13,9)` |  | Swap Rate |  |  | S/4 only entity |
| `LiquidityEffectValue` |  |  | `Decimal(13,9)` |  | Liquidity Effect |  |  | S/4 only entity |
| `CurrencyPair` |  |  | `String(20)` |  | Currency Pair |  |  | S/4 only entity |
| `EffectiveInterestRate` |  |  | `Decimal(10,7)` |  | Effect.Interest Rate |  |  | S/4 only entity |
| `EffectiveInterestMethod` |  |  | `String(1)` |  | Effect. Int. Method |  |  | S/4 only entity |
| `LetterOfCredit` |  |  | `String(16)` |  | Letter of Credit No. |  |  | S/4 only entity |
| `TreasuryApplicant` |  |  | `String(10)` |  | Applicant |  |  | S/4 only entity |
| `TreasuryBeneficiary` |  |  | `String(10)` |  | Beneficiary |  |  | S/4 only entity |
| `TrsyMnllyEnteredBnfcyName` |  |  | `String(25)` |  | Benefic. Name (Man.) |  |  | S/4 only entity |
| `TrsyMnllyEnteredApplcntName` |  |  | `String(25)` |  | ApplicantName (Man.) |  |  | S/4 only entity |
| `TreasuryAdvisingBank` |  |  | `String(10)` |  | Advising Bank |  |  | S/4 only entity |
| `TreasuryIssuingBank` |  |  | `String(10)` |  | Issuing Bank |  |  | S/4 only entity |
| `BankGuaranteeNumber` |  |  | `String(16)` |  | Bank Guarantee No. |  |  | S/4 only entity |
| `BankGuaranteeType` |  |  | `String(4)` |  | Bank Guarantee Type |  |  | S/4 only entity |


## Entity: `ForeignExchangeFixingReference`

- **ABAP Name:** `I_FXFixingReference`
- **Label:** Foreign Exchange Fixing Reference
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `ForeignExchangeFixingReference` |  |  | `String(30)` | Y | Fixing Reference ID |  |  | S/4 only entity |


## Entity: `TradeFinanceCategory`

- **ABAP Name:** `I_TradeFinanceCategory`
- **Label:** Trade Finance Category
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `TradeFinanceCategory` |  |  | `String(1)` | Y | Trade Finance Cat. |  |  | S/4 only entity |


## Entity: `TradeFinanceCategoryText`

- **ABAP Name:** `I_TradeFinanceCategoryText`
- **Label:** Trade Finance Category - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `TradeFinanceCategory` |  |  | `String(1)` | Y | Trade Finance Cat. |  |  | S/4 only entity |
| `Language` |  |  | `String(2)` | Y | Lang. |  |  | S/4 only entity |
| `TradeFinanceCategoryName` |  |  | `String(60)` |  | Category Name |  |  | S/4 only entity |


## Entity: `TreasuryContractType`

- **ABAP Name:** `I_TreasuryContractType`
- **Label:** Treasury Contract Type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `TreasuryContractType` |  |  | `String(1)` | Y | Contract Type |  |  | S/4 only entity |
| `DomainValue` |  |  | `String(10)` |  | Lower Value |  |  | S/4 only entity |


## Entity: `TreasuryContractTypeText`

- **ABAP Name:** `I_TreasuryContractTypeText`
- **Label:** Treasury Contract Type - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `Language` |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity |
| `TreasuryContractType` |  |  | `String(1)` | Y | Contract Type |  | _ContractType | S/4 only entity |
| `DomainValue` |  |  | `String(10)` |  | Lower Value |  |  | S/4 only entity |
| `TreasuryContractTypeName` |  |  | `String(60)` |  | Contract Type Name |  |  | S/4 only entity |


## Entity: `TreasuryPortfolio`

- **ABAP Name:** `I_TreasuryPortfolio`
- **Label:** Portfolio
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `CompanyCode` | `T001` | `BUKRS` | `String(4)` | Y | Company Code |  |  |  |
| `Portfolio` |  |  | `String(10)` | Y | Portfolio |  |  | S/4 only entity |


## Entity: `TreasuryPortfolioText`

- **ABAP Name:** `I_TreasuryPortfolioText`
- **Label:** Portfolio - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `CompanyCode` | `T001` | `BUKRS` | `String(4)` | Y | Company Code |  |  |  |
| `Portfolio` |  |  | `String(10)` | Y | Portfolio |  | _TreasuryPortfolio | S/4 only entity |
| `Language` |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity |
| `PortfolioName` |  |  | `String(30)` |  | Portfolio Name |  |  | S/4 only entity |


## Entity: `TreasuryProductCategory`

- **ABAP Name:** `I_FinancialInstrProdCat`
- **Label:** Product Category
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `FinancialInstrProductCategory` |  |  | `String(3)` | Y | Product Category |  |  | S/4 only entity |
| `TreasuryContractType` |  |  | `String(1)` |  | Contract Type |  |  | S/4 only entity |


## Entity: `TreasuryProductCategoryText`

- **ABAP Name:** `I_FinancialInstrProdCatText`
- **Label:** Product Category - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `Language` |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity |
| `FinancialInstrProductCategory` |  |  | `String(3)` | Y | Product Category |  | _FinancialInstrProdCat | S/4 only entity |
| `FinInstrProductCategoryName` |  |  | `String(30)` |  | Text |  |  | S/4 only entity |


## Entity: `TreasuryReversalReason`

- **ABAP Name:** `I_TreasuryReversalReason`
- **Label:** Treasury Reversal Reason
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `TreasuryReversalReason` |  |  | `String(2)` | Y | Reason for Reversal |  |  | S/4 only entity |


## Entity: `TreasuryReversalReasonText`

- **ABAP Name:** `I_TreasuryReversalReasonText`
- **Label:** Treasury Reversal Reason - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `Language` |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity |
| `TreasuryReversalReason` |  |  | `String(2)` | Y | Reason for Reversal |  | _ReversalReason | S/4 only entity |
| `TreasuryReversalReasonName` |  |  | `String(60)` |  | Long name |  |  | S/4 only entity |
