# ProfitCenter

> Source file: `sap-s4com-ProfitCenter-v1.json`


## Entity: `PrftCtrCompanyCodeAssignment`

- **ABAP Name:** `I_PrftCtrCompanyCodeAssignment`
- **Label:** Company code assignment to profit center
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `ControllingArea` |  |  |  | `String(4)` | Y | Controlling Area |  |  | S/4 only entity — no ECC CDC mapping |
| `ProfitCenter` |  |  |  | `String(10)` | Y | Profit Center |  |  | S/4 only entity — no ECC CDC mapping |
| `CompanyCode` |  |  |  | `String(4)` | Y |  |  |  | S/4 only entity — no ECC CDC mapping |
| `JointVentureObjectType` |  |  |  | `String(4)` |  | JV Object Type |  |  | S/4 only entity — no ECC CDC mapping |
| `JointVentureClass` |  |  |  | `String(3)` |  | JIB/JIBE Class |  |  | S/4 only entity — no ECC CDC mapping |
| `JointVentureSubClass` |  |  |  | `String(5)` |  | JIB/JIBE Subclass A |  |  | S/4 only entity — no ECC CDC mapping |
| `JointVenture` |  |  |  | `String(6)` |  | Joint Venture |  |  | S/4 only entity — no ECC CDC mapping |
| `JointVentureRecoveryCode` |  |  |  | `String(2)` |  | Recovery Indicator |  |  | S/4 only entity — no ECC CDC mapping |
| `JointVentureEquityType` |  |  |  | `String(3)` |  | Equity Type |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `ProfitCenter`

- **ABAP Name:** `I_ProfitCenter`
- **Label:** Profit Center
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `ControllingArea` |  |  |  | `String(4)` | Y | Controlling Area |  |  | S/4 only entity — no ECC CDC mapping |
| `ProfitCenter` |  |  |  | `String(10)` | Y | Profit Center |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityEndDate` |  |  |  | `Date` | Y | Valid To |  |  | S/4 only entity — no ECC CDC mapping |
| `ProfitCtrResponsiblePersonName` |  |  |  | `String(20)` |  | Person Resp. for PC |  |  | S/4 only entity — no ECC CDC mapping |
| `CompanyCode` |  |  |  | `String(4)` |  | Company Code |  |  | S/4 only entity — no ECC CDC mapping |
| `ProfitCtrResponsibleUser` |  |  |  | `String(12)` |  | User Responsible |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityStartDate` |  |  |  | `Date` |  | Valid From |  |  | S/4 only entity — no ECC CDC mapping |
| `Department` |  |  |  | `String(12)` |  | Department |  |  | S/4 only entity — no ECC CDC mapping |
| `ProfitCenterStandardHierarchy` |  |  |  | `String(12)` |  | Hierarchy Area |  |  | S/4 only entity — no ECC CDC mapping |
| `Segment` |  |  |  | `String(10)` |  | Segment |  |  | S/4 only entity — no ECC CDC mapping |
| `ProfitCenterIsBlocked` |  |  |  | `Boolean` |  | Lock indicator |  |  | S/4 only entity — no ECC CDC mapping |
| `FormulaPlanningTemplate` |  |  |  | `String(10)` |  | Form. Planning Temp. |  |  | S/4 only entity — no ECC CDC mapping |
| `FormOfAddress` |  |  |  | `String(15)` |  | Title |  |  | S/4 only entity — no ECC CDC mapping |
| `AddressName` |  |  |  | `String(35)` |  | Name |  |  | S/4 only entity — no ECC CDC mapping |
| `AdditionalName` |  |  |  | `String(35)` |  | Name 2 |  |  | S/4 only entity — no ECC CDC mapping |
| `ProfitCenterAddrName3` |  |  |  | `String(35)` |  | Name 3 |  |  | S/4 only entity — no ECC CDC mapping |
| `ProfitCenterAddrName4` |  |  |  | `String(35)` |  | Name 4 |  |  | S/4 only entity — no ECC CDC mapping |
| `StreetAddressName` |  |  |  | `String(35)` |  | Street |  |  | S/4 only entity — no ECC CDC mapping |
| `POBox` |  |  |  | `String(10)` |  | PO Box |  |  | S/4 only entity — no ECC CDC mapping |
| `CityName` |  |  |  | `String(35)` |  | City |  |  | S/4 only entity — no ECC CDC mapping |
| `PostalCode` |  |  |  | `String(10)` |  | Postal Code |  |  | S/4 only entity — no ECC CDC mapping |
| `POBoxPostalCode` |  |  |  | `String(10)` |  | PO Box Postal Code |  |  | S/4 only entity — no ECC CDC mapping |
| `District` |  |  |  | `String(35)` |  | District |  |  | S/4 only entity — no ECC CDC mapping |
| `Country` |  |  |  | `String(3)` |  | Country/Region Key |  |  | S/4 only entity — no ECC CDC mapping |
| `Region` |  |  |  | `String(3)` |  | Region |  |  | S/4 only entity — no ECC CDC mapping |
| `TaxJurisdiction` |  |  |  | `String(15)` |  | Tax Jurisdiction |  |  | S/4 only entity — no ECC CDC mapping |
| `Language` |  |  |  | `String(2)` |  | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `PhoneNumber1` |  |  |  | `String(16)` |  | Telephone 1 |  |  | S/4 only entity — no ECC CDC mapping |
| `PhoneNumber2` |  |  |  | `String(16)` |  | Telephone 2 |  |  | S/4 only entity — no ECC CDC mapping |
| `TeleboxNumber` |  |  |  | `String(15)` |  | Telebox Number |  |  | S/4 only entity — no ECC CDC mapping |
| `TelexNumber` |  |  |  | `String(30)` |  | Telex Number |  |  | S/4 only entity — no ECC CDC mapping |
| `FaxNumber` |  |  |  | `String(31)` |  | Fax Number |  |  | S/4 only entity — no ECC CDC mapping |
| `TeletexNumber` |  |  |  | `String(30)` |  | Teletex Number |  |  | S/4 only entity — no ECC CDC mapping |
| `DataCommunicationPhoneNumber` |  |  |  | `String(14)` |  | Data line |  |  | S/4 only entity — no ECC CDC mapping |
| `ProfitCenterPrinterName` |  |  |  | `String(4)` |  | Printer name |  |  | S/4 only entity — no ECC CDC mapping |
| `ProfitCenterCreatedByUser` |  |  |  | `String(12)` |  | Created By |  |  | S/4 only entity — no ECC CDC mapping |
| `ProfitCenterCreationDate` |  |  |  | `Date` |  | Entered On |  |  | S/4 only entity — no ECC CDC mapping |
| `LogicalSystem` |  |  |  | `String(10)` |  | Logical System |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `ProfitCenterHierarchy`

