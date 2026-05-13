# Document Type Reference — BLART Classification

SAP document types (`BKPF.BLART`) classify the origin and purpose of every accounting document.
Use this to filter or categorize GL postings in FP&A models.

---

## Standard SAP Document Types

### FI — General Ledger / Manual Postings

| BLART | Description | Origin | FP&A Category | Notes |
|---|---|---|---|---|
| `SA` | G/L Account Document | Manual (FB01, FB50) | Accruals / Adjustments | General journal entries |
| `AB` | Accounting Document | Various (batch, interface) | Depends on content | Catch-all for automated postings |
| `SB` | G/L Account Posting (special) | FB01 variant | Accruals | |
| `ZP` | Payment Posting | F110 auto-payment | Cash / Liquidity | |
| `DA` | Customer Document | AR manual | Revenue Adjustment | |

### FI-AP — Accounts Payable

| BLART | Description | Origin | FP&A Category | Notes |
|---|---|---|---|---|
| `KR` | Vendor Invoice | MIRO, FB60 | Expense / COGS | Most common AP posting |
| `KG` | Vendor Credit Memo | FB65, MIRO | Expense Reversal | |
| `KZ` | Vendor Payment | F110, F-53 | Cash / Liquidity | Clears open KR item |
| `KA` | Vendor Document | FB01 | Vendor Subledger | |
| `KN` | Net Vendor Posting | | | |
| `ZK` | Vendor Payment (custom) | | Cash | Client-specific variant |

### FI-AR — Accounts Receivable

| BLART | Description | Origin | FP&A Category | Notes |
|---|---|---|---|---|
| `DR` | Customer Invoice | FB70, SD billing interface | Revenue | Posted when billing doc is released |
| `DG` | Customer Credit Memo | FB75 | Revenue Reversal | |
| `DZ` | Customer Payment | F110, F-28 | Cash / Liquidity | Clears open DR item |
| `DA` | Customer Document | FB01 | AR Subledger | |
| `DN` | Net Customer Posting | | | |
| `RV` | Billing Document Transfer | VF01 SD→FI interface | Revenue | SD-generated; links to VBRK |

### MM — Materials Management / Procurement

| BLART | Description | Origin | FP&A Category | Notes |
|---|---|---|---|---|
| `WA` | Goods Issue | MIGO, MB1A | COGS / Expense | Stock reduction + P&L cost |
| `WE` | Goods Receipt | MIGO, MB01 | COGS / Inventory | GR/IR posting; links to PO |
| `WL` | Goods Issue for Delivery | VL01N | COGS | SD-triggered goods issue |
| `WI` | Inventory Document | MI07 inventory adj | Inventory Adjustment | |
| `RE` | Invoice Receipt (MM) | MIRO | Expense / AP | Vendor invoice for PO; clears GR/IR |
| `RN` | Invoice Cancellation | MR8M | Expense Reversal | |
| `PR` | Price Change | MR21 | Inventory Revaluation | |

### CO — Controlling

| BLART | Description | Origin | FP&A Category | Notes |
|---|---|---|---|---|
| `RKP` | CO Reposting | KB21N | Cost Reallocation | Moves cost between cost centers |
| `KO` | Internal Order Settlement | KO88 | Cost Allocation | Order costs settled to cost center/asset |
| `AA` | Asset Accounting | AFAB depreciation run | Depreciation | FI-AA integration |
| `AF` | Depreciation Run | | Depreciation | |
| `AN` | Net Asset Posting | | Asset | |
| `AW` | Asset Retirement | ABAON | Asset Write-off | |

### Tax / Special

| BLART | Description | Origin | FP&A Category |
|---|---|---|---|
| `EU` | Euro Rounding | | FX / Rounding |
| `ML` | Material Ledger | CKMLCP | Actual Costing |
| `UE` | Transfer Posting | | Internal Transfer |
| `SK` | Cash Discount | | Discount / Rebate |

---

## FP&A Grouping — Suggested Classification

Use this in a Gold layer lookup to group document types for FP&A reporting:

