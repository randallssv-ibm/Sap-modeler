# CostCenter

> Source file: `sap-s4com-CostCenter-v1.json`


## Entity: `CostCenter`

- **ABAP CDS Name:** `I_CostCenter`
- **Label:** Cost Center
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** CSKS, CSKT

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `ControllingArea` |  | `CSKS` | `KOKRS` |  |  | `String(4)` | Y | Controlling Area |  |  |
| `CostCenter` |  | `CSKS` | `KOSTL` |  |  | `String(10)` | Y | Cost Center |  |  |
| `ValidityEndDate` |  | `CSKS` | `DATBI` |  |  | `Date` | Y | Valid To |  |  |
| `ValidityStartDate` |  | `CSKS` | `DATAB` |  |  | `Date` |  | Valid From |  |  |
| `IsBlkdForPrimaryCostsPosting` |  |  |  |  |  | `Boolean` |  | Actual primary costs |  |  |
| `IsBlockedForPlanPrimaryCosts` |  |  |  |  |  | `Boolean` |  | Plan primary costs |  |  |
| `CompanyCode` |  | `CSKS` | `BUKRS` |  |  | `String(4)` |  | Company Code |  |  |
| `BusinessArea` |  | `CSKS` | `GSBER` |  |  | `String(4)` |  | Business Area |  |  |
| `CostCenterCategory` |  | `CSKS` | `KOSAR` |  |  | `String(1)` |  | Cost Center Category |  |  |
| `CostCtrResponsiblePersonName` |  |  |  |  |  | `String(20)` |  | Person Responsible |  |  |
| `CostCtrResponsibleUser` |  |  |  |  |  | `String(12)` |  | User Responsible |  |  |
| `CostCenterCurrency` |  |  |  |  |  | `String(5)` |  | Currency |  |  |
| `CostingSheet` |  |  |  |  |  | `String(6)` |  | Costing Sheet |  |  |
| `TaxJurisdiction` |  |  |  |  |  | `String(15)` |  | Tax Jurisdiction |  |  |
| `ProfitCenter` |  | `CSKS` | `PRCTR` |  |  | `String(10)` |  | Profit Center |  |  |
| `Plant` |  | `CSKS` | `WERKS` |  |  | `String(4)` |  | Plant |  |  |
| `LogicalSystem` |  |  |  |  |  | `String(10)` |  | Logical System |  |  |
| `CostCenterCreationDate` |  |  |  |  |  | `Date` |  | Entered On |  |  |
| `CostCenterCreatedByUser` |  |  |  |  |  | `String(12)` |  | Created By |  |  |
| `IsBlkdForSecondaryCostsPosting` |  |  |  |  |  | `Boolean` |  | Actl Sec. Costs |  |  |
| `IsBlockedForRevenuePosting` |  |  |  |  |  | `Boolean` |  | Actual Revenues |  |  |
| `IsBlockedForCommitmentPosting` |  |  |  |  |  | `Boolean` |  | Commitment Update |  |  |
| `IsBlockedForPlanSecondaryCosts` |  |  |  |  |  | `Boolean` |  | Lock Plan Sec Costs |  |  |
| `IsBlockedForPlanRevenues` |  |  |  |  |  | `Boolean` |  | Lock Planning Revn |  |  |
| `CostCenterAllocationMethod` |  |  |  |  |  | `String(2)` |  | Allocation Methods |  |  |
| `ConsumptionQtyIsRecorded` |  |  |  |  |  | `Boolean` |  | Record Quantity |  |  |
| `Department` |  | `CSKS` | `ABTEI` |  |  | `String(12)` |  | Department |  |  |
| `SubsequentCostCenter` |  |  |  |  |  | `String(10)` |  | Subsequent Cost Ctr. |  |  |
| `ConditionUsage` |  |  |  |  |  | `String(1)` |  | Usage |  |  |
| `ConditionApplication` |  |  |  |  |  | `String(2)` |  | Application |  |  |
| `CostCenterAccountingOverhead` |  |  |  |  |  | `String(6)` |  | Overhead Key |  |  |
| `Country` |  | `CSKS` | `LAND1` |  |  | `String(3)` |  | Country/Region Key |  |  |
| `FormOfAddress` |  |  |  |  |  | `String(15)` |  | Title |  |  |
| `AddressName` |  |  |  |  |  | `String(35)` |  | Name |  |  |
| `AddressAdditionalName` |  |  |  |  |  | `String(35)` |  | Name 2 |  |  |
| `CostCenterAddrName3` |  |  |  |  |  | `String(35)` |  | Name 3 |  |  |
| `CostCenterAddrName4` |  |  |  |  |  | `String(35)` |  | Name 4 |  |  |
| `CityName` |  |  |  |  |  | `String(35)` |  | City |  |  |
| `District` |  |  |  |  |  | `String(35)` |  | District |  |  |
| `StreetAddressName` |  |  |  |  |  | `String(35)` |  | Street |  |  |
| `POBox` |  |  |  |  |  | `String(10)` |  | PO Box |  |  |
| `PostalCode` |  |  |  |  |  | `String(10)` |  | Postal Code |  |  |
| `POBoxPostalCode` |  |  |  |  |  | `String(10)` |  | PO Box Postal Code |  |  |
| `Region` |  |  |  |  |  | `String(3)` |  | Region |  |  |
| `Language` |  | `CSKT` | `SPRAS` |  |  | `String(2)` |  | Language Key |  |  |
| `TeleboxNumber` |  |  |  |  |  | `String(15)` |  | Telebox Number |  |  |
| `PhoneNumber1` |  |  |  |  |  | `String(16)` |  | Telephone 1 |  |  |
| `PhoneNumber2` |  |  |  |  |  | `String(16)` |  | Telephone 2 |  |  |
| `FaxNumber` |  |  |  |  |  | `String(31)` |  | Fax Number |  |  |
| `TeletexNumber` |  |  |  |  |  | `String(30)` |  | Teletex Number |  |  |
| `TelexNumber` |  |  |  |  |  | `String(30)` |  | Telex Number |  |  |
| `DataCommunicationPhoneNumber` |  |  |  |  |  | `String(14)` |  | Data line |  |  |
| `CostCenterPrinterDestination` |  |  |  |  |  | `String(4)` |  | Printer Destination |  |  |
| `CostCenterStandardHierArea` |  |  |  |  |  | `String(12)` |  | Hierarchy Area |  |  |
| `CostCollector` |  |  |  |  |  | `String(23)` |  | Cost Collector Key |  |  |
| `CostCenterIsComplete` |  |  |  |  |  | `Boolean` |  | Complete |  |  |
| `IsStatisticalCostCenter` |  |  |  |  |  | `Boolean` |  | Cost Center Is Stat. |  |  |
| `ObjectInternalID` |  |  |  |  |  | `String(22)` |  | Object Number |  |  |
| `CostCenterFunction` |  |  |  |  |  | `String(3)` |  | Function |  |  |
| `CostCenterAlternativeFunction` |  |  |  |  |  | `String(3)` |  | Altern. Function |  |  |
| `FunctionalArea` |  | `CSKS` | `FUNC_AREA` |  |  | `String(16)` |  | Functional Area |  |  |
| `ActyIndepFormulaPlanningTmpl` |  |  |  |  |  | `String(10)` |  | Activity-Indep.Temp. |  |  |
| `ActyDepdntFormulaPlanningTmpl` |  |  |  |  |  | `String(10)` |  | Activity-Dep.Tmp |  |  |
| `ActyIndependentAllocationTmpl` |  |  |  |  |  | `String(10)` |  | Acty-IndepTemplAlloc |  |  |
| `ActyDependentAllocationTmpl` |  |  |  |  |  | `String(10)` |  | Acty-Dep Templ.Alloc |  |  |
| `ActlIndepStatisticalKeyFigures` |  |  |  |  |  | `String(10)` |  | Templ.: Stat. KF |  |  |
| `ActlDepStatisticalKeyFigures` |  |  |  |  |  | `String(10)` |  | Templ.: Stat. KF |  |  |
| `JointVenture` |  |  |  |  |  | `String(6)` |  | Joint Venture |  |  |
| `JointVentureRecoveryCode` |  |  |  |  |  | `String(2)` |  | Recovery Indicator |  |  |
| `JointVentureEquityType` |  |  |  |  |  | `String(3)` |  | Equity Type |  |  |
| `JointVentureObjectType` |  |  |  |  |  | `String(4)` |  | JV Object Type |  |  |
| `JointVentureClass` |  |  |  |  |  | `String(3)` |  | JIB/JIBE Class |  |  |
| `JointVentureSubClass` |  |  |  |  |  | `String(5)` |  | JIB/JIBE Subclass A |  |  |
| `BudgetCarryingCostCenter` |  |  |  |  |  | `String(10)` |  | Budget Cost Center |  |  |
| `AvailabilityControlProfile` |  |  |  |  |  | `String(6)` |  | Availy Ctrl Prfl |  |  |
| `AvailabilityControlIsActive` |  |  |  |  |  | `Boolean` |  | AVC is Active |  |  |
| `Fund` |  |  |  |  |  | `String(10)` |  | Fund |  |  |
| `GrantID` |  |  |  |  |  | `String(20)` |  | Grant |  |  |
| `FundIsFixAssigned` |  |  |  |  |  | `Boolean` |  | Fund Fixed Assignment |  |  |
| `GrantIDIsFixAssigned` |  |  |  |  |  | `Boolean` |  | Grant Fixed Assignment |  |  |
| `FunctionalAreaIsFixAssigned` |  |  |  |  |  | `Boolean` |  | Functional Area Fixed Assignment |  |  |
| `CostCenterCreationTime` |  |  |  |  |  | `String(6)` |  | Created At |  |  |
| `CostCenterLastChangedByUser` |  |  |  |  |  | `String(12)` |  | Last Changed By |  |  |
| `CostCenterLastChangedOnDate` |  |  |  |  |  | `Date` |  | Last Changed On |  |  |
| `CostCenterLastChangedAtTime` |  |  |  |  |  | `String(6)` |  | Last Changed At |  |  |


