# ProfitCenter

> Source file: `sap-s4com-ProfitCenter-v1.json`


## Entity: `PrftCtrCompanyCodeAssignment`

- **ABAP Name:** `I_PrftCtrCompanyCodeAssignment`
- **Label:** Company code assignment to profit center
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `ControllingArea` | `ControllingArea` | `String(4)` | Y | Controlling Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProfitCenter` | `ProfitCenter` | `String(10)` | Y | Profit Center |  |  | S/4 only entity (no ECC CDC mapping) |
| `CompanyCode` | `CompanyCode` | `String(4)` | Y |  |  |  | S/4 only entity (no ECC CDC mapping) |
| `JointVentureObjectType` | `JointVentureObjectType` | `String(4)` |  | JV Object Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `JointVentureClass` | `JointVentureClass` | `String(3)` |  | JIB/JIBE Class |  |  | S/4 only entity (no ECC CDC mapping) |
| `JointVentureSubClass` | `JointVentureSubClass` | `String(5)` |  | JIB/JIBE Subclass A |  |  | S/4 only entity (no ECC CDC mapping) |
| `JointVenture` | `JointVenture` | `String(6)` |  | Joint Venture |  |  | S/4 only entity (no ECC CDC mapping) |
| `JointVentureRecoveryCode` | `JointVentureRecoveryCode` | `String(2)` |  | Recovery Indicator |  |  | S/4 only entity (no ECC CDC mapping) |
| `JointVentureEquityType` | `JointVentureEquityType` | `String(3)` |  | Equity Type |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `ProfitCenter`

- **ABAP Name:** `I_ProfitCenter`
- **Label:** Profit Center
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `ControllingArea` | `ControllingArea` | `String(4)` | Y | Controlling Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProfitCenter` | `ProfitCenter` | `String(10)` | Y | Profit Center |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityEndDate` | `ValidityEndDate` | `Date` | Y | Valid To |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProfitCtrResponsiblePersonName` | `ProfitCtrResponsiblePersonName` | `String(20)` |  | Person Resp. for PC |  |  | S/4 only entity (no ECC CDC mapping) |
| `CompanyCode` | `CompanyCode` | `String(4)` |  | Company Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProfitCtrResponsibleUser` | `ProfitCtrResponsibleUser` | `String(12)` |  | User Responsible |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityStartDate` | `ValidityStartDate` | `Date` |  | Valid From |  |  | S/4 only entity (no ECC CDC mapping) |
| `Department` | `Department` | `String(12)` |  | Department |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProfitCenterStandardHierarchy` | `ProfitCenterStandardHierarchy` | `String(12)` |  | Hierarchy Area |  |  | S/4 only — no ECC equivalent; S/4 only entity (no ECC CDC mapping) |
| `Segment` | `Segment` | `String(10)` |  | Segment |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProfitCenterIsBlocked` | `ProfitCenterIsBlocked` | `Boolean` |  | Lock indicator |  |  | S/4 only entity (no ECC CDC mapping) |
| `FormulaPlanningTemplate` | `FormulaPlanningTemplate` | `String(10)` |  | Form. Planning Temp. |  |  | S/4 only entity (no ECC CDC mapping) |
| `FormOfAddress` | `FormOfAddress` | `String(15)` |  | Title |  |  | S/4 only entity (no ECC CDC mapping) |
| `AddressName` | `AddressName` | `String(35)` |  | Name |  |  | S/4 only entity (no ECC CDC mapping) |
| `AdditionalName` | `AdditionalName` | `String(35)` |  | Name 2 |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProfitCenterAddrName3` | `ProfitCenterAddrName3` | `String(35)` |  | Name 3 |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProfitCenterAddrName4` | `ProfitCenterAddrName4` | `String(35)` |  | Name 4 |  |  | S/4 only entity (no ECC CDC mapping) |
| `StreetAddressName` | `StreetAddressName` | `String(35)` |  | Street |  |  | S/4 only entity (no ECC CDC mapping) |
| `POBox` | `POBox` | `String(10)` |  | PO Box |  |  | S/4 only entity (no ECC CDC mapping) |
| `CityName` | `CityName` | `String(35)` |  | City |  |  | S/4 only entity (no ECC CDC mapping) |
| `PostalCode` | `PostalCode` | `String(10)` |  | Postal Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `POBoxPostalCode` | `POBoxPostalCode` | `String(10)` |  | PO Box Postal Code |  |  | S/4 only entity (no ECC CDC mapping) |
| `District` | `District` | `String(35)` |  | District |  |  | S/4 only entity (no ECC CDC mapping) |
| `Country` | `Country` | `String(3)` |  | Country/Region Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `Region` | `Region` | `String(3)` |  | Region |  |  | S/4 only entity (no ECC CDC mapping) |
| `TaxJurisdiction` | `TaxJurisdiction` | `String(15)` |  | Tax Jurisdiction |  |  | S/4 only entity (no ECC CDC mapping) |
| `Language` | `Language` | `String(2)` |  | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `PhoneNumber1` | `PhoneNumber1` | `String(16)` |  | Telephone 1 |  |  | S/4 only entity (no ECC CDC mapping) |
| `PhoneNumber2` | `PhoneNumber2` | `String(16)` |  | Telephone 2 |  |  | S/4 only entity (no ECC CDC mapping) |
| `TeleboxNumber` | `TeleboxNumber` | `String(15)` |  | Telebox Number |  |  | S/4 only entity (no ECC CDC mapping) |
| `TelexNumber` | `TelexNumber` | `String(30)` |  | Telex Number |  |  | S/4 only entity (no ECC CDC mapping) |
| `FaxNumber` | `FaxNumber` | `String(31)` |  | Fax Number |  |  | S/4 only entity (no ECC CDC mapping) |
| `TeletexNumber` | `TeletexNumber` | `String(30)` |  | Teletex Number |  |  | S/4 only entity (no ECC CDC mapping) |
| `DataCommunicationPhoneNumber` | `DataCommunicationPhoneNumber` | `String(14)` |  | Data line |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProfitCenterPrinterName` | `ProfitCenterPrinterName` | `String(4)` |  | Printer name |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProfitCenterCreatedByUser` | `ProfitCenterCreatedByUser` | `String(12)` |  | Created By |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProfitCenterCreationDate` | `ProfitCenterCreationDate` | `Date` |  | Entered On |  |  | S/4 only entity (no ECC CDC mapping) |
| `LogicalSystem` | `LogicalSystem` | `String(10)` |  | Logical System |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `ProfitCenterHierarchy`

- **ABAP Name:** `I_ProfitCenterHierarchy`
- **Label:** Profit Center Hierarchy
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `ControllingArea` | `ControllingArea` | `String(4)` | Y | Controlling Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProfitCenterHierarchy` | `ProfitCenterHierarchy` | `String(40)` | Y | Profit Center Hierarchy |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityEndDate` | `ValidityEndDate` | `Date` | Y | Validity End Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityStartDate` | `ValidityStartDate` | `Date` |  | Validity Start Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `LastChangedByUser` | `LastChangedByUser` | `String(12)` |  | Last Changed By |  |  | S/4 only entity (no ECC CDC mapping) |
| `LastChangeDateTime` | `LastChangeDateTime` | `DateTime` |  | Updated At |  |  | S/4 only entity (no ECC CDC mapping) |
| `LastChangeTime` | `LastChangeTime` | `DateTime` |  | Updated At |  |  | S/4 only entity (no ECC CDC mapping) |
| `HierarchyShortID` | `HierarchyShortID` | `String(20)` |  | Hierarchy ID |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `ProfitCenterHierarchyNode`

