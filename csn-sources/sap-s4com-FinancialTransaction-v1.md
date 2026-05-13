# FinancialTransaction

> Source file: `sap-s4com-FinancialTransaction-v1.json`


## Entity: `FXFixingReferenceText`

- **ABAP Name:** `I_FXFixingReferenceText`
- **Label:** Foreign Exchange Fixing Reference - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `ForeignExchangeFixingReference` | `ForeignExchangeFixingReference` | `String(30)` | Y | Fixing Reference ID |  | _FixingReference | S/4 only entity (no ECC CDC mapping) |
| `FXFixingReferenceName` | `FXFixingReferenceName` | `String(40)` |  | Fixing Ref. Desc. |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `FinInstrActivityCategoryText`

- **ABAP Name:** `I_FinInstrActivityCategoryText`
- **Label:** Fin Instrument Activity Category - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinancialInstrProductCategory` | `FinancialInstrProductCategory` | `String(3)` | Y | Product Category |  | _ProductCategory | S/4 only entity (no ECC CDC mapping) |
| `FinInstrTransactionCategory` | `FinInstrTransactionCategory` | `String(3)` | Y | Transaction Category |  | _TransactionCategory | S/4 only entity (no ECC CDC mapping) |
| `FinancialInstrActivityCategory` | `FinancialInstrActivityCategory` | `String(2)` | Y | Activity Category |  | _ActivityCategory | S/4 only entity (no ECC CDC mapping) |
| `FinInstrActivityCategoryName` | `FinInstrActivityCategoryName` | `String(30)` |  | Activity Cat. Name |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `FinInstrProductTypeSupplement`

- **ABAP Name:** `I_FinInstrProdTypeSuplmnt`
- **Label:** Product Type Supplements
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `FinancialInstrumentProductType` | `FinancialInstrumentProductType` | `String(3)` | Y | Product Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `TreasurySettlementType` | `TreasurySettlementType` | `String(1)` |  | Settlement |  |  | S/4 only entity (no ECC CDC mapping) |
| `OptionExerciseType` | `OptionExerciseType` | `String(1)` |  | Exercise Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `TradeFinanceCategory` | `TradeFinanceCategory` | `String(1)` |  | Trade Finance Cat. |  |  | S/4 only entity (no ECC CDC mapping) |
| `OptionUnderlyingProductType` | `OptionUnderlyingProductType` | `String(3)` |  | UL Product Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `OptionUndrlgTransactionType` | `OptionUndrlgTransactionType` | `String(3)` |  | Underly.Trans.Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `IntrstRateSwapIsCrossCurrency` | `IntrstRateSwapIsCrossCurrency` | `Boolean` |  | Currency Swap |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProductTypeCashFlowCalculation` | `ProductTypeCashFlowCalculation` | `String(2)` |  | CF Calculation |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `FinInstrProductTypeText`

- **ABAP Name:** `I_FinancialInstrProdTypeText`
- **Label:** Product Type - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinancialInstrumentProductType` | `FinancialInstrumentProductType` | `String(3)` | Y | Product Type |  | _FinancialInstrProductType | S/4 only entity (no ECC CDC mapping) |
| `FinancialInstrProdTypeName` | `FinancialInstrProdTypeName` | `String(30)` |  | Product Type Name |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `FinInstrTransCategoryText`

- **ABAP Name:** `I_FinInstrTransCatText`
- **Label:** Transaction Category - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinancialInstrProductCategory` | `FinancialInstrProductCategory` | `String(3)` | Y | Product Category |  | _FinancialInstrProdCat | S/4 only entity (no ECC CDC mapping) |
| `FinInstrTransactionCategory` | `FinInstrTransactionCategory` | `String(3)` | Y | Transaction Category |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinInstrTransCategoryName` | `FinInstrTransCategoryName` | `String(30)` |  | Trans. Category Name |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `FinInstrTransactionCategory`

- **ABAP Name:** `I_FinInstrTransCat`
- **Label:** Transaction Category
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `FinancialInstrProductCategory` | `FinancialInstrProductCategory` | `String(3)` | Y | Product Category |  | _FinancialInstrProdCat | S/4 only entity (no ECC CDC mapping) |
| `FinInstrTransactionCategory` | `FinInstrTransactionCategory` | `String(3)` | Y | Transaction Category |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `FinInstrTransactionTypeText`

- **ABAP Name:** `I_FinancialInstrTransTypeText`
- **Label:** Transaction Type - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinancialInstrumentProductType` | `FinancialInstrumentProductType` | `String(3)` | Y | Product Type |  | _Financialinstrproducttype | S/4 only entity (no ECC CDC mapping) |
| `FinancialInstrTransactionType` | `FinancialInstrTransactionType` | `String(3)` | Y | Transaction Type |  | _FinancialInstrTransType | S/4 only entity (no ECC CDC mapping) |
| `FinancialInstrTransTypeName` | `FinancialInstrTransTypeName` | `String(30)` |  | Trans. Type Name |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `FinInstrumentActivityCategory`

