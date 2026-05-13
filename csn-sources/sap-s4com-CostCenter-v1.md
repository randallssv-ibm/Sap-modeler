# CostCenter

> Source file: `sap-s4com-CostCenter-v1.json`


## Entity: `CostCenter`

- **ABAP Name:** `I_CostCenter`
- **Label:** Cost Center
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `ControllingArea` | `CSKS` | `KOKRS` | `String(4)` | Y | Controlling Area |  |  |  |
| `CostCenter` | `CSKS` | `KOSTL` | `String(10)` | Y | Cost Center |  |  |  |
| `ValidityEndDate` | `CSKS` | `DATBI` | `Date` | Y | Valid To |  |  |  |
| `ValidityStartDate` | `CSKS` | `DATAB` | `Date` |  | Valid From |  |  |  |
| `IsBlkdForPrimaryCostsPosting` |  |  | `Boolean` |  | Actual primary costs |  |  | S/4 only entity |
| `IsBlockedForPlanPrimaryCosts` |  |  | `Boolean` |  | Plan primary costs |  |  | S/4 only entity |
| `CompanyCode` | `CSKS` | `BUKRS` | `String(4)` |  | Company Code |  |  |  |
| `BusinessArea` | `CSKS` | `GSBER` | `String(4)` |  | Business Area |  |  |  |
| `CostCenterCategory` | `CSKS` | `KOSAR` | `String(1)` |  | Cost Center Category |  | _CostCenterCategory |  |
| `CostCtrResponsiblePersonName` |  |  | `String(20)` |  | Person Responsible |  |  | S/4 only entity |
| `CostCtrResponsibleUser` |  |  | `String(12)` |  | User Responsible |  |  | S/4 only entity |
| `CostCenterCurrency` |  |  | `String(5)` |  | Currency |  |  | S/4 only entity |
| `CostingSheet` |  |  | `String(6)` |  | Costing Sheet |  |  | S/4 only entity |
| `TaxJurisdiction` |  |  | `String(15)` |  | Tax Jurisdiction |  |  | S/4 only entity |
| `ProfitCenter` | `CSKS` | `PRCTR` | `String(10)` |  | Profit Center |  |  |  |
| `Plant` | `CSKS` | `WERKS` | `String(4)` |  | Plant |  |  |  |
| `LogicalSystem` |  |  | `String(10)` |  | Logical System |  |  | S/4 only entity |
| `CostCenterCreationDate` |  |  | `Date` |  | Entered On |  |  | S/4 only entity |
| `CostCenterCreatedByUser` |  |  | `String(12)` |  | Created By |  |  | S/4 only entity |
| `IsBlkdForSecondaryCostsPosting` |  |  | `Boolean` |  | Actl Sec. Costs |  |  | S/4 only entity |
| `IsBlockedForRevenuePosting` |  |  | `Boolean` |  | Actual Revenues |  |  | S/4 only entity |
| `IsBlockedForCommitmentPosting` |  |  | `Boolean` |  | Commitment Update |  |  | S/4 only entity |
| `IsBlockedForPlanSecondaryCosts` |  |  | `Boolean` |  | Lock Plan Sec Costs |  |  | S/4 only entity |
| `IsBlockedForPlanRevenues` |  |  | `Boolean` |  | Lock Planning Revn |  |  | S/4 only entity |
| `CostCenterAllocationMethod` |  |  | `String(2)` |  | Allocation Methods |  |  | S/4 only entity |
| `ConsumptionQtyIsRecorded` |  |  | `Boolean` |  | Record Quantity |  |  | S/4 only entity |
| `Department` | `CSKS` | `ABTEI` | `String(12)` |  | Department |  |  |  |
| `SubsequentCostCenter` |  |  | `String(10)` |  | Subsequent Cost Ctr. |  |  | S/4 only entity |
| `ConditionUsage` |  |  | `String(1)` |  | Usage |  |  | S/4 only entity |
| `ConditionApplication` |  |  | `String(2)` |  | Application |  |  | S/4 only entity |
| `CostCenterAccountingOverhead` |  |  | `String(6)` |  | Overhead Key |  |  | S/4 only entity |
| `Country` | `CSKS` | `LAND1` | `String(3)` |  | Country/Region Key |  |  |  |
| `FormOfAddress` |  |  | `String(15)` |  | Title |  |  | S/4 only entity |
| `AddressName` |  |  | `String(35)` |  | Name |  |  | S/4 only entity |
| `AddressAdditionalName` |  |  | `String(35)` |  | Name 2 |  |  | S/4 only entity |
| `CostCenterAddrName3` |  |  | `String(35)` |  | Name 3 |  |  | S/4 only entity |
| `CostCenterAddrName4` |  |  | `String(35)` |  | Name 4 |  |  | S/4 only entity |
| `CityName` |  |  | `String(35)` |  | City |  |  | S/4 only entity |
| `District` |  |  | `String(35)` |  | District |  |  | S/4 only entity |
| `StreetAddressName` |  |  | `String(35)` |  | Street |  |  | S/4 only entity |
| `POBox` |  |  | `String(10)` |  | PO Box |  |  | S/4 only entity |
| `PostalCode` |  |  | `String(10)` |  | Postal Code |  |  | S/4 only entity |
| `POBoxPostalCode` |  |  | `String(10)` |  | PO Box Postal Code |  |  | S/4 only entity |
| `Region` |  |  | `String(3)` |  | Region |  |  | S/4 only entity |
| `Language` | `CSKT` | `SPRAS` | `String(2)` |  | Language Key |  |  |  |
| `TeleboxNumber` |  |  | `String(15)` |  | Telebox Number |  |  | S/4 only entity |
| `PhoneNumber1` |  |  | `String(16)` |  | Telephone 1 |  |  | S/4 only entity |
| `PhoneNumber2` |  |  | `String(16)` |  | Telephone 2 |  |  | S/4 only entity |
| `FaxNumber` |  |  | `String(31)` |  | Fax Number |  |  | S/4 only entity |
| `TeletexNumber` |  |  | `String(30)` |  | Teletex Number |  |  | S/4 only entity |
| `TelexNumber` |  |  | `String(30)` |  | Telex Number |  |  | S/4 only entity |
| `DataCommunicationPhoneNumber` |  |  | `String(14)` |  | Data line |  |  | S/4 only entity |
| `CostCenterPrinterDestination` |  |  | `String(4)` |  | Printer Destination |  |  | S/4 only entity |
| `CostCenterStandardHierArea` |  |  | `String(12)` |  | Hierarchy Area |  |  | S/4 only entity |
| `CostCollector` |  |  | `String(23)` |  | Cost Collector Key |  |  | S/4 only entity |
| `CostCenterIsComplete` |  |  | `Boolean` |  | Complete |  |  | S/4 only entity |
| `IsStatisticalCostCenter` |  |  | `Boolean` |  | Cost Center Is Stat. |  |  | S/4 only entity |
| `ObjectInternalID` |  |  | `String(22)` |  | Object Number |  |  | S/4 only entity |
| `CostCenterFunction` |  |  | `String(3)` |  | Function |  |  | S/4 only entity |
| `CostCenterAlternativeFunction` |  |  | `String(3)` |  | Altern. Function |  |  | S/4 only entity |
| `FunctionalArea` | `CSKS` | `FUNC_AREA` | `String(16)` |  | Functional Area |  |  |  |
| `ActyIndepFormulaPlanningTmpl` |  |  | `String(10)` |  | Activity-Indep.Temp. |  |  | S/4 only entity |
| `ActyDepdntFormulaPlanningTmpl` |  |  | `String(10)` |  | Activity-Dep.Tmp |  |  | S/4 only entity |
| `ActyIndependentAllocationTmpl` |  |  | `String(10)` |  | Acty-IndepTemplAlloc |  |  | S/4 only entity |
| `ActyDependentAllocationTmpl` |  |  | `String(10)` |  | Acty-Dep Templ.Alloc |  |  | S/4 only entity |
| `ActlIndepStatisticalKeyFigures` |  |  | `String(10)` |  | Templ.: Stat. KF |  |  | S/4 only entity |
| `ActlDepStatisticalKeyFigures` |  |  | `String(10)` |  | Templ.: Stat. KF |  |  | S/4 only entity |
| `JointVenture` |  |  | `String(6)` |  | Joint Venture |  |  | S/4 only entity |
| `JointVentureRecoveryCode` |  |  | `String(2)` |  | Recovery Indicator |  |  | S/4 only entity |
| `JointVentureEquityType` |  |  | `String(3)` |  | Equity Type |  |  | S/4 only entity |
| `JointVentureObjectType` |  |  | `String(4)` |  | JV Object Type |  |  | S/4 only entity |
| `JointVentureClass` |  |  | `String(3)` |  | JIB/JIBE Class |  |  | S/4 only entity |
| `JointVentureSubClass` |  |  | `String(5)` |  | JIB/JIBE Subclass A |  |  | S/4 only entity |
| `BudgetCarryingCostCenter` |  |  | `String(10)` |  | Budget Cost Center |  |  | S/4 only entity |
| `AvailabilityControlProfile` |  |  | `String(6)` |  | Availy Ctrl Prfl |  |  | S/4 only entity |
| `AvailabilityControlIsActive` |  |  | `Boolean` |  | AVC is Active |  |  | S/4 only entity |
| `Fund` |  |  | `String(10)` |  | Fund |  |  | S/4 only entity |
| `GrantID` |  |  | `String(20)` |  | Grant |  |  | S/4 only entity |
| `FundIsFixAssigned` |  |  | `Boolean` |  | Fund Fixed Assignment |  |  | S/4 only entity |
| `GrantIDIsFixAssigned` |  |  | `Boolean` |  | Grant Fixed Assignment |  |  | S/4 only entity |
| `FunctionalAreaIsFixAssigned` |  |  | `Boolean` |  | Functional Area Fixed Assignment |  |  | S/4 only entity |
| `CostCenterCreationTime` |  |  | `String(6)` |  | Created At |  |  | S/4 only entity |
| `CostCenterLastChangedByUser` |  |  | `String(12)` |  | Last Changed By |  |  | S/4 only entity |
| `CostCenterLastChangedOnDate` |  |  | `Date` |  | Last Changed On |  |  | S/4 only entity |
| `CostCenterLastChangedAtTime` |  |  | `String(6)` |  | Last Changed At |  |  | S/4 only entity |