- **ABAP Name:** `I_ProfitCenterHierarchy`
- **Label:** Profit Center Hierarchy
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `ControllingArea` |  |  |  | `String(4)` | Y | Controlling Area |  |  | S/4 only entity — no ECC CDC mapping |
| `ProfitCenterHierarchy` |  |  |  | `String(40)` | Y | Profit Center Hierarchy |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityEndDate` |  |  |  | `Date` | Y | Validity End Date |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityStartDate` |  |  |  | `Date` |  | Validity Start Date |  |  | S/4 only entity — no ECC CDC mapping |
| `LastChangedByUser` |  |  |  | `String(12)` |  | Last Changed By |  |  | S/4 only entity — no ECC CDC mapping |
| `LastChangeDateTime` |  |  |  | `DateTime` |  | Updated At |  |  | S/4 only entity — no ECC CDC mapping |
| `LastChangeTime` |  |  |  | `DateTime` |  | Updated At |  |  | S/4 only entity — no ECC CDC mapping |
| `HierarchyShortID` |  |  |  | `String(20)` |  | Hierarchy ID |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `ProfitCenterHierarchyNode`

- **ABAP Name:** `I_ProfitCenterHierarchyNode`
- **Label:** Profit Center Hierarchy Node
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `ControllingArea` |  |  |  | `String(4)` | Y | Controlling Area |  |  | S/4 only entity — no ECC CDC mapping |
| `ProfitCenterHierarchy` |  |  |  | `String(40)` | Y | Profit Center Hierarchy |  | _Hierarchy | S/4 only entity — no ECC CDC mapping |
| `HierarchyNode` |  |  |  | `String(50)` | Y | Node |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityEndDate` |  |  |  | `Date` | Y | Validity End Date |  |  | S/4 only entity — no ECC CDC mapping |
| `ParentNode` |  |  |  | `String(50)` |  | Par. Node |  |  | S/4 only entity — no ECC CDC mapping |
| `HierarchyVersion` |  |  |  | `String(15)` |  | Version |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityStartDate` |  |  |  | `Date` |  | Validity Start Date |  |  | S/4 only entity — no ECC CDC mapping |
| `ProfitCenter` |  |  |  | `String(10)` |  | Profit Center |  | _ProfitCenter | S/4 only entity — no ECC CDC mapping |
| `SequenceNumber` |  |  |  | `String(56)` |  |  |  |  | S/4 only entity — no ECC CDC mapping |
| `HierarchyNodeSequence` |  |  |  | `String(6)` |  | Sequence Number |  |  | S/4 only entity — no ECC CDC mapping |
| `HierarchyNodeLevel` |  |  |  | `String(6)` |  | Hierarchy Level |  |  | S/4 only entity — no ECC CDC mapping |
| `NodeType` |  |  |  | `String(1)` |  | Node Type |  |  | S/4 only entity — no ECC CDC mapping |
| `HierarchyNodeVal` |  |  |  | `String(40)` |  | Value |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `ProfitCenterHierarchyNodeText`