- **ABAP Name:** `I_FinInstrActivityCategory`
- **Label:** Financial Instrument Activity Category
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `FinancialInstrProductCategory` | `FinancialInstrProductCategory` | `String(3)` | Y | Product Category |  | _ProductCategory | S/4 only entity (no ECC CDC mapping) |
| `FinInstrTransactionCategory` | `FinInstrTransactionCategory` | `String(3)` | Y | Transaction Category |  | _TransactionCategory | S/4 only entity (no ECC CDC mapping) |
| `FinancialInstrActivityCategory` | `FinancialInstrActivityCategory` | `String(2)` | Y | Activity Category |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransGenActivityCategory` | `FinTransGenActivityCategory` | `String(3)` |  | General Activity Category |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `FinTransNoticePeriodUnit`

- **ABAP Name:** `I_FinTransNoticePeriodUnit`
- **Label:** Financial Transaction Notice Period Unit
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `FinTransNoticePeriodUnit` | `FinTransNoticePeriodUnit` | `String(1)` | Y | Unit |  |  | S/4 only entity (no ECC CDC mapping) |
| `DomainValue` | `DomainValue` | `String(10)` |  | Lower Value |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `FinTransNoticePeriodUnitText`

- **ABAP Name:** `I_FinTransNoticePeriodUnitText`
- **Label:** Fin Trans Notice Period Unit - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransNoticePeriodUnit` | `FinTransNoticePeriodUnit` | `String(1)` | Y | Unit |  | _NoticePeriodUnit | S/4 only entity (no ECC CDC mapping) |
| `DomainValue` | `DomainValue` | `String(10)` |  | Lower Value |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransNoticePeriodUnitName` | `FinTransNoticePeriodUnitName` | `String(60)` |  | NoticePer. Unit Name |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `FinTransOptionExerciseType`

- **ABAP Name:** `I_OptionExerciseType`
- **Label:** Option exercise type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `OptionExerciseType` | `OptionExerciseType` | `String(1)` | Y | Exercise Type |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `FinTransOptionExerciseTypeText`

- **ABAP Name:** `I_OptionExerciseTypeText`
- **Label:** Option exercise type - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `OptionExerciseType` | `OptionExerciseType` | `String(1)` | Y | Exercise Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `Language` | `Language` | `String(2)` | Y | Lang. |  |  | S/4 only entity (no ECC CDC mapping) |
| `OptionExerciseTypeName` | `OptionExerciseTypeName` | `String(60)` |  | Option Exercise Type |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `FinTransOptionSettlementType`

- **ABAP Name:** `I_OptionSettlementType`
- **Label:** Option settlement type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `OptionSettlementType` | `OptionSettlementType` | `String(1)` | Y | Settlement Type |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `FinTransOptnSettlementTypeText`

- **ABAP Name:** `I_OptionSettlementTypeText`
- **Label:** Option settlement type - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `OptionSettlementType` | `OptionSettlementType` | `String(1)` | Y | Settlement Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `Language` | `Language` | `String(2)` | Y | Lang. |  |  | S/4 only entity (no ECC CDC mapping) |
| `OptionSettlementTypeName` | `OptionSettlementTypeName` | `String(60)` |  | Option Settlemt Type |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `FinTransOptnUndrlgAllocation`

- **ABAP Name:** `I_FinTransOptnUndrlgAllocation`
- **Label:** Fin Trans Option Underlying Allocation
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `FinTransOptionNumber` | `FinTransOptionNumber` | `String(13)` | Y | Class |  |  | S/4 only entity (no ECC CDC mapping) |
| `OptionUnderlyingTransaction` | `OptionUnderlyingTransaction` | `String(13)` | Y | Transaction |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinancialTransactionFromExer` | `FinancialTransactionFromExer` | `String(13)` |  | Exercise Transaction |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `FinTransReleaseStatus`

- **ABAP Name:** `I_FinTransReleaseStatus`
- **Label:** Financial Transaction Release Status
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `FinTransReleaseStatus` | `FinTransReleaseStatus` | `String(1)` | Y | Release Status |  |  | S/4 only entity (no ECC CDC mapping) |
| `DomainValue` | `DomainValue` | `String(10)` |  | Lower Value |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `FinTransReleaseStatusText`

- **ABAP Name:** `I_FinTransReleaseStatusText`
- **Label:** Fin Transaction Release Status - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransReleaseStatus` | `FinTransReleaseStatus` | `String(1)` | Y | Release Status |  | _ReleaseStatus | S/4 only entity (no ECC CDC mapping) |
| `DomainValue` | `DomainValue` | `String(10)` |  | Lower Value |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransReleaseStatusName` | `FinTransReleaseStatusName` | `String(60)` |  | Release Status Name |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `FinTransUnderlyingFlow`

