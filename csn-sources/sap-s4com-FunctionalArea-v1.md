# FunctionalArea

> Source file: `sap-s4com-FunctionalArea-v1.json`


## Entity: `FunctionalArea`

- **ABAP CDS Name:** `I_FunctionalArea`
- **Label:** Functional Area
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** TFKB, TFKBT

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `FunctionalArea` |  | `TFKB` | `FKBER` |  |  | `String(16)` | Y | Functional Area |  |  |
| `CreationDate` |  |  |  |  |  | `Date` |  | Entered On |  |  |
| `LastChangeDate` |  |  |  |  |  | `Date` |  | Changed On |  |  |


## Entity: `FunctionalAreaHierNodeText`

- **ABAP CDS Name:** `I_FunctionalAreaHierNodeT`
- **Label:** Functional Area Hierarchy Node - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** SETHEADERT

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `FunctionalAreaHierarchy` |  |  |  |  |  | `String(42)` | Y | Func. Area Hierarchy |  |  |
| `HierarchyNode` |  |  |  |  |  | `String(50)` | Y | Node |  |  |
| `ValidityEndDate` |  |  |  |  |  | `Date` | Y | Validity End Date |  |  |
| `Language` |  |  |  |  |  | `String(2)` | Y | Language Key |  |  |
| `HierarchyNodeText` |  |  |  |  |  | `String(50)` |  | Description |  |  |
| `ValidityStartDate` |  |  |  |  |  | `Date` |  | Validity Start Date |  |  |


## Entity: `FunctionalAreaHierarchy`

- **ABAP CDS Name:** `I_FunctionalAreaHierarchy`
- **Label:** Functional Area Hierarchy
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** SETHEADER, SETHEADERT

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `FunctionalAreaHierarchy` |  |  |  |  |  | `String(42)` | Y | Func. Area Hierarchy |  |  |
| `ValidityEndDate` |  |  |  |  |  | `Date` | Y | Validity End Date |  |  |
| `ValidityStartDate` |  |  |  |  |  | `Date` |  | Validity Start Date |  |  |
| `LastChangedByUser` |  |  |  |  |  | `String(12)` |  | Last Changed By |  |  |
| `LastChangeDateTime` |  |  |  |  |  | `DateTime` |  | Updated At |  |  |
| `LastChangeTime` |  |  |  |  |  | `DateTime` |  | Updated At |  |  |
| `HierarchyShortID` |  |  |  |  |  | `String(20)` |  | Hierarchy ID |  |  |


## Entity: `FunctionalAreaHierarchyNode`

- **ABAP CDS Name:** `I_FunctionalAreaHierNode`
- **Label:** Functional Area Hierarchy Node
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** SETHEADER, SETNODE, SETLEAF

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `FunctionalAreaHierarchy` |  |  |  |  |  | `String(42)` | Y | Func. Area Hierarchy |  |  |
| `HierarchyNode` |  |  |  |  |  | `String(50)` | Y | Node |  |  |
| `ValidityEndDate` |  |  |  |  |  | `Date` | Y | Validity End Date |  |  |
| `ValidityStartDate` |  |  |  |  |  | `Date` |  | Validity Start Date |  |  |
| `ParentNode` |  |  |  |  |  | `String(50)` |  | Par. Node |  |  |
| `HierarchyVersion` |  |  |  |  |  | `String(15)` |  | Version |  |  |
| `FunctionalArea` |  |  |  |  |  | `String(16)` |  | Functional Area |  |  |
| `SequenceNumber` |  |  |  |  |  | `String(56)` |  |  |  |  |
| `HierarchyNodeSequence` |  |  |  |  |  | `String(6)` |  | Sequence Number |  |  |
| `HierarchyNodeLevel` |  |  |  |  |  | `String(6)` |  | Hierarchy Level |  |  |
| `NodeType` |  |  |  |  |  | `String(1)` |  | Node Type |  |  |
| `HierarchyNodeVal` |  |  |  |  |  | `String(40)` |  | Value |  |  |


## Entity: `FunctionalAreaHierarchyText`

- **ABAP CDS Name:** `I_FunctionalAreaHierarchyT`
- **Label:** Functional Area Hierarchy - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** SETHEADERT

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `FunctionalAreaHierarchy` |  |  |  |  |  | `String(42)` | Y | Func. Area Hierarchy |  |  |
| `ValidityEndDate` |  |  |  |  |  | `Date` | Y | Validity End Date |  |  |
| `Language` |  |  |  |  |  | `String(2)` | Y | Language Key |  |  |
| `ValidityStartDate` |  |  |  |  |  | `Date` |  | Validity Start Date |  |  |
| `FunctionalAreaHierarchyName` |  |  |  |  |  | `String(50)` |  | Description |  |  |


## Entity: `FunctionalAreaText`

- **ABAP CDS Name:** `I_FunctionalAreaText`
- **Label:** Functional Area - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** TFKBT

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Language` |  |  |  |  |  | `String(2)` | Y | Language Key |  |  |
| `FunctionalArea` |  |  |  |  |  | `String(16)` | Y | Functional Area |  |  |
| `FunctionalAreaName` |  |  |  |  |  | `String(25)` |  | Functional Area Name |  |  |