## Entity: `CostCenterCategory`

- **ABAP Name:** `I_CostCenterCategory`
- **Label:** Cost Center Category
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `CostCenterCategory` |  |  | `String(1)` | Y | Cost Center Category |  |  | S/4 only entity |
| `IsBlkdForPrimaryCostsPosting` |  |  | `Boolean` |  | Actual primary costs |  |  | S/4 only entity |
| `IsBlkdForSecondaryCostsPosting` |  |  | `Boolean` |  | Actl Sec. Costs |  |  | S/4 only entity |
| `IsBlockedForRevenuePosting` |  |  | `Boolean` |  | Actual Revenues |  |  | S/4 only entity |
| `IsBlockedForCommitmentPosting` |  |  | `Boolean` |  | Commitment Update |  |  | S/4 only entity |
| `IsBlockedForPlanPrimaryCosts` |  |  | `Boolean` |  | Plan primary costs |  |  | S/4 only entity |
| `IsBlockedForPlanSecondaryCosts` |  |  | `Boolean` |  | Lock Plan Sec Costs |  |  | S/4 only entity |
| `IsBlockedForPlanRevenues` |  |  | `Boolean` |  | Lock Planning Revn |  |  | S/4 only entity |
| `CostCenterAllocationMethod` |  |  | `String(2)` |  | Allocation Methods |  |  | S/4 only entity |
| `ConsumptionQtyIsRecorded` |  |  | `Boolean` |  | Record Quantity |  |  | S/4 only entity |
| `FunctionalArea` |  |  | `String(16)` |  | Functional Area |  |  | S/4 only entity |


