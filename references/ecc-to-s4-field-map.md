# ECC → S/4HANA Field Mapping

Complete mapping from ECC ABAP technical names to S/4HANA CDS entity field names.
Use this during migration to rewire Bronze pipelines without touching Silver/Gold.

Silver column names are pre-aligned to CDS names — only the Bronze source query changes.

---

## GL Line Item — BKPF+BSEG → GeneralLedgerAccountLineItem

| Silver Column | ECC Source | ECC Table.Field | S/4 CDS Entity | S/4 CDS Field | Notes |
|---|---|---|---|---|---|
| `company_code` | BUKRS | BKPF.BUKRS | GeneralLedgerAccountLineItem | CompanyCode | |
| `fiscal_year` | GJAHR | BKPF.GJAHR | | FiscalYear | |
| `accounting_document` | BELNR | BKPF.BELNR | | AccountingDocument | |
| `line_item` | BUZEI | BSEG.BUZEI | | LedgerGLLineItem | |
| `source_ledger` | _(null in ECC)_ | — | | SourceLedger | ECC has no ledger concept; default to '0L' or null |
| `posting_date` | BUDAT | BKPF.BUDAT | | PostingDate | |
| `document_date` | BLDAT | BKPF.BLDAT | | DocumentDate | |
| `fiscal_period` | MONAT | BKPF.MONAT | | FiscalPeriod | ECC: '3'; S4: '003' — pad in Bronze |
| `fiscal_year_period` | _(derived)_ | GJAHR+LPAD(MONAT,3,'0') | | FiscalYearPeriod | Derive same way in both sources |
| `document_type` | BLART | BKPF.BLART | | AccountingDocumentType | |
| `debit_credit_code` | SHKZG | BSEG.SHKZG | | DebitCreditCode | S=debit, H=credit (same values) |
| `reference_document` | XBLNR | BKPF.XBLNR | | ReferenceDocument | |
| `transaction_code` | TCODE | BKPF.TCODE | | TransactionCode | |
| `document_text` | BKTXT | BKPF.BKTXT | | AccountingDocumentHeaderText | |
| `gl_account` | HKONT | BSEG.HKONT | | GLAccount | |
| `chart_of_accounts` | _(from T001)_ | T001.KTOPL | | ChartOfAccounts | ECC: join T001; S4: embedded |
| `controlling_area` | KOKRS | BSEG.KOKRS | | ControllingArea | |
| `cost_center` | KOSTL | BSEG.KOSTL | | CostCenter | |
| `profit_center` | PRCTR | BSEG.PRCTR | | ProfitCenter | |
| `functional_area` | FKBER | BSEG.FKBER | | FunctionalArea | |
| `business_area` | GSBER | BSEG.GSBER | | BusinessArea | |
| `segment` | SEGMENT | BSEG.SEGMENT | | Segment | |
| `internal_order` | AUFNR | BSEG.AUFNR | | OrderID | |
| `wbs_element` | PS_PSP_PNR | BSEG.PS_PSP_PNR | | WBSElement | ECC: internal number; S4: POSID-style display |
| `cost_element` | KSTAR | BSEG.KSTAR | | CostElement | |
| `supplier` | LIFNR | BSEG.LIFNR | | Supplier | |
| `customer` | KUNNR | BSEG.KUNNR | | Customer | |
| `sales_document` | VBELN/AUBEL | BSEG.VBELN or AUBEL | | SalesDocument | |
| `sales_document_item` | VBPOS/AUPOS | BSEG.VBPOS | | SalesDocumentItem | |
| `purchasing_document` | EBELN | BSEG.EBELN | | PurchasingDocument | |
| `purchasing_doc_item` | EBELP | BSEG.EBELP | | PurchasingDocumentItem | |
| `asset_number` | ANLN1 | BSEG.ANLN1 | | MasterFixedAsset | |
| `asset_subnumber` | ANLN2 | BSEG.ANLN2 | | FixedAsset | |
| `special_gl_indicator` | UMSKZ | BSEG.UMSKZ | | SpecialGeneralLedgerCode | |
| `tax_code` | MWSKZ | BSEG.MWSKZ | | TaxCode | |
| `assignment` | ZUONR | BSEG.ZUONR | | AssignmentReference | |
| `item_text` | SGTXT | BSEG.SGTXT | | DocumentItemText | |
| `amount_txn_currency` | WRBTR | BSEG.WRBTR | | AmountInTransactionCurrency | |
| `transaction_currency` | WAERS | BKPF.WAERS | | TransactionCurrency | |
| `amount_cc_currency` | DMBTR | BSEG.DMBTR | | AmountInCompanyCodeCurrency | |
| `company_code_currency` | _(from T001)_ | T001.WAERS | | CompanyCodeCurrency | ECC: join T001; S4: embedded |
| `amount_global` | _(FX-derived)_ | Not in BSEG | | AmountInGlobalCurrency | **Gap**: ECC requires separate FX step |
| `global_currency` | _(config)_ | Not in BSEG | | GlobalCurrency | |
| `amount_functional` | _(not standard)_ | — | | AmountInFunctionalCurrency | S4 only |
| `reversal_document` | STBLG | BKPF.STBLG | | ReversalDocument | |
| `reversal_fiscal_year` | STJAH | BKPF.STJAH | | ReversalFiscalYear | |

