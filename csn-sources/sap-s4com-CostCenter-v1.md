# CostCenter

> Source file: `sap-s4com-CostCenter-v1.json`


## Entity: `CostCenter`

- **ABAP Name:** `I_CostCenter`
- **Label:** Cost Center
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `ControllingArea` |  |  |  | `String(4)` | Y | Controlling Area |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCenter` |  |  |  | `String(10)` | Y | Cost Center |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityEndDate` |  |  |  | `Date` | Y | Valid To |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityStartDate` |  |  |  | `Date` |  | Valid From |  |  | S/4 only entity — no ECC CDC mapping |
| `IsBlkdForPrimaryCostsPosting` |  |  |  | `Boolean` |  | Actual primary costs |  |  | S/4 only entity — no ECC CDC mapping |
| `IsBlockedForPlanPrimaryCosts` |  |  |  | `Boolean` |  | Plan primary costs |  |  | S/4 only entity — no ECC CDC mapping |
| `CompanyCode` |  |  |  | `String(4)` |  | Company Code |  |  | S/4 only entity — no ECC CDC mapping |
| `BusinessArea` |  |  |  | `String(4)` |  | Business Area |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCenterCategory` |  |  |  | `String(1)` |  | Cost Center Category |  | _CostCenterCategory | S/4 only entity — no ECC CDC mapping |
| `CostCtrResponsiblePersonName` |  |  |  | `String(20)` |  | Person Responsible |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCtrResponsibleUser` |  |  |  | `String(12)` |  | User Responsible |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCenterCurrency` |  |  |  | `String(5)` |  | Currency |  |  | S/4 only entity — no ECC CDC mapping |
| `CostingSheet` |  |  |  | `String(6)` |  | Costing Sheet |  |  | S/4 only entity — no ECC CDC mapping |
| `TaxJurisdiction` |  |  |  | `String(15)` |  | Tax Jurisdiction |  |  | S/4 only entity — no ECC CDC mapping |
| `ProfitCenter` |  |  |  | `String(10)` |  | Profit Center |  |  | S/4 only entity — no ECC CDC mapping |
| `Plant` |  |  |  | `String(4)` |  | Plant |  |  | S/4 only entity — no ECC CDC mapping |
| `LogicalSystem` |  |  |  | `String(10)` |  | Logical System |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCenterCreationDate` |  |  |  | `Date` |  | Entered On |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCenterCreatedByUser` |  |  |  | `String(12)` |  | Created By |  |  | S/4 only entity — no ECC CDC mapping |
| `IsBlkdForSecondaryCostsPosting` |  |  |  | `Boolean` |  | Actl Sec. Costs |  |  | S/4 only entity — no ECC CDC mapping |
| `IsBlockedForRevenuePosting` |  |  |  | `Boolean` |  | Actual Revenues |  |  | S/4 only entity — no ECC CDC mapping |
| `IsBlockedForCommitmentPosting` |  |  |  | `Boolean` |  | Commitment Update |  |  | S/4 only entity — no ECC CDC mapping |
| `IsBlockedForPlanSecondaryCosts` |  |  |  | `Boolean` |  | Lock Plan Sec Costs |  |  | S/4 only entity — no ECC CDC mapping |
| `IsBlockedForPlanRevenues` |  |  |  | `Boolean` |  | Lock Planning Revn |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCenterAllocationMethod` |  |  |  | `String(2)` |  | Allocation Methods |  |  | S/4 only entity — no ECC CDC mapping |
| `ConsumptionQtyIsRecorded` |  |  |  | `Boolean` |  | Record Quantity |  |  | S/4 only entity — no ECC CDC mapping |
| `Department` |  |  |  | `String(12)` |  | Department |  |  | S/4 only entity — no ECC CDC mapping |
| `SubsequentCostCenter` |  |  |  | `String(10)` |  | Subsequent Cost Ctr. |  |  | S/4 only entity — no ECC CDC mapping |
| `ConditionUsage` |  |  |  | `String(1)` |  | Usage |  |  | S/4 only entity — no ECC CDC mapping |
| `ConditionApplication` |  |  |  | `String(2)` |  | Application |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCenterAccountingOverhead` |  |  |  | `String(6)` |  | Overhead Key |  |  | S/4 only entity — no ECC CDC mapping |
| `Country` |  |  |  | `String(3)` |  | Country/Region Key |  |  | S/4 only entity — no ECC CDC mapping |
| `FormOfAddress` |  |  |  | `String(15)` |  | Title |  |  | S/4 only entity — no ECC CDC mapping |
| `AddressName` |  |  |  | `String(35)` |  | Name |  |  | S/4 only entity — no ECC CDC mapping |
| `AddressAdditionalName` |  |  |  | `String(35)` |  | Name 2 |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCenterAddrName3` |  |  |  | `String(35)` |  | Name 3 |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCenterAddrName4` |  |  |  | `String(35)` |  | Name 4 |  |  | S/4 only entity — no ECC CDC mapping |
| `CityName` |  |  |  | `String(35)` |  | City |  |  | S/4 only entity — no ECC CDC mapping |
| `District` |  |  |  | `String(35)` |  | District |  |  | S/4 only entity — no ECC CDC mapping |
| `StreetAddressName` |  |  |  | `String(35)` |  | Street |  |  | S/4 only entity — no ECC CDC mapping |
| `POBox` |  |  |  | `String(10)` |  | PO Box |  |  | S/4 only entity — no ECC CDC mapping |
| `PostalCode` |  |  |  | `String(10)` |  | Postal Code |  |  | S/4 only entity — no ECC CDC mapping |
| `POBoxPostalCode` |  |  |  | `String(10)` |  | PO Box Postal Code |  |  | S/4 only entity — no ECC CDC mapping |
| `Region` |  |  |  | `String(3)` |  | Region |  |  | S/4 only entity — no ECC CDC mapping |
| `Language` |  |  |  | `String(2)` |  | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `TeleboxNumber` |  |  |  | `String(15)` |  | Telebox Number |  |  | S/4 only entity — no ECC CDC mapping |
| `PhoneNumber1` |  |  |  | `String(16)` |  | Telephone 1 |  |  | S/4 only entity — no ECC CDC mapping |
| `PhoneNumber2` |  |  |  | `String(16)` |  | Telephone 2 |  |  | S/4 only entity — no ECC CDC mapping |
| `FaxNumber` |  |  |  | `String(31)` |  | Fax Number |  |  | S/4 only entity — no ECC CDC mapping |
| `TeletexNumber` |  |  |  | `String(30)` |  | Teletex Number |  |  | S/4 only entity — no ECC CDC mapping |
| `TelexNumber` |  |  |  | `String(30)` |  | Telex Number |  |  | S/4 only entity — no ECC CDC mapping |
| `DataCommunicationPhoneNumber` |  |  |  | `String(14)` |  | Data line |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCenterPrinterDestination` |  |  |  | `String(4)` |  | Printer Destination |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCenterStandardHierArea` |  |  |  | `String(12)` |  | Hierarchy Area |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCollector` |  |  |  | `String(23)` |  | Cost Collector Key |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCenterIsComplete` |  |  |  | `Boolean` |  | Complete |  |  | S/4 only entity — no ECC CDC mapping |
| `IsStatisticalCostCenter` |  |  |  | `Boolean` |  | Cost Center Is Stat. |  |  | S/4 only entity — no ECC CDC mapping |
| `ObjectInternalID` |  |  |  | `String(22)` |  | Object Number |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCenterFunction` |  |  |  | `String(3)` |  | Function |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCenterAlternativeFunction` |  |  |  | `String(3)` |  | Altern. Function |  |  | S/4 only entity — no ECC CDC mapping |
| `FunctionalArea` |  |  |  | `String(16)` |  | Functional Area |  |  | S/4 only entity — no ECC CDC mapping |
| `ActyIndepFormulaPlanningTmpl` |  |  |  | `String(10)` |  | Activity-Indep.Temp. |  |  | S/4 only entity — no ECC CDC mapping |
| `ActyDepdntFormulaPlanningTmpl` |  |  |  | `String(10)` |  | Activity-Dep.Tmp |  |  | S/4 only entity — no ECC CDC mapping |
| `ActyIndependentAllocationTmpl` |  |  |  | `String(10)` |  | Acty-IndepTemplAlloc |  |  | S/4 only entity — no ECC CDC mapping |
| `ActyDependentAllocationTmpl` |  |  |  | `String(10)` |  | Acty-Dep Templ.Alloc |  |  | S/4 only entity — no ECC CDC mapping |
| `ActlIndepStatisticalKeyFigures` |  |  |  | `String(10)` |  | Templ.: Stat. KF |  |  | S/4 only entity — no ECC CDC mapping |
| `ActlDepStatisticalKeyFigures` |  |  |  | `String(10)` |  | Templ.: Stat. KF |  |  | S/4 only entity — no ECC CDC mapping |
| `JointVenture` |  |  |  | `String(6)` |  | Joint Venture |  |  | S/4 only entity — no ECC CDC mapping |
| `JointVentureRecoveryCode` |  |  |  | `String(2)` |  | Recovery Indicator |  |  | S/4 only entity — no ECC CDC mapping |
| `JointVentureEquityType` |  |  |  | `String(3)` |  | Equity Type |  |  | S/4 only entity — no ECC CDC mapping |
| `JointVentureObjectType` |  |  |  | `String(4)` |  | JV Object Type |  |  | S/4 only entity — no ECC CDC mapping |
| `JointVentureClass` |  |  |  | `String(3)` |  | JIB/JIBE Class |  |  | S/4 only entity — no ECC CDC mapping |
| `JointVentureSubClass` |  |  |  | `String(5)` |  | JIB/JIBE Subclass A |  |  | S/4 only entity — no ECC CDC mapping |
| `BudgetCarryingCostCenter` |  |  |  | `String(10)` |  | Budget Cost Center |  |  | S/4 only entity — no ECC CDC mapping |
| `AvailabilityControlProfile` |  |  |  | `String(6)` |  | Availy Ctrl Prfl |  |  | S/4 only entity — no ECC CDC mapping |
| `AvailabilityControlIsActive` |  |  |  | `Boolean` |  | AVC is Active |  |  | S/4 only entity — no ECC CDC mapping |
| `Fund` |  |  |  | `String(10)` |  | Fund |  |  | S/4 only entity — no ECC CDC mapping |
| `GrantID` |  |  |  | `String(20)` |  | Grant |  |  | S/4 only entity — no ECC CDC mapping |
| `FundIsFixAssigned` |  |  |  | `Boolean` |  | Fund Fixed Assignment |  |  | S/4 only entity — no ECC CDC mapping |
| `GrantIDIsFixAssigned` |  |  |  | `Boolean` |  | Grant Fixed Assignment |  |  | S/4 only entity — no ECC CDC mapping |
| `FunctionalAreaIsFixAssigned` |  |  |  | `Boolean` |  | Functional Area Fixed Assignment |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCenterCreationTime` |  |  |  | `String(6)` |  | Created At |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCenterLastChangedByUser` |  |  |  | `String(12)` |  | Last Changed By |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCenterLastChangedOnDate` |  |  |  | `Date` |  | Last Changed On |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCenterLastChangedAtTime` |  |  |  | `String(6)` |  | Last Changed At |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `CostCenterCategory`