- **ABAP Name:** `I_ProfitCenterHierarchyNodeT`
- **Label:** Profit Center Hierarchy Node - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `ControllingArea` |  |  |  | `String(4)` | Y | Controlling Area |  |  | S/4 only entity — no ECC CDC mapping |
| `ProfitCenterHierarchy` |  |  |  | `String(40)` | Y | Profit Center Hierarchy |  | _Hierarchy | S/4 only entity — no ECC CDC mapping |
| `HierarchyNode` |  |  |  | `String(50)` | Y | Node |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityEndDate` |  |  |  | `Date` | Y | Validity End Date |  |  | S/4 only entity — no ECC CDC mapping |
| `Language` |  |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `HierarchyNodeText` |  |  |  | `String(50)` |  | Description |  |  | S/4 only entity — no ECC CDC mapping |
| `HierarchyNodeShortText` |  |  |  | `String(20)` |  |  |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityStartDate` |  |  |  | `Date` |  | Validity Start Date |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `ProfitCenterHierarchyText`

- **ABAP Name:** `I_ProfitCenterHierarchyText`
- **Label:** Profit Center Hierarchy - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `ControllingArea` |  |  |  | `String(12)` | Y | Hierarchy Class |  |  | S/4 only entity — no ECC CDC mapping |
| `ProfitCenterHierarchy` |  |  |  | `String(40)` | Y | Profit Center Hierarchy |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityEndDate` |  |  |  | `Date` | Y | Valid To |  |  | S/4 only entity — no ECC CDC mapping |
| `Language` |  |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityStartDate` |  |  |  | `Date` |  | Valid From |  |  | S/4 only entity — no ECC CDC mapping |
| `ProfitCenterHierarchyName` |  |  |  | `String(50)` |  | Description |  |  | S/4 only entity — no ECC CDC mapping |


## Entity: `ProfitCenterText`

- **ABAP Name:** `I_ProfitCenterText`
- **Label:** Profit Center - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Data Element | ABAP Field | ABAP Table | Type | Key | Label | Curr/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|
| `Language` |  |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity — no ECC CDC mapping |
| `ControllingArea` |  |  |  | `String(4)` | Y | Controlling Area |  |  | S/4 only entity — no ECC CDC mapping |
| `ProfitCenter` |  |  |  | `String(10)` | Y | Profit Center |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityEndDate` |  |  |  | `Date` | Y | Valid To |  |  | S/4 only entity — no ECC CDC mapping |
| `ValidityStartDate` |  |  |  | `Date` |  | Valid From |  |  | S/4 only entity — no ECC CDC mapping |
| `ProfitCenterName` |  |  |  | `String(20)` |  | Profit Center Name |  |  | S/4 only entity — no ECC CDC mapping |
| `ProfitCenterLongName` |  |  |  | `String(40)` |  | Profit Center Description |  |  | S/4 only entity — no ECC CDC mapping |
