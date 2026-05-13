# CostCenterActivityType

> Source file: `sap-s4com-CostCenterActivityType-v1.json`


## Entity: `CostCenterActivityType`

- **ABAP CDS Name:** `I_CostCenterActivityType`
- **Label:** Cost Center Activity Type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `ControllingArea` | `FIS_KOKRS` |  |  |  |  | `String(4)` | Y | Controlling Area |  | S/4 only entity |
| `CostCtrActivityType` | `LSTAR` |  |  |  |  | `String(6)` | Y | Activity Type |  | S/4 only entity |
| `ValidityEndDate` | `DATBI` |  |  |  |  | `Date` | Y | Valid To |  | S/4 only entity |
| `ValidityStartDate` | `DATAB` |  |  |  |  | `Date` |  | Valid From |  | S/4 only entity |
| `CostCtrActivityTypeQtyUnit` | `LEINH` |  |  |  |  | `String(3)` |  | Activity Unit |  | S/4 only entity |
| `CostCtrActivityTypeCategory` | `LATYP` |  |  |  |  | `String(1)` |  | ATyp category |  | S/4 only entity |
| `AllocationCostElement` | `VKSTA` |  |  |  |  | `String(10)` |  | Allocation cost elem |  | S/4 only entity |
| `CostCtrActivityTypeOutpQtyUnit` | `AUSEH` |  |  |  |  | `String(3)` |  | Output Unit |  | S/4 only entity |
| `CreationDate` | `ERFDT` |  |  |  |  | `Date` |  | Entered On |  | S/4 only entity |
| `EnteredByUser` | `ERFNM` |  |  |  |  | `String(12)` |  | Created By |  | S/4 only entity |
| `CostOriginGroup` | `HRKFT` |  |  |  |  | `String(4)` |  | Origin Group |  | S/4 only entity |
| `ActlPostgCostCenterActyTypeCat` | `LATYPI` |  |  |  |  | `String(1)` |  | Actl Acty Type Cat. |  | S/4 only entity |
| `OutputQuantityFactor` | `AUSFK` |  |  |  |  | `Decimal(5,2)` |  | Output factor |  | S/4 only entity |
| `ActivityTypeIsBlocked` | `SPRKZ` |  |  |  |  | `Boolean` |  | Lock indicator |  | S/4 only entity |
| `FixedCostIsPredistributed` | `CO_FIXVO` |  |  |  |  | `Boolean` |  | PreDistFixCosts |  | S/4 only entity |
| `PriceAllocationMethod` | `TARKZ` |  |  |  |  | `String(3)` |  | Price indicator |  | S/4 only entity |
| `PeriodPriceIsAverage` | `CO_YRATE` |  |  |  |  | `Boolean` |  | Average price |  | S/4 only entity |
| `ActualPriceAllocationMethod` | `CO_TARKZ_I` |  |  |  |  | `String(3)` |  | Act. price indicator |  | S/4 only entity |
| `ActualQuantityIsSetManually` | `CO_MANIST` |  |  |  |  | `Boolean` |  | Actual qty set |  | S/4 only entity |
| `PlanQuantityIsSetManually` | `CO_MANPLAN` |  |  |  |  | `Boolean` |  | Plan qty set |  | S/4 only entity |
| `CostCtrActivityTypeValidCat` | `KSTTY` |  |  |  |  | `String(8)` |  | CCtr Categories |  | S/4 only entity |
| `CostCtrActyTypeIsCtrlgRlvtComp` |  |  |  |  |  | `Boolean` |  | Comp.RelevanceCO |  | S/4 only entity |
| `CostCtrActyTypeIsHumRsceRlvt` |  |  |  |  |  | `Boolean` |  | Comp. relevance, HR |  | S/4 only entity |


## Entity: `CostCenterActivityTypeCatText`