- **ABAP Name:** `I_CostCenterCategory`
- **Label:** Cost Center Category
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `CostCenterCategory` |  |  |  | `String(1)` | Y | Cost Center Category |  |  | S/4 only entity — no ECC CDC mapping |
| `IsBlkdForPrimaryCostsPosting` |  |  |  | `Boolean` |  | Actual primary costs |  |  | S/4 only entity — no ECC CDC mapping |
| `IsBlkdForSecondaryCostsPosting` |  |  |  | `Boolean` |  | Actl Sec. Costs |  |  | S/4 only entity — no ECC CDC mapping |
| `IsBlockedForRevenuePosting` |  |  |  | `Boolean` |  | Actual Revenues |  |  | S/4 only entity — no ECC CDC mapping |
| `IsBlockedForCommitmentPosting` |  |  |  | `Boolean` |  | Commitment Update |  |  | S/4 only entity — no ECC CDC mapping |
| `IsBlockedForPlanPrimaryCosts` |  |  |  | `Boolean` |  | Plan primary costs |  |  | S/4 only entity — no ECC CDC mapping |
| `IsBlockedForPlanSecondaryCosts` |  |  |  | `Boolean` |  | Lock Plan Sec Costs |  |  | S/4 only entity — no ECC CDC mapping |
| `IsBlockedForPlanRevenues` |  |  |  | `Boolean` |  | Lock Planning Revn |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCenterAllocationMethod` |  |  |  | `String(2)` |  | Allocation Methods |  |  | S/4 only entity — no ECC CDC mapping |
| `ConsumptionQtyIsRecorded` |  |  |  | `Boolean` |  | Record Quantity |  |  | S/4 only entity — no ECC CDC mapping |
| `FunctionalArea` |  |  |  | `String(16)` |  | Functional Area |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `CostCenterCategoryText`

- **ABAP Name:** `I_CostCenterCategoryText`
- **Label:** Cost Center Category - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Language` |  |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCenterCategory` |  |  |  | `String(1)` | Y | Cost Center Category |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCenterCategoryName` |  |  |  | `String(20)` |  | Cost Ctr Cat Name |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `CostCenterHierarchy`

