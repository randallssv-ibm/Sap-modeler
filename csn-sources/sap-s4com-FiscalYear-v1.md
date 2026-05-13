# FiscalYear

> Source file: `sap-s4com-FiscalYear-v1.json`


## Entity: `FiscalYear`

- **ABAP CDS Name:** `I_FiscalYearForVariant`
- **Label:** Fiscal Year For Fiscal Year Variant
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `FiscalYearVariant` |  | `T009` | `PERIV` |  |  | `String(2)` | Y | Fiscal Year Variant |  |  |
| `FiscalYear` |  |  |  |  |  | `String(4)` | Y | Fiscal Year |  | S/4 only entity |
| `FiscalYearStartDate` |  | `T009B` | `XJABJ` |  |  | `Date` |  | Start of Fiscal Year |  |  |
| `FiscalYearEndDate` |  |  |  |  |  | `Date` |  | End of Fiscal Year |  | S/4 only entity |


## Entity: `FiscalYearVariant`

- **ABAP CDS Name:** `I_FiscalYearVariant`
- **Label:** Fiscal Year Variant
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `FiscalYearVariant` |  |  |  |  |  | `String(2)` | Y | Fiscal Year Variant |  | S/4 only entity |
| `FiscalPeriodIsEqualMonth` |  |  |  |  |  | `Boolean` |  | Fscl Perd Equal Mnth |  | S/4 only entity |
| `IsYearDependent` |  |  |  |  |  | `Boolean` |  | Year-dependent |  | S/4 only entity |
| `PostingPeriodsNumberVal` |  |  |  |  |  | `String(3)` |  | Posting Period |  | S/4 only entity |
| `NumberOfSpecialPeriods` |  |  |  |  |  | `String(2)` |  | No. Special Periods |  | S/4 only entity |
| `FsclWeekStartIsFsclYearStart` |  |  |  |  |  | `Boolean` |  | Fiscal Week Start |  | S/4 only entity |
| `FiscalCalendarIsWeekBased` |  |  |  |  |  | `Boolean` |  | Weekly Calendar |  | S/4 only entity |


## Entity: `FiscalYearVariantText`

- **ABAP CDS Name:** `I_FiscalYearVariantText`
- **Label:** Fiscal Year Variant Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Language` |  |  |  |  |  | `String(2)` | Y | Language Key |  | S/4 only entity |
| `FiscalYearVariant` |  |  |  |  |  | `String(2)` | Y | Fiscal Year Variant |  | S/4 only entity |
| `FiscalYearVariantDescription` |  |  |  |  |  | `String(30)` |  | Fiscal Year Variant Name |  | S/4 only entity |