- **ABAP CDS Name:** `I_CostCenterActivityTypeCatT`
- **Label:** Category of Activity Type - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `CostCtrActivityTypeCategory` | `LATYP` |  |  |  |  | `String(1)` | Y | ATyp category |  | S/4 only entity |
| `Language` | `SPRAS` |  |  |  |  | `String(2)` | Y | Language Key |  | S/4 only entity |
| `CostCtrActivityTypeCatName` | `FIS_LATYP_TEXT` |  |  |  |  | `String(60)` |  | Act. Type Cat. Name |  | S/4 only entity |


## Entity: `CostCenterActivityTypeCategory`

- **ABAP CDS Name:** `I_CostCenterActivityTypeCat`
- **Label:** Cost Center Activity Type Category
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `CostCtrActivityTypeCategory` | `LATYP` |  |  |  |  | `String(1)` | Y | ATyp category |  | S/4 only entity |


## Entity: `CostCenterActivityTypeText`

- **ABAP CDS Name:** `I_CostCenterActivityTypeText`
- **Label:** Cost Center Activity Type - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `ValidityEndDate` | `DATBI` |  |  |  |  | `Date` | Y | Valid To |  | S/4 only entity |
| `ControllingArea` | `FIS_KOKRS` |  |  |  |  | `String(4)` | Y | Controlling Area |  | S/4 only entity |
| `CostCtrActivityType` | `LSTAR` |  |  |  |  | `String(6)` | Y | Activity Type |  | S/4 only entity |
| `Language` | `SPRAS` |  |  |  |  | `String(2)` | Y | Language Key |  | S/4 only entity |
| `CostCtrActivityTypeName` | `FIS_COSTCTRACTIVITYTYPENAME` |  |  |  |  | `String(20)` |  | Cost Center Activity Type Name |  | S/4 only entity |
| `CostCtrActivityTypeDesc` | `FIS_COSTCTRACTIVITYTYPEDESC` |  |  |  |  | `String(40)` |  | Cost Center Activity Type Description |  | S/4 only entity |
| `ValidityStartDate` | `DATAB` |  |  |  |  | `Date` |  | Valid From |  | S/4 only entity |
| `CostCtrActyTypeTxtSearchTerm` | `MCDS4` |  |  |  |  | `String(20)` |  | Act. Type Short Text |  | S/4 only entity |


## Entity: `CostCtrActivityTypeHierNdeText`

- **ABAP CDS Name:** `I_CostCtrActivityTypeHierNodeT`
- **Label:** CostCtr Activty Type Hierarchy Node - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `ControllingArea` | `FIS_KOKRS` |  |  |  |  | `String(4)` | Y | Controlling Area |  | S/4 only entity |
| `CostCtrActivityTypeHierarchy` | `FIS_HRYID_CCTRACTTYTPE` |  |  |  |  | `String(40)` | Y | Cctr Acttype Hryid |  | S/4 only entity |
| `HierarchyNode` | `HRYNODE` |  |  |  |  | `String(50)` | Y | Node |  | S/4 only entity |
| `ValidityEndDate` | `DATBI` |  |  |  |  | `Date` | Y | Valid To |  | S/4 only entity |
| `Language` | `SPRAS` |  |  |  |  | `String(2)` | Y | Language Key |  | S/4 only entity |
| `HierarchyNodeText` | `NODETXT` |  |  |  |  | `String(50)` |  | Description |  | S/4 only entity |
| `HierarchyNodeShortText` |  |  |  |  |  | `String(20)` |  |  |  | S/4 only entity |
| `ValidityStartDate` | `DATAB` |  |  |  |  | `Date` |  | Valid From |  | S/4 only entity |


## Entity: `CostCtrActivityTypeHierNode`