## Entity: `CostCenterCategory`

- **ABAP CDS Name:** `I_CostCenterCategory`
- **Label:** Cost Center Category
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** CSKS

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `CostCenterCategory` |  |  |  |  |  | `String(1)` | Y | Cost Center Category |  |  |
| `IsBlkdForPrimaryCostsPosting` |  |  |  |  |  | `Boolean` |  | Actual primary costs |  |  |
| `IsBlkdForSecondaryCostsPosting` |  |  |  |  |  | `Boolean` |  | Actl Sec. Costs |  |  |
| `IsBlockedForRevenuePosting` |  |  |  |  |  | `Boolean` |  | Actual Revenues |  |  |
| `IsBlockedForCommitmentPosting` |  |  |  |  |  | `Boolean` |  | Commitment Update |  |  |
| `IsBlockedForPlanPrimaryCosts` |  |  |  |  |  | `Boolean` |  | Plan primary costs |  |  |
| `IsBlockedForPlanSecondaryCosts` |  |  |  |  |  | `Boolean` |  | Lock Plan Sec Costs |  |  |
| `IsBlockedForPlanRevenues` |  |  |  |  |  | `Boolean` |  | Lock Planning Revn |  |  |
| `CostCenterAllocationMethod` |  |  |  |  |  | `String(2)` |  | Allocation Methods |  |  |
| `ConsumptionQtyIsRecorded` |  |  |  |  |  | `Boolean` |  | Record Quantity |  |  |
| `FunctionalArea` |  |  |  |  |  | `String(16)` |  | Functional Area |  |  |