- **ABAP Name:** `I_CostCenterHierarchy`
- **Label:** Cost Center Hierarchy
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `ControllingArea` |  |  |  | `String(4)` | Y | Controlling Area |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCenterHierarchy` |  |  |  | `String(40)` | Y | Cost Center Hierarchy |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityEndDate` |  |  |  | `Date` | Y | Validity End Date |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityStartDate` |  |  |  | `Date` |  | Validity Start Date |  |  | S/4 only entity — no ECC CDC mapping |
| `LastChangedByUser` |  |  |  | `String(12)` |  | Last Changed By |  |  | S/4 only entity — no ECC CDC mapping |
| `LastChangeDateTime` |  |  |  | `DateTime` |  | Updated At |  |  | S/4 only entity — no ECC CDC mapping |
| `LastChangeTime` |  |  |  | `DateTime` |  | Updated At |  |  | S/4 only entity — no ECC CDC mapping |
| `HierarchyShortID` |  |  |  | `String(20)` |  | Hierarchy ID |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `CostCenterHierarchyNode`

- **ABAP Name:** `I_CostCenterHierarchyNode`
- **Label:** Cost Center Hierarchy Node
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `ControllingArea` |  |  |  | `String(4)` | Y | Controlling Area |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCenterHierarchy` |  |  |  | `String(40)` | Y | Cost Center Hierarchy |  | _Hierarchy | S/4 only entity — no ECC CDC mapping |
| `HierarchyNode` |  |  |  | `String(50)` | Y | Node |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityEndDate` |  |  |  | `Date` | Y | Validity End Date |  |  | S/4 only entity — no ECC CDC mapping |
| `ParentNode` |  |  |  | `String(50)` |  | Par. Node |  |  | S/4 only entity — no ECC CDC mapping |
| `HierarchyVersion` |  |  |  | `String(15)` |  | Version |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityStartDate` |  |  |  | `Date` |  | Validity Start Date |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCenter` |  |  |  | `String(10)` |  | Cost Center |  | _CostCenter | S/4 only entity — no ECC CDC mapping |
| `SequenceNumber` |  |  |  | `String(56)` |  |  |  |  | S/4 only entity — no ECC CDC mapping |
| `HierarchyNodeSequence` |  |  |  | `String(6)` |  | Sequence Number |  |  | S/4 only entity — no ECC CDC mapping |
| `HierarchyNodeLevel` |  |  |  | `String(6)` |  | Hierarchy Level |  |  | S/4 only entity — no ECC CDC mapping |
| `NodeType` |  |  |  | `String(1)` |  | Node Type |  |  | S/4 only entity — no ECC CDC mapping |
| `HierarchyNodeVal` |  |  |  | `String(40)` |  | Value |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `CostCenterHierarchyNodeText`

- **ABAP Name:** `I_CostCenterHierarchyNodeT`
- **Label:** Cost Center Hierarchy Node - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `ControllingArea` |  |  |  | `String(4)` | Y | Controlling Area |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCenterHierarchy` |  |  |  | `String(40)` | Y | Cost Center Hierarchy |  | _Hierarchy | S/4 only entity — no ECC CDC mapping |
| `HierarchyNode` |  |  |  | `String(50)` | Y | Node |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityEndDate` |  |  |  | `Date` | Y | Valid To |  |  | S/4 only entity — no ECC CDC mapping |
| `Language` |  |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `HierarchyNodeText` |  |  |  | `String(50)` |  | Description |  |  | S/4 only entity — no ECC CDC mapping |
| `HierarchyNodeShortText` |  |  |  | `String(20)` |  |  |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityStartDate` |  |  |  | `Date` |  | Valid From |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `CostCenterHierarchyText`