- **ABAP Name:** `I_FinTransUnderlyingFlow`
- **Label:** Fin Transaction Underlying Flow
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `OptionUnderlyingTransaction` | `OptionUnderlyingTransaction` | `String(13)` | Y | Transaction |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinancialInstrumentActivity` | `FinancialInstrumentActivity` | `String(5)` | Y | Activity |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransFlowCreationDate` | `FinTransFlowCreationDate` | `Date` | Y | Entered On |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransFlowCreationTime` | `FinTransFlowCreationTime` | `String(6)` | Y | Entry Time |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransFlowNumber` | `FinTransFlowNumber` | `String(4)` | Y | Flow |  |  | S/4 only entity (no ECC CDC mapping) |
| `CreatedByUser` | `CreatedByUser` | `String(12)` |  | Entered By |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransCreationDate` | `FinTransCreationDate` | `Date` |  | Created On |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransCreationTime` | `FinTransCreationTime` | `String(6)` |  | Entry Time |  |  | S/4 only entity (no ECC CDC mapping) |
| `LastChangedByUser` | `LastChangedByUser` | `String(12)` |  | Last Changed By |  |  | S/4 only entity (no ECC CDC mapping) |
| `LastChangeDate` | `LastChangeDate` | `Date` |  | Changed On |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinInstrumentLastChangedTime` | `FinInstrumentLastChangedTime` | `String(6)` |  | Time Changed |  |  | S/4 only entity (no ECC CDC mapping) |
| `TreasuryContractType` | `TreasuryContractType` | `String(1)` |  | Contract Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransFlowType` | `FinTransFlowType` | `String(4)` |  | Flow Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransFlowCategory` | `FinTransFlowCategory` | `String(2)` |  | Flow Category |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransFlowPaytAmtDirection` | `FinTransFlowPaytAmtDirection` | `String(1)` |  | Direction |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinancialTransactionDirection` | `FinancialTransactionDirection` | `String(1)` |  | Direction |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransFlowSource` | `FinTransFlowSource` | `String(4)` |  | Source |  |  | S/4 only entity (no ECC CDC mapping) |
| `PayerPayee` | `PayerPayee` | `String(10)` |  | Payer/Payee |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransFlowPaymentDate` | `FinTransFlowPaymentDate` | `Date` |  | Payment Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransFlowPaytAmt` | `FinTransFlowPaytAmt` | `Decimal(34,4)` |  | Payment Amnt in PyC | FinTransFlowPaytAmtCrcy |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransFlowPaytAmtCrcy` | `FinTransFlowPaytAmtCrcy` | `String(5)` |  | Payment Currency |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransFlowInLoclCrcyPaytAmt` | `FinTransFlowInLoclCrcyPaytAmt` | `Decimal(34,4)` |  | Pmnt Amnt in LCurr | FinTransFlowPaytAmtCrcy |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransFlowLoclCrcyCnvrsnRate` | `FinTransFlowLoclCrcyCnvrsnRate` | `Decimal(9,5)` |  | Crcy Cnvrsn Rate |  |  | S/4 only entity (no ECC CDC mapping) |
| `CalculationDate` | `CalculationDate` | `Date` |  | Calculation Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `CalculationPeriodStartDate` | `CalculationPeriodStartDate` | `Date` |  | Calculation From |  |  | S/4 only entity (no ECC CDC mapping) |
| `CalculationPeriodEndDate` | `CalculationPeriodEndDate` | `Date` |  | Calculation To |  |  | S/4 only entity (no ECC CDC mapping) |
| `CalcPeriodEndDateIsInclusive` | `CalcPeriodEndDateIsInclusive` | `String(1)` |  | Inclusive End Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `CalcPeriodStartDateIsExclusive` | `CalcPeriodStartDateIsExclusive` | `String(1)` |  | Exclusive Start Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `CalcPeriodEndDateIsMonthEnd` | `CalcPeriodEndDateIsMonthEnd` | `Boolean` |  | Month-End End Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `CalcPeriodStartDateIsMonthEnd` | `CalcPeriodStartDateIsMonthEnd` | `Boolean` |  | Month-End Start Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `NumberOfCalculationDays` | `NumberOfCalculationDays` | `String(6)` |  | Number of Days |  |  | S/4 only entity (no ECC CDC mapping) |
| `NrOfBaseDaysPerCalcPeriod` | `NrOfBaseDaysPerCalcPeriod` | `String(6)` |  | No. of base days |  |  | S/4 only entity (no ECC CDC mapping) |
| `InterestCalculationMethod` | `InterestCalculationMethod` | `String(1)` |  | Int. Calc. Method |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransFlowCalcBaseAmount` | `FinTransFlowCalcBaseAmount` | `Decimal(34,4)` |  | Base Amount | FinTransFlowCalcBaseAmountCrcy |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransFlowCalcBaseAmountCrcy` | `FinTransFlowCalcBaseAmountCrcy` | `String(5)` |  | Calculatn Basis Crcy |  |  | S/4 only entity (no ECC CDC mapping) |
| `IntrstCalcMethFactoryCalendar` | `IntrstCalcMethFactoryCalendar` | `String(2)` |  | Interest Calendar |  |  | S/4 only entity (no ECC CDC mapping) |
| `InterestBaseDaysMethod` | `InterestBaseDaysMethod` | `String(1)` |  | Base Days Method |  |  | S/4 only entity (no ECC CDC mapping) |
| `InterestCalculationType` | `InterestCalculationType` | `String(1)` |  | Int. Calc. Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `ConditionPercentageRate` | `ConditionPercentageRate` | `Decimal(10,7)` |  | Percentage Rate |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinCndnPctgRateFixingDate` | `FinCndnPctgRateFixingDate` | `Date` |  | PercFixingDte |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransFlowIntrstRateFixDate` | `FinTransFlowIntrstRateFixDate` | `Date` |  | Int.Rate Fixing Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransPositionValueDate` | `FinTransPositionValueDate` | `Date` |  | Position Value Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransFlowPositionAmount` | `FinTransFlowPositionAmount` | `Decimal(34,4)` |  | PositionAmount | FinTransFlwPosAmtCrcy |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransFlwPosAmtCrcy` | `FinTransFlwPosAmtCrcy` | `String(5)` |  | Position Currency |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransFlowNomAmt` | `FinTransFlowNomAmt` | `Decimal(34,4)` |  | Nominal Amount | FinTransFlowNomAmtCrcy |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransFlowNomAmtCrcy` | `FinTransFlowNomAmtCrcy` | `String(5)` |  | Nominal Amount Currency |  |  | S/4 only entity (no ECC CDC mapping) |
| `MarketValueInQtanCurrency` | `MarketValueInQtanCurrency` | `Decimal(34,4)` |  | Mkt Val. in QC | QuotationCurrency |  | S/4 only entity (no ECC CDC mapping) |
| `QuotationCurrency` | `QuotationCurrency` | `String(5)` |  | Price Currency |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransTradedNumberOfUnits` | `FinTransTradedNumberOfUnits` | `Decimal(24,14)` |  | Number of Units |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransTrdPriceCrcyUnitRate` | `FinTransTrdPriceCrcyUnitRate` | `Decimal(23,14)` |  | Price (Unit-Quoted) |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransTradedPriceCrcyUnit` | `FinTransTradedPriceCrcyUnit` | `String(5)` |  | Currency Unit |  |  | S/4 only entity (no ECC CDC mapping) |
| `SecurityExchange` | `SecurityExchange` | `String(10)` |  | Exchange |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinConditionItem` | `FinConditionItem` | `String(4)` |  | Condition |  |  | S/4 only entity (no ECC CDC mapping) |
| `ConditionItemValidityStartDate` | `ConditionItemValidityStartDate` | `Date` |  | Item Effective From |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinConditionSubItem` | `FinConditionSubItem` | `String(2)` |  | Level Number |  |  | S/4 only entity (no ECC CDC mapping) |
| `InterestConditionType` | `InterestConditionType` | `String(4)` |  | Condition Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinInstrConditionLogicGroup` | `FinInstrConditionLogicGroup` | `String(4)` |  | Condition Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinCndnCrsRefcdAccmlnCndnGrp` | `FinCndnCrsRefcdAccmlnCndnGrp` | `String(4)` |  | Accum. Cond.Grp |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransFlwReltdAccumulatingID` | `FinTransFlwReltdAccumulatingID` | `String(40)` |  | Rel.AccumFlowID |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransFlowAccumulatingFlowID` | `FinTransFlowAccumulatingFlowID` | `String(40)` |  | Accum. Flow ID |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransTradedPricePercent` | `FinTransTradedPricePercent` | `Decimal(23,14)` |  | Price (%) |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `FinancialInstrTransactionType`

