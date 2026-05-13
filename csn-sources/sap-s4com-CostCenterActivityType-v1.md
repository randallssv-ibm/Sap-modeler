# CostCenterActivityType

> Source file: `sap-s4com-CostCenterActivityType-v1.json`


## Entity: `CostCenterActivityType`

- **ABAP Name:** `I_CostCenterActivityType`
- **Label:** Cost Center Activity Type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `ControllingArea` | `ControllingArea` | `String(4)` | Y | Controlling Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCtrActivityType` | `CostCtrActivityType` | `String(6)` | Y | Activity Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityEndDate` | `ValidityEndDate` | `Date` | Y | Valid To |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityStartDate` | `ValidityStartDate` | `Date` |  | Valid From |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCtrActivityTypeQtyUnit` | `CostCtrActivityTypeQtyUnit` | `String(3)` |  | Activity Unit |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCtrActivityTypeCategory` | `CostCtrActivityTypeCategory` | `String(1)` |  | ATyp category |  | _CostCtrActivityTypeCategory | S/4 only entity (no ECC CDC mapping) |
| `AllocationCostElement` | `AllocationCostElement` | `String(10)` |  | Allocation cost elem |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCtrActivityTypeOutpQtyUnit` | `CostCtrActivityTypeOutpQtyUnit` | `String(3)` |  | Output Unit |  |  | S/4 only entity (no ECC CDC mapping) |
| `CreationDate` | `CreationDate` | `Date` |  | Entered On |  |  | S/4 only entity (no ECC CDC mapping) |
| `EnteredByUser` | `EnteredByUser` | `String(12)` |  | Created By |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostOriginGroup` | `CostOriginGroup` | `String(4)` |  | Origin Group |  |  | S/4 only entity (no ECC CDC mapping) |
| `ActlPostgCostCenterActyTypeCat` | `ActlPostgCostCenterActyTypeCat` | `String(1)` |  | Actl Acty Type Cat. |  |  | S/4 only entity (no ECC CDC mapping) |
| `OutputQuantityFactor` | `OutputQuantityFactor` | `Decimal(5,2)` |  | Output factor |  |  | S/4 only entity (no ECC CDC mapping) |
| `ActivityTypeIsBlocked` | `ActivityTypeIsBlocked` | `Boolean` |  | Lock indicator |  |  | S/4 only entity (no ECC CDC mapping) |
| `FixedCostIsPredistributed` | `FixedCostIsPredistributed` | `Boolean` |  | PreDistFixCosts |  |  | S/4 only entity (no ECC CDC mapping) |
| `PriceAllocationMethod` | `PriceAllocationMethod` | `String(3)` |  | Price indicator |  |  | S/4 only entity (no ECC CDC mapping) |
| `PeriodPriceIsAverage` | `PeriodPriceIsAverage` | `Boolean` |  | Average price |  |  | S/4 only entity (no ECC CDC mapping) |
| `ActualPriceAllocationMethod` | `ActualPriceAllocationMethod` | `String(3)` |  | Act. price indicator |  |  | S/4 only entity (no ECC CDC mapping) |
| `ActualQuantityIsSetManually` | `ActualQuantityIsSetManually` | `Boolean` |  | Actual qty set |  |  | S/4 only entity (no ECC CDC mapping) |
| `PlanQuantityIsSetManually` | `PlanQuantityIsSetManually` | `Boolean` |  | Plan qty set |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCtrActivityTypeValidCat` | `CostCtrActivityTypeValidCat` | `String(8)` |  | CCtr Categories |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCtrActyTypeIsCtrlgRlvtComp` | `CostCtrActyTypeIsCtrlgRlvtComp` | `Boolean` |  | Comp.RelevanceCO |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCtrActyTypeIsHumRsceRlvt` | `CostCtrActyTypeIsHumRsceRlvt` | `Boolean` |  | Comp. relevance, HR |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `CostCenterActivityTypeCatText`

- **ABAP Name:** `I_CostCenterActivityTypeCatT`
- **Label:** Category of Activity Type - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `CostCtrActivityTypeCategory` | `CostCtrActivityTypeCategory` | `String(1)` | Y | ATyp category |  |  | S/4 only entity (no ECC CDC mapping) |
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCtrActivityTypeCatName` | `CostCtrActivityTypeCatName` | `String(60)` |  | Act. Type Cat. Name |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `CostCenterActivityTypeCategory`

- **ABAP Name:** `I_CostCenterActivityTypeCat`
- **Label:** Cost Center Activity Type Category
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `CostCtrActivityTypeCategory` | `CostCtrActivityTypeCategory` | `String(1)` | Y | ATyp category |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `CostCenterActivityTypeText`

- **ABAP Name:** `I_CostCenterActivityTypeText`
- **Label:** Cost Center Activity Type - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `ValidityEndDate` | `ValidityEndDate` | `Date` | Y | Valid To |  |  | S/4 only entity (no ECC CDC mapping) |
| `ControllingArea` | `ControllingArea` | `String(4)` | Y | Controlling Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCtrActivityType` | `CostCtrActivityType` | `String(6)` | Y | Activity Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCtrActivityTypeName` | `CostCtrActivityTypeName` | `String(20)` |  | Cost Center Activity Type Name |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCtrActivityTypeDesc` | `CostCtrActivityTypeDesc` | `String(40)` |  | Cost Center Activity Type Description |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityStartDate` | `ValidityStartDate` | `Date` |  | Valid From |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCtrActyTypeTxtSearchTerm` | `CostCtrActyTypeTxtSearchTerm` | `String(20)` |  | Act. Type Short Text |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `CostCtrActivityTypeHierNdeText`