- **ABAP Name:** `I_CostCenterHierarchyText`
- **Label:** Cost Center Hierarchy - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `ControllingArea` |  |  |  | `String(12)` | Y | Hierarchy Class |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCenterHierarchy` |  |  |  | `String(40)` | Y | Cost Center Hierarchy |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityEndDate` |  |  |  | `Date` | Y | Valid To |  |  | S/4 only entity — no ECC CDC mapping |
| `Language` |  |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityStartDate` |  |  |  | `Date` |  | Valid From |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCenterHierarchyName` |  |  |  | `String(50)` |  | Description |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `CostCenterText`

- **ABAP Name:** `I_CostCenterText`
- **Label:** Cost Center - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `CostCenter` |  |  |  | `String(10)` | Y | Cost Center |  |  | S/4 only entity — no ECC CDC mapping |
| `ControllingArea` |  |  |  | `String(4)` | Y | Controlling Area |  |  | S/4 only entity — no ECC CDC mapping |
| `Language` |  |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityEndDate` |  |  |  | `Date` | Y | Valid To |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityStartDate` |  |  |  | `Date` |  | Valid From |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCenterName` |  |  |  | `String(20)` |  | Cost Center Name |  |  | S/4 only entity — no ECC CDC mapping |
| `CostCenterDescription` |  |  |  | `String(40)` |  | Cost Center Desc. |  |  | S/4 only entity — no ECC CDC mapping |
