# ProfitCenter

> Source file: `sap-s4com-ProfitCenter-v1.json`


## Entity: `PrftCtrCompanyCodeAssignment`

- **ABAP CDS Name:** `I_PrftCtrCompanyCodeAssignment`
- **Label:** Company code assignment to profit center
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** CEPC

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `ControllingArea` |  |  |  |  |  | `String(4)` | Y | Controlling Area |  |  |
| `ProfitCenter` |  |  |  |  |  | `String(10)` | Y | Profit Center |  |  |
| `CompanyCode` |  |  |  |  |  | `String(4)` | Y |  |  |  |
| `JointVentureObjectType` |  |  |  |  |  | `String(4)` |  | JV Object Type |  |  |
| `JointVentureClass` |  |  |  |  |  | `String(3)` |  | JIB/JIBE Class |  |  |
| `JointVentureSubClass` |  |  |  |  |  | `String(5)` |  | JIB/JIBE Subclass A |  |  |
| `JointVenture` |  |  |  |  |  | `String(6)` |  | Joint Venture |  |  |
| `JointVentureRecoveryCode` |  |  |  |  |  | `String(2)` |  | Recovery Indicator |  |  |
| `JointVentureEquityType` |  |  |  |  |  | `String(3)` |  | Equity Type |  |  |


## Entity: `ProfitCenter`

- **ABAP CDS Name:** `I_ProfitCenter`
- **Label:** Profit Center
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** CEPC, CEPCT

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `ControllingArea` |  | `CEPC` | `KOKRS` |  |  | `String(4)` | Y | Controlling Area |  |  |
| `ProfitCenter` |  | `CEPC` | `PRCTR` |  |  | `String(10)` | Y | Profit Center |  |  |
| `ValidityEndDate` |  | `CEPC` | `DATBI` |  |  | `Date` | Y | Valid To |  |  |
| `ProfitCtrResponsiblePersonName` |  |  |  |  |  | `String(20)` |  | Person Resp. for PC |  |  |
| `CompanyCode` |  | `CEPC` | `BUKRS` |  |  | `String(4)` |  | Company Code |  |  |
| `ProfitCtrResponsibleUser` |  |  |  |  |  | `String(12)` |  | User Responsible |  |  |
| `ValidityStartDate` |  | `CEPC` | `DATAB` |  |  | `Date` |  | Valid From |  |  |
| `Department` |  | `CEPC` | `ABTEI` |  |  | `String(12)` |  | Department |  |  |
| `ProfitCenterStandardHierarchy` |  |  |  |  |  | `String(12)` |  | Hierarchy Area |  |  |
| `Segment` |  | `CEPC` | `SEGMENT` |  |  | `String(10)` |  | Segment |  |  |
| `ProfitCenterIsBlocked` |  |  |  |  |  | `Boolean` |  | Lock indicator |  |  |
| `FormulaPlanningTemplate` |  |  |  |  |  | `String(10)` |  | Form. Planning Temp. |  |  |
| `FormOfAddress` |  |  |  |  |  | `String(15)` |  | Title |  |  |
| `AddressName` |  |  |  |  |  | `String(35)` |  | Name |  |  |
| `AdditionalName` |  |  |  |  |  | `String(35)` |  | Name 2 |  |  |
| `ProfitCenterAddrName3` |  |  |  |  |  | `String(35)` |  | Name 3 |  |  |
| `ProfitCenterAddrName4` |  |  |  |  |  | `String(35)` |  | Name 4 |  |  |
| `StreetAddressName` |  |  |  |  |  | `String(35)` |  | Street |  |  |
| `POBox` |  |  |  |  |  | `String(10)` |  | PO Box |  |  |
| `CityName` |  |  |  |  |  | `String(35)` |  | City |  |  |
| `PostalCode` |  |  |  |  |  | `String(10)` |  | Postal Code |  |  |
| `POBoxPostalCode` |  |  |  |  |  | `String(10)` |  | PO Box Postal Code |  |  |
| `District` |  |  |  |  |  | `String(35)` |  | District |  |  |
| `Country` |  | `CEPC` | `LAND1` |  |  | `String(3)` |  | Country/Region Key |  |  |
| `Region` |  |  |  |  |  | `String(3)` |  | Region |  |  |
| `TaxJurisdiction` |  |  |  |  |  | `String(15)` |  | Tax Jurisdiction |  |  |
| `Language` |  | `CEPCT` | `SPRAS` |  |  | `String(2)` |  | Language Key |  |  |
| `PhoneNumber1` |  |  |  |  |  | `String(16)` |  | Telephone 1 |  |  |
| `PhoneNumber2` |  |  |  |  |  | `String(16)` |  | Telephone 2 |  |  |
| `TeleboxNumber` |  |  |  |  |  | `String(15)` |  | Telebox Number |  |  |
| `TelexNumber` |  |  |  |  |  | `String(30)` |  | Telex Number |  |  |
| `FaxNumber` |  |  |  |  |  | `String(31)` |  | Fax Number |  |  |
| `TeletexNumber` |  |  |  |  |  | `String(30)` |  | Teletex Number |  |  |
| `DataCommunicationPhoneNumber` |  |  |  |  |  | `String(14)` |  | Data line |  |  |
| `ProfitCenterPrinterName` |  |  |  |  |  | `String(4)` |  | Printer name |  |  |
| `ProfitCenterCreatedByUser` |  |  |  |  |  | `String(12)` |  | Created By |  |  |
| `ProfitCenterCreationDate` |  |  |  |  |  | `Date` |  | Entered On |  |  |
| `LogicalSystem` |  |  |  |  |  | `String(10)` |  | Logical System |  |  |