- **ABAP Name:** `I_FinancialInstrTransType`
- **Label:** Transaction Type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `FinancialInstrTransactionType` | `FinancialInstrTransactionType` | `String(3)` | Y | Transaction Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinancialInstrumentProductType` | `FinancialInstrumentProductType` | `String(3)` | Y | Product Type |  | _FinancialInstrProductType | S/4 only entity (no ECC CDC mapping) |
| `FinInstrTransactionCategory` | `FinInstrTransactionCategory` | `String(3)` |  | Transaction Category |  |  | S/4 only entity (no ECC CDC mapping) |
| `TreasuryContractType` | `TreasuryContractType` | `String(1)` |  | Contract Type |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `FinancialInstrumentProductType`

- **ABAP Name:** `I_FinancialinstrProductType`
- **Label:** Product Type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `FinancialInstrumentProductType` | `FinancialInstrumentProductType` | `String(3)` | Y | Product Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `TreasuryContractType` | `TreasuryContractType` | `String(1)` |  | Contract Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinancialInstrProductCategory` | `FinancialInstrProductCategory` | `String(3)` |  | Product Category |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinCndnTypeAllocCndnGroup` | `FinCndnTypeAllocCndnGroup` | `String(3)` |  | Condition Group |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `FinancialInstrumentStatus`

- **ABAP Name:** `I_FinInstrumentStatus`
- **Label:** Financial Instrument Status
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `FinancialInstrumentStatus` | `FinancialInstrumentStatus` | `String(1)` | Y | Active Status |  |  | S/4 only entity (no ECC CDC mapping) |
| `DomainValue` | `DomainValue` | `String(10)` |  | Lower Value |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `FinancialInstrumentStatusText`

- **ABAP Name:** `I_FinInstrumentStatusText`
- **Label:** Financial Instrument Status - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinancialInstrumentStatus` | `FinancialInstrumentStatus` | `String(1)` | Y | Active Status |  | _Status | S/4 only entity (no ECC CDC mapping) |
| `DomainValue` | `DomainValue` | `String(10)` |  | Lower Value |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinancialInstrumentStatusName` | `FinancialInstrumentStatusName` | `String(60)` |  | Active Status Name |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `FinancialTransaction`

- **ABAP Name:** `I_FinancialTransactionDEX`
- **Label:** Financial Transaction
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `CompanyCode` | `CompanyCode` | `String(4)` | Y | Company Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinancialTransaction` | `FinancialTransaction` | `String(13)` | Y | Transaction |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransCreationDate` | `FinTransCreationDate` | `Date` |  | Created On |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransCreationTime` | `FinTransCreationTime` | `String(6)` |  | Entry Time |  |  | S/4 only entity (no ECC CDC mapping) |
| `LastChangeDate` | `LastChangeDate` | `Date` |  | Changed On |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinInstrumentLastChangedTime` | `FinInstrumentLastChangedTime` | `String(6)` |  | Time Changed |  |  | S/4 only entity (no ECC CDC mapping) |
| `TreasuryContractType` | `TreasuryContractType` | `String(1)` |  | Contract Type |  | _ContractType | S/4 only entity (no ECC CDC mapping) |
| `FinancialInstrProductCategory` | `FinancialInstrProductCategory` | `String(3)` |  | Product Category |  | _FinancialInstrProdCat | S/4 only entity (no ECC CDC mapping) |
| `FinancialInstrumentProductType` | `FinancialInstrumentProductType` | `String(3)` |  | Product Type |  | _FinancialInstrProdType | S/4 only entity (no ECC CDC mapping) |
| `FinInstrTransactionCategory` | `FinInstrTransactionCategory` | `String(3)` |  | Transaction Category |  | _FinInstrTransCat | S/4 only entity (no ECC CDC mapping) |
| `FinancialInstrTransactionType` | `FinancialInstrTransactionType` | `String(3)` |  | Transaction Type |  | _FinancialInstrTransType | S/4 only entity (no ECC CDC mapping) |
| `TermStartDate` | `TermStartDate` | `Date` |  | Term Start |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransNoticePeriod` | `FinTransNoticePeriod` | `String(3)` |  | Period of Notice |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransNoticePeriodUnit` | `FinTransNoticePeriodUnit` | `String(1)` |  | Unit |  | _NoticePeriodUnit | S/4 only entity (no ECC CDC mapping) |
| `FinTransFactoryCalendar1` | `FinTransFactoryCalendar1` | `String(2)` |  | Calendar |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransFactoryCalendar2` | `FinTransFactoryCalendar2` | `String(2)` |  | Calendar |  |  | S/4 only entity (no ECC CDC mapping) |
| `Counterparty` | `Counterparty` | `String(10)` |  | Counterparty |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinancialInstrumentGuarantor` | `FinancialInstrumentGuarantor` | `String(10)` |  | Guarantor |  |  | S/4 only entity (no ECC CDC mapping) |
| `Portfolio` | `Portfolio` | `String(10)` |  | Portfolio |  | _Portfolio | S/4 only entity (no ECC CDC mapping) |
| `TreasuryFinanceProject` | `TreasuryFinanceProject` | `String(13)` |  | Finance Project |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinancialInstrumentAssignment` | `FinancialInstrumentAssignment` | `String(18)` |  | Free Assignment |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinancialInstrumentReference` | `FinancialInstrumentReference` | `String(16)` |  | Free Internal Ref. |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinancialInstrCharacteristic` | `FinancialInstrCharacteristic` | `String(25)` |  | Free Charact. |  |  | S/4 only entity (no ECC CDC mapping) |
| `ControllingArea` | `ControllingArea` | `String(4)` |  | Controlling Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCenter` | `CostCenter` | `String(10)` |  | Cost Center |  |  | S/4 only entity (no ECC CDC mapping) |
| `HedgingClassification` | `HedgingClassification` | `String(5)` |  | Hedging Classificatn |  |  | S/4 only entity (no ECC CDC mapping) |
| `HedgeRequestIdentifier` | `HedgeRequestIdentifier` | `String(13)` |  | Hedge Request ID |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProfitCenter` | `ProfitCenter` | `String(10)` |  | Profit Center |  |  | S/4 only entity (no ECC CDC mapping) |
| `WBSElementInternalID` | `WBSElementInternalID` | `String(8)` |  | WBS Internal ID |  |  | S/4 only entity (no ECC CDC mapping) |
| `TreasuryFacilityCompanyCode` | `TreasuryFacilityCompanyCode` | `String(4)` |  | CoCd of Facility |  |  | S/4 only entity (no ECC CDC mapping) |
| `TreasuryFacility` | `TreasuryFacility` | `String(13)` |  | Facility |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinancialInstrumentStatus` | `FinancialInstrumentStatus` | `String(1)` |  | Active Status |  | _Status | S/4 only entity (no ECC CDC mapping) |
| `FinTransReleaseStatus` | `FinTransReleaseStatus` | `String(1)` |  | Release Status |  | _ReleaseStatus | S/4 only entity (no ECC CDC mapping) |
| `TransactionCurrency` | `TransactionCurrency` | `String(5)` |  | Transaction Currency |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinInstrumentOutgoingCurrency` | `FinInstrumentOutgoingCurrency` | `String(5)` |  | Outgoing Currency |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinInstrumentIncomingCurrency` | `FinInstrumentIncomingCurrency` | `String(5)` |  | Incoming Currency |  |  | S/4 only entity (no ECC CDC mapping) |
| `TradedCurrency` | `TradedCurrency` | `String(5)` |  | Traded Currency |  |  | S/4 only entity (no ECC CDC mapping) |
| `SecurityClass` | `SecurityClass` | `String(13)` |  | Security Class |  |  | S/4 only entity (no ECC CDC mapping) |
| `ClassificationOfFinInstr` | `ClassificationOfFinInstr` | `String(6)` |  | CFI Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `SecurityAccount` | `SecurityAccount` | `String(10)` |  | Securities Account |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransIsRiskMitigating` | `FinTransIsRiskMitigating` | `Boolean` |  | Risk Mitigation |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinInstrLastActiveActivity` | `FinInstrLastActiveActivity` | `String(5)` |  | Last Active Activity |  |  | S/4 only entity (no ECC CDC mapping) |
| `TrsyTradedAmountBuySellCode` | `TrsyTradedAmountBuySellCode` | `String(1)` |  | Buy/Sell |  |  | S/4 only entity (no ECC CDC mapping) |
| `Segment` | `Segment` | `String(10)` |  | Segment |  |  | S/4 only entity (no ECC CDC mapping) |
| `OnBehalfOfCompany` | `OnBehalfOfCompany` | `String(4)` |  | On Behalf of CoCode |  |  | S/4 only entity (no ECC CDC mapping) |
| `MarketIdentifierCode` | `MarketIdentifierCode` | `String(4)` |  | MIC |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransRoundingCategory` | `FinTransRoundingCategory` | `String(1)` |  | Round |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransGeneralValuationClass` | `FinTransGeneralValuationClass` | `String(4)` |  | Gen. Valn Class |  |  | S/4 only entity (no ECC CDC mapping) |
| `Fund` | `Fund` | `String(10)` |  | Fund |  |  | S/4 only entity (no ECC CDC mapping) |
| `GrantID` | `GrantID` | `String(20)` |  | Grant |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransAuthorizationGroup` | `FinTransAuthorizationGroup` | `String(4)` |  | Authorization Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `BusinessPlace` | `BusinessPlace` | `String(4)` |  | Business Place |  |  | S/4 only entity (no ECC CDC mapping) |
| `FunctionalArea` | `FunctionalArea` | `String(16)` |  | Functional Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `TrsyPosCustomDiffntnTerm1` | `TrsyPosCustomDiffntnTerm1` | `String(20)` |  | Cust.Diff.Term Val. |  |  | S/4 only entity (no ECC CDC mapping) |
| `TrsyPosCustomDiffntnTerm2` | `TrsyPosCustomDiffntnTerm2` | `String(20)` |  | Cust.Diff.Term Val. |  |  | S/4 only entity (no ECC CDC mapping) |
| `TrsyPosCustomDiffntnTerm3` | `TrsyPosCustomDiffntnTerm3` | `String(20)` |  | Cust.Diff.Term Val. |  |  | S/4 only entity (no ECC CDC mapping) |
| `TrsyPosCustomDiffntnTerm4` | `TrsyPosCustomDiffntnTerm4` | `String(20)` |  | Cust.Diff.Term Val. |  |  | S/4 only entity (no ECC CDC mapping) |
| `TrsyPosCustomDiffntnTerm5` | `TrsyPosCustomDiffntnTerm5` | `String(20)` |  | Cust.Diff.Term Val. |  |  | S/4 only entity (no ECC CDC mapping) |
| `UniqueProductIdentifier` | `UniqueProductIdentifier` | `String(12)` |  | Unique Product ID |  |  | S/4 only entity (no ECC CDC mapping) |
| `InternationalSecuritiesIdnNmbr` | `InternationalSecuritiesIdnNmbr` | `String(12)` |  | Security ID (ISIN) |  |  | S/4 only entity (no ECC CDC mapping) |
| `ReportTrackingNumber` | `ReportTrackingNumber` | `String(52)` |  | Report Tracking No. |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransOptionNumber` | `FinTransOptionNumber` | `String(13)` |  | Class |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinancialInstrActivityCategory` | `FinancialInstrActivityCategory` | `String(2)` |  | Activity Category |  | _ActivityCategory | S/4 only entity (no ECC CDC mapping) |
| `TermEndDate` | `TermEndDate` | `Date` |  | Term End |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransTermCategory` | `FinTransTermCategory` | `String(1)` |  | Term Category |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransTermStartEndInclusive` | `FinTransTermStartEndInclusive` | `String(1)` |  | Term Start and End Inclusive |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransNoticeDate` | `FinTransNoticeDate` | `Date` |  | Notice Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransActyConclusionDate` | `FinTransActyConclusionDate` | `Date` |  | Conclusion Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransActyConclusionTime` | `FinTransActyConclusionTime` | `String(6)` |  | Contract.Concl.Time |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransActyConclusionTimeZone` | `FinTransActyConclusionTimeZone` | `String(6)` |  | Time Zone Contr.Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransRolloverDate` | `FinTransRolloverDate` | `Date` |  | Term Start |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransExerciseDate` | `FinTransExerciseDate` | `Date` |  | Term End |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransOrderValidityEndDate` | `FinTransOrderValidityEndDate` | `Date` |  | Limit Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinTransFixingDate` | `FinTransFixingDate` | `Date` |  | Fixing Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `ForeignExchangeFixingReference` | `ForeignExchangeFixingReference` | `String(30)` |  | Fixing Reference ID |  | _FixingReference | S/4 only entity (no ECC CDC mapping) |
| `Trader` | `Trader` | `String(12)` |  | Trader |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinancialInstrContactPerson` | `FinancialInstrContactPerson` | `String(19)` |  | Contact Person |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinInstrExternalReference` | `FinInstrExternalReference` | `String(16)` |  | External Reference |  |  | S/4 only entity (no ECC CDC mapping) |
| `TreasuryReversalReason` | `TreasuryReversalReason` | `String(2)` |  | Reason for Reversal |  | _ReversalReason | S/4 only entity (no ECC CDC mapping) |
| `LeadingCurrency` | `LeadingCurrency` | `String(5)` |  | Leading Currency |  |  | S/4 only entity (no ECC CDC mapping) |
| `FollowingCurrency` | `FollowingCurrency` | `String(5)` |  | Following Currency |  |  | S/4 only entity (no ECC CDC mapping) |
| `ExchangeRate` | `ExchangeRate` | `Decimal(13,9)` |  | Transaction Rate |  |  | S/4 only entity (no ECC CDC mapping) |
| `SpotExchangeRate` | `SpotExchangeRate` | `Decimal(13,9)` |  | Spot Rate |  |  | S/4 only entity (no ECC CDC mapping) |
| `SwapExchangeRate` | `SwapExchangeRate` | `Decimal(13,9)` |  | Swap Rate |  |  | S/4 only entity (no ECC CDC mapping) |
| `LiquidityEffectValue` | `LiquidityEffectValue` | `Decimal(13,9)` |  | Liquidity Effect |  |  | S/4 only entity (no ECC CDC mapping) |
| `CurrencyPair` | `CurrencyPair` | `String(20)` |  | Currency Pair |  |  | S/4 only entity (no ECC CDC mapping) |
| `EffectiveInterestRate` | `EffectiveInterestRate` | `Decimal(10,7)` |  | Effect.Interest Rate |  |  | S/4 only entity (no ECC CDC mapping) |
| `EffectiveInterestMethod` | `EffectiveInterestMethod` | `String(1)` |  | Effect. Int. Method |  |  | S/4 only entity (no ECC CDC mapping) |
| `LetterOfCredit` | `LetterOfCredit` | `String(16)` |  | Letter of Credit No. |  |  | S/4 only entity (no ECC CDC mapping) |
| `TreasuryApplicant` | `TreasuryApplicant` | `String(10)` |  | Applicant |  |  | S/4 only entity (no ECC CDC mapping) |
| `TreasuryBeneficiary` | `TreasuryBeneficiary` | `String(10)` |  | Beneficiary |  |  | S/4 only entity (no ECC CDC mapping) |
| `TrsyMnllyEnteredBnfcyName` | `TrsyMnllyEnteredBnfcyName` | `String(25)` |  | Benefic. Name (Man.) |  |  | S/4 only entity (no ECC CDC mapping) |
| `TrsyMnllyEnteredApplcntName` | `TrsyMnllyEnteredApplcntName` | `String(25)` |  | ApplicantName (Man.) |  |  | S/4 only entity (no ECC CDC mapping) |
| `TreasuryAdvisingBank` | `TreasuryAdvisingBank` | `String(10)` |  | Advising Bank |  |  | S/4 only entity (no ECC CDC mapping) |
| `TreasuryIssuingBank` | `TreasuryIssuingBank` | `String(10)` |  | Issuing Bank |  |  | S/4 only entity (no ECC CDC mapping) |
| `BankGuaranteeNumber` | `BankGuaranteeNumber` | `String(16)` |  | Bank Guarantee No. |  |  | S/4 only entity (no ECC CDC mapping) |
| `BankGuaranteeType` | `BankGuaranteeType` | `String(4)` |  | Bank Guarantee Type |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `ForeignExchangeFixingReference`