## Entity: `CostCenterCategoryText`

- **ABAP Name:** `I_CostCenterCategoryText`
- **Label:** Cost Center Category - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `Language` |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity |
| `CostCenterCategory` |  |  | `String(1)` | Y | Cost Center Category |  |  | S/4 only entity |
| `CostCenterCategoryName` |  |  | `String(20)` |  | Cost Ctr Cat Name |  |  | S/4 only entity |


## Entity: `CostCenterHierarchy`

- **ABAP Name:** `I_CostCenterHierarchy`
- **Label:** Cost Center Hierarchy
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `ControllingArea` | `TKA01` | `KOKRS` | `String(4)` | Y | Controlling Area |  |  |  |
| `CostCenterHierarchy` |  |  | `String(40)` | Y | Cost Center Hierarchy |  |  | S/4 only entity |
| `ValidityEndDate` |  |  | `Date` | Y | Validity End Date |  |  | S/4 only entity |
| `ValidityStartDate` |  |  | `Date` |  | Validity Start Date |  |  | S/4 only entity |
| `LastChangedByUser` |  |  | `String(12)` |  | Last Changed By |  |  | S/4 only entity |
| `LastChangeDateTime` |  |  | `DateTime` |  | Updated At |  |  | S/4 only entity |
| `LastChangeTime` |  |  | `DateTime` |  | Updated At |  |  | S/4 only entity |
| `HierarchyShortID` |  |  | `String(20)` |  | Hierarchy ID |  |  | S/4 only entity |


