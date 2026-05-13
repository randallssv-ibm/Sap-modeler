# CostCenterActivityType

> Source file: `sap-s4com-CostCenterActivityType-v1.json`


## Entity: `CostCenterActivityType`

- **ABAP Name:** `I_CostCenterActivityType`
- **Label:** Cost Center Activity Type
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `ControllingArea` | `FIS_KOKRS` | `KOKRS` |  | `String(4)` | Y | Controlling Area |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCtrActivityType` | `LSTAR` | `LSTAR` |  | `String(6)` | Y | Activity Type |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityEndDate` | `DATBI` | `DATBI` |  | `Date` | Y | Valid To |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityStartDate` | `DATAB` | `DATAB` |  | `Date` |  | Valid From |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCtrActivityTypeQtyUnit` | `LEINH` | `LEINH` |  | `String(3)` |  | Activity Unit |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCtrActivityTypeCategory` | `LATYP` | `LATYP` |  | `String(1)` |  | ATyp category |  | _CostCtrActivityTypeCategory | S/4 only entity — no ECC CDC mapping |
| `AllocationCostElement` | `VKSTA` | `VKSTA` |  | `String(10)` |  | Allocation cost elem |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCtrActivityTypeOutpQtyUnit` | `AUSEH` | `AUSEH` |  | `String(3)` |  | Output Unit |  |  | S/4 only entity — no ECC CDC mapping |
| `CreationDate` | `ERFDT` | `ERFDT` |  | `Date` |  | Entered On |  |  | S/4 only entity — no ECC CDC mapping |
| `EnteredByUser` | `ERFNM` | `ERFNM` |  | `String(12)` |  | Created By |  |  | S/4 only entity — no ECC CDC mapping |
| `CostOriginGroup` | `HRKFT` | `HRKFT` |  | `String(4)` |  | Origin Group |  |  | S/4 only entity — no ECC CDC mapping |
| `ActlPostgCostCenterActyTypeCat` | `LATYPI` | `LATYPI` |  | `String(1)` |  | Actl Acty Type Cat. |  |  | S/4 only entity — no ECC CDC mapping |
| `OutputQuantityFactor` | `AUSFK` | `AUSFK` |  | `Decimal(5,2)` |  | Output factor |  |  | S/4 only entity — no ECC CDC mapping |
| `ActivityTypeIsBlocked` | `SPRKZ` | `SPRKZ` |  | `Boolean` |  | Lock indicator |  |  | S/4 only entity — no ECC CDC mapping |
| `FixedCostIsPredistributed` | `CO_FIXVO` | `CO_FIXVO` |  | `Boolean` |  | PreDistFixCosts |  |  | S/4 only entity — no ECC CDC mapping |
| `PriceAllocationMethod` | `TARKZ` | `TARKZ` |  | `String(3)` |  | Price indicator |  |  | S/4 only entity — no ECC CDC mapping |
| `PeriodPriceIsAverage` | `CO_YRATE` | `CO_YRATE` |  | `Boolean` |  | Average price |  |  | S/4 only entity — no ECC CDC mapping |
| `ActualPriceAllocationMethod` | `CO_TARKZ_I` | `CO_TARKZ_I` |  | `String(3)` |  | Act. price indicator |  |  | S/4 only entity — no ECC CDC mapping |
| `ActualQuantityIsSetManually` | `CO_MANIST` | `CO_MANIST` |  | `Boolean` |  | Actual qty set |  |  | S/4 only entity — no ECC CDC mapping |
| `PlanQuantityIsSetManually` | `CO_MANPLAN` | `CO_MANPLAN` |  | `Boolean` |  | Plan qty set |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCtrActivityTypeValidCat` | `KSTTY` | `KSTTY` |  | `String(8)` |  | CCtr Categories |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCtrActyTypeIsCtrlgRlvtComp` |  |  |  | `Boolean` |  | Comp.RelevanceCO |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCtrActyTypeIsHumRsceRlvt` |  |  |  | `Boolean` |  | Comp. relevance, HR |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `CostCenterActivityTypeCatText`

- **ABAP Name:** `I_CostCenterActivityTypeCatT`
- **Label:** Category of Activity Type - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `CostCtrActivityTypeCategory` | `LATYP` | `LATYP` |  | `String(1)` | Y | ATyp category |  |  | S/4 only entity — no ECC CDC mapping |
| `Language` | `SPRAS` | `SPRAS` |  | `String(2)` | Y | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCtrActivityTypeCatName` | `FIS_LATYP_TEXT` | `LATYP_TEXT` |  | `String(60)` |  | Act. Type Cat. Name |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `CostCenterActivityTypeCategory`