- **ABAP Name:** `I_FXFixingReference`
- **Label:** Foreign Exchange Fixing Reference
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `ForeignExchangeFixingReference` | `ForeignExchangeFixingReference` | `String(30)` | Y | Fixing Reference ID |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `TradeFinanceCategory`

- **ABAP Name:** `I_TradeFinanceCategory`
- **Label:** Trade Finance Category
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `TradeFinanceCategory` | `TradeFinanceCategory` | `String(1)` | Y | Trade Finance Cat. |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `TradeFinanceCategoryText`

- **ABAP Name:** `I_TradeFinanceCategoryText`
- **Label:** Trade Finance Category - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `TradeFinanceCategory` | `TradeFinanceCategory` | `String(1)` | Y | Trade Finance Cat. |  |  | S/4 only entity (no ECC CDC mapping) |
| `Language` | `Language` | `String(2)` | Y | Lang. |  |  | S/4 only entity (no ECC CDC mapping) |
| `TradeFinanceCategoryName` | `TradeFinanceCategoryName` | `String(60)` |  | Category Name |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `TreasuryContractType`

- **ABAP Name:** `I_TreasuryContractType`
- **Label:** Treasury Contract Type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `TreasuryContractType` | `TreasuryContractType` | `String(1)` | Y | Contract Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `DomainValue` | `DomainValue` | `String(10)` |  | Lower Value |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `TreasuryContractTypeText`

