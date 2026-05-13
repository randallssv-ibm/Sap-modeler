# CostOriginGroup

> Source file: `sap-s4com-CostOriginGroup-v1.json`

**Technical Name:** `` | **Data Category:** `DIMENSION` | **VDM Type:** `BASIC` | **Size:** `S`


## Entity: `CostOriginGroup`

- **ABAP Name:** `I_CostOriginGroup`
- **Label:** Cost Origin Group
- **VDM Type:** `BASIC` | **Data Category:** `DIMENSION`
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `ControllingArea` | `TKA01` | `KOKRS` | `String(4)` | Y | Controlling Area |  |  |  |
| `CostOriginType` |  |  | `String(2)` | Y | Origin type |  |  | S/4 only entity |
| `CostOriginGroup` |  |  | `String(4)` | Y | Origin Group |  |  | S/4 only entity |


## Entity: `CostOriginGroupText`

- **ABAP Name:** `I_CostOriginGroupText`
- **Label:** Cost Origin Group - Text
- **VDM Type:** `BASIC` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `CostOriginGroup` |  |  | `String(4)` | Y | Origin Group |  |  | S/4 only entity |
| `CostOriginType` |  |  | `String(2)` | Y | Origin type |  |  | S/4 only entity |
| `ControllingArea` | `TKA01` | `KOKRS` | `String(4)` | Y | Controlling Area |  |  |  |
| `Language` |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity |
| `CostOriginGroupName` |  |  | `String(40)` |  | Name |  |  | S/4 only entity |