- **ABAP Name:** `I_CostCtrActivityTypeHierNodeT`
- **Label:** CostCtr Activty Type Hierarchy Node - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `ControllingArea` | `ControllingArea` | `String(4)` | Y | Controlling Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCtrActivityTypeHierarchy` | `CostCtrActivityTypeHierarchy` | `String(40)` | Y | Cctr Acttype Hryid |  | _Hierarchy | S/4 only entity (no ECC CDC mapping) |
| `HierarchyNode` | `HierarchyNode` | `String(50)` | Y | Node |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityEndDate` | `ValidityEndDate` | `Date` | Y | Valid To |  |  | S/4 only entity (no ECC CDC mapping) |
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `HierarchyNodeText` | `HierarchyNodeText` | `String(50)` |  | Description |  |  | S/4 only entity (no ECC CDC mapping) |
| `HierarchyNodeShortText` | `HierarchyNodeShortText` | `String(20)` |  |  |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityStartDate` | `ValidityStartDate` | `Date` |  | Valid From |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `CostCtrActivityTypeHierNode`

- **ABAP Name:** `I_CostCtrActivityTypeHierNode`
- **Label:** Cost Center Activity Type Hierarchy Node
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `ControllingArea` | `ControllingArea` | `String(4)` | Y | Controlling Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCtrActivityTypeHierarchy` | `CostCtrActivityTypeHierarchy` | `String(40)` | Y | Cctr Acttype Hryid |  | _Hierarchy | S/4 only entity (no ECC CDC mapping) |
| `HierarchyNode` | `HierarchyNode` | `String(50)` | Y | Node |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityEndDate` | `ValidityEndDate` | `Date` | Y | Validity End Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `ParentNode` | `ParentNode` | `String(50)` |  | Par. Node |  |  | S/4 only entity (no ECC CDC mapping) |
| `HierarchyVersion` | `HierarchyVersion` | `String(15)` |  | Version |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityStartDate` | `ValidityStartDate` | `Date` |  | Validity Start Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCtrActivityType` | `CostCtrActivityType` | `String(6)` |  | Activity Type |  | _CostCenterActivity | S/4 only entity (no ECC CDC mapping) |
| `SequenceNumber` | `SequenceNumber` | `String(56)` |  |  |  |  | S/4 only entity (no ECC CDC mapping) |
| `HierarchyNodeSequence` | `HierarchyNodeSequence` | `String(6)` |  | Sequence Number |  |  | S/4 only entity (no ECC CDC mapping) |
| `HierarchyNodeLevel` | `HierarchyNodeLevel` | `String(6)` |  | Hierarchy Level |  |  | S/4 only entity (no ECC CDC mapping) |
| `NodeType` | `NodeType` | `String(1)` |  | Node Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `HierarchyNodeVal` | `HierarchyNodeVal` | `String(40)` |  | Value |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `CostCtrActivityTypeHierText`

- **ABAP Name:** `I_CostCtrActivityTypeHierText`
- **Label:** Activity Type Hierarchy - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `ControllingArea` | `ControllingArea` | `String(12)` | Y | Hierarchy Class |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCtrActivityTypeHierarchy` | `CostCtrActivityTypeHierarchy` | `String(40)` | Y | Cctr Acttype Hryid |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityEndDate` | `ValidityEndDate` | `Date` | Y | Valid To |  |  | S/4 only entity (no ECC CDC mapping) |
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityStartDate` | `ValidityStartDate` | `Date` |  | Valid From |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCtrActivityTypeHierName` | `CostCtrActivityTypeHierName` | `String(50)` |  | Description |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `CostCtrActivityTypeHierarchy`

- **ABAP Name:** `I_CostCtrActivityTypeHierarchy`
- **Label:** Cost Center Activity Type Hierarchy
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `ControllingArea` | `ControllingArea` | `String(4)` | Y | Controlling Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCtrActivityTypeHierarchy` | `CostCtrActivityTypeHierarchy` | `String(40)` | Y | Cctr Acttype Hryid |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityEndDate` | `ValidityEndDate` | `Date` | Y | Validity End Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityStartDate` | `ValidityStartDate` | `Date` |  | Validity Start Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `LastChangedByUser` | `LastChangedByUser` | `String(12)` |  | Last Changed By |  |  | S/4 only entity (no ECC CDC mapping) |
| `LastChangeDateTime` | `LastChangeDateTime` | `DateTime` |  | Updated At |  |  | S/4 only entity (no ECC CDC mapping) |
| `LastChangeTime` | `LastChangeTime` | `DateTime` |  | Updated At |  |  | S/4 only entity (no ECC CDC mapping) |
| `HierarchyShortID` | `HierarchyShortID` | `String(20)` |  | Hierarchy ID |  |  | S/4 only entity (no ECC CDC mapping) |