- **ABAP Name:** `I_CostCenterActivityTypeCat`
- **Label:** Cost Center Activity Type Category
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `CostCtrActivityTypeCategory` | `LATYP` | `LATYP` |  | `String(1)` | Y | ATyp category |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `CostCenterActivityTypeText`

- **ABAP Name:** `I_CostCenterActivityTypeText`
- **Label:** Cost Center Activity Type - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `ValidityEndDate` | `DATBI` | `DATBI` |  | `Date` | Y | Valid To |  |  | S/4 only entity — no ECC CDC mapping |
| `ControllingArea` | `FIS_KOKRS` | `KOKRS` |  | `String(4)` | Y | Controlling Area |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCtrActivityType` | `LSTAR` | `LSTAR` |  | `String(6)` | Y | Activity Type |  |  | S/4 only entity — no ECC CDC mapping |
| `Language` | `SPRAS` | `SPRAS` |  | `String(2)` | Y | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCtrActivityTypeName` | `FIS_COSTCTRACTIVITYTYPENAME` | `COSTCTRACTIVITYTYPENAME` |  | `String(20)` |  | Cost Center Activity Type Name |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCtrActivityTypeDesc` | `FIS_COSTCTRACTIVITYTYPEDESC` | `COSTCTRACTIVITYTYPEDESC` |  | `String(40)` |  | Cost Center Activity Type Description |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityStartDate` | `DATAB` | `DATAB` |  | `Date` |  | Valid From |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCtrActyTypeTxtSearchTerm` | `MCDS4` | `MCDS4` |  | `String(20)` |  | Act. Type Short Text |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `CostCtrActivityTypeHierNdeText`

- **ABAP Name:** `I_CostCtrActivityTypeHierNodeT`
- **Label:** CostCtr Activty Type Hierarchy Node - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `ControllingArea` | `FIS_KOKRS` | `KOKRS` |  | `String(4)` | Y | Controlling Area |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCtrActivityTypeHierarchy` | `FIS_HRYID_CCTRACTTYTPE` | `HRYID_CCTRACTTYTPE` |  | `String(40)` | Y | Cctr Acttype Hryid |  | _Hierarchy | S/4 only entity — no ECC CDC mapping |
| `HierarchyNode` | `HRYNODE` | `HRYNODE` |  | `String(50)` | Y | Node |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityEndDate` | `DATBI` | `DATBI` |  | `Date` | Y | Valid To |  |  | S/4 only entity — no ECC CDC mapping |
| `Language` | `SPRAS` | `SPRAS` |  | `String(2)` | Y | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `HierarchyNodeText` | `NODETXT` | `NODETXT` |  | `String(50)` |  | Description |  |  | S/4 only entity — no ECC CDC mapping |
| `HierarchyNodeShortText` |  |  |  | `String(20)` |  |  |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityStartDate` | `DATAB` | `DATAB` |  | `Date` |  | Valid From |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `CostCtrActivityTypeHierNode`

