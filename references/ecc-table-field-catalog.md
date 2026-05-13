# ECC Table Field Catalog — FP&A Domain

Full field reference for the core ECC tables used in FP&A modeling.
Fields marked `[KEY]` are part of the primary key. Fields marked `[FP&A]` are the minimum set for a finance domain model.

---

## BKPF — Accounting Document Header

Table key: `MANDT + BUKRS + GJAHR + BELNR`

| Field | Type | Len | Business Name | FP&A | Notes |
|---|---|---|---|---|---|
| `MANDT` | CLNT | 3 | Client | — | [KEY] Filter only, never store |
| `BUKRS` | CHAR | 4 | Company Code | [FP&A] | [KEY] FK → T001 |
| `GJAHR` | NUMC | 4 | Fiscal Year | [FP&A] | [KEY] |
| `BELNR` | CHAR | 10 | Accounting Document Number | [FP&A] | [KEY] |
| `BLART` | CHAR | 2 | Document Type | [FP&A] | SA, KR, DR, RE, etc. → see document-type-reference.md |
| `BLDAT` | DATS | 8 | Document Date | [FP&A] | Invoice/original document date |
| `BUDAT` | DATS | 8 | Posting Date | [FP&A] | Used for period assignment and master data joins |
| `MONAT` | NUMC | 2 | Fiscal Period | [FP&A] | 01–12 normal, 13–16 special |
| `WAERS` | CUKY | 5 | Currency Key | [FP&A] | Transaction currency for WRBTR amounts |
| `KURSF` | DEC | 9 | Exchange Rate | | Rate used for currency translation |
| `BKTXT` | CHAR | 25 | Document Header Text | | Descriptive text |
| `XBLNR` | CHAR | 16 | Reference Document Number | [FP&A] | External document reference (invoice#, etc.) |
| `AWTYP` | CHAR | 5 | Reference Transaction | | Origin object type (VBRK=billing, MKPF=GR, etc.) |
| `AWKEY` | CHAR | 20 | Reference Key | | Object key for AWTYP |
| `TCODE` | CHAR | 20 | Transaction Code | | FB01, VF01, MIRO, etc. |
| `USNAM` | CHAR | 12 | User Name | | Who posted |
| `CPUDT` | DATS | 8 | Entry Date | | When it was entered in system |
| `CPUTM` | TIMS | 6 | Entry Time | | |
| `STBLG` | CHAR | 10 | Reversal Document Number | | Populated if this doc was reversed |
| `STJAH` | NUMC | 4 | Reversal Fiscal Year | | |
| `STGRD` | CHAR | 2 | Reason for Reversal | | |
| `XREVERSAL` | CHAR | 1 | Is Reversal Document | | 'X' if this IS the reversal |
| `BVORG` | CHAR | 16 | Cross-Company Code Number | | For intercompany postings |
| `GLVOR` | CHAR | 4 | Business Transaction | | Functional classification |
| `NUMPG` | NUMC | 3 | Number of Pages | | |
| `BRNCH` | CHAR | 4 | Branch | | |
| `BUKRS_AUT` | CHAR | 4 | Authorizing Company Code | | |
| `DBBLG` | CHAR | 10 | Recurring Entry Doc | | |
| `WWERT` | DATS | 8 | Translation Date | | For currency conversion |
| `VATDATE` | DATS | 8 | VAT Date | | Tax reporting date |

---

## BSEG — Accounting Document Line Item

Table key: `MANDT + BUKRS + GJAHR + BELNR + BUZEI`

> **Performance note**: BSEG is a cluster table in ECC — very wide, slow on full scans. Always filter by BUKRS+GJAHR+BELNR. Use `BSIS` (open items) or `BSAS` (cleared items) for GL-only reporting at scale.

| Field | Type | Len | Business Name | FP&A | Notes |
|---|---|---|---|---|---|
| `MANDT` | CLNT | 3 | Client | — | [KEY] |
| `BUKRS` | CHAR | 4 | Company Code | [FP&A] | [KEY] |
| `GJAHR` | NUMC | 4 | Fiscal Year | [FP&A] | [KEY] |
| `BELNR` | CHAR | 10 | Accounting Document | [FP&A] | [KEY] |
| `BUZEI` | NUMC | 3 | Line Item Number | [FP&A] | [KEY] |
| `KOART` | CHAR | 1 | Account Type | [FP&A] | S=GL, D=customer, K=vendor, A=asset, M=material |
| `HKONT` | CHAR | 10 | GL Account | [FP&A] | FK → SKA1 (always populated for S-type) |
| `SHKZG` | CHAR | 1 | Debit/Credit Indicator | [FP&A] | S=Soll(debit), H=Haben(credit) |
| `DMBTR` | CURR | 13 | Amount in Company Code Currency | [FP&A] | Always in BKPF.WAERS... actually local currency |
| `DMBE2` | CURR | 13 | Amount in Second Local Currency | | Parallel valuation |
| `DMBE3` | CURR | 13 | Amount in Third Local Currency | | Parallel valuation |
| `WRBTR` | CURR | 13 | Amount in Transaction Currency | [FP&A] | In BKPF.WAERS |
| `TXBHW` | CURR | 13 | Tax Base Amount (CC currency) | | |
| `TXBFW` | CURR | 13 | Tax Base Amount (txn currency) | | |
| `MWSTS` | CURR | 13 | Tax Amount (CC currency) | | |
| `MWSKZ` | CHAR | 2 | Tax Code | | FK → T007A |
| `KOSTL` | CHAR | 10 | Cost Center | [FP&A] | FK → CSKS (time-dependent) |
| `PRCTR` | CHAR | 18 | Profit Center | [FP&A] | FK → CEPC (time-dependent) |
| `FKBER` | CHAR | 16 | Functional Area | [FP&A] | Cost-of-sales dimension |
| `KOKRS` | CHAR | 4 | Controlling Area | [FP&A] | FK → TKA01 |
| `GSBER` | CHAR | 4 | Business Area | | Sub-entity for internal reporting |
| `SEGMENT` | CHAR | 10 | Segment | | IFRS 8 segment |
| `AUFNR` | CHAR | 12 | Internal Order | | FK → AUFK |
| `PS_PSP_PNR` | NUMC | 8 | WBS Element (internal) | | Use POSID from PRPS for display |
| `NPLNR` | CHAR | 12 | Network | | Project networks |
| `KSTAR` | CHAR | 10 | Cost Element | | CO cost element (≈ GL account in CO) |
| `LIFNR` | CHAR | 10 | Vendor | [FP&A] | FK → LFA1 (KOART=K) |
| `KUNNR` | CHAR | 10 | Customer | [FP&A] | FK → KNA1 (KOART=D) |
| `ANLN1` | CHAR | 12 | Main Asset Number | | FK → ANLA (KOART=A) |
| `ANLN2` | CHAR | 4 | Asset Sub-number | | |
| `MATNR` | CHAR | 18 | Material Number | | FK → MARA |
| `WERKS` | CHAR | 4 | Plant | | FK → T001W |
| `MENGE` | QUAN | 13 | Quantity | | With MEINS unit |
| `MEINS` | UNIT | 3 | Base Unit of Measure | | |
| `VBELN` | CHAR | 10 | SD Document (billing/delivery) | [FP&A] | Links to VBRK or LIKP |
| `VBPOS` | NUMC | 6 | SD Document Item | | |
| `AUBEL` | CHAR | 10 | Sales Order | | Links to VBAK |
| `AUPOS` | NUMC | 6 | Sales Order Item | | |
| `EBELN` | CHAR | 10 | Purchase Order | [FP&A] | FK → EKKO |
| `EBELP` | NUMC | 5 | PO Line Item | [FP&A] | FK → EKPO |
| `ANBWA` | CHAR | 3 | Asset Transaction Type | | For FI-AA postings |
| `ZUONR` | CHAR | 18 | Assignment Field | | Free-text reference, often doc number |
| `SGTXT` | CHAR | 50 | Item Text | | Line-level description |
| `BEWAR` | CHAR | 3 | Transaction Type | | For consolidation/intercompany |
| `UMSKZ` | CHAR | 1 | Special GL Indicator | | A=down payment, W=bill of exchange, etc. |
| `ZTERM` | CHAR | 4 | Payment Terms | | |
| `ZBD1T` | DEC | 3 | Cash Discount Days 1 | | |
| `ZBD1P` | DEC | 5 | Cash Discount Percentage 1 | | |
| `ZLSCH` | CHAR | 1 | Payment Method | | |
| `BVTYP` | CHAR | 4 | Partner Bank Type | | |
| `REBZG` | CHAR | 10 | Invoice Reference | | For clearing: original invoice number |
| `REBZJ` | NUMC | 4 | Invoice Reference Fiscal Year | | |
| `REBZT` | CHAR | 1 | Follow-On Document Type | | |

---

## CSKS — Cost Center Master Data

Table key: `MANDT + KOKRS + KOSTL + DATBI`

> Time-dependent: one row per validity period. Always join on `DATAB <= posting_date <= DATBI`.

| Field | Type | Len | Business Name | FP&A | Notes |
|---|---|---|---|---|---|
| `MANDT` | CLNT | 3 | Client | — | [KEY] |
| `KOKRS` | CHAR | 4 | Controlling Area | [FP&A] | [KEY] FK → TKA01 |
| `KOSTL` | CHAR | 10 | Cost Center | [FP&A] | [KEY] |
| `DATBI` | DATS | 8 | Valid To Date | [FP&A] | [KEY] End of validity period |
| `DATAB` | DATS | 8 | Valid From Date | [FP&A] | Start of validity period |
| `BUKRS` | CHAR | 4 | Company Code | [FP&A] | FK → T001 |
| `GSBER` | CHAR | 4 | Business Area | | |
| `PRCTR` | CHAR | 18 | Default Profit Center | [FP&A] | Default only — not authoritative for GL postings |
| `KHINR` | CHAR | 12 | Standard Hierarchy Area | [FP&A] | Links to SETHEADER.SETNAME |
| `KOSAR` | CHAR | 1 | Cost Center Category | [FP&A] | E=expense, L=leistungsstelle, F=Fertigung, I=invest |
| `VERAK` | CHAR | 20 | Person Responsible | | |
| `ABTEI` | CHAR | 12 | Department | [FP&A] | Org attribute |
| `FUNC_AREA` | CHAR | 16 | Functional Area | | Default FA for postings to this CC |
| `WERKS` | CHAR | 4 | Plant | | |
| `LSTAR` | CHAR | 6 | Activity Type | | Default activity type |
| `LAND1` | CHAR | 3 | Country | | |
| `WAERS` | CUKY | 5 | Currency | | CC object currency |

> Texts in `CSKT` (key: SPRAS+KOKRS+KOSTL+DATBI): fields `MCTXT` (short name), `KTEXT` (long name).

---

## CEPC — Profit Center Master Data

Table key: `MANDT + KOKRS + PRCTR + DATBI`

> Time-dependent: same join rule as CSKS.

| Field | Type | Len | Business Name | FP&A | Notes |
|---|---|---|---|---|---|
| `MANDT` | CLNT | 3 | Client | — | [KEY] |
| `KOKRS` | CHAR | 4 | Controlling Area | [FP&A] | [KEY] |
| `PRCTR` | CHAR | 18 | Profit Center | [FP&A] | [KEY] |
| `DATBI` | DATS | 8 | Valid To Date | [FP&A] | [KEY] |
| `DATAB` | DATS | 8 | Valid From Date | [FP&A] | |
| `BUKRS` | CHAR | 4 | Company Code | [FP&A] | |
| `GSBER` | CHAR | 4 | Business Area | | |
| `SEGMENT` | CHAR | 10 | Segment | [FP&A] | IFRS 8 segment reporting |
| `FUNC_AREA` | CHAR | 16 | Functional Area | | Default FA |
| `PCTBK` | CHAR | 1 | Profit Center Type | | 0=normal, 1=dummy |
| `VERAK` | CHAR | 20 | Person Responsible | | |
| `ABTEI` | CHAR | 12 | Department | [FP&A] | |
| `KHINR` | CHAR | 12 | Standard Hierarchy Area | [FP&A] | Links to PC hierarchy in SETHEADER (SETCLASS='0106') |
| `WAERS` | CUKY | 5 | PC Object Currency | | |
| `LAND1` | CHAR | 3 | Country | | |

> Texts in `CEPCT` (key: SPRAS+KOKRS+PRCTR+DATBI): `MCTXT` (short), `KTEXT` (long).

---

## SKA1 — GL Account Master (Chart of Accounts Level)

Table key: `MANDT + KTOPL + SAKNR`

| Field | Type | Len | Business Name | FP&A | Notes |
|---|---|---|---|---|---|
| `MANDT` | CLNT | 3 | Client | — | [KEY] |
| `KTOPL` | CHAR | 4 | Chart of Accounts | [FP&A] | [KEY] FK → T004 |
| `SAKNR` | CHAR | 10 | GL Account Number | [FP&A] | [KEY] |
| `BILKT` | CHAR | 10 | Alternative Account Number | | Group chart of accounts reference |
| `KTOKS` | CHAR | 4 | Account Group | [FP&A] | Controls field selection; groups P&L vs BS |
| `XBILK` | CHAR | 1 | Balance Sheet Account | [FP&A] | 'X'=balance sheet, ' '=P&L |
| `GVTYP` | CHAR | 2 | P&L Statement Account Type | [FP&A] | See gl-account-type-classification.md |
| `XLOEV` | CHAR | 1 | Deletion Flag | | Exclude if 'X' |
| `XSPEA` | CHAR | 1 | Blocked for Posting | | Exclude if 'X' |
| `XSPEB` | CHAR | 1 | Blocked for Planning | | |
| `MUSTR` | CHAR | 2 | Sample Account | | |
| `FUNC_AREA` | CHAR | 16 | Functional Area | | |

> Account texts in `SKAT` (key: SPRAS+KTOPL+SAKNR): `TXT20` (short), `TXT50` (long).

---

## SKB1 — GL Account Master (Company Code Level)

Table key: `MANDT + BUKRS + SAKNR`

| Field | Type | Len | Business Name | FP&A | Notes |
|---|---|---|---|---|---|
| `MANDT` | CLNT | 3 | Client | — | [KEY] |
| `BUKRS` | CHAR | 4 | Company Code | [FP&A] | [KEY] |
| `SAKNR` | CHAR | 10 | GL Account Number | [FP&A] | [KEY] |
| `WAERS` | CUKY | 5 | Account Currency | | If set, postings must use this currency |
| `XSALH` | CHAR | 1 | Only Balances in Local Currency | | |
| `MWSKZ` | CHAR | 2 | Tax Category | | |
| `XMWNO` | CHAR | 1 | Posting Without Tax Allowed | | |
| `FSTAG` | CHAR | 2 | Field Status Group | | Controls required/optional fields |
| `MITKZ` | CHAR | 2 | Reconciliation Account For | | D=customer, K=vendor, A=asset |
| `XOPVW` | CHAR | 1 | Open Item Management | | 'X'=managed as open items |
| `XKRES` | CHAR | 1 | Line Item Display | | 'X'=line items stored |
| `HBKID` | CHAR | 5 | House Bank | | For bank accounts |
| `HKTID` | CHAR | 5 | Account ID | | For bank accounts |
| `XLOEV` | CHAR | 1 | Deletion Flag (CC level) | | |
| `ZUAWA` | CHAR | 3 | Sort Key | | Determines BSEG.ZUONR content |

---

## EKKO — Purchase Order Header

Table key: `MANDT + EBELN`

| Field | Type | Len | Business Name | FP&A | Notes |
|---|---|---|---|---|---|
| `MANDT` | CLNT | 3 | Client | — | [KEY] |
| `EBELN` | CHAR | 10 | Purchase Order Number | [FP&A] | [KEY] |
| `BUKRS` | CHAR | 4 | Company Code | [FP&A] | |
| `BSTYP` | CHAR | 1 | PO Category | | F=standard PO, K=contract, L=scheduling agr |
| `BSART` | CHAR | 4 | Order Type | [FP&A] | NB=standard, FO=framework order |
| `EKGRP` | CHAR | 3 | Purchasing Group | | |
| `EKORG` | CHAR | 4 | Purchasing Organization | | |
| `LIFNR` | CHAR | 10 | Vendor | [FP&A] | FK → LFA1 |
| `ZTERM` | CHAR | 4 | Payment Terms | | |
| `WAERS` | CUKY | 5 | Currency | [FP&A] | PO currency |
| `WKURS` | DEC | 9 | Exchange Rate | | |
| `BEDAT` | DATS | 8 | PO Date | [FP&A] | |
| `KDATB` | DATS | 8 | Start of Validity Period | | For outline agreements |
| `KDATE` | DATS | 8 | End of Validity Period | | |
| `KNUMV` | CHAR | 10 | Conditions (Pricing) Doc | | Links to KONV |
| `INCO1` | CHAR | 3 | Incoterms | | |
| `INCO2` | CHAR | 28 | Incoterms Location | | |
| `LOEKZ` | CHAR | 1 | Deletion Indicator | | Exclude if set |

---

## EKPO — Purchase Order Item

Table key: `MANDT + EBELN + EBELP`

| Field | Type | Len | Business Name | FP&A | Notes |
|---|---|---|---|---|---|
| `MANDT` | CLNT | 3 | Client | — | [KEY] |
| `EBELN` | CHAR | 10 | Purchase Order Number | [FP&A] | [KEY] |
| `EBELP` | NUMC | 5 | PO Item | [FP&A] | [KEY] |
| `MATNR` | CHAR | 18 | Material | | FK → MARA (blank for service items) |
| `TXZ01` | CHAR | 40 | Short Text | | Item description |
| `WERKS` | CHAR | 4 | Plant | [FP&A] | |
| `LGORT` | CHAR | 4 | Storage Location | | |
| `MATKL` | CHAR | 9 | Material Group | | |
| `MENGE` | QUAN | 13 | PO Quantity | | |
| `MEINS` | UNIT | 3 | Unit of Measure | | |
| `NETPR` | CURR | 11 | Net Price | [FP&A] | Per price unit |
| `PEINH` | DEC | 5 | Price Unit | | |
| `NETWR` | CURR | 13 | Net Order Value | [FP&A] | In PO currency |
| `BRTWR` | CURR | 13 | Gross Order Value | | |
| `WAERS` | CUKY | 5 | Currency | | |
| `KNTTP` | CHAR | 1 | Account Assignment Category | [FP&A] | K=cost center, P=project, A=asset, blank=stock |
| `PSTYP` | CHAR | 1 | Item Category | | 0=standard, 2=consignment, 9=service |
| `ELIKZ` | CHAR | 1 | Delivery Completed Indicator | | |
| `EINDT` | DATS | 8 | Delivery Date | | |
| `LOEKZ` | CHAR | 1 | Deletion Indicator | | |
| `SAKTO` | CHAR | 10 | GL Account | [FP&A] | Account assignment (for non-stock) |
| `KOSTL` | CHAR | 10 | Cost Center | [FP&A] | When KNTTP=K (see EKKN for multi-acct) |
| `PRCTR` | CHAR | 18 | Profit Center | [FP&A] | |

---

## EKKN — Purchase Order Account Assignment

Table key: `MANDT + EBELN + EBELP + ZEKKN`

> Use when a PO item has multiple account assignments (cost center split). One row per assignment.

| Field | Type | Len | Business Name | FP&A | Notes |
|---|---|---|---|---|---|
| `MANDT` | CLNT | 3 | Client | — | [KEY] |
| `EBELN` | CHAR | 10 | PO Number | [FP&A] | [KEY] |
| `EBELP` | NUMC | 5 | PO Item | [FP&A] | [KEY] |
| `ZEKKN` | NUMC | 2 | Sequential Number | [FP&A] | [KEY] |
| `KOSTL` | CHAR | 10 | Cost Center | [FP&A] | |
| `SAKTO` | CHAR | 10 | GL Account | [FP&A] | |
| `PRCTR` | CHAR | 18 | Profit Center | [FP&A] | |
| `FKBER` | CHAR | 16 | Functional Area | | |
| `KOKRS` | CHAR | 4 | Controlling Area | | |
| `AUFNR` | CHAR | 12 | Internal Order | | |
| `PS_PSP_PNR` | NUMC | 8 | WBS Element | | |
| `NPLNR` | CHAR | 12 | Network | | |
| `VBELN` | CHAR | 10 | Sales Order | | |
| `VBELP` | NUMC | 6 | Sales Order Item | | |
| `MENGE` | QUAN | 13 | Quantity | | Partial quantity for this assignment |
| `MEINS` | UNIT | 3 | Unit of Measure | | |

---

## SET Hierarchy Tables — CO Hierarchy Framework

### SETHEADER — Hierarchy Root

Table key: `MANDT + SETCLASS + SUBCLASS + SETNAME`

| Field | Business Name | Notes |
|---|---|---|
| `SETCLASS` | Set Class | `0101`=cost center, `0106`=profit center, `0102`=cost element |
| `SUBCLASS` | Sub-class | Controlling Area code |
| `SETNAME` | Set Name | Hierarchy name (= CSKS.KHINR for standard CC hierarchy) |
| `RCOMP` | Comparative Set | |
| `DESCRIPT` | Description | |

### SETNODE — Internal (Group) Nodes

Table key: `MANDT + SETCLASS + SUBCLASS + SETNAME + SUBSETNAME`

| Field | Business Name | Notes |
|---|---|---|
| `SETNAME` | Parent Set Name | Parent node |
| `SUBSETNAME` | Child Set Name | Child node → recurse to SETHEADER |
| `SEQNR` | Sequence Number | Display order |

### SETLEAF — Leaf Values (Actual CC/PC Assignments)

Table key: `MANDT + SETCLASS + SUBCLASS + SETNAME + VFROM + VTO` (simplified)

| Field | Business Name | Notes |
|---|---|---|
| `SETNAME` | Set Name | Which node contains this leaf |
| `FROM_VALUE` | From Value | Cost center / PC range start |
| `TO_VALUE` | To Value | Range end (often = FROM_VALUE for single values) |

> **Flattening pattern**: See SKILL.md → "ECC Hierarchy Model (SET Framework)" for the recursive CTE.

---

## VBRK — Billing Document Header

Table key: `MANDT + VBELN`

| Field | Type | Len | Business Name | FP&A | Notes |
|---|---|---|---|---|---|
| `MANDT` | CLNT | 3 | Client | — | [KEY] |
| `VBELN` | CHAR | 10 | Billing Document | [FP&A] | [KEY] |
| `FKART` | CHAR | 4 | Billing Type | [FP&A] | F2=invoice, G2=credit memo, L2=debit memo |
| `FKTYP` | CHAR | 1 | Billing Category | | F=invoice, S=cancellation |
| `VBTYPL` | CHAR | 4 | SD Document Category | | |
| `FKDAT` | DATS | 8 | Billing Date | [FP&A] | Used for period assignment |
| `ERDAT` | DATS | 8 | Created On | | |
| `VKORG` | CHAR | 4 | Sales Organization | [FP&A] | FK → TVKO |
| `VTWEG` | CHAR | 2 | Distribution Channel | [FP&A] | |
| `SPART` | CHAR | 2 | Division | | |
| `BUKRS` | CHAR | 4 | Company Code | [FP&A] | FK → T001 |
| `GJAHR` | NUMC | 4 | Fiscal Year | [FP&A] | |
| `BELNR` | CHAR | 10 | Accounting Document | [FP&A] | FK → BKPF — link to GL posting |
| `NETWR` | CURR | 15 | Net Value | [FP&A] | Header total in WAERK |
| `MWSBP` | CURR | 15 | Tax Amount | | |
| `WAERK` | CUKY | 5 | Document Currency | [FP&A] | Transaction currency |
| `KUNAG` | CHAR | 10 | Sold-to Party | [FP&A] | FK → KNA1 |
| `KUNRG` | CHAR | 10 | Payer | [FP&A] | Who pays the invoice; FK → KNA1 |
| `KUNWE` | CHAR | 10 | Ship-to Party | | |
| `KUNRE` | CHAR | 10 | Bill-to Party | | |
| `RFBSK` | CHAR | 1 | Accounting Transfer Status | [FP&A] | C=fully posted to FI; filter on this |
| `FKSTO` | CHAR | 1 | Cancelled | [FP&A] | 'X' = cancelled; exclude from revenue |
| `SFAKN` | CHAR | 10 | Cancelled Billing Doc | | Points to original doc being cancelled |
| `XBLNR` | CHAR | 16 | Reference | | External reference number |
| `GBSTK` | CHAR | 1 | Overall Status | | |
| `KUNNR` | CHAR | 10 | Sold-to (redundant) | | Same as KUNAG in most cases |

> **GL Linkage**: `BKPF.AWTYP = 'VBRK'` and `BKPF.AWKEY = VBELN + GJAHR` traces a GL document to its billing origin. The `BELNR` field on VBRK is the direct accounting document link.

---

## VBRP — Billing Document Item

Table key: `MANDT + VBELN + POSNR`

| Field | Type | Len | Business Name | FP&A | Notes |
|---|---|---|---|---|---|
| `MANDT` | CLNT | 3 | Client | — | [KEY] |
| `VBELN` | CHAR | 10 | Billing Document | [FP&A] | [KEY] FK → VBRK |
| `POSNR` | NUMC | 6 | Item | [FP&A] | [KEY] |
| `MATNR` | CHAR | 18 | Material | [FP&A] | FK → MARA |
| `WERKS` | CHAR | 4 | Plant | [FP&A] | |
| `ARKTX` | CHAR | 40 | Item Description | | |
| `FKIMG` | QUAN | 13 | Invoiced Quantity | [FP&A] | |
| `VRKME` | UNIT | 3 | Sales Unit | [FP&A] | |
| `NETWR` | CURR | 15 | Net Value | [FP&A] | In WAERK |
| `WAVWR` | CURR | 15 | Cost | [FP&A] | Standard cost — for margin calculation |
| `MWSBP` | CURR | 15 | Tax Amount | | |
| `AUBEL` | CHAR | 10 | Sales Document | [FP&A] | FK → VBAK — originating sales order |
| `AUPOS` | NUMC | 6 | Sales Document Item | [FP&A] | FK → VBAP |
| `PRCTR` | CHAR | 18 | Profit Center | [FP&A] | |
| `KOSTL` | CHAR | 10 | Cost Center | | |
| `KOKRS` | CHAR | 4 | Controlling Area | | |
| `GSBER` | CHAR | 4 | Business Area | | |
| `PS_PSP_PNR` | NUMC | 8 | WBS Element | | |
| `FKART` | CHAR | 4 | Billing Type | | Repeated from header |
| `SPART` | CHAR | 2 | Division | | |
| `KZWI1`–`KZWI6` | CURR | 15 | Pricing Subtotals | | Intermediate pricing conditions |

---

## VBAK — Sales Order Header

Table key: `MANDT + VBELN`

| Field | Type | Len | Business Name | FP&A | Notes |
|---|---|---|---|---|---|
| `MANDT` | CLNT | 3 | Client | — | [KEY] |
| `VBELN` | CHAR | 10 | Sales Document | [FP&A] | [KEY] |
| `AUART` | CHAR | 4 | Sales Order Type | [FP&A] | OR=standard, RE=return, KR=credit order |
| `AUDAT` | DATS | 8 | Document Date | [FP&A] | |
| `VKORG` | CHAR | 4 | Sales Organization | [FP&A] | |
| `VTWEG` | CHAR | 2 | Distribution Channel | [FP&A] | |
| `SPART` | CHAR | 2 | Division | | |
| `KUNNR` | CHAR | 10 | Sold-to Party | [FP&A] | FK → KNA1 |
| `WAERK` | CUKY | 5 | Document Currency | [FP&A] | |
| `NETWR` | CURR | 15 | Net Value | [FP&A] | Header total |
| `BSTNK` | CHAR | 35 | Customer Reference | | Customer PO number |
| `ERDAT` | DATS | 8 | Created On | | |
| `GBSTK` | CHAR | 1 | Overall Status | | A=open, B=partial, C=complete |
| `LFSTK` | CHAR | 1 | Delivery Status | | |
| `FKSTK` | CHAR | 1 | Billing Status | | |
| `ABSTK` | CHAR | 1 | Rejection Status | | |
| `LIFSK` | CHAR | 2 | Delivery Block | | |
| `FAKSK` | CHAR | 2 | Billing Block | | |

> Complement with `VBKD` (key: MANDT+VBELN+POSNR) for payment terms (DZTERM), incoterms (INCO1, INCO2), and fixed value dates.

---

## VBAP — Sales Order Item

Table key: `MANDT + VBELN + POSNR`

| Field | Type | Len | Business Name | FP&A | Notes |
|---|---|---|---|---|---|
| `MANDT` | CLNT | 3 | Client | — | [KEY] |
| `VBELN` | CHAR | 10 | Sales Document | [FP&A] | [KEY] |
| `POSNR` | NUMC | 6 | Item | [FP&A] | [KEY] |
| `PSTYV` | CHAR | 4 | Item Category | [FP&A] | TAN=standard, TANN=free, TAD=service |
| `MATNR` | CHAR | 18 | Material | [FP&A] | FK → MARA |
| `ARKTX` | CHAR | 40 | Item Description | | |
| `WERKS` | CHAR | 4 | Plant | [FP&A] | |
| `LGORT` | CHAR | 4 | Storage Location | | |
| `KWMENG` | QUAN | 15 | Order Quantity | [FP&A] | In VRKME |
| `VRKME` | UNIT | 3 | Sales Unit | [FP&A] | |
| `NETPR` | CURR | 11 | Net Price | [FP&A] | Per KPEIN price unit |
| `KPEIN` | DEC | 5 | Price Unit | | |
| `NETWR` | CURR | 15 | Net Value | [FP&A] | In WAERK |
| `WAVWR` | CURR | 15 | Cost | [FP&A] | Standard cost; margin = NETWR - WAVWR |
| `PRCTR` | CHAR | 18 | Profit Center | [FP&A] | FK → CEPC |
| `GSBER` | CHAR | 4 | Business Area | | |
| `KOKRS` | CHAR | 4 | Controlling Area | | |
| `PS_PSP_PNR` | NUMC | 8 | WBS Element | | |
| `ABGRU` | CHAR | 2 | Rejection Reason | [FP&A] | Non-blank = item rejected — exclude from open orders |
| `FKSTA` | CHAR | 1 | Item Billing Status | | A=not billed, B=partial, C=complete |
| `LFSTA` | CHAR | 1 | Item Delivery Status | | |
| `SPART` | CHAR | 2 | Division | | |
| `MATKL` | CHAR | 9 | Material Group | | |
| `KZWI1`–`KZWI6` | CURR | 15 | Pricing Subtotals | | |

> **Open order definition**: `ABGRU = ' '` AND `FKSTA != 'C'`. For backlog value, use `NETWR` of open, undelivered items.

---

## LFA1 — Vendor Master (General)

Table key: `MANDT + LIFNR`

| Field | Type | Len | Business Name | FP&A | Notes |
|---|---|---|---|---|---|
| `MANDT` | CLNT | 3 | Client | — | [KEY] |
| `LIFNR` | CHAR | 10 | Vendor Number | [FP&A] | [KEY] |
| `NAME1` | CHAR | 35 | Vendor Name | [FP&A] | |
| `NAME2` | CHAR | 35 | Name 2 | | |
| `ORT01` | CHAR | 35 | City | | |
| `LAND1` | CHAR | 3 | Country | [FP&A] | |
| `REGIO` | CHAR | 3 | Region | | |
| `KTOKK` | CHAR | 4 | Vendor Account Group | [FP&A] | Controls field selection |
| `STCD1` | CHAR | 16 | Tax Number 1 | | |
| `STCD2` | CHAR | 11 | Tax Number 2 | | |
| `SPRAS` | LANG | 1 | Language | | |
| `ADRNR` | CHAR | 10 | Address Number | | FK → ADRC |
| `LOEVM` | CHAR | 1 | Deletion Flag | | Exclude if 'X' |

> Company code-level data (payment terms, reconciliation account) in `LFB1` (key: MANDT+LIFNR+BUKRS). Purchasing org data in `LFM1` (key: MANDT+LIFNR+EKORG).

---

## KNA1 — Customer Master (General)

Table key: `MANDT + KUNNR`

| Field | Type | Len | Business Name | FP&A | Notes |
|---|---|---|---|---|---|
| `MANDT` | CLNT | 3 | Client | — | [KEY] |
| `KUNNR` | CHAR | 10 | Customer Number | [FP&A] | [KEY] |
| `NAME1` | CHAR | 35 | Customer Name | [FP&A] | |
| `NAME2` | CHAR | 35 | Name 2 | | |
| `ORT01` | CHAR | 35 | City | | |
| `LAND1` | CHAR | 3 | Country | [FP&A] | |
| `REGIO` | CHAR | 3 | Region | | |
| `KTOKD` | CHAR | 4 | Customer Account Group | [FP&A] | |
| `STCD1` | CHAR | 16 | Tax Number 1 | | |
| `KUNNR_EXT` | CHAR | 18 | External Customer Number | | |
| `ADRNR` | CHAR | 10 | Address Number | | FK → ADRC |
| `LOEVM` | CHAR | 1 | Deletion Flag | | Exclude if 'X' |
| `SPERR` | CHAR | 1 | Posting Block | | |

> Company code-level data (reconciliation account, payment terms, dunning) in `KNB1` (key: MANDT+KUNNR+BUKRS). Dunning history in `KNB5`. Sales area data in `KNVV`.

---

## Supporting Reference Tables

| Table | Description | Key | Silver Use |
|---|---|---|---|
| `T001` | Company Codes | BUKRS | Enrich with country, currency, fiscal year variant |
| `T009` | Fiscal Year Variants | PERIV | Period calendar definition |
| `T009B` | Fiscal Period Dates | PERIV+BUMON+POPER | Map period number → date range |
| `TKA01` | Controlling Areas | KOKRS | CO area master: currency, chart of accounts |
| `T004` | Chart of Accounts | KTOPL | CoA description |
| `T007A` | Tax Keys | MSKWZ+KALSM | Tax code descriptions |
| `T001W` | Plants | WERKS | Plant master |
| `T024` | Purchasing Groups | EKGRP | Purchasing group description |
| `T024E` | Purchasing Organizations | EKORG | Purchasing org description |