- **ABAP Name:** `I_ProfitCenterHierarchyNode`
- **Label:** Profit Center Hierarchy Node
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `ControllingArea` | `ControllingArea` | `String(4)` | Y | Controlling Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProfitCenterHierarchy` | `ProfitCenterHierarchy` | `String(40)` | Y | Profit Center Hierarchy |  | _Hierarchy | S/4 only entity (no ECC CDC mapping) |
| `HierarchyNode` | `HierarchyNode` | `String(50)` | Y | Node |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityEndDate` | `ValidityEndDate` | `Date` | Y | Validity End Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `ParentNode` | `ParentNode` | `String(50)` |  | Par. Node |  |  | S/4 only entity (no ECC CDC mapping) |
| `HierarchyVersion` | `HierarchyVersion` | `String(15)` |  | Version |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityStartDate` | `ValidityStartDate` | `Date` |  | Validity Start Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProfitCenter` | `ProfitCenter` | `String(10)` |  | Profit Center |  | _ProfitCenter | S/4 only entity (no ECC CDC mapping) |
| `SequenceNumber` | `SequenceNumber` | `String(56)` |  |  |  |  | S/4 only entity (no ECC CDC mapping) |
| `HierarchyNodeSequence` | `HierarchyNodeSequence` | `String(6)` |  | Sequence Number |  |  | S/4 only entity (no ECC CDC mapping) |
| `HierarchyNodeLevel` | `HierarchyNodeLevel` | `String(6)` |  | Hierarchy Level |  |  | S/4 only entity (no ECC CDC mapping) |
| `NodeType` | `NodeType` | `String(1)` |  | Node Type |  |  | S/4 only entity (no ECC CDC mapping) |
| `HierarchyNodeVal` | `HierarchyNodeVal` | `String(40)` |  | Value |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `ProfitCenterHierarchyNodeText`

