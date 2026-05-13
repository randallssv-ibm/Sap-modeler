# CostOriginGroup

> Source file: `sap-s4com-CostOriginGroup-v1.json`

**Technical Name:** `` | **Data Category:** `DIMENSION` | **VDM Type:** `BASIC` | **Size:** `S`


## Entity: `CostOriginGroup`

- **ABAP Name:** `I_CostOriginGroup`
- **Label:** Cost Origin Group
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `ControllingArea` | `FIS_KOKRS` | `KOKRS` |  | `String(4)` | Y | Controlling Area |  |  | S/4 only entity — no ECC CDC mapping |
| `CostOriginType` | `HRKTYP` | `HRKTYP` |  | `String(2)` | Y | Origin type |  |  | S/4 only entity — no ECC CDC mapping |
| `CostOriginGroup` | `HRKFT` | `HRKFT` |  | `String(4)` | Y | Origin Group |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `CostOriginGroupText`

- **ABAP Name:** `I_CostOriginGroupText`
- **Label:** Cost Origin Group - Text
- **VDM Type:** `BASIC` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `CostOriginGroup` | `HRKFT` | `HRKFT` |  | `String(4)` | Y | Origin Group |  |  | S/4 only entity — no ECC CDC mapping |
| `CostOriginType` | `HRKTYP` | `HRKTYP` |  | `String(2)` | Y | Origin type |  |  | S/4 only entity — no ECC CDC mapping |
| `ControllingArea` | `FIS_KOKRS` | `KOKRS` |  | `String(4)` | Y | Controlling Area |  |  | S/4 only entity — no ECC CDC mapping |
| `Language` | `SPRAS` | `SPRAS` |  | `String(2)` | Y | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `CostOriginGroupName` | `HRTXT` | `HRTXT` |  | `String(40)` |  | Name |  |  | S/4 only entity — no ECC CDC mapping |