## Entity: `CostCenterHierarchyNode`

- **ABAP Name:** `I_CostCenterHierarchyNode`
- **Label:** Cost Center Hierarchy Node
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `ControllingArea` | `TKA01` | `KOKRS` | `String(4)` | Y | Controlling Area |  |  |  |
| `CostCenterHierarchy` |  |  | `String(40)` | Y | Cost Center Hierarchy |  | _Hierarchy | S/4 only entity |
| `HierarchyNode` |  |  | `String(50)` | Y | Node |  |  | S/4 only entity |
| `ValidityEndDate` |  |  | `Date` | Y | Validity End Date |  |  | S/4 only entity |
| `ParentNode` |  |  | `String(50)` |  | Par. Node |  |  | S/4 only entity |
| `HierarchyVersion` |  |  | `String(15)` |  | Version |  |  | S/4 only entity |
| `ValidityStartDate` |  |  | `Date` |  | Validity Start Date |  |  | S/4 only entity |
| `CostCenter` |  |  | `String(10)` |  | Cost Center |  | _CostCenter | S/4 only entity |
| `SequenceNumber` |  |  | `String(56)` |  |  |  |  | S/4 only entity |
| `HierarchyNodeSequence` |  |  | `String(6)` |  | Sequence Number |  |  | S/4 only entity |
| `HierarchyNodeLevel` |  |  | `String(6)` |  | Hierarchy Level |  |  | S/4 only entity |
| `NodeType` |  |  | `String(1)` |  | Node Type |  |  | S/4 only entity |
| `HierarchyNodeVal` |  |  | `String(40)` |  | Value |  |  | S/4 only entity |


## Entity: `CostCenterHierarchyNodeText`

- **ABAP Name:** `I_CostCenterHierarchyNodeT`
- **Label:** Cost Center Hierarchy Node - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `ControllingArea` | `TKA01` | `KOKRS` | `String(4)` | Y | Controlling Area |  |  |  |
| `CostCenterHierarchy` |  |  | `String(40)` | Y | Cost Center Hierarchy |  | _Hierarchy | S/4 only entity |
| `HierarchyNode` |  |  | `String(50)` | Y | Node |  |  | S/4 only entity |
| `ValidityEndDate` |  |  | `Date` | Y | Valid To |  |  | S/4 only entity |
| `Language` |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity |
| `HierarchyNodeText` |  |  | `String(50)` |  | Description |  |  | S/4 only entity |
| `HierarchyNodeShortText` |  |  | `String(20)` |  |  |  |  | S/4 only entity |
| `ValidityStartDate` |  |  | `Date` |  | Valid From |  |  | S/4 only entity |


## Entity: `CostCenterHierarchyText`

- **ABAP Name:** `I_CostCenterHierarchyText`
- **Label:** Cost Center Hierarchy - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `ControllingArea` | `TKA01` | `KOKRS` | `String(12)` | Y | Hierarchy Class |  |  |  |
| `CostCenterHierarchy` |  |  | `String(40)` | Y | Cost Center Hierarchy |  |  | S/4 only entity |
| `ValidityEndDate` |  |  | `Date` | Y | Valid To |  |  | S/4 only entity |
| `Language` |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity |
| `ValidityStartDate` |  |  | `Date` |  | Valid From |  |  | S/4 only entity |
| `CostCenterHierarchyName` |  |  | `String(50)` |  | Description |  |  | S/4 only entity |


## Entity: `CostCenterText`

- **ABAP Name:** `I_CostCenterText`
- **Label:** Cost Center - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `CostCenter` |  |  | `String(10)` | Y | Cost Center |  |  | S/4 only entity |
| `ControllingArea` | `TKA01` | `KOKRS` | `String(4)` | Y | Controlling Area |  |  |  |
| `Language` |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity |
| `ValidityEndDate` |  |  | `Date` | Y | Valid To |  |  | S/4 only entity |
| `ValidityStartDate` |  |  | `Date` |  | Valid From |  |  | S/4 only entity |
| `CostCenterName` |  |  | `String(20)` |  | Cost Center Name |  |  | S/4 only entity |
| `CostCenterDescription` |  |  | `String(40)` |  | Cost Center Desc. |  |  | S/4 only entity |