| FP&A Group | BLART Values | Description |
|---|---|---|
| `REVENUE` | RV, DR | SD-billed revenue + manual AR invoices |
| `REVENUE_ADJ` | DG, DA | Customer credit memos, AR adjustments |
| `COGS` | WA, WL | Goods issues to production/delivery |
| `VENDOR_EXPENSE` | KR, RE | Vendor invoices (services, materials) |
| `VENDOR_CREDIT` | KG, RN | Vendor credit memos and cancellations |
| `PAYMENT_AP` | KZ, ZK | Outgoing payments |
| `PAYMENT_AR` | DZ | Incoming payments |
| `ACCRUAL` | SA, SB, AB | Manual GL entries, accruals, adjustments |
| `COST_ALLOCATION` | RKP, KO | CO internal cost movements |
| `DEPRECIATION` | AA, AF | Asset depreciation |
| `INVENTORY` | WE, WI, PR | Goods receipts, inventory adjustments |
| `FX_ROUNDING` | EU | Exclude from operational FP&A |

```sql
-- Gold layer: add FP&A group
SELECT
  gl.*,
  CASE gl.document_type
    WHEN 'RV' THEN 'REVENUE'  WHEN 'DR' THEN 'REVENUE'
    WHEN 'DG' THEN 'REVENUE_ADJ'
    WHEN 'WA' THEN 'COGS'     WHEN 'WL' THEN 'COGS'
    WHEN 'KR' THEN 'VENDOR_EXPENSE' WHEN 'RE' THEN 'VENDOR_EXPENSE'
    WHEN 'KG' THEN 'VENDOR_CREDIT'  WHEN 'RN' THEN 'VENDOR_CREDIT'
    WHEN 'KZ' THEN 'PAYMENT_AP'
    WHEN 'DZ' THEN 'PAYMENT_AR'
    WHEN 'SA' THEN 'ACCRUAL'  WHEN 'SB' THEN 'ACCRUAL' WHEN 'AB' THEN 'ACCRUAL'
    WHEN 'RKP' THEN 'COST_ALLOCATION' WHEN 'KO' THEN 'COST_ALLOCATION'
    WHEN 'AA' THEN 'DEPRECIATION' WHEN 'AF' THEN 'DEPRECIATION'
    WHEN 'WE' THEN 'INVENTORY' WHEN 'WI' THEN 'INVENTORY'
    ELSE 'OTHER'
  END AS fpa_doc_group
FROM silver.gl_line_item gl
```

---

## Reversal Detection

Reversed documents are common in FP&A — they must not be double-counted.

```sql
-- Exclude reversed documents from P&L actuals
WHERE (reversal_document IS NULL OR reversal_document = '')   -- not reversed
  AND (reference_document NOT LIKE 'STORNO%')                 -- not a reversal itself
```

More robust approach: join BKPF to itself on STBLG and exclude pairs:

```sql
-- In Silver: add reversal flag
CASE
  WHEN h.STBLG IS NOT NULL AND h.STBLG != '' THEN true
  ELSE false
END AS is_reversed
```

Filter in Gold: `WHERE is_reversed = false`

---

## Origin Tracing via AWTYP / AWKEY (BKPF)

For cross-domain lineage — tracing which SD/MM object generated a GL posting:

| AWTYP | Description | AWKEY Format | Joins To |
|---|---|---|---|
| `VBRK` | SD Billing Document | BillingDocument + FiscalYear | VBRK.VBELN |
| `MKPF` | Goods Movement | MaterialDocument + FiscalYear | MKPF.MBLNR |
| `RBKP` | Vendor Invoice (LIV) | InvoiceDoc + FiscalYear | RBKP.BELNR |
| `BKPF` | FI Document (cross-ref) | CompanyCode + Document + FiscalYear | BKPF itself |
| `COPA` | CO-PA Line Items | — | CE1xxxx |

Use `AWTYP + AWKEY` in Silver `journal_entry_header` for lineage joins to SD/MM without relying on BSEG foreign key fields.
