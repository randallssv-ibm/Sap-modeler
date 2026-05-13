# CostCenterActivityType

> Source file: `sap-s4com-CostCenterActivityType-v1.json`


## Entity: `CostCenterActivityType`

- **ABAP Name:** `I_CostCenterActivityType`
- **Label:** Cost Center Activity Type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `ControllingArea` | `TKA01` | `KOKRS` | `String(4)` | Y | Controlling Area |  |  |  |
| `CostCtrActivityType` |  |  | `String(6)` | Y | Activity Type |  |  | S/4 only entity |
| `ValidityEndDate` |  |  | `Date` | Y | Valid To |  |  | S/4 only entity |
| `ValidityStartDate` |  |  | `Date` |  | Valid From |  |  | S/4 only entity |
| `CostCtrActivityTypeQtyUnit` |  |  | `String(3)` |  | Activity Unit |  |  | S/4 only entity |
| `CostCtrActivityTypeCategory` |  |  | `String(1)` |  | ATyp category |  | _CostCtrActivityTypeCategory | S/4 only entity |
| `AllocationCostElement` |  |  | `String(10)` |  | Allocation cost elem |  |  | S/4 only entity |
| `CostCtrActivityTypeOutpQtyUnit` |  |  | `String(3)` |  | Output Unit |  |  | S/4 only entity |
| `CreationDate` |  |  | `Date` |  | Entered On |  |  | S/4 only entity |
| `EnteredByUser` |  |  | `String(12)` |  | Created By |  |  | S/4 only entity |
| `CostOriginGroup` |  |  | `String(4)` |  | Origin Group |  |  | S/4 only entity |
| `ActlPostgCostCenterActyTypeCat` |  |  | `String(1)` |  | Actl Acty Type Cat. |  |  | S/4 only entity |
| `OutputQuantityFactor` |  |  | `Decimal(5,2)` |  | Output factor |  |  | S/4 only entity |
| `ActivityTypeIsBlocked` |  |  | `Boolean` |  | Lock indicator |  |  | S/4 only entity |
| `FixedCostIsPredistributed` |  |  | `Boolean` |  | PreDistFixCosts |  |  | S/4 only entity |
| `PriceAllocationMethod` |  |  | `String(3)` |  | Price indicator |  |  | S/4 only entity |
| `PeriodPriceIsAverage` |  |  | `Boolean` |  | Average price |  |  | S/4 only entity |
| `ActualPriceAllocationMethod` |  |  | `String(3)` |  | Act. price indicator |  |  | S/4 only entity |
| `ActualQuantityIsSetManually` |  |  | `Boolean` |  | Actual qty set |  |  | S/4 only entity |
| `PlanQuantityIsSetManually` |  |  | `Boolean` |  | Plan qty set |  |  | S/4 only entity |
| `CostCtrActivityTypeValidCat` |  |  | `String(8)` |  | CCtr Categories |  |  | S/4 only entity |
| `CostCtrActyTypeIsCtrlgRlvtComp` |  |  | `Boolean` |  | Comp.RelevanceCO |  |  | S/4 only entity |
| `CostCtrActyTypeIsHumRsceRlvt` |  |  | `Boolean` |  | Comp. relevance, HR |  |  | S/4 only entity |


## Entity: `CostCenterActivityTypeCatText`

- **ABAP Name:** `I_CostCenterActivityTypeCatT`
- **Label:** Category of Activity Type - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `CostCtrActivityTypeCategory` |  |  | `String(1)` | Y | ATyp category |  |  | S/4 only entity |
| `Language` |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity |
| `CostCtrActivityTypeCatName` |  |  | `String(60)` |  | Act. Type Cat. Name |  |  | S/4 only entity |


## Entity: `CostCenterActivityTypeCategory`

- **ABAP Name:** `I_CostCenterActivityTypeCat`
- **Label:** Cost Center Activity Type Category
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `CostCtrActivityTypeCategory` |  |  | `String(1)` | Y | ATyp category |  |  | S/4 only entity |


## Entity: `CostCenterActivityTypeText`

- **ABAP Name:** `I_CostCenterActivityTypeText`
- **Label:** Cost Center Activity Type - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `ValidityEndDate` |  |  | `Date` | Y | Valid To |  |  | S/4 only entity |
| `ControllingArea` | `TKA01` | `KOKRS` | `String(4)` | Y | Controlling Area |  |  |  |
| `CostCtrActivityType` |  |  | `String(6)` | Y | Activity Type |  |  | S/4 only entity |
| `Language` |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity |
| `CostCtrActivityTypeName` |  |  | `String(20)` |  | Cost Center Activity Type Name |  |  | S/4 only entity |
| `CostCtrActivityTypeDesc` |  |  | `String(40)` |  | Cost Center Activity Type Description |  |  | S/4 only entity |
| `ValidityStartDate` |  |  | `Date` |  | Valid From |  |  | S/4 only entity |
| `CostCtrActyTypeTxtSearchTerm` |  |  | `String(20)` |  | Act. Type Short Text |  |  | S/4 only entity |