### ECC Bronze Query Pattern (GL)

```sql
-- Bronze: ECC GL line item (join BKPF + BSEG)
SELECT
  'ECC'               AS _source_system,
  :client             AS _sap_client,
  current_timestamp() AS _extracted_at,
  h.BUKRS             AS company_code,
  h.GJAHR             AS fiscal_year,
  h.BELNR             AS accounting_document,
  l.BUZEI             AS line_item,
  NULL                AS source_ledger,       -- not in ECC
  h.BUDAT             AS posting_date,
  h.BLDAT             AS document_date,
  h.MONAT             AS fiscal_period,
  CONCAT(h.GJAHR, LPAD(h.MONAT, 3, '0'))  AS fiscal_year_period,
  h.BLART             AS document_type,
  l.SHKZG             AS debit_credit_code,
  h.XBLNR             AS reference_document,
  l.HKONT             AS gl_account,
  t.KTOPL             AS chart_of_accounts,
  l.KOKRS             AS controlling_area,
  l.KOSTL             AS cost_center,
  l.PRCTR             AS profit_center,
  l.FKBER             AS functional_area,
  l.GSBER             AS business_area,
  l.AUFNR             AS internal_order,
  l.PS_PSP_PNR        AS wbs_element,
  l.LIFNR             AS supplier,
  l.KUNNR             AS customer,
  l.EBELN             AS purchasing_document,
  l.EBELP             AS purchasing_doc_item,
  l.WRBTR             AS amount_txn_currency,
  h.WAERS             AS transaction_currency,
  l.DMBTR             AS amount_cc_currency,
  t.WAERS             AS company_code_currency,
  NULL                AS amount_global,        -- populated via FX join if needed
  NULL                AS global_currency,
  l.ZUONR             AS assignment,
  l.SGTXT             AS item_text
FROM BKPF h
JOIN BSEG l
  ON l.MANDT = h.MANDT
  AND l.BUKRS = h.BUKRS
  AND l.GJAHR = h.GJAHR
  AND l.BELNR = h.BELNR
JOIN T001 t
  ON t.MANDT = h.MANDT
  AND t.BUKRS = h.BUKRS
WHERE h.MANDT = :client
  AND l.KOART = 'S'   -- GL account line items only
```

### S/4 Bronze Query Pattern (GL)

```sql
-- Bronze: S/4 GL line item (single CDS entity)
SELECT
  'S4'                                  AS _source_system,
  :client                               AS _sap_client,
  current_timestamp()                   AS _extracted_at,
  CompanyCode                           AS company_code,
  FiscalYear                            AS fiscal_year,
  AccountingDocument                    AS accounting_document,
  LedgerGLLineItem                      AS line_item,
  SourceLedger                          AS source_ledger,
  PostingDate                           AS posting_date,
  DocumentDate                          AS document_date,
  FiscalPeriod                          AS fiscal_period,
  FiscalYearPeriod                      AS fiscal_year_period,
  AccountingDocumentType                AS document_type,
  DebitCreditCode                       AS debit_credit_code,
  ReferenceDocument                     AS reference_document,
  GLAccount                             AS gl_account,
  ChartOfAccounts                       AS chart_of_accounts,
  ControllingArea                       AS controlling_area,
  CostCenter                            AS cost_center,
  ProfitCenter                          AS profit_center,
  FunctionalArea                        AS functional_area,
  BusinessArea                          AS business_area,
  OrderID                               AS internal_order,
  WBSElement                            AS wbs_element,
  Supplier                              AS supplier,
  Customer                              AS customer,
  PurchasingDocument                    AS purchasing_document,
  PurchasingDocumentItem                AS purchasing_doc_item,
  AmountInTransactionCurrency           AS amount_txn_currency,
  TransactionCurrency                   AS transaction_currency,
  AmountInCompanyCodeCurrency           AS amount_cc_currency,
  CompanyCodeCurrency                   AS company_code_currency,
  AmountInGlobalCurrency                AS amount_global,
  GlobalCurrency                        AS global_currency,
  AssignmentReference                   AS assignment,
  DocumentItemText                      AS item_text
FROM GeneralLedgerAccountLineItem
WHERE SourceLedger = '0L'   -- leading ledger only
```