## Entity: `ProfitCenterHierarchy`

- **ABAP CDS Name:** `I_ProfitCenterHierarchy`
- **Label:** Profit Center Hierarchy
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** SETHEADER, SETHEADERT

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `ControllingArea` |  |  |  |  |  | `String(4)` | Y | Controlling Area |  |  |
| `ProfitCenterHierarchy` |  |  |  |  |  | `String(40)` | Y | Profit Center Hierarchy |  |  |
| `ValidityEndDate` |  |  |  |  |  | `Date` | Y | Validity End Date |  |  |
| `ValidityStartDate` |  |  |  |  |  | `Date` |  | Validity Start Date |  |  |
| `LastChangedByUser` |  |  |  |  |  | `String(12)` |  | Last Changed By |  |  |
| `LastChangeDateTime` |  |  |  |  |  | `DateTime` |  | Updated At |  |  |
| `LastChangeTime` |  |  |  |  |  | `DateTime` |  | Updated At |  |  |
| `HierarchyShortID` |  |  |  |  |  | `String(20)` |  | Hierarchy ID |  |  |


## Entity: `ProfitCenterHierarchyNode`

- **ABAP CDS Name:** `I_ProfitCenterHierarchyNode`
- **Label:** Profit Center Hierarchy Node
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** SETHEADER, SETNODE, SETLEAF

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `ControllingArea` |  |  |  |  |  | `String(4)` | Y | Controlling Area |  |  |
| `ProfitCenterHierarchy` |  |  |  |  |  | `String(40)` | Y | Profit Center Hierarchy |  |  |
| `HierarchyNode` |  |  |  |  |  | `String(50)` | Y | Node |  |  |
| `ValidityEndDate` |  |  |  |  |  | `Date` | Y | Validity End Date |  |  |
| `ParentNode` |  |  |  |  |  | `String(50)` |  | Par. Node |  |  |
| `HierarchyVersion` |  |  |  |  |  | `String(15)` |  | Version |  |  |
| `ValidityStartDate` |  |  |  |  |  | `Date` |  | Validity Start Date |  |  |
| `ProfitCenter` |  |  |  |  |  | `String(10)` |  | Profit Center |  |  |
| `SequenceNumber` |  |  |  |  |  | `String(56)` |  |  |  |  |
| `HierarchyNodeSequence` |  |  |  |  |  | `String(6)` |  | Sequence Number |  |  |
| `HierarchyNodeLevel` |  |  |  |  |  | `String(6)` |  | Hierarchy Level |  |  |
| `NodeType` |  |  |  |  |  | `String(1)` |  | Node Type |  |  |
| `HierarchyNodeVal` |  |  |  |  |  | `String(40)` |  | Value |  |  |


## Entity: `ProfitCenterHierarchyNodeText`

- **ABAP CDS Name:** `I_ProfitCenterHierarchyNodeT`
- **Label:** Profit Center Hierarchy Node - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** SETHEADERT

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `ControllingArea` |  |  |  |  |  | `String(4)` | Y | Controlling Area |  |  |
| `ProfitCenterHierarchy` |  |  |  |  |  | `String(40)` | Y | Profit Center Hierarchy |  |  |
| `HierarchyNode` |  |  |  |  |  | `String(50)` | Y | Node |  |  |
| `ValidityEndDate` |  |  |  |  |  | `Date` | Y | Validity End Date |  |  |
| `Language` |  |  |  |  |  | `String(2)` | Y | Language Key |  |  |
| `HierarchyNodeText` |  |  |  |  |  | `String(50)` |  | Description |  |  |
| `HierarchyNodeShortText` |  |  |  |  |  | `String(20)` |  |  |  |  |
| `ValidityStartDate` |  |  |  |  |  | `Date` |  | Validity Start Date |  |  |


## Entity: `ProfitCenterHierarchyText`

- **ABAP CDS Name:** `I_ProfitCenterHierarchyText`
- **Label:** Profit Center Hierarchy - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** SETHEADERT

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `ControllingArea` |  |  |  |  |  | `String(12)` | Y | Hierarchy Class |  |  |
| `ProfitCenterHierarchy` |  |  |  |  |  | `String(40)` | Y | Profit Center Hierarchy |  |  |
| `ValidityEndDate` |  |  |  |  |  | `Date` | Y | Valid To |  |  |
| `Language` |  |  |  |  |  | `String(2)` | Y | Language Key |  |  |
| `ValidityStartDate` |  |  |  |  |  | `Date` |  | Valid From |  |  |
| `ProfitCenterHierarchyName` |  |  |  |  |  | `String(50)` |  | Description |  |  |


## Entity: `ProfitCenterText`

- **ABAP CDS Name:** `I_ProfitCenterText`
- **Label:** Profit Center - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** CEPCT

| CDS Field | ABAP Data Element | ECC Table | ECC Field | S/4 Table | S/4 Field | CDS Type | Key | Label | Curr/UOM | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|---|---|
| `Language` |  |  |  |  |  | `String(2)` | Y | Language Key |  |  |
| `ControllingArea` |  |  |  |  |  | `String(4)` | Y | Controlling Area |  |  |
| `ProfitCenter` |  |  |  |  |  | `String(10)` | Y | Profit Center |  |  |
| `ValidityEndDate` |  |  |  |  |  | `Date` | Y | Valid To |  |  |
| `ValidityStartDate` |  |  |  |  |  | `Date` |  | Valid From |  |  |
| `ProfitCenterName` |  |  |  |  |  | `String(20)` |  | Profit Center Name |  |  |
| `ProfitCenterLongName` |  |  |  |  |  | `String(40)` |  | Profit Center Description |  |  |