## Entity: `CostCtrActivityTypeHierNdeText`

- **ABAP Name:** `I_CostCtrActivityTypeHierNodeT`
- **Label:** CostCtr Activty Type Hierarchy Node - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `ControllingArea` | `TKA01` | `KOKRS` | `String(4)` | Y | Controlling Area |  |  |  |
| `CostCtrActivityTypeHierarchy` |  |  | `String(40)` | Y | Cctr Acttype Hryid |  | _Hierarchy | S/4 only entity |
| `HierarchyNode` |  |  | `String(50)` | Y | Node |  |  | S/4 only entity |
| `ValidityEndDate` |  |  | `Date` | Y | Valid To |  |  | S/4 only entity |
| `Language` |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity |
| `HierarchyNodeText` |  |  | `String(50)` |  | Description |  |  | S/4 only entity |
| `HierarchyNodeShortText` |  |  | `String(20)` |  |  |  |  | S/4 only entity |
| `ValidityStartDate` |  |  | `Date` |  | Valid From |  |  | S/4 only entity |


## Entity: `CostCtrActivityTypeHierNode`

- **ABAP Name:** `I_CostCtrActivityTypeHierNode`
- **Label:** Cost Center Activity Type Hierarchy Node
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `ControllingArea` | `TKA01` | `KOKRS` | `String(4)` | Y | Controlling Area |  |  |  |
| `CostCtrActivityTypeHierarchy` |  |  | `String(40)` | Y | Cctr Acttype Hryid |  | _Hierarchy | S/4 only entity |
| `HierarchyNode` |  |  | `String(50)` | Y | Node |  |  | S/4 only entity |
| `ValidityEndDate` |  |  | `Date` | Y | Validity End Date |  |  | S/4 only entity |
| `ParentNode` |  |  | `String(50)` |  | Par. Node |  |  | S/4 only entity |
| `HierarchyVersion` |  |  | `String(15)` |  | Version |  |  | S/4 only entity |
| `ValidityStartDate` |  |  | `Date` |  | Validity Start Date |  |  | S/4 only entity |
| `CostCtrActivityType` |  |  | `String(6)` |  | Activity Type |  | _CostCenterActivity | S/4 only entity |
| `SequenceNumber` |  |  | `String(56)` |  |  |  |  | S/4 only entity |
| `HierarchyNodeSequence` |  |  | `String(6)` |  | Sequence Number |  |  | S/4 only entity |
| `HierarchyNodeLevel` |  |  | `String(6)` |  | Hierarchy Level |  |  | S/4 only entity |
| `NodeType` |  |  | `String(1)` |  | Node Type |  |  | S/4 only entity |
| `HierarchyNodeVal` |  |  | `String(40)` |  | Value |  |  | S/4 only entity |


## Entity: `CostCtrActivityTypeHierText`

- **ABAP Name:** `I_CostCtrActivityTypeHierText`
- **Label:** Activity Type Hierarchy - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `ControllingArea` | `TKA01` | `KOKRS` | `String(12)` | Y | Hierarchy Class |  |  |  |
| `CostCtrActivityTypeHierarchy` |  |  | `String(40)` | Y | Cctr Acttype Hryid |  |  | S/4 only entity |
| `ValidityEndDate` |  |  | `Date` | Y | Valid To |  |  | S/4 only entity |
| `Language` |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity |
| `ValidityStartDate` |  |  | `Date` |  | Valid From |  |  | S/4 only entity |
| `CostCtrActivityTypeHierName` |  |  | `String(50)` |  | Description |  |  | S/4 only entity |


## Entity: `CostCtrActivityTypeHierarchy`

- **ABAP Name:** `I_CostCtrActivityTypeHierarchy`
- **Label:** Cost Center Activity Type Hierarchy
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `ControllingArea` | `TKA01` | `KOKRS` | `String(4)` | Y | Controlling Area |  |  |  |
| `CostCtrActivityTypeHierarchy` |  |  | `String(40)` | Y | Cctr Acttype Hryid |  |  | S/4 only entity |
| `ValidityEndDate` |  |  | `Date` | Y | Validity End Date |  |  | S/4 only entity |
| `ValidityStartDate` |  |  | `Date` |  | Validity Start Date |  |  | S/4 only entity |
| `LastChangedByUser` |  |  | `String(12)` |  | Last Changed By |  |  | S/4 only entity |
| `LastChangeDateTime` |  |  | `DateTime` |  | Updated At |  |  | S/4 only entity |
| `LastChangeTime` |  |  | `DateTime` |  | Updated At |  |  | S/4 only entity |
| `HierarchyShortID` |  |  | `String(20)` |  | Hierarchy ID |  |  | S/4 only entity |