- **ABAP CDS Name:** `I_CostCtrActivityTypeHierNode`
- **Label:** Cost Center Activity Type Hierarchy Node
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `ControllingArea` | `FIS_KOKRS` |  |  |  |  | `String(4)` | Y | Controlling Area |  | S/4 only entity |
| `CostCtrActivityTypeHierarchy` | `FIS_HRYID_CCTRACTTYTPE` |  |  |  |  | `String(40)` | Y | Cctr Acttype Hryid |  | S/4 only entity |
| `HierarchyNode` | `HRYNODE` |  |  |  |  | `String(50)` | Y | Node |  | S/4 only entity |
| `ValidityEndDate` | `FIS_DATBI` |  |  |  |  | `Date` | Y | Validity End Date |  | S/4 only entity |
| `ParentNode` | `PARNODE` |  |  |  |  | `String(50)` |  | Par. Node |  | S/4 only entity |
| `HierarchyVersion` | `HRYVERSN` |  |  |  |  | `String(15)` |  | Version |  | S/4 only entity |
| `ValidityStartDate` | `FIS_DATAB` |  |  |  |  | `Date` |  | Validity Start Date |  | S/4 only entity |
| `CostCtrActivityType` | `LSTAR` |  |  |  |  | `String(6)` |  | Activity Type |  | S/4 only entity |
| `SequenceNumber` |  |  |  |  |  | `String(56)` |  |  |  | S/4 only entity |
| `HierarchyNodeSequence` | `HRYSEQNBR` |  |  |  |  | `String(6)` |  | Sequence Number |  | S/4 only entity |
| `HierarchyNodeLevel` | `HRYLEVEL` |  |  |  |  | `String(6)` |  | Hierarchy Level |  | S/4 only entity |
| `NodeType` | `NODETYP` |  |  |  |  | `String(1)` |  | Node Type |  | S/4 only entity |
| `HierarchyNodeVal` | `NODEVALUE` |  |  |  |  | `String(40)` |  | Value |  | S/4 only entity |


## Entity: `CostCtrActivityTypeHierText`

- **ABAP CDS Name:** `I_CostCtrActivityTypeHierText`
- **Label:** Activity Type Hierarchy - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `ControllingArea` | `HRYCLS` |  |  |  |  | `String(12)` | Y | Hierarchy Class |  | S/4 only entity |
| `CostCtrActivityTypeHierarchy` | `FIS_HRYID_CCTRACTTYTPE` |  |  |  |  | `String(40)` | Y | Cctr Acttype Hryid |  | S/4 only entity |
| `ValidityEndDate` | `DATBI` |  |  |  |  | `Date` | Y | Valid To |  | S/4 only entity |
| `Language` | `SPRAS` |  |  |  |  | `String(2)` | Y | Language Key |  | S/4 only entity |
| `ValidityStartDate` | `DATAB` |  |  |  |  | `Date` |  | Valid From |  | S/4 only entity |
| `CostCtrActivityTypeHierName` | `HRYTXT` |  |  |  |  | `String(50)` |  | Description |  | S/4 only entity |


## Entity: `CostCtrActivityTypeHierarchy`

- **ABAP CDS Name:** `I_CostCtrActivityTypeHierarchy`
- **Label:** Cost Center Activity Type Hierarchy
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `ControllingArea` | `FIS_KOKRS` |  |  |  |  | `String(4)` | Y | Controlling Area |  | S/4 only entity |
| `CostCtrActivityTypeHierarchy` | `FIS_HRYID_CCTRACTTYTPE` |  |  |  |  | `String(40)` | Y | Cctr Acttype Hryid |  | S/4 only entity |
| `ValidityEndDate` | `FIS_DATBI` |  |  |  |  | `Date` | Y | Validity End Date |  | S/4 only entity |
| `ValidityStartDate` | `FIS_DATAB` |  |  |  |  | `Date` |  | Validity Start Date |  | S/4 only entity |
| `LastChangedByUser` | `UPNAM` |  |  |  |  | `String(12)` |  | Last Changed By |  | S/4 only entity |
| `LastChangeDateTime` | `HRYUPDTIME` |  |  |  |  | `DateTime` |  | Updated At |  | S/4 only entity |
| `LastChangeTime` | `HRYUPDTIME` |  |  |  |  | `DateTime` |  | Updated At |  | S/4 only entity |
| `HierarchyShortID` | `VHRID` |  |  |  |  | `String(20)` |  | Hierarchy ID |  | S/4 only entity |