---

## Cost Center — CSKS+CSKT → CostCenter

| Silver Column | ECC Table.Field | S/4 CDS Entity | S/4 CDS Field | Notes |
|---|---|---|---|---|
| `controlling_area` | CSKS.KOKRS | CostCenter | ControllingArea | |
| `cost_center` | CSKS.KOSTL | | CostCenter | |
| `validity_start_date` | CSKS.DATAB | | ValidityStartDate | |
| `validity_end_date` | CSKS.DATBI | | ValidityEndDate | |
| `company_code` | CSKS.BUKRS | | CompanyCode | |
| `default_profit_center` | CSKS.PRCTR | | ProfitCenter | Default only |
| `cost_center_category` | CSKS.KOSAR | | CostCenterCategory | |
| `hierarchy_area` | CSKS.KHINR | | CostCenterStandardHierarchyNode | ECC: set name; S4: hierarchy node ref |
| `department` | CSKS.ABTEI | | Department | |
| `responsible_person` | CSKS.VERAK | | ResponsiblePerson | |
| `cost_center_name` | CSKT.KTEXT | | (from CostCenter entity) | ECC: join CSKT; S4: embedded |

---

## Profit Center — CEPC+CEPCT → ProfitCenter

| Silver Column | ECC Table.Field | S/4 CDS Entity | S/4 CDS Field | Notes |
|---|---|---|---|---|
| `controlling_area` | CEPC.KOKRS | ProfitCenter | ControllingArea | |
| `profit_center` | CEPC.PRCTR | | ProfitCenter | |
| `validity_start_date` | CEPC.DATAB | | ValidityStartDate | |
| `validity_end_date` | CEPC.DATBI | | ValidityEndDate | |
| `company_code` | CEPC.BUKRS | | CompanyCode | Via PrftCtrCompanyCodeAssignment in S4 |
| `segment` | CEPC.SEGMENT | | Segment | |
| `department` | CEPC.ABTEI | | Department | |
| `responsible_person` | CEPC.VERAK | | ResponsiblePerson | |
| `profit_center_name` | CEPCT.KTEXT | | (from ProfitCenter entity) | |

---

## GL Account — SKA1+SKAT+SKB1 → GeneralLedgerAccount

| Silver Column | ECC Table.Field | S/4 CDS Entity | S/4 CDS Field | Notes |
|---|---|---|---|---|
| `chart_of_accounts` | SKA1.KTOPL | GeneralLedgerAccount | ChartOfAccounts | |
| `gl_account` | SKA1.SAKNR | | GLAccount | |
| `account_group` | SKA1.KTOKS | | GLAccountGroup | |
| `is_balance_sheet` | SKA1.XBILK | | IsBalanceSheetAccount | 'X'=true |
| `pl_account_type` | SKA1.GVTYP | | ProfitLossAccountType | See gl-account-type-classification.md |
| `alternative_account` | SKA1.BILKT | | AlternativeGLAccount | Group CoA reference |
| `account_name_short` | SKAT.TXT20 | | (from entity) | |
| `account_name` | SKAT.TXT50 | | GLAccountName | |
| `company_code_currency` | SKB1.WAERS | | AccountCurrency | |
| `is_open_item` | SKB1.XOPVW | | IsOpenItemManaged | |
| `reconciliation_type` | SKB1.MITKZ | | ReconciliationAccountType | D/K/A |
| `field_status_group` | SKB1.FSTAG | | FieldStatusGroup | |

---

## Customer — KNA1+KNB1 → Customer+CustomerCompanyCode

| Silver Column | ECC Table.Field | S/4 CDS Entity | S/4 CDS Field |
|---|---|---|---|
| `customer` | KNA1.KUNNR | Customer | Customer |
| `customer_name` | KNA1.NAME1 | | CustomerFullName |
| `country` | KNA1.LAND1 | | Country |
| `city` | KNA1.ORT01 | | CityName |
| `customer_account_group` | KNA1.KTOKD | | CustomerAccountGroup |
| `company_code` | KNB1.BUKRS | CustomerCompanyCode | CompanyCode |
| `payment_terms` | KNB1.ZTERM | | PaymentTerms |
| `reconciliation_account` | KNB1.AKONT | | ReconciliationAccount |

---

## Supplier/Vendor — LFA1+LFB1 → Supplier+SupplierCompanyCode

| Silver Column | ECC Table.Field | S/4 CDS Entity | S/4 CDS Field |
|---|---|---|---|
| `supplier` | LFA1.LIFNR | Supplier | Supplier |
| `supplier_name` | LFA1.NAME1 | | SupplierFullName |
| `country` | LFA1.LAND1 | | Country |
| `city` | LFA1.ORT01 | | CityName |
| `vendor_account_group` | LFA1.KTOKK | | SupplierAccountGroup |
| `company_code` | LFB1.BUKRS | SupplierCompanyCode | CompanyCode |
| `payment_terms` | LFB1.ZTERM | | PaymentTerms |
| `reconciliation_account` | LFB1.AKONT | | ReconciliationAccount |

