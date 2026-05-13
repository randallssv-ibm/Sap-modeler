# Plant

> Source file: `sap-s4com-Plant-v1.json`


## Entity: `Plant`

- **ABAP Name:** `I_Plant`
- **Label:** Plant
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Plant` | `Plant` | `String(4)` | Y | Plant |  |  | S/4 only entity (no ECC CDC mapping) |
| `PlantName` | `PlantName` | `String(30)` |  | Plant Name |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValuationArea` | `ValuationArea` | `String(4)` |  | Valuation Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `PlantCustomer` | `PlantCustomer` | `String(10)` |  | Customer No Plant |  |  | S/4 only entity (no ECC CDC mapping) |
| `PlantSupplier` | `PlantSupplier` | `String(10)` |  | Sppl. No. Plnt |  |  | S/4 only entity (no ECC CDC mapping) |
| `FactoryCalendar` | `FactoryCalendar` | `String(2)` |  | Factory Calendar |  |  | S/4 only entity (no ECC CDC mapping) |
| `DefaultPurchasingOrganization` | `DefaultPurchasingOrganization` | `String(4)` |  | Purch. Organization |  |  | S/4 only entity (no ECC CDC mapping) |
| `SalesOrganization` | `SalesOrganization` | `String(4)` |  | Sls Organization ICB |  |  | S/4 only entity (no ECC CDC mapping) |
| `AddressID` | `AddressID` | `String(10)` |  | Address |  |  | S/4 only entity (no ECC CDC mapping) |
| `PlantCategory` | `PlantCategory` | `String(1)` |  | Plant Cat. |  |  | S/4 only entity (no ECC CDC mapping) |
| `DistributionChannel` | `DistributionChannel` | `String(2)` |  | Distrib.Channel |  |  | S/4 only entity (no ECC CDC mapping) |
| `Division` | `Division` | `String(2)` |  | Interco. Billing Div |  |  | S/4 only entity (no ECC CDC mapping) |
| `Language` | `Language` | `String(2)` |  | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsMarkedForArchiving` | `IsMarkedForArchiving` | `Boolean` |  | Archiving Flag |  |  | S/4 only entity (no ECC CDC mapping) |
| `BusinessPlace` | `BusinessPlace` | `String(4)` |  | Business Place |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `PlantCategory`

- **ABAP Name:** `I_PlantCategoryT`
- **Label:** Plant Category - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `PlantCategory` | `PlantCategory` | `String(1)` | Y | Plant Cat. |  |  | S/4 only entity (no ECC CDC mapping) |
| `Language` | `Language` | `String(2)` | Y | Lang. |  |  | S/4 only entity (no ECC CDC mapping) |
| `PlantCategoryName` | `PlantCategoryName` | `String(60)` |  | Short Description |  |  | S/4 only entity (no ECC CDC mapping) |