- **ABAP Name:** `I_TreasuryContractTypeText`
- **Label:** Treasury Contract Type - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `TreasuryContractType` | `TreasuryContractType` | `String(1)` | Y | Contract Type |  | _ContractType | S/4 only entity (no ECC CDC mapping) |
| `DomainValue` | `DomainValue` | `String(10)` |  | Lower Value |  |  | S/4 only entity (no ECC CDC mapping) |
| `TreasuryContractTypeName` | `TreasuryContractTypeName` | `String(60)` |  | Contract Type Name |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `TreasuryPortfolio`

- **ABAP Name:** `I_TreasuryPortfolio`
- **Label:** Portfolio
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `CompanyCode` | `CompanyCode` | `String(4)` | Y | Company Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `Portfolio` | `Portfolio` | `String(10)` | Y | Portfolio |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `TreasuryPortfolioText`

- **ABAP Name:** `I_TreasuryPortfolioText`
- **Label:** Portfolio - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `CompanyCode` | `CompanyCode` | `String(4)` | Y | Company Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `Portfolio` | `Portfolio` | `String(10)` | Y | Portfolio |  | _TreasuryPortfolio | S/4 only entity (no ECC CDC mapping) |
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `PortfolioName` | `PortfolioName` | `String(30)` |  | Portfolio Name |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `TreasuryProductCategory`

