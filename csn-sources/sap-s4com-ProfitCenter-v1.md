# ProfitCenter

> Source file: `sap-s4com-ProfitCenter-v1.json`


## Entity: `PrftCtrCompanyCodeAssignment`

- **ABAP Name:** `I_PrftCtrCompanyCodeAssignment`
- **Label:** Company code assignment to profit center
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `ControllingArea` | `TKA01` | `KOKRS` | `String(4)` | Y | Controlling Area |  |  |  |
| `ProfitCenter` |  |  | `String(10)` | Y | Profit Center |  |  | S/4 only entity |
| `CompanyCode` | `T001` | `BUKRS` | `String(4)` | Y |  |  |  |  |
| `JointVentureObjectType` |  |  | `String(4)` |  | JV Object Type |  |  | S/4 only entity |
| `JointVentureClass` |  |  | `String(3)` |  | JIB/JIBE Class |  |  | S/4 only entity |
| `JointVentureSubClass` |  |  | `String(5)` |  | JIB/JIBE Subclass A |  |  | S/4 only entity |
| `JointVenture` |  |  | `String(6)` |  | Joint Venture |  |  | S/4 only entity |
| `JointVentureRecoveryCode` |  |  | `String(2)` |  | Recovery Indicator |  |  | S/4 only entity |
| `JointVentureEquityType` |  |  | `String(3)` |  | Equity Type |  |  | S/4 only entity |


## Entity: `ProfitCenter`

- **ABAP Name:** `I_ProfitCenter`
- **Label:** Profit Center
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `ControllingArea` | `CEPC` | `KOKRS` | `String(4)` | Y | Controlling Area |  |  |  |
| `ProfitCenter` | `CEPC` | `PRCTR` | `String(10)` | Y | Profit Center |  |  |  |
| `ValidityEndDate` | `CEPC` | `DATBI` | `Date` | Y | Valid To |  |  |  |
| `ProfitCtrResponsiblePersonName` |  |  | `String(20)` |  | Person Resp. for PC |  |  | S/4 only entity |
| `CompanyCode` | `CEPC` | `BUKRS` | `String(4)` |  | Company Code |  |  |  |
| `ProfitCtrResponsibleUser` |  |  | `String(12)` |  | User Responsible |  |  | S/4 only entity |
| `ValidityStartDate` | `CEPC` | `DATAB` | `Date` |  | Valid From |  |  |  |
| `Department` | `CEPC` | `ABTEI` | `String(12)` |  | Department |  |  |  |
| `ProfitCenterStandardHierarchy` |  |  | `String(12)` |  | Hierarchy Area |  |  | S/4 only entity |
| `Segment` | `CEPC` | `SEGMENT` | `String(10)` |  | Segment |  |  |  |
| `ProfitCenterIsBlocked` |  |  | `Boolean` |  | Lock indicator |  |  | S/4 only entity |
| `FormulaPlanningTemplate` |  |  | `String(10)` |  | Form. Planning Temp. |  |  | S/4 only entity |
| `FormOfAddress` |  |  | `String(15)` |  | Title |  |  | S/4 only entity |
| `AddressName` |  |  | `String(35)` |  | Name |  |  | S/4 only entity |
| `AdditionalName` |  |  | `String(35)` |  | Name 2 |  |  | S/4 only entity |
| `ProfitCenterAddrName3` |  |  | `String(35)` |  | Name 3 |  |  | S/4 only entity |
| `ProfitCenterAddrName4` |  |  | `String(35)` |  | Name 4 |  |  | S/4 only entity |
| `StreetAddressName` |  |  | `String(35)` |  | Street |  |  | S/4 only entity |
| `POBox` |  |  | `String(10)` |  | PO Box |  |  | S/4 only entity |
| `CityName` |  |  | `String(35)` |  | City |  |  | S/4 only entity |
| `PostalCode` |  |  | `String(10)` |  | Postal Code |  |  | S/4 only entity |
| `POBoxPostalCode` |  |  | `String(10)` |  | PO Box Postal Code |  |  | S/4 only entity |
| `District` |  |  | `String(35)` |  | District |  |  | S/4 only entity |
| `Country` | `CEPC` | `LAND1` | `String(3)` |  | Country/Region Key |  |  |  |
| `Region` |  |  | `String(3)` |  | Region |  |  | S/4 only entity |
| `TaxJurisdiction` |  |  | `String(15)` |  | Tax Jurisdiction |  |  | S/4 only entity |
| `Language` | `CEPCT` | `SPRAS` | `String(2)` |  | Language Key |  |  |  |
| `PhoneNumber1` |  |  | `String(16)` |  | Telephone 1 |  |  | S/4 only entity |
| `PhoneNumber2` |  |  | `String(16)` |  | Telephone 2 |  |  | S/4 only entity |
| `TeleboxNumber` |  |  | `String(15)` |  | Telebox Number |  |  | S/4 only entity |
| `TelexNumber` |  |  | `String(30)` |  | Telex Number |  |  | S/4 only entity |
| `FaxNumber` |  |  | `String(31)` |  | Fax Number |  |  | S/4 only entity |
| `TeletexNumber` |  |  | `String(30)` |  | Teletex Number |  |  | S/4 only entity |
| `DataCommunicationPhoneNumber` |  |  | `String(14)` |  | Data line |  |  | S/4 only entity |
| `ProfitCenterPrinterName` |  |  | `String(4)` |  | Printer name |  |  | S/4 only entity |
| `ProfitCenterCreatedByUser` |  |  | `String(12)` |  | Created By |  |  | S/4 only entity |
| `ProfitCenterCreationDate` |  |  | `Date` |  | Entered On |  |  | S/4 only entity |
| `LogicalSystem` |  |  | `String(10)` |  | Logical System |  |  | S/4 only entity |