- **ABAP Name:** `I_CostCtrActivityTypeHierNode`
- **Label:** Cost Center Activity Type Hierarchy Node
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `ControllingArea` | `FIS_KOKRS` | `KOKRS` |  | `String(4)` | Y | Controlling Area |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCtrActivityTypeHierarchy` | `FIS_HRYID_CCTRACTTYTPE` | `HRYID_CCTRACTTYTPE` |  | `String(40)` | Y | Cctr Acttype Hryid |  | _Hierarchy | S/4 only entity — no ECC CDC mapping |
| `HierarchyNode` | `HRYNODE` | `HRYNODE` |  | `String(50)` | Y | Node |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityEndDate` | `FIS_DATBI` | `DATBI` |  | `Date` | Y | Validity End Date |  |  | S/4 only entity — no ECC CDC mapping |
| `ParentNode` | `PARNODE` | `PARNODE` |  | `String(50)` |  | Par. Node |  |  | S/4 only entity — no ECC CDC mapping |
| `HierarchyVersion` | `HRYVERSN` | `HRYVERSN` |  | `String(15)` |  | Version |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityStartDate` | `FIS_DATAB` | `DATAB` |  | `Date` |  | Validity Start Date |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCtrActivityType` | `LSTAR` | `LSTAR` |  | `String(6)` |  | Activity Type |  | _CostCenterActivity | S/4 only entity — no ECC CDC mapping |
| `SequenceNumber` |  |  |  | `String(56)` |  |  |  |  | S/4 only entity — no ECC CDC mapping |
| `HierarchyNodeSequence` | `HRYSEQNBR` | `HRYSEQNBR` |  | `String(6)` |  | Sequence Number |  |  | S/4 only entity — no ECC CDC mapping |
| `HierarchyNodeLevel` | `HRYLEVEL` | `HRYLEVEL` |  | `String(6)` |  | Hierarchy Level |  |  | S/4 only entity — no ECC CDC mapping |
| `NodeType` | `NODETYP` | `NODETYP` |  | `String(1)` |  | Node Type |  |  | S/4 only entity — no ECC CDC mapping |
| `HierarchyNodeVal` | `NODEVALUE` | `NODEVALUE` |  | `String(40)` |  | Value |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `CostCtrActivityTypeHierText`

- **ABAP Name:** `I_CostCtrActivityTypeHierText`
- **Label:** Activity Type Hierarchy - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `ControllingArea` | `HRYCLS` | `HRYCLS` |  | `String(12)` | Y | Hierarchy Class |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCtrActivityTypeHierarchy` | `FIS_HRYID_CCTRACTTYTPE` | `HRYID_CCTRACTTYTPE` |  | `String(40)` | Y | Cctr Acttype Hryid |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityEndDate` | `DATBI` | `DATBI` |  | `Date` | Y | Valid To |  |  | S/4 only entity — no ECC CDC mapping |
| `Language` | `SPRAS` | `SPRAS` |  | `String(2)` | Y | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityStartDate` | `DATAB` | `DATAB` |  | `Date` |  | Valid From |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCtrActivityTypeHierName` | `HRYTXT` | `HRYTXT` |  | `String(50)` |  | Description |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `CostCtrActivityTypeHierarchy`

- **ABAP Name:** `I_CostCtrActivityTypeHierarchy`
- **Label:** Cost Center Activity Type Hierarchy
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `ControllingArea` | `FIS_KOKRS` | `KOKRS` |  | `String(4)` | Y | Controlling Area |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCtrActivityTypeHierarchy` | `FIS_HRYID_CCTRACTTYTPE` | `HRYID_CCTRACTTYTPE` |  | `String(40)` | Y | Cctr Acttype Hryid |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityEndDate` | `FIS_DATBI` | `DATBI` |  | `Date` | Y | Validity End Date |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityStartDate` | `FIS_DATAB` | `DATAB` |  | `Date` |  | Validity Start Date |  |  | S/4 only entity — no ECC CDC mapping |
| `LastChangedByUser` | `UPNAM` | `UPNAM` |  | `String(12)` |  | Last Changed By |  |  | S/4 only entity — no ECC CDC mapping |
| `LastChangeDateTime` | `HRYUPDTIME` | `HRYUPDTIME` |  | `DateTime` |  | Updated At |  |  | S/4 only entity — no ECC CDC mapping |
| `LastChangeTime` | `HRYUPDTIME` | `HRYUPDTIME` |  | `DateTime` |  | Updated At |  |  | S/4 only entity — no ECC CDC mapping |
| `HierarchyShortID` | `VHRID` | `VHRID` |  | `String(20)` |  | Hierarchy ID |  |  | S/4 only entity — no ECC CDC mapping |
