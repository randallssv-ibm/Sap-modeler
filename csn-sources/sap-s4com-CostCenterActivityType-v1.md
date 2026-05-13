# CostCenterActivityType

> Source file: `sap-s4com-CostCenterActivityType-v1.json`


## Entity: `CostCenterActivityType`

- **ABAP CDS Name:** `I_CostCenterActivityType`
- **Label:** Cost Center Activity Type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** CSLA, CSLT

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `ControllingArea` | `FIS_KOKRS` |  |  |  |  | `String(4)` | Y | Controlling Area |  |  |
| `CostCtrActivityType` | `LSTAR` |  |  |  |  | `String(6)` | Y | Activity Type |  |  |
| `ValidityEndDate` | `DATBI` |  |  |  |  | `Date` | Y | Valid To |  |  |
| `ValidityStartDate` | `DATAB` |  |  |  |  | `Date` |  | Valid From |  |  |
| `CostCtrActivityTypeQtyUnit` | `LEINH` |  |  |  |  | `String(3)` |  | Activity Unit |  |  |
| `CostCtrActivityTypeCategory` | `LATYP` |  |  |  |  | `String(1)` |  | ATyp category |  |  |
| `AllocationCostElement` | `VKSTA` |  |  |  |  | `String(10)` |  | Allocation cost elem |  |  |
| `CostCtrActivityTypeOutpQtyUnit` | `AUSEH` |  |  |  |  | `String(3)` |  | Output Unit |  |  |
| `CreationDate` | `ERFDT` |  |  |  |  | `Date` |  | Entered On |  |  |
| `EnteredByUser` | `ERFNM` |  |  |  |  | `String(12)` |  | Created By |  |  |
| `CostOriginGroup` | `HRKFT` |  |  |  |  | `String(4)` |  | Origin Group |  |  |
| `ActlPostgCostCenterActyTypeCat` | `LATYPI` |  |  |  |  | `String(1)` |  | Actl Acty Type Cat. |  |  |
| `OutputQuantityFactor` | `AUSFK` |  |  |  |  | `Decimal(5,2)` |  | Output factor |  |  |
| `ActivityTypeIsBlocked` | `SPRKZ` |  |  |  |  | `Boolean` |  | Lock indicator |  |  |
| `FixedCostIsPredistributed` | `CO_FIXVO` |  |  |  |  | `Boolean` |  | PreDistFixCosts |  |  |
| `PriceAllocationMethod` | `TARKZ` |  |  |  |  | `String(3)` |  | Price indicator |  |  |
| `PeriodPriceIsAverage` | `CO_YRATE` |  |  |  |  | `Boolean` |  | Average price |  |  |
| `ActualPriceAllocationMethod` | `CO_TARKZ_I` |  |  |  |  | `String(3)` |  | Act. price indicator |  |  |
| `ActualQuantityIsSetManually` | `CO_MANIST` |  |  |  |  | `Boolean` |  | Actual qty set |  |  |
| `PlanQuantityIsSetManually` | `CO_MANPLAN` |  |  |  |  | `Boolean` |  | Plan qty set |  |  |
| `CostCtrActivityTypeValidCat` | `KSTTY` |  |  |  |  | `String(8)` |  | CCtr Categories |  |  |
| `CostCtrActyTypeIsCtrlgRlvtComp` |  |  |  |  |  | `Boolean` |  | Comp.RelevanceCO |  |  |
| `CostCtrActyTypeIsHumRsceRlvt` |  |  |  |  |  | `Boolean` |  | Comp. relevance, HR |  |  |


## Entity: `CostCenterActivityTypeCatText`

- **ABAP CDS Name:** `I_CostCenterActivityTypeCatT`
- **Label:** Category of Activity Type - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `CostCtrActivityTypeCategory` | `LATYP` |  |  |  |  | `String(1)` | Y | ATyp category |  | S/4 only entity |
| `Language` | `SPRAS` |  |  |  |  | `String(2)` | Y | Language Key |  | S/4 only entity |
| `CostCtrActivityTypeCatName` | `FIS_LATYP_TEXT` |  |  |  |  | `String(60)` |  | Act. Type Cat. Name |  | S/4 only entity |


## Entity: `CostCenterActivityTypeCategory`

- **ABAP CDS Name:** `I_CostCenterActivityTypeCat`
- **Label:** Cost Center Activity Type Category
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** CSLA

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `CostCtrActivityTypeCategory` | `LATYP` |  |  |  |  | `String(1)` | Y | ATyp category |  |  |


## Entity: `CostCenterActivityTypeText`

- **ABAP CDS Name:** `I_CostCenterActivityTypeText`
- **Label:** Cost Center Activity Type - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** CSLT

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `ValidityEndDate` | `DATBI` |  |  |  |  | `Date` | Y | Valid To |  |  |
| `ControllingArea` | `FIS_KOKRS` |  |  |  |  | `String(4)` | Y | Controlling Area |  |  |
| `CostCtrActivityType` | `LSTAR` |  |  |  |  | `String(6)` | Y | Activity Type |  |  |
| `Language` | `SPRAS` |  |  |  |  | `String(2)` | Y | Language Key |  |  |
| `CostCtrActivityTypeName` | `FIS_COSTCTRACTIVITYTYPENAME` |  |  |  |  | `String(20)` |  | Cost Center Activity Type Name |  |  |
| `CostCtrActivityTypeDesc` | `FIS_COSTCTRACTIVITYTYPEDESC` |  |  |  |  | `String(40)` |  | Cost Center Activity Type Description |  |  |
| `ValidityStartDate` | `DATAB` |  |  |  |  | `Date` |  | Valid From |  |  |
| `CostCtrActyTypeTxtSearchTerm` | `MCDS4` |  |  |  |  | `String(20)` |  | Act. Type Short Text |  |  |


