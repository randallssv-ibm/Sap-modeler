# FunctionalArea

> Source file: `sap-s4com-FunctionalArea-v1.json`


## Entity: `FunctionalArea`

- **ABAP CDS Name:** `I_FunctionalArea`
- **Label:** Functional Area
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `FunctionalArea` |  | `TFKB` | `FKBER` |  |  | `String(16)` | Y | Functional Area |  |  |
| `CreationDate` |  |  |  |  |  | `Date` |  | Entered On |  | S/4 only entity |
| `LastChangeDate` |  |  |  |  |  | `Date` |  | Changed On |  | S/4 only entity |


## Entity: `FunctionalAreaHierNodeText`

- **ABAP CDS Name:** `I_FunctionalAreaHierNodeT`
- **Label:** Functional Area Hierarchy Node - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `FunctionalAreaHierarchy` |  |  |  |  |  | `String(42)` | Y | Func. Area Hierarchy |  | S/4 only entity |
| `HierarchyNode` |  |  |  |  |  | `String(50)` | Y | Node |  | S/4 only entity |
| `ValidityEndDate` |  |  |  |  |  | `Date` | Y | Validity End Date |  | S/4 only entity |
| `Language` |  |  |  |  |  | `String(2)` | Y | Language Key |  | S/4 only entity |
| `HierarchyNodeText` |  |  |  |  |  | `String(50)` |  | Description |  | S/4 only entity |
| `ValidityStartDate` |  |  |  |  |  | `Date` |  | Validity Start Date |  | S/4 only entity |


## Entity: `FunctionalAreaHierarchy`

- **ABAP CDS Name:** `I_FunctionalAreaHierarchy`
- **Label:** Functional Area Hierarchy
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `FunctionalAreaHierarchy` |  |  |  |  |  | `String(42)` | Y | Func. Area Hierarchy |  | S/4 only entity |
| `ValidityEndDate` |  |  |  |  |  | `Date` | Y | Validity End Date |  | S/4 only entity |
| `ValidityStartDate` |  |  |  |  |  | `Date` |  | Validity Start Date |  | S/4 only entity |
| `LastChangedByUser` |  |  |  |  |  | `String(12)` |  | Last Changed By |  | S/4 only entity |
| `LastChangeDateTime` |  |  |  |  |  | `DateTime` |  | Updated At |  | S/4 only entity |
| `LastChangeTime` |  |  |  |  |  | `DateTime` |  | Updated At |  | S/4 only entity |
| `HierarchyShortID` |  |  |  |  |  | `String(20)` |  | Hierarchy ID |  | S/4 only entity |


## Entity: `FunctionalAreaHierarchyNode`

- **ABAP CDS Name:** `I_FunctionalAreaHierNode`
- **Label:** Functional Area Hierarchy Node
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `FunctionalAreaHierarchy` |  |  |  |  |  | `String(42)` | Y | Func. Area Hierarchy |  | S/4 only entity |
| `HierarchyNode` |  |  |  |  |  | `String(50)` | Y | Node |  | S/4 only entity |
| `ValidityEndDate` |  |  |  |  |  | `Date` | Y | Validity End Date |  | S/4 only entity |
| `ValidityStartDate` |  |  |  |  |  | `Date` |  | Validity Start Date |  | S/4 only entity |
| `ParentNode` |  |  |  |  |  | `String(50)` |  | Par. Node |  | S/4 only entity |
| `HierarchyVersion` |  |  |  |  |  | `String(15)` |  | Version |  | S/4 only entity |
| `FunctionalArea` |  |  |  |  |  | `String(16)` |  | Functional Area |  | S/4 only entity |
| `SequenceNumber` |  |  |  |  |  | `String(56)` |  |  |  | S/4 only entity |
| `HierarchyNodeSequence` |  |  |  |  |  | `String(6)` |  | Sequence Number |  | S/4 only entity |
| `HierarchyNodeLevel` |  |  |  |  |  | `String(6)` |  | Hierarchy Level |  | S/4 only entity |
| `NodeType` |  |  |  |  |  | `String(1)` |  | Node Type |  | S/4 only entity |
| `HierarchyNodeVal` |  |  |  |  |  | `String(40)` |  | Value |  | S/4 only entity |


## Entity: `FunctionalAreaHierarchyText`

- **ABAP CDS Name:** `I_FunctionalAreaHierarchyT`
- **Label:** Functional Area Hierarchy - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `FunctionalAreaHierarchy` |  |  |  |  |  | `String(42)` | Y | Func. Area Hierarchy |  | S/4 only entity |
| `ValidityEndDate` |  |  |  |  |  | `Date` | Y | Validity End Date |  | S/4 only entity |
| `Language` |  |  |  |  |  | `String(2)` | Y | Language Key |  | S/4 only entity |
| `ValidityStartDate` |  |  |  |  |  | `Date` |  | Validity Start Date |  | S/4 only entity |
| `FunctionalAreaHierarchyName` |  |  |  |  |  | `String(50)` |  | Description |  | S/4 only entity |


## Entity: `FunctionalAreaText`

- **ABAP CDS Name:** `I_FunctionalAreaText`
- **Label:** Functional Area - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Language` |  |  |  |  |  | `String(2)` | Y | Language Key |  | S/4 only entity |
| `FunctionalArea` |  |  |  |  |  | `String(16)` | Y | Functional Area |  | S/4 only entity |
| `FunctionalAreaName` |  |  |  |  |  | `String(25)` |  | Functional Area Name |  | S/4 only entity |
