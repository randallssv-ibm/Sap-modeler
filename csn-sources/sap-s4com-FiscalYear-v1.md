# FiscalYear

> Source file: `sap-s4com-FiscalYear-v1.json`


## Entity: `FiscalYear`

- **ABAP Name:** `I_FiscalYearForVariant`
- **Label:** Fiscal Year For Fiscal Year Variant
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `FiscalYearVariant` | `FiscalYearVariant` | `String(2)` | Y | Fiscal Year Variant |  | _FiscalYearVariant | S/4 only entity (no ECC CDC mapping) |
| `FiscalYear` | `FiscalYear` | `String(4)` | Y | Fiscal Year |  |  | S/4 only entity (no ECC CDC mapping) |
| `FiscalYearStartDate` | `FiscalYearStartDate` | `Date` |  | Start of Fiscal Year |  |  | S/4 only entity (no ECC CDC mapping) |
| `FiscalYearEndDate` | `FiscalYearEndDate` | `Date` |  | End of Fiscal Year |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `FiscalYearVariant`

- **ABAP Name:** `I_FiscalYearVariant`
- **Label:** Fiscal Year Variant
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `FiscalYearVariant` | `FiscalYearVariant` | `String(2)` | Y | Fiscal Year Variant |  |  | S/4 only entity (no ECC CDC mapping) |
| `FiscalPeriodIsEqualMonth` | `FiscalPeriodIsEqualMonth` | `Boolean` |  | Fscl Perd Equal Mnth |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsYearDependent` | `IsYearDependent` | `Boolean` |  | Year-dependent |  |  | S/4 only entity (no ECC CDC mapping) |
| `PostingPeriodsNumberVal` | `PostingPeriodsNumberVal` | `String(3)` |  | Posting Period |  |  | S/4 only entity (no ECC CDC mapping) |
| `NumberOfSpecialPeriods` | `NumberOfSpecialPeriods` | `String(2)` |  | No. Special Periods |  |  | S/4 only entity (no ECC CDC mapping) |
| `FsclWeekStartIsFsclYearStart` | `FsclWeekStartIsFsclYearStart` | `Boolean` |  | Fiscal Week Start |  |  | S/4 only entity (no ECC CDC mapping) |
| `FiscalCalendarIsWeekBased` | `FiscalCalendarIsWeekBased` | `Boolean` |  | Weekly Calendar |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `FiscalYearVariantText`

- **ABAP Name:** `I_FiscalYearVariantText`
- **Label:** Fiscal Year Variant Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `FiscalYearVariant` | `FiscalYearVariant` | `String(2)` | Y | Fiscal Year Variant |  |  | S/4 only entity (no ECC CDC mapping) |
| `FiscalYearVariantDescription` | `FiscalYearVariantDescription` | `String(30)` |  | Fiscal Year Variant Name |  |  | S/4 only entity (no ECC CDC mapping) |
