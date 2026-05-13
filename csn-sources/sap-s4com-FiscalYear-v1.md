# FiscalYear

> Source file: `sap-s4com-FiscalYear-v1.json`


## Entity: `FiscalYear`

- **ABAP CDS Name:** `I_FiscalYearForVariant`
- **Label:** Fiscal Year For Fiscal Year Variant
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** T009B

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `FiscalYearVariant` |  | `T009` | `PERIV` |  |  | `String(2)` | Y | Fiscal Year Variant |  |  |
| `FiscalYear` |  |  |  |  |  | `String(4)` | Y | Fiscal Year |  |  |
| `FiscalYearStartDate` |  | `T009B` | `XJABJ` |  |  | `Date` |  | Start of Fiscal Year |  |  |
| `FiscalYearEndDate` |  |  |  |  |  | `Date` |  | End of Fiscal Year |  |  |


## Entity: `FiscalYearVariant`

- **ABAP CDS Name:** `I_FiscalYearVariant`
- **Label:** Fiscal Year Variant
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** T009

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `FiscalYearVariant` |  |  |  |  |  | `String(2)` | Y | Fiscal Year Variant |  |  |
| `FiscalPeriodIsEqualMonth` |  |  |  |  |  | `Boolean` |  | Fscl Perd Equal Mnth |  |  |
| `IsYearDependent` |  |  |  |  |  | `Boolean` |  | Year-dependent |  |  |
| `PostingPeriodsNumberVal` |  |  |  |  |  | `String(3)` |  | Posting Period |  |  |
| `NumberOfSpecialPeriods` |  |  |  |  |  | `String(2)` |  | No. Special Periods |  |  |
| `FsclWeekStartIsFsclYearStart` |  |  |  |  |  | `Boolean` |  | Fiscal Week Start |  |  |
| `FiscalCalendarIsWeekBased` |  |  |  |  |  | `Boolean` |  | Weekly Calendar |  |  |


## Entity: `FiscalYearVariantText`

- **ABAP CDS Name:** `I_FiscalYearVariantText`
- **Label:** Fiscal Year Variant Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** T009T

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Language` |  |  |  |  |  | `String(2)` | Y | Language Key |  |  |
| `FiscalYearVariant` |  |  |  |  |  | `String(2)` | Y | Fiscal Year Variant |  |  |
| `FiscalYearVariantDescription` |  |  |  |  |  | `String(30)` |  | Fiscal Year Variant Name |  |  |
