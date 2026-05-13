# CostOriginGroup

> Source file: `sap-s4com-CostOriginGroup-v1.json`

**Technical Name:** `` | **Data Category:** `DIMENSION` | **VDM Type:** `BASIC` | **Size:** `S`


## Entity: `CostOriginGroup`

- **ABAP CDS Name:** `I_CostOriginGroup`
- **Label:** Cost Origin Group
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** CSKG

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `ControllingArea` | `FIS_KOKRS` |  |  |  |  | `String(4)` | Y | Controlling Area |  |  |
| `CostOriginType` | `HRKTYP` |  |  |  |  | `String(2)` | Y | Origin type |  |  |
| `CostOriginGroup` | `HRKFT` |  |  |  |  | `String(4)` | Y | Origin Group |  |  |


## Entity: `CostOriginGroupText`

- **ABAP CDS Name:** `I_CostOriginGroupText`
- **Label:** Cost Origin Group - Text
- **VDM Type:** `BASIC` | **Data Category:** ``
- **ECC Source Tables:** CSKGT

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `CostOriginGroup` | `HRKFT` |  |  |  |  | `String(4)` | Y | Origin Group |  |  |
| `CostOriginType` | `HRKTYP` |  |  |  |  | `String(2)` | Y | Origin type |  |  |
| `ControllingArea` | `FIS_KOKRS` |  |  |  |  | `String(4)` | Y | Controlling Area |  |  |
| `Language` | `SPRAS` |  |  |  |  | `String(2)` | Y | Language Key |  |  |
| `CostOriginGroupName` | `HRTXT` |  |  |  |  | `String(40)` |  | Name |  |  |