- **ABAP Name:** `I_ProfitCenterHierarchyNodeT`
- **Label:** Profit Center Hierarchy Node - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `ControllingArea` | `ControllingArea` | `String(4)` | Y | Controlling Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProfitCenterHierarchy` | `ProfitCenterHierarchy` | `String(40)` | Y | Profit Center Hierarchy |  | _Hierarchy | S/4 only entity (no ECC CDC mapping) |
| `HierarchyNode` | `HierarchyNode` | `String(50)` | Y | Node |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityEndDate` | `ValidityEndDate` | `Date` | Y | Validity End Date |  |  | S/4 only entity (no ECC CDC mapping) |
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `HierarchyNodeText` | `HierarchyNodeText` | `String(50)` |  | Description |  |  | S/4 only entity (no ECC CDC mapping) |
| `HierarchyNodeShortText` | `HierarchyNodeShortText` | `String(20)` |  |  |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityStartDate` | `ValidityStartDate` | `Date` |  | Validity Start Date |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `ProfitCenterHierarchyText`

- **ABAP Name:** `I_ProfitCenterHierarchyText`
- **Label:** Profit Center Hierarchy - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `ControllingArea` | `ControllingArea` | `String(12)` | Y | Hierarchy Class |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProfitCenterHierarchy` | `ProfitCenterHierarchy` | `String(40)` | Y | Profit Center Hierarchy |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityEndDate` | `ValidityEndDate` | `Date` | Y | Valid To |  |  | S/4 only entity (no ECC CDC mapping) |
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityStartDate` | `ValidityStartDate` | `Date` |  | Valid From |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProfitCenterHierarchyName` | `ProfitCenterHierarchyName` | `String(50)` |  | Description |  |  | S/4 only entity (no ECC CDC mapping) |


## Entity: `ProfitCenterText`

- **ABAP Name:** `I_ProfitCenterText`
- **Label:** Profit Center - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Name | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|
| `Language` | `Language` | `String(2)` | Y | Language Key |  |  | S/4 only entity (no ECC CDC mapping) |
| `ControllingArea` | `ControllingArea` | `String(4)` | Y | Controlling Area |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProfitCenter` | `ProfitCenter` | `String(10)` | Y | Profit Center |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityEndDate` | `ValidityEndDate` | `Date` | Y | Valid To |  |  | S/4 only entity (no ECC CDC mapping) |
| `ValidityStartDate` | `ValidityStartDate` | `Date` |  | Valid From |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProfitCenterName` | `ProfitCenterName` | `String(20)` |  | Profit Center Name |  |  | S/4 only entity (no ECC CDC mapping) |
| `ProfitCenterLongName` | `ProfitCenterLongName` | `String(40)` |  | Profit Center Description |  |  | S/4 only entity (no ECC CDC mapping) |