## Entity: `ProfitCenterHierarchy`

- **ABAP Name:** `I_ProfitCenterHierarchy`
- **Label:** Profit Center Hierarchy
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `ControllingArea` | `TKA01` | `KOKRS` | `String(4)` | Y | Controlling Area |  |  |  |
| `ProfitCenterHierarchy` |  |  | `String(40)` | Y | Profit Center Hierarchy |  |  | S/4 only entity |
| `ValidityEndDate` |  |  | `Date` | Y | Validity End Date |  |  | S/4 only entity |
| `ValidityStartDate` |  |  | `Date` |  | Validity Start Date |  |  | S/4 only entity |
| `LastChangedByUser` |  |  | `String(12)` |  | Last Changed By |  |  | S/4 only entity |
| `LastChangeDateTime` |  |  | `DateTime` |  | Updated At |  |  | S/4 only entity |
| `LastChangeTime` |  |  | `DateTime` |  | Updated At |  |  | S/4 only entity |
| `HierarchyShortID` |  |  | `String(20)` |  | Hierarchy ID |  |  | S/4 only entity |


## Entity: `ProfitCenterHierarchyNode`

- **ABAP Name:** `I_ProfitCenterHierarchyNode`
- **Label:** Profit Center Hierarchy Node
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `ControllingArea` | `TKA01` | `KOKRS` | `String(4)` | Y | Controlling Area |  |  |  |
| `ProfitCenterHierarchy` |  |  | `String(40)` | Y | Profit Center Hierarchy |  | _Hierarchy | S/4 only entity |
| `HierarchyNode` |  |  | `String(50)` | Y | Node |  |  | S/4 only entity |
| `ValidityEndDate` |  |  | `Date` | Y | Validity End Date |  |  | S/4 only entity |
| `ParentNode` |  |  | `String(50)` |  | Par. Node |  |  | S/4 only entity |
| `HierarchyVersion` |  |  | `String(15)` |  | Version |  |  | S/4 only entity |
| `ValidityStartDate` |  |  | `Date` |  | Validity Start Date |  |  | S/4 only entity |
| `ProfitCenter` |  |  | `String(10)` |  | Profit Center |  | _ProfitCenter | S/4 only entity |
| `SequenceNumber` |  |  | `String(56)` |  |  |  |  | S/4 only entity |
| `HierarchyNodeSequence` |  |  | `String(6)` |  | Sequence Number |  |  | S/4 only entity |
| `HierarchyNodeLevel` |  |  | `String(6)` |  | Hierarchy Level |  |  | S/4 only entity |
| `NodeType` |  |  | `String(1)` |  | Node Type |  |  | S/4 only entity |
| `HierarchyNodeVal` |  |  | `String(40)` |  | Value |  |  | S/4 only entity |


## Entity: `ProfitCenterHierarchyNodeText`

- **ABAP Name:** `I_ProfitCenterHierarchyNodeT`
- **Label:** Profit Center Hierarchy Node - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `ControllingArea` | `TKA01` | `KOKRS` | `String(4)` | Y | Controlling Area |  |  |  |
| `ProfitCenterHierarchy` |  |  | `String(40)` | Y | Profit Center Hierarchy |  | _Hierarchy | S/4 only entity |
| `HierarchyNode` |  |  | `String(50)` | Y | Node |  |  | S/4 only entity |
| `ValidityEndDate` |  |  | `Date` | Y | Validity End Date |  |  | S/4 only entity |
| `Language` |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity |
| `HierarchyNodeText` |  |  | `String(50)` |  | Description |  |  | S/4 only entity |
| `HierarchyNodeShortText` |  |  | `String(20)` |  |  |  |  | S/4 only entity |
| `ValidityStartDate` |  |  | `Date` |  | Validity Start Date |  |  | S/4 only entity |


## Entity: `ProfitCenterHierarchyText`

- **ABAP Name:** `I_ProfitCenterHierarchyText`
- **Label:** Profit Center Hierarchy - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `ControllingArea` | `TKA01` | `KOKRS` | `String(12)` | Y | Hierarchy Class |  |  |  |
| `ProfitCenterHierarchy` |  |  | `String(40)` | Y | Profit Center Hierarchy |  |  | S/4 only entity |
| `ValidityEndDate` |  |  | `Date` | Y | Valid To |  |  | S/4 only entity |
| `Language` |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity |
| `ValidityStartDate` |  |  | `Date` |  | Valid From |  |  | S/4 only entity |
| `ProfitCenterHierarchyName` |  |  | `String(50)` |  | Description |  |  | S/4 only entity |


## Entity: `ProfitCenterText`

- **ABAP Name:** `I_ProfitCenterText`
- **Label:** Profit Center - Text
- **VDM Type:** `` | **Data Category:** ``
- **ECC Source Tables:** —

| CDS Field | ABAP Table | ABAP Field | Type | Key | Label | Currency/UOM Ref | FK Association | ECC / S4 Diff |
|---|---|---|---|---|---|---|---|---|
| `Language` |  |  | `String(2)` | Y | Language Key |  |  | S/4 only entity |
| `ControllingArea` | `TKA01` | `KOKRS` | `String(4)` | Y | Controlling Area |  |  |  |
| `ProfitCenter` |  |  | `String(10)` | Y | Profit Center |  |  | S/4 only entity |
| `ValidityEndDate` |  |  | `Date` | Y | Valid To |  |  | S/4 only entity |
| `ValidityStartDate` |  |  | `Date` |  | Valid From |  |  | S/4 only entity |
| `ProfitCenterName` |  |  | `String(20)` |  | Profit Center Name |  |  | S/4 only entity |
| `ProfitCenterLongName` |  |  | `String(40)` |  | Profit Center Description |  |  | S/4 only entity |
