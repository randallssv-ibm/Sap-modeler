# Plant

> Source file: `sap-s4com-Plant-v1.json`


## Entity: `Plant`

- **ABAP Name:** `I_Plant`
- **Label:** Plant
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Plant` |  |  |  | `String(4)` | Y | Plant |  |  | S/4 only entity — no ECC CDC mapping |
| `PlantName` |  |  |  | `String(30)` |  | Plant Name |  |  | S/4 only entity — no ECC CDC mapping |
| `ValuationArea` |  |  |  | `String(4)` |  | Valuation Area |  |  | S/4 only entity — no ECC CDC mapping |
| `PlantCustomer` |  |  |  | `String(10)` |  | Customer No Plant |  |  | S/4 only entity — no ECC CDC mapping |
| `PlantSupplier` |  |  |  | `String(10)` |  | Sppl. No. Plnt |  |  | S/4 only entity — no ECC CDC mapping |
| `FactoryCalendar` |  |  |  | `String(2)` |  | Factory Calendar |  |  | S/4 only entity — no ECC CDC mapping |
| `DefaultPurchasingOrganization` |  |  |  | `String(4)` |  | Purch. Organization |  |  | S/4 only entity — no ECC CDC mapping |
| `SalesOrganization` |  |  |  | `String(4)` |  | Sls Organization ICB |  |  | S/4 only entity — no ECC CDC mapping |
| `AddressID` |  |  |  | `String(10)` |  | Address |  |  | S/4 only entity — no ECC CDC mapping |
| `PlantCategory` |  |  |  | `String(1)` |  | Plant Cat. |  |  | S/4 only entity — no ECC CDC mapping |
| `DistributionChannel` |  |  |  | `String(2)` |  | Distrib.Channel |  |  | S/4 only entity — no ECC CDC mapping |
| `Division` |  |  |  | `String(2)` |  | Interco. Billing Div |  |  | S/4 only entity — no ECC CDC mapping |
| `Language` |  |  |  | `String(2)` |  | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `IsMarkedForArchiving` |  |  |  | `Boolean` |  | Archiving Flag |  |  | S/4 only entity — no ECC CDC mapping |
| `BusinessPlace` |  |  |  | `String(4)` |  | Business Place |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `PlantCategory`

- **ABAP Name:** `I_PlantCategoryT`
- **Label:** Plant Category - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `PlantCategory` |  |  |  | `String(1)` | Y | Plant Cat. |  |  | S/4 only entity — no ECC CDC mapping |
| `Language` |  |  |  | `String(2)` | Y | Lang. |  |  | S/4 only entity — no ECC CDC mapping |
| `PlantCategoryName` |  |  |  | `String(60)` |  | Short Description |  |  | S/4 only entity — no ECC CDC mapping |
