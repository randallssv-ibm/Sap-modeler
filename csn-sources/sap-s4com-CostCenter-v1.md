# CostCenter

> Source file: `sap-s4com-CostCenter-v1.json`


## Entity: `CostCenter`

- **ABAP Name:** `I_CostCenter`
- **Label:** Cost Center
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `ControllingArea` | `ControllingArea` | `String(4)` | Y | Controlling Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCenter` | `CostCenter` | `String(10)` | Y | Cost Center |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityEndDate` | `ValidityEndDate` | `Date` | Y | Valid To |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityStartDate` | `ValidityStartDate` | `Date` |  | Valid From |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsBlkdForPrimaryCostsPosting` | `IsBlkdForPrimaryCostsPosting` | `Boolean` |  | Actual primary costs |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsBlockedForPlanPrimaryCosts` | `IsBlockedForPlanPrimaryCosts` | `Boolean` |  | Plan primary costs |  |  | S/4 only entity (no ECC CDC mapping) |
| `CompanyCode` | `CompanyCode` | `String(4)` |  | Company Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `BusinessArea` | `BusinessArea` | `String(4)` |  | Business Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCenterCategory` | `CostCenterCategory` | `String(1)` |  | Cost Center Category |  | _CostCenterCategory | S/4 only entity (no ECC CDC mapping) |
| `CostCtrResponsiblePersonName` | `CostCtrResponsiblePersonName` | `String(20)` |  | Person Responsible |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCtrResponsibleUser` | `CostCtrResponsibleUser` | `String(12)` |  | User Responsible |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCenterCurrency` | `CostCenterCurrency` | `String(5)` |  | Currency |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostingSheet` | `CostingSheet` | `String(6)` |  | Costing Sheet |  |  | S/4 only entity (no ECC CDC mapping) |
| `TaxJurisdiction` | `TaxJurisdiction` | `String(15)` |  | Tax Jurisdiction |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProfitCenter` | `ProfitCenter` | `String(10)` |  | Profit Center |  |  | S/4 only entity (no ECC CDC mapping) |
| `Plant` | `Plant` | `String(4)` |  | Plant |  |  | S/4 only entity (no ECC CDC mapping) |
| `LogicalSystem` | `LogicalSystem` | `String(10)` |  | Logical System |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCenterCreationDate` | `CostCenterCreationDate` | `Date` |  | Entered On |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCenterCreatedByUser` | `CostCenterCreatedByUser` | `String(12)` |  | Created By |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsBlkdForSecondaryCostsPosting` | `IsBlkdForSecondaryCostsPosting` | `Boolean` |  | Actl Sec. Costs |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsBlockedForRevenuePosting` | `IsBlockedForRevenuePosting` | `Boolean` |  | Actual Revenues |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsBlockedForCommitmentPosting` | `IsBlockedForCommitmentPosting` | `Boolean` |  | Commitment Update |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsBlockedForPlanSecondaryCosts` | `IsBlockedForPlanSecondaryCosts` | `Boolean` |  | Lock Plan Sec Costs |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsBlockedForPlanRevenues` | `IsBlockedForPlanRevenues` | `Boolean` |  | Lock Planning Revn |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCenterAllocationMethod` | `CostCenterAllocationMethod` | `String(2)` |  | Allocation Methods |  |  | S/4 only entity (no ECC CDC mapping) |
| `ConsumptionQtyIsRecorded` | `ConsumptionQtyIsRecorded` | `Boolean` |  | Record Quantity |  |  | S/4 only entity (no ECC CDC mapping) |
| `Department` | `Department` | `String(12)` |  | Department |  |  | S/4 only entity (no ECC CDC mapping) |
| `SubsequentCostCenter` | `SubsequentCostCenter` | `String(10)` |  | Subsequent Cost Ctr. |  |  | S/4 only entity (no ECC CDC mapping) |
| `ConditionUsage` | `ConditionUsage` | `String(1)` |  | Usage |  |  | S/4 only entity (no ECC CDC mapping) |
| `ConditionApplication` | `ConditionApplication` | `String(2)` |  | Application |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCenterAccountingOverhead` | `CostCenterAccountingOverhead` | `String(6)` |  | Overhead Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `Country` | `Country` | `String(3)` |  | Country/Region Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `FormOfAddress` | `FormOfAddress` | `String(15)` |  | Title |  |  | S/4 only entity (no ECC CDC mapping) |
| `AddressName` | `AddressName` | `String(35)` |  | Name |  |  | S/4 only entity (no ECC CDC mapping) |
| `AddressAdditionalName` | `AddressAdditionalName` | `String(35)` |  | Name 2 |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCenterAddrName3` | `CostCenterAddrName3` | `String(35)` |  | Name 3 |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCenterAddrName4` | `CostCenterAddrName4` | `String(35)` |  | Name 4 |  |  | S/4 only entity (no ECC CDC mapping) |
| `CityName` | `CityName` | `String(35)` |  | City |  |  | S/4 only entity (no ECC CDC mapping) |
| `District` | `District` | `String(35)` |  | District |  |  | S/4 only entity (no ECC CDC mapping) |
| `StreetAddressName` | `StreetAddressName` | `String(35)` |  | Street |  |  | S/4 only entity (no ECC CDC mapping) |
| `POBox` | `POBox` | `String(10)` |  | PO Box |  |  | S/4 only entity (no ECC CDC mapping) |
| `PostalCode` | `PostalCode` | `String(10)` |  | Postal Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `POBoxPostalCode` | `POBoxPostalCode` | `String(10)` |  | PO Box Postal Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `Region` | `Region` | `String(3)` |  | Region |  |  | S/4 only entity (no ECC CDC mapping) |
| `Language` | `Language` | `String(2)` |  | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `TeleboxNumber` | `TeleboxNumber` | `String(15)` |  | Telebox Number |  |  | S/4 only entity (no ECC CDC mapping) |
| `PhoneNumber1` | `PhoneNumber1` | `String(16)` |  | Telephone 1 |  |  | S/4 only entity (no ECC CDC mapping) |
| `PhoneNumber2` | `PhoneNumber2` | `String(16)` |  | Telephone 2 |  |  | S/4 only entity (no ECC CDC mapping) |
| `FaxNumber` | `FaxNumber` | `String(31)` |  | Fax Number |  |  | S/4 only entity (no ECC CDC mapping) |
| `TeletexNumber` | `TeletexNumber` | `String(30)` |  | Teletex Number |  |  | S/4 only entity (no ECC CDC mapping) |
| `TelexNumber` | `TelexNumber` | `String(30)` |  | Telex Number |  |  | S/4 only entity (no ECC CDC mapping) |
| `DataCommunicationPhoneNumber` | `DataCommunicationPhoneNumber` | `String(14)` |  | Data line |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCenterPrinterDestination` | `CostCenterPrinterDestination` | `String(4)` |  | Printer Destination |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCenterStandardHierArea` | `CostCenterStandardHierArea` | `String(12)` |  | Hierarchy Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCollector` | `CostCollector` | `String(23)` |  | Cost Collector Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCenterIsComplete` | `CostCenterIsComplete` | `Boolean` |  | Complete |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsStatisticalCostCenter` | `IsStatisticalCostCenter` | `Boolean` |  | Cost Center Is Stat. |  |  | S/4 only entity (no ECC CDC mapping) |
| `ObjectInternalID` | `ObjectInternalID` | `String(22)` |  | Object Number |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCenterFunction` | `CostCenterFunction` | `String(3)` |  | Function |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCenterAlternativeFunction` | `CostCenterAlternativeFunction` | `String(3)` |  | Altern. Function |  |  | S/4 only entity (no ECC CDC mapping) |
| `FunctionalArea` | `FunctionalArea` | `String(16)` |  | Functional Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `ActyIndepFormulaPlanningTmpl` | `ActyIndepFormulaPlanningTmpl` | `String(10)` |  | Activity-Indep.Temp. |  |  | S/4 only entity (no ECC CDC mapping) |
| `ActyDepdntFormulaPlanningTmpl` | `ActyDepdntFormulaPlanningTmpl` | `String(10)` |  | Activity-Dep.Tmp |  |  | S/4 only entity (no ECC CDC mapping) |
| `ActyIndependentAllocationTmpl` | `ActyIndependentAllocationTmpl` | `String(10)` |  | Acty-IndepTemplAlloc |  |  | S/4 only entity (no ECC CDC mapping) |
| `ActyDependentAllocationTmpl` | `ActyDependentAllocationTmpl` | `String(10)` |  | Acty-Dep Templ.Alloc |  |  | S/4 only entity (no ECC CDC mapping) |
| `ActlIndepStatisticalKeyFigures` | `ActlIndepStatisticalKeyFigures` | `String(10)` |  | Templ.: Stat. KF |  |  | S/4 only entity (no ECC CDC mapping) |
| `ActlDepStatisticalKeyFigures` | `ActlDepStatisticalKeyFigures` | `String(10)` |  | Templ.: Stat. KF |  |  | S/4 only entity (no ECC CDC mapping) |
| `JointVenture` | `JointVenture` | `String(6)` |  | Joint Venture |  |  | S/4 only entity (no ECC CDC mapping) |
| `JointVentureRecoveryCode` | `JointVentureRecoveryCode` | `String(2)` |  | Recovery Indicator |  |  | S/4 only entity (no ECC CDC mapping) |
| `JointVentureEquityType` | `JointVentureEquityType` | `String(3)` |  | Equity Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `JointVentureObjectType` | `JointVentureObjectType` | `String(4)` |  | JV Object Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `JointVentureClass` | `JointVentureClass` | `String(3)` |  | JIB/JIBE Class |  |  | S/4 only entity (no ECC CDC mapping) |
| `JointVentureSubClass` | `JointVentureSubClass` | `String(5)` |  | JIB/JIBE Subclass A |  |  | S/4 only entity (no ECC CDC mapping) |
| `BudgetCarryingCostCenter` | `BudgetCarryingCostCenter` | `String(10)` |  | Budget Cost Center |  |  | S/4 only entity (no ECC CDC mapping) |
| `AvailabilityControlProfile` | `AvailabilityControlProfile` | `String(6)` |  | Availy Ctrl Prfl |  |  | S/4 only entity (no ECC CDC mapping) |
| `AvailabilityControlIsActive` | `AvailabilityControlIsActive` | `Boolean` |  | AVC is Active |  |  | S/4 only entity (no ECC CDC mapping) |
| `Fund` | `Fund` | `String(10)` |  | Fund |  |  | S/4 only entity (no ECC CDC mapping) |
| `GrantID` | `GrantID` | `String(20)` |  | Grant |  |  | S/4 only entity (no ECC CDC mapping) |
| `FundIsFixAssigned` | `FundIsFixAssigned` | `Boolean` |  | Fund Fixed Assignment |  |  | S/4 only entity (no ECC CDC mapping) |
| `GrantIDIsFixAssigned` | `GrantIDIsFixAssigned` | `Boolean` |  | Grant Fixed Assignment |  |  | S/4 only entity (no ECC CDC mapping) |
| `FunctionalAreaIsFixAssigned` | `FunctionalAreaIsFixAssigned` | `Boolean` |  | Functional Area Fixed Assignment |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCenterCreationTime` | `CostCenterCreationTime` | `String(6)` |  | Created At |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCenterLastChangedByUser` | `CostCenterLastChangedByUser` | `String(12)` |  | Last Changed By |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCenterLastChangedOnDate` | `CostCenterLastChangedOnDate` | `Date` |  | Last Changed On |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCenterLastChangedAtTime` | `CostCenterLastChangedAtTime` | `String(6)` |  | Last Changed At |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `CostCenterCategory`