## Entity: `CostCtrActivityTypeHierNdeText`

- **ABAP CDS Name:** `I_CostCtrActivityTypeHierNodeT`
- **Label:** CostCtr Activty Type Hierarchy Node - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** SETHEADERT

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `ControllingArea` | `FIS_KOKRS` |  |  |  |  | `String(4)` | Y | Controlling Area |  |  |
| `CostCtrActivityTypeHierarchy` | `FIS_HRYID_CCTRACTTYTPE` |  |  |  |  | `String(40)` | Y | Cctr Acttype Hryid |  |  |
| `HierarchyNode` | `HRYNODE` |  |  |  |  | `String(50)` | Y | Node |  |  |
| `ValidityEndDate` | `DATBI` |  |  |  |  | `Date` | Y | Valid To |  |  |
| `Language` | `SPRAS` |  |  |  |  | `String(2)` | Y | Language Key |  |  |
| `HierarchyNodeText` | `NODETXT` |  |  |  |  | `String(50)` |  | Description |  |  |
| `HierarchyNodeShortText` |  |  |  |  |  | `String(20)` |  |  |  |  |
| `ValidityStartDate` | `DATAB` |  |  |  |  | `Date` |  | Valid From |  |  |


## Entity: `CostCtrActivityTypeHierNode`

- **ABAP CDS Name:** `I_CostCtrActivityTypeHierNode`
- **Label:** Cost Center Activity Type Hierarchy Node
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** SETHEADER, SETNODE, SETLEAF

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `ControllingArea` | `FIS_KOKRS` |  |  |  |  | `String(4)` | Y | Controlling Area |  |  |
| `CostCtrActivityTypeHierarchy` | `FIS_HRYID_CCTRACTTYTPE` |  |  |  |  | `String(40)` | Y | Cctr Acttype Hryid |  |  |
| `HierarchyNode` | `HRYNODE` |  |  |  |  | `String(50)` | Y | Node |  |  |
| `ValidityEndDate` | `FIS_DATBI` |  |  |  |  | `Date` | Y | Validity End Date |  |  |
| `ParentNode` | `PARNODE` |  |  |  |  | `String(50)` |  | Par. Node |  |  |
| `HierarchyVersion` | `HRYVERSN` |  |  |  |  | `String(15)` |  | Version |  |  |
| `ValidityStartDate` | `FIS_DATAB` |  |  |  |  | `Date` |  | Validity Start Date |  |  |
| `CostCtrActivityType` | `LSTAR` |  |  |  |  | `String(6)` |  | Activity Type |  |  |
| `SequenceNumber` |  |  |  |  |  | `String(56)` |  |  |  |  |
| `HierarchyNodeSequence` | `HRYSEQNBR` |  |  |  |  | `String(6)` |  | Sequence Number |  |  |
| `HierarchyNodeLevel` | `HRYLEVEL` |  |  |  |  | `String(6)` |  | Hierarchy Level |  |  |
| `NodeType` | `NODETYP` |  |  |  |  | `String(1)` |  | Node Type |  |  |
| `HierarchyNodeVal` | `NODEVALUE` |  |  |  |  | `String(40)` |  | Value |  |  |


## Entity: `CostCtrActivityTypeHierText`

- **ABAP CDS Name:** `I_CostCtrActivityTypeHierText`
- **Label:** Activity Type Hierarchy - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** SETHEADERT

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `ControllingArea` | `HRYCLS` |  |  |  |  | `String(12)` | Y | Hierarchy Class |  |  |
| `CostCtrActivityTypeHierarchy` | `FIS_HRYID_CCTRACTTYTPE` |  |  |  |  | `String(40)` | Y | Cctr Acttype Hryid |  |  |
| `ValidityEndDate` | `DATBI` |  |  |  |  | `Date` | Y | Valid To |  |  |
| `Language` | `SPRAS` |  |  |  |  | `String(2)` | Y | Language Key |  |  |
| `ValidityStartDate` | `DATAB` |  |  |  |  | `Date` |  | Valid From |  |  |
| `CostCtrActivityTypeHierName` | `HRYTXT` |  |  |  |  | `String(50)` |  | Description |  |  |


## Entity: `CostCtrActivityTypeHierarchy`

- **ABAP CDS Name:** `I_CostCtrActivityTypeHierarchy`
- **Label:** Cost Center Activity Type Hierarchy
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** SETHEADER, SETHEADERT

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `ControllingArea` | `FIS_KOKRS` |  |  |  |  | `String(4)` | Y | Controlling Area |  |  |
| `CostCtrActivityTypeHierarchy` | `FIS_HRYID_CCTRACTTYTPE` |  |  |  |  | `String(40)` | Y | Cctr Acttype Hryid |  |  |
| `ValidityEndDate` | `FIS_DATBI` |  |  |  |  | `Date` | Y | Validity End Date |  |  |
| `ValidityStartDate` | `FIS_DATAB` |  |  |  |  | `Date` |  | Validity Start Date |  |  |
| `LastChangedByUser` | `UPNAM` |  |  |  |  | `String(12)` |  | Last Changed By |  |  |
| `LastChangeDateTime` | `HRYUPDTIME` |  |  |  |  | `DateTime` |  | Updated At |  |  |
| `LastChangeTime` | `HRYUPDTIME` |  |  |  |  | `DateTime` |  | Updated At |  |  |
| `HierarchyShortID` | `VHRID` |  |  |  |  | `String(20)` |  | Hierarchy ID |  |  |
