# Plant

> Source file: `sap-s4com-Plant-v1.json`


## Entity: `Plant`

- **ABAP Name:** `I_Plant`
- **Label:** Plant
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `Plant` |  |  | `String(4)` | Y | Plant |  |  | S/4 only entity |
| `PlantName` |  |  | `String(30)` |  | Plant Name |  |  | S/4 only entity |
| `ValuationArea` |  |  | `String(4)` |  | Valuation Area |  |  | S/4 only entity |
| `PlantCustomer` |  |  | `String(10)` |  | Customer No Plant |  |  | S/4 only entity |
| `PlantSupplier` |  |  | `String(10)` |  | Sppl. No. Plnt |  |  | S/4 only entity |
| `FactoryCalendar` |  |  | `String(2)` |  | Factory Calendar |  |  | S/4 only entity |
| `DefaultPurchasingOrganization` |  |  | `String(4)` |  | Purch. Organization |  |  | S/4 only entity |
| `SalesOrganization` |  |  | `String(4)` |  | Sls Organization ICB |  |  | S/4 only entity |
| `AddressID` |  |  | `String(10)` |  | Address |  |  | S/4 only entity |
| `PlantCategory` |  |  | `String(1)` |  | Plant Cat. |  |  | S/4 only entity |
| `DistributionChannel` |  |  | `String(2)` |  | Distrib.Channel |  |  | S/4 only entity |
| `Division` |  |  | `String(2)` |  | Interco. Billing Div |  |  | S/4 only entity |
| `Language` |  |  | `String(2)` |  | Language Key |  |  | S/4 only entity |
| `IsMarkedForArchiving` |  |  | `Boolean` |  | Archiving Flag |  |  | S/4 only entity |
| `BusinessPlace` |  |  | `String(4)` |  | Business Place |  |  | S/4 only entity |


## Entity: `PlantCategory`

- **ABAP Name:** `I_PlantCategoryT`
- **Label:** Plant Category - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `PlantCategory` |  |  | `String(1)` | Y | Plant Cat. |  |  | S/4 only entity |
| `Language` |  |  | `String(2)` | Y | Lang. |  |  | S/4 only entity |
| `PlantCategoryName` |  |  | `String(60)` |  | Short Description |  |  | S/4 only entity |