- **ABAP Name:** `I_CostCenterCategory`
- **Label:** Cost Center Category
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `CostCenterCategory` | `CostCenterCategory` | `String(1)` | Y | Cost Center Category |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsBlkdForPrimaryCostsPosting` | `IsBlkdForPrimaryCostsPosting` | `Boolean` |  | Actual primary costs |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsBlkdForSecondaryCostsPosting` | `IsBlkdForSecondaryCostsPosting` | `Boolean` |  | Actl Sec. Costs |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsBlockedForRevenuePosting` | `IsBlockedForRevenuePosting` | `Boolean` |  | Actual Revenues |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsBlockedForCommitmentPosting` | `IsBlockedForCommitmentPosting` | `Boolean` |  | Commitment Update |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsBlockedForPlanPrimaryCosts` | `IsBlockedForPlanPrimaryCosts` | `Boolean` |  | Plan primary costs |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsBlockedForPlanSecondaryCosts` | `IsBlockedForPlanSecondaryCosts` | `Boolean` |  | Lock Plan Sec Costs |  |  | S/4 only entity (no ECC CDC mapping) |
| `IsBlockedForPlanRevenues` | `IsBlockedForPlanRevenues` | `Boolean` |  | Lock Planning Revn |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCenterAllocationMethod` | `CostCenterAllocationMethod` | `String(2)` |  | Allocation Methods |  |  | S/4 only entity (no ECC CDC mapping) |
| `ConsumptionQtyIsRecorded` | `ConsumptionQtyIsRecorded` | `Boolean` |  | Record Quantity |  |  | S/4 only entity (no ECC CDC mapping) |
| `FunctionalArea` | `FunctionalArea` | `String(16)` |  | Functional Area |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `CostCenterCategoryText`

- **ABAP Name:** `I_CostCenterCategoryText`
- **Label:** Cost Center Category - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCenterCategory` | `CostCenterCategory` | `String(1)` | Y | Cost Center Category |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCenterCategoryName` | `CostCenterCategoryName` | `String(20)` |  | Cost Ctr Cat Name |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `CostCenterHierarchy`

- **ABAP Name:** `I_CostCenterHierarchy`
- **Label:** Cost Center Hierarchy
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `ControllingArea` | `ControllingArea` | `String(4)` | Y | Controlling Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCenterHierarchy` | `CostCenterHierarchy` | `String(40)` | Y | Cost Center Hierarchy |  |  | S/4 only — no ECC equivalent; S/4 only entity (no ECC CDC mapping) |
| `ValidityEndDate` | `ValidityEndDate` | `Date` | Y | Validity End Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityStartDate` | `ValidityStartDate` | `Date` |  | Validity Start Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `LastChangedByUser` | `LastChangedByUser` | `String(12)` |  | Last Changed By |  |  | S/4 only entity (no ECC CDC mapping) |
| `LastChangeDateTime` | `LastChangeDateTime` | `DateTime` |  | Updated At |  |  | S/4 only entity (no ECC CDC mapping) |
| `LastChangeTime` | `LastChangeTime` | `DateTime` |  | Updated At |  |  | S/4 only entity (no ECC CDC mapping) |
| `HierarchyShortID` | `HierarchyShortID` | `String(20)` |  | Hierarchy ID |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `CostCenterHierarchyNode`

- **ABAP Name:** `I_CostCenterHierarchyNode`
- **Label:** Cost Center Hierarchy Node
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `ControllingArea` | `ControllingArea` | `String(4)` | Y | Controlling Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCenterHierarchy` | `CostCenterHierarchy` | `String(40)` | Y | Cost Center Hierarchy |  | _Hierarchy | S/4 only — no ECC equivalent; S/4 only entity (no ECC CDC mapping) |
| `HierarchyNode` | `HierarchyNode` | `String(50)` | Y | Node |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityEndDate` | `ValidityEndDate` | `Date` | Y | Validity End Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `ParentNode` | `ParentNode` | `String(50)` |  | Par. Node |  |  | S/4 only entity (no ECC CDC mapping) |
| `HierarchyVersion` | `HierarchyVersion` | `String(15)` |  | Version |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityStartDate` | `ValidityStartDate` | `Date` |  | Validity Start Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCenter` | `CostCenter` | `String(10)` |  | Cost Center |  | _CostCenter | S/4 only entity (no ECC CDC mapping) |
| `SequenceNumber` | `SequenceNumber` | `String(56)` |  |  |  |  | S/4 only entity (no ECC CDC mapping) |
| `HierarchyNodeSequence` | `HierarchyNodeSequence` | `String(6)` |  | Sequence Number |  |  | S/4 only entity (no ECC CDC mapping) |
| `HierarchyNodeLevel` | `HierarchyNodeLevel` | `String(6)` |  | Hierarchy Level |  |  | S/4 only entity (no ECC CDC mapping) |
| `NodeType` | `NodeType` | `String(1)` |  | Node Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `HierarchyNodeVal` | `HierarchyNodeVal` | `String(40)` |  | Value |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `CostCenterHierarchyNodeText`

- **ABAP Name:** `I_CostCenterHierarchyNodeT`
- **Label:** Cost Center Hierarchy Node - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `ControllingArea` | `ControllingArea` | `String(4)` | Y | Controlling Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCenterHierarchy` | `CostCenterHierarchy` | `String(40)` | Y | Cost Center Hierarchy |  | _Hierarchy | S/4 only — no ECC equivalent; S/4 only entity (no ECC CDC mapping) |
| `HierarchyNode` | `HierarchyNode` | `String(50)` | Y | Node |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityEndDate` | `ValidityEndDate` | `Date` | Y | Valid To |  |  | S/4 only entity (no ECC CDC mapping) |
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `HierarchyNodeText` | `HierarchyNodeText` | `String(50)` |  | Description |  |  | S/4 only entity (no ECC CDC mapping) |
| `HierarchyNodeShortText` | `HierarchyNodeShortText` | `String(20)` |  |  |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityStartDate` | `ValidityStartDate` | `Date` |  | Valid From |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `CostCenterHierarchyText`

