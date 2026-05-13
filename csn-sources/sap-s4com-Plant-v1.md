# Plant

> Source file: `sap-s4com-Plant-v1.json`


## Entity: `Plant`

- **ABAP CDS Name:** `I_Plant`
- **Label:** Plant
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** T001W

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Plant` |  | `T001W` | `WERKS` |  |  | `String(4)` | Y | Plant |  |  |
| `PlantName` |  | `T001W` | `NAME1` |  |  | `String(30)` |  | Plant Name |  |  |
| `ValuationArea` |  |  |  |  |  | `String(4)` |  | Valuation Area |  |  |
| `PlantCustomer` |  |  |  |  |  | `String(10)` |  | Customer No Plant |  |  |
| `PlantSupplier` |  |  |  |  |  | `String(10)` |  | Sppl. No. Plnt |  |  |
| `FactoryCalendar` |  | `T001W` | `FABKL` |  |  | `String(2)` |  | Factory Calendar |  |  |
| `DefaultPurchasingOrganization` |  |  |  |  |  | `String(4)` |  | Purch. Organization |  |  |
| `SalesOrganization` |  |  |  |  |  | `String(4)` |  | Sls Organization ICB |  |  |
| `AddressID` |  |  |  |  |  | `String(10)` |  | Address |  |  |
| `PlantCategory` |  |  |  |  |  | `String(1)` |  | Plant Cat. |  |  |
| `DistributionChannel` |  |  |  |  |  | `String(2)` |  | Distrib.Channel |  |  |
| `Division` |  |  |  |  |  | `String(2)` |  | Interco. Billing Div |  |  |
| `Language` |  | `T001W` | `SPRAS` |  |  | `String(2)` |  | Language Key |  |  |
| `IsMarkedForArchiving` |  |  |  |  |  | `Boolean` |  | Archiving Flag |  |  |
| `BusinessPlace` |  |  |  |  |  | `String(4)` |  | Business Place |  |  |


## Entity: `PlantCategory`

- **ABAP CDS Name:** `I_PlantCategoryT`
- **Label:** Plant Category - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** T001W

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `PlantCategory` |  |  |  |  |  | `String(1)` | Y | Plant Cat. |  |  |
| `Language` |  |  |  |  |  | `String(2)` | Y | Lang. |  |  |
| `PlantCategoryName` |  |  |  |  |  | `String(60)` |  | Short Description |  |  |
