# FunctionalArea

> Source file: `sap-s4com-FunctionalArea-v1.json`


## Entity: `FunctionalArea`

- **ABAP Name:** `I_FunctionalArea`
- **Label:** Functional Area
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `FunctionalArea` |  |  |  | `String(16)` | Y | Functional Area |  |  | S/4 only entity — no ECC CDC mapping |
| `CreationDate` |  |  |  | `Date` |  | Entered On |  |  | S/4 only entity — no ECC CDC mapping |
| `LastChangeDate` |  |  |  | `Date` |  | Changed On |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `FunctionalAreaHierNodeText`

- **ABAP Name:** `I_FunctionalAreaHierNodeT`
- **Label:** Functional Area Hierarchy Node - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `FunctionalAreaHierarchy` |  |  |  | `String(42)` | Y | Func. Area Hierarchy |  | _Hierarchy | S/4 only entity — no ECC CDC mapping |
| `HierarchyNode` |  |  |  | `String(50)` | Y | Node |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityEndDate` |  |  |  | `Date` | Y | Validity End Date |  |  | S/4 only entity — no ECC CDC mapping |
| `Language` |  |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `HierarchyNodeText` |  |  |  | `String(50)` |  | Description |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityStartDate` |  |  |  | `Date` |  | Validity Start Date |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `FunctionalAreaHierarchy`

- **ABAP Name:** `I_FunctionalAreaHierarchy`
- **Label:** Functional Area Hierarchy
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `FunctionalAreaHierarchy` |  |  |  | `String(42)` | Y | Func. Area Hierarchy |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityEndDate` |  |  |  | `Date` | Y | Validity End Date |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityStartDate` |  |  |  | `Date` |  | Validity Start Date |  |  | S/4 only entity — no ECC CDC mapping |
| `LastChangedByUser` |  |  |  | `String(12)` |  | Last Changed By |  |  | S/4 only entity — no ECC CDC mapping |
| `LastChangeDateTime` |  |  |  | `DateTime` |  | Updated At |  |  | S/4 only entity — no ECC CDC mapping |
| `LastChangeTime` |  |  |  | `DateTime` |  | Updated At |  |  | S/4 only entity — no ECC CDC mapping |
| `HierarchyShortID` |  |  |  | `String(20)` |  | Hierarchy ID |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `FunctionalAreaHierarchyNode`

- **ABAP Name:** `I_FunctionalAreaHierNode`
- **Label:** Functional Area Hierarchy Node
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `FunctionalAreaHierarchy` |  |  |  | `String(42)` | Y | Func. Area Hierarchy |  | _Hierarchy | S/4 only entity — no ECC CDC mapping |
| `HierarchyNode` |  |  |  | `String(50)` | Y | Node |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityEndDate` |  |  |  | `Date` | Y | Validity End Date |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityStartDate` |  |  |  | `Date` |  | Validity Start Date |  |  | S/4 only entity — no ECC CDC mapping |
| `ParentNode` |  |  |  | `String(50)` |  | Par. Node |  |  | S/4 only entity — no ECC CDC mapping |
| `HierarchyVersion` |  |  |  | `String(15)` |  | Version |  |  | S/4 only entity — no ECC CDC mapping |
| `FunctionalArea` |  |  |  | `String(16)` |  | Functional Area |  | _FunctionalArea | S/4 only entity — no ECC CDC mapping |
| `SequenceNumber` |  |  |  | `String(56)` |  |  |  |  | S/4 only entity — no ECC CDC mapping |
| `HierarchyNodeSequence` |  |  |  | `String(6)` |  | Sequence Number |  |  | S/4 only entity — no ECC CDC mapping |
| `HierarchyNodeLevel` |  |  |  | `String(6)` |  | Hierarchy Level |  |  | S/4 only entity — no ECC CDC mapping |
| `NodeType` |  |  |  | `String(1)` |  | Node Type |  |  | S/4 only entity — no ECC CDC mapping |
| `HierarchyNodeVal` |  |  |  | `String(40)` |  | Value |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `FunctionalAreaHierarchyText`

- **ABAP Name:** `I_FunctionalAreaHierarchyT`
- **Label:** Functional Area Hierarchy - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `FunctionalAreaHierarchy` |  |  |  | `String(42)` | Y | Func. Area Hierarchy |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityEndDate` |  |  |  | `Date` | Y | Validity End Date |  |  | S/4 only entity — no ECC CDC mapping |
| `Language` |  |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityStartDate` |  |  |  | `Date` |  | Validity Start Date |  |  | S/4 only entity — no ECC CDC mapping |
| `FunctionalAreaHierarchyName` |  |  |  | `String(50)` |  | Description |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `FunctionalAreaText`

- **ABAP Name:** `I_FunctionalAreaText`
- **Label:** Functional Area - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Language` |  |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `FunctionalArea` |  |  |  | `String(16)` | Y | Functional Area |  |  | S/4 only entity — no ECC CDC mapping |
| `FunctionalAreaName` |  |  |  | `String(25)` |  | Functional Area Name |  |  | S/4 only entity — no ECC CDC mapping |