## Entity: `CostCenterCategoryText`

- **ABAP CDS Name:** `I_CostCenterCategoryText`
- **Label:** Cost Center Category - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** S/4 only

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Language` |  |  |  |  |  | `String(2)` | Y | Language Key |  | S/4 only entity |
| `CostCenterCategory` |  |  |  |  |  | `String(1)` | Y | Cost Center Category |  | S/4 only entity |
| `CostCenterCategoryName` |  |  |  |  |  | `String(20)` |  | Cost Ctr Cat Name |  | S/4 only entity |


## Entity: `CostCenterHierarchy`

- **ABAP CDS Name:** `I_CostCenterHierarchy`
- **Label:** Cost Center Hierarchy
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** SETHEADER, SETHEADERT

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `ControllingArea` |  |  |  |  |  | `String(4)` | Y | Controlling Area |  |  |
| `CostCenterHierarchy` |  |  |  |  |  | `String(40)` | Y | Cost Center Hierarchy |  |  |
| `ValidityEndDate` |  |  |  |  |  | `Date` | Y | Validity End Date |  |  |
| `ValidityStartDate` |  |  |  |  |  | `Date` |  | Validity Start Date |  |  |
| `LastChangedByUser` |  |  |  |  |  | `String(12)` |  | Last Changed By |  |  |
| `LastChangeDateTime` |  |  |  |  |  | `DateTime` |  | Updated At |  |  |
| `LastChangeTime` |  |  |  |  |  | `DateTime` |  | Updated At |  |  |
| `HierarchyShortID` |  |  |  |  |  | `String(20)` |  | Hierarchy ID |  |  |


## Entity: `CostCenterHierarchyNode`

- **ABAP CDS Name:** `I_CostCenterHierarchyNode`
- **Label:** Cost Center Hierarchy Node
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** SETHEADER, SETNODE, SETLEAF

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `ControllingArea` |  |  |  |  |  | `String(4)` | Y | Controlling Area |  |  |
| `CostCenterHierarchy` |  |  |  |  |  | `String(40)` | Y | Cost Center Hierarchy |  |  |
| `HierarchyNode` |  |  |  |  |  | `String(50)` | Y | Node |  |  |
| `ValidityEndDate` |  |  |  |  |  | `Date` | Y | Validity End Date |  |  |
| `ParentNode` |  |  |  |  |  | `String(50)` |  | Par. Node |  |  |
| `HierarchyVersion` |  |  |  |  |  | `String(15)` |  | Version |  |  |
| `ValidityStartDate` |  |  |  |  |  | `Date` |  | Validity Start Date |  |  |
| `CostCenter` |  |  |  |  |  | `String(10)` |  | Cost Center |  |  |
| `SequenceNumber` |  |  |  |  |  | `String(56)` |  |  |  |  |
| `HierarchyNodeSequence` |  |  |  |  |  | `String(6)` |  | Sequence Number |  |  |
| `HierarchyNodeLevel` |  |  |  |  |  | `String(6)` |  | Hierarchy Level |  |  |
| `NodeType` |  |  |  |  |  | `String(1)` |  | Node Type |  |  |
| `HierarchyNodeVal` |  |  |  |  |  | `String(40)` |  | Value |  |  |


## Entity: `CostCenterHierarchyNodeText`

- **ABAP CDS Name:** `I_CostCenterHierarchyNodeT`
- **Label:** Cost Center Hierarchy Node - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** SETHEADERT

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `ControllingArea` |  |  |  |  |  | `String(4)` | Y | Controlling Area |  |  |
| `CostCenterHierarchy` |  |  |  |  |  | `String(40)` | Y | Cost Center Hierarchy |  |  |
| `HierarchyNode` |  |  |  |  |  | `String(50)` | Y | Node |  |  |
| `ValidityEndDate` |  |  |  |  |  | `Date` | Y | Valid To |  |  |
| `Language` |  |  |  |  |  | `String(2)` | Y | Language Key |  |  |
| `HierarchyNodeText` |  |  |  |  |  | `String(50)` |  | Description |  |  |
| `HierarchyNodeShortText` |  |  |  |  |  | `String(20)` |  |  |  |  |
| `ValidityStartDate` |  |  |  |  |  | `Date` |  | Valid From |  |  |


## Entity: `CostCenterHierarchyText`

- **ABAP CDS Name:** `I_CostCenterHierarchyText`
- **Label:** Cost Center Hierarchy - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** SETHEADERT

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `ControllingArea` |  |  |  |  |  | `String(12)` | Y | Hierarchy Class |  |  |
| `CostCenterHierarchy` |  |  |  |  |  | `String(40)` | Y | Cost Center Hierarchy |  |  |
| `ValidityEndDate` |  |  |  |  |  | `Date` | Y | Valid To |  |  |
| `Language` |  |  |  |  |  | `String(2)` | Y | Language Key |  |  |
| `ValidityStartDate` |  |  |  |  |  | `Date` |  | Valid From |  |  |
| `CostCenterHierarchyName` |  |  |  |  |  | `String(50)` |  | Description |  |  |


## Entity: `CostCenterText`

- **ABAP CDS Name:** `I_CostCenterText`
- **Label:** Cost Center - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** CSKT

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `CostCenter` |  |  |  |  |  | `String(10)` | Y | Cost Center |  |  |
| `ControllingArea` |  |  |  |  |  | `String(4)` | Y | Controlling Area |  |  |
| `Language` |  |  |  |  |  | `String(2)` | Y | Language Key |  |  |
| `ValidityEndDate` |  |  |  |  |  | `Date` | Y | Valid To |  |  |
| `ValidityStartDate` |  |  |  |  |  | `Date` |  | Valid From |  |  |
| `CostCenterName` |  |  |  |  |  | `String(20)` |  | Cost Center Name |  |  |
| `CostCenterDescription` |  |  |  |  |  | `String(40)` |  | Cost Center Desc. |  |  |