---

## Purchase Order — EKKO+EKPO+EKKN → PurchaseOrder+PurchaseOrderItem+PurchaseOrderAccountAssignment

| Silver Column | ECC Table.Field | S/4 CDS Entity | S/4 CDS Field |
|---|---|---|---|
| `purchasing_document` | EKKO.EBELN | PurchaseOrder | PurchaseOrder |
| `company_code` | EKKO.BUKRS | | CompanyCode |
| `document_type` | EKKO.BSART | | PurchaseOrderType |
| `supplier` | EKKO.LIFNR | | Supplier |
| `purchasing_org` | EKKO.EKORG | | PurchasingOrganization |
| `purchasing_group` | EKKO.EKGRP | | PurchasingGroup |
| `po_date` | EKKO.BEDAT | | PurchaseOrderDate |
| `currency` | EKKO.WAERS | | DocumentCurrency |
| `po_item` | EKPO.EBELP | PurchaseOrderItem | PurchaseOrderItem |
| `material` | EKPO.MATNR | | Material |
| `plant` | EKPO.WERKS | | Plant |
| `item_text` | EKPO.TXZ01 | | PurchaseOrderItemText |
| `net_value` | EKPO.NETWR | | NetPriceAmount |
| `acct_assign_category` | EKPO.KNTTP | | AccountAssignmentCategory |
| `gl_account` | EKKN.SAKTO | PurchaseOrderAccountAssignment | GLAccount |
| `cost_center` | EKKN.KOSTL | | CostCenter |
| `profit_center` | EKKN.PRCTR | | ProfitCenter |
| `internal_order` | EKKN.AUFNR | | InternalOrder |
| `wbs_element` | EKKN.PS_PSP_PNR | | WBSElement |
| `acct_assign_number` | EKKN.ZEKKN | | AccountAssignmentNumber |

---

## Hierarchy — SETHEADER+SETNODE+SETLEAF → CostCenterHierarchyNode

| Concept | ECC Tables | ECC Fields | S/4 CDS Entity | S/4 CDS Fields |
|---|---|---|---|---|
| Hierarchy definition | SETHEADER | SETCLASS+SUBCLASS+SETNAME | CostCenterHierarchy | ControllingArea+CostCenterHierarchy |
| Parent→child link | SETNODE | SETNAME→SUBSETNAME | CostCenterHierarchyNode | HierarchyNode+ParentNode |
| Node level | _(derived from recursion depth)_ | — | CostCenterHierarchyNode | HierarchyNodeLevel |
| Leaf cost center | SETLEAF | FROM_VALUE, TO_VALUE | CostCenterHierarchyNode | CostCenter (when NodeType='LEAF') |
| Node display text | SETHEADERT | DESCRIPT | CostCenterHierarchyNodeText | NodeDescription |

**Migration note**: ECC SET hierarchy uses range-based leaf values (FROM_VALUE, TO_VALUE), which means a single leaf node can cover a range of cost centers. S/4HANA hierarchy nodes are explicit (one node per CC). When migrating, expand ECC ranges to individual CC rows in the bridge table.

---

## Key Migration Differences to Handle in Bronze

| Topic | ECC Behavior | S/4 Behavior | Silver Impact |
|---|---|---|---|
| Global currency amount | Not in BSEG — requires FX derivation | `AmountInGlobalCurrency` native | `amount_global` nullable in ECC Bronze |
| Ledger | No ledger concept (single ledger) | Multi-ledger — always filter `SourceLedger = '0L'` | Add ledger filter in S4 Bronze |
| Fiscal period format | MONAT = '3' (no padding) | FiscalPeriod = '003' (zero-padded) | Pad in ECC Bronze: `LPAD(MONAT,3,'0')` |
| Hierarchy model | SET tables (range-based leaves) | CDS HierarchyNode (explicit per-object) | Pre-expand ECC ranges at Silver |
| Master data texts | Separate text tables (CSKT, CEPCT, SKAT) | Embedded in CDS entity | Join in ECC Bronze; direct in S4 Bronze |
| CO-PA line items | Separate `CE1xxxx` tables | Unified in ACDOCA | ECC: separate ingestion; S4: same GL entity |
| Company code currency | Join T001.WAERS | Embedded in CDS field | Join in ECC Bronze |
| Chart of accounts | Join T001.KTOPL | Embedded in CDS field | Join in ECC Bronze |
| Client field | MANDT on every table | Transparent in CDS | Filter in ECC Bronze only |