- **ABAP Name:** `I_CostCenterHierarchyText`
- **Label:** Cost Center Hierarchy - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `ControllingArea` | `ControllingArea` | `String(12)` | Y | Hierarchy Class |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCenterHierarchy` | `CostCenterHierarchy` | `String(40)` | Y | Cost Center Hierarchy |  |  | S/4 only — no ECC equivalent; S/4 only entity (no ECC CDC mapping) |
| `ValidityEndDate` | `ValidityEndDate` | `Date` | Y | Valid To |  |  | S/4 only entity (no ECC CDC mapping) |
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityStartDate` | `ValidityStartDate` | `Date` |  | Valid From |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCenterHierarchyName` | `CostCenterHierarchyName` | `String(50)` |  | Description |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `CostCenterText`

- **ABAP Name:** `I_CostCenterText`
- **Label:** Cost Center - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `CostCenter` | `CostCenter` | `String(10)` | Y | Cost Center |  |  | S/4 only entity (no ECC CDC mapping) |
| `ControllingArea` | `ControllingArea` | `String(4)` | Y | Controlling Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityEndDate` | `ValidityEndDate` | `Date` | Y | Valid To |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityStartDate` | `ValidityStartDate` | `Date` |  | Valid From |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCenterName` | `CostCenterName` | `String(20)` |  | Cost Center Name |  |  | S/4 only entity (no ECC CDC mapping) |
| `CostCenterDescription` | `CostCenterDescription` | `String(40)` |  | Cost Center Desc. |  |  | S/4 only entity (no ECC CDC mapping) |