- **ABAP Name:** `I_FinancialInstrProdCat`
- **Label:** Product Category
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `FinancialInstrProductCategory` | `FinancialInstrProductCategory` | `String(3)` | Y | Product Category |  |  | S/4 only entity (no ECC CDC mapping) |
| `TreasuryContractType` | `TreasuryContractType` | `String(1)` |  | Contract Type |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `TreasuryProductCategoryText`

- **ABAP Name:** `I_FinancialInstrProdCatText`
- **Label:** Product Category - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `FinancialInstrProductCategory` | `FinancialInstrProductCategory` | `String(3)` | Y | Product Category |  | _FinancialInstrProdCat | S/4 only entity (no ECC CDC mapping) |
| `FinInstrProductCategoryName` | `FinInstrProductCategoryName` | `String(30)` |  | Text |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `TreasuryReversalReason`

- **ABAP Name:** `I_TreasuryReversalReason`
- **Label:** Treasury Reversal Reason
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `TreasuryReversalReason` | `TreasuryReversalReason` | `String(2)` | Y | Reason for Reversal |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `TreasuryReversalReasonText`

- **ABAP Name:** `I_TreasuryReversalReasonText`
- **Label:** Treasury Reversal Reason - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `TreasuryReversalReason` | `TreasuryReversalReason` | `String(2)` | Y | Reason for Reversal |  | _ReversalReason | S/4 only entity (no ECC CDC mapping) |
| `TreasuryReversalReasonName` | `TreasuryReversalReasonName` | `String(60)` |  | Long name |  |  | S/4 only entity (no ECC CDC mapping) |
