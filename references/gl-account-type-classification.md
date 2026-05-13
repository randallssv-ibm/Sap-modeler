# GL Account Type Classification — FP&A Sign Convention

Reference for classifying GL accounts and applying correct debit/credit sign logic in FP&A reporting.

---

## Account Classification Fields (SKA1)

Two fields in `SKA1` (chart of accounts level) determine how an account behaves in P&L reporting:

| Field | Table | Values | Meaning |
|---|---|---|---|
| `XBILK` | SKA1 | `'X'` = balance sheet, `' '` = P&L | Primary split: BS vs income statement |
| `GVTYP` | SKA1 | See table below | P&L sub-type (only relevant if XBILK = ' ') |

---

## GVTYP — P&L Account Type Values

| GVTYP | German Name | English | Sign Convention | FP&A Category |
|---|---|---|---|---|
| _(blank)_ | _(not a P&L account)_ | Balance Sheet account | — | Exclude from P&L |
| `X` | Aufwand / Ertrag | Expense / Revenue (generic) | Credit-normal for revenue; debit-normal for expense | Depends on normal balance |
| `L` | Leistungserlöse | Operating Revenue / Sales | **Credit-normal** → negate for reporting | Revenue |
| `M` | Material-aufwand | Material Expense / COGS | **Debit-normal** → use as-is | COGS / Direct Expense |
| `P` | Personalaufwand | Personnel Expense | **Debit-normal** | Labor / Personnel Cost |
| `R` | Raumkosten | Space / Facility Costs | **Debit-normal** | Overhead |
| `S` | Sonstige betriebl. Aufwendungen | Other Operating Expense | **Debit-normal** | SG&A / Other OpEx |
| `E` | Erträge | Other Income | **Credit-normal** → negate | Other Income |
| `F` | Finanzergebnis | Financial Result (interest) | Mixed | Financial Income/Expense |
| `G` | Außerord. Ergebnis | Extraordinary Result | Mixed | Below-the-line |

> Note: GVTYP usage varies by client configuration. Always validate against actual chart of accounts data. The most critical split is `XBILK`: filter `XBILK = ' '` for P&L accounts.

---

## Account Type (BSEG.KOART) — Line Item Level

| KOART | Account Type | Reconciliation | FP&A Handling |
|---|---|---|---|
| `S` | GL Account | Direct | Primary for P&L/BS reporting |
| `D` | Customer (Debtor) | Customer recon account | AR aging; not direct GL |
| `K` | Vendor (Creditor) | Vendor recon account | AP aging; not direct GL |
| `A` | Asset | Asset recon account | Fixed asset reporting |
| `M` | Material | Material recon account | Inventory; GR/IR |

For FP&A GL reporting: filter `KOART = 'S'` in Bronze to get pure GL account lines. D/K/A/M lines post to reconciliation accounts automatically.

---

## Debit/Credit Sign Convention

SAP stores all amounts as **absolute (unsigned) values**. The `SHKZG` field (BSEG) indicates direction.

| SHKZG | German | Direction | Standard Sign |
|---|---|---|---|
| `S` | Soll | Debit | `+` (positive) |
| `H` | Haben | Credit | `-` (negative) |

### Apply sign in Silver

```sql
CASE debit_credit_code
  WHEN 'S' THEN  amount_cc_currency
  WHEN 'H' THEN -amount_cc_currency
END AS signed_amount
```

---

## P&L Sign Logic for FP&A Reporting

After applying debit/credit sign, apply account-type sign convention for income statement presentation:

### Normal Balance by Account Category

| Account Category | Normal Balance | SKA1.XBILK | Typical GVTYP | FP&A Sign Rule |
|---|---|---|---|---|
| Revenue / Sales | Credit | `' '` | L, E | Negate signed_amount → positive = revenue earned |
| COGS / Material | Debit | `' '` | M | Use signed_amount as-is → positive = cost incurred |
| Personnel / Labor | Debit | `' '` | P | Use as-is |
| Operating Expense | Debit | `' '` | S, R | Use as-is |
| Financial Income | Credit | `' '` | F | Negate |
| Financial Expense | Debit | `' '` | F | Use as-is |
| Balance Sheet | Mixed | `'X'` | _(blank)_ | Exclude from P&L; use for BS reporting |

### Gold Layer Sign Pattern

```sql
-- Gold P&L: normalize so positive = favorable (revenue adds, expense subtracts)
SELECT
  gl.cost_center,
  gl.profit_center,
  gl.fiscal_year,
  gl.fiscal_period,
  acc.account_name,
  acc.pl_account_type,
  -- Signed amount from Silver
  gl.signed_amount,
  -- FP&A-normalized: positive = income contribution
  CASE
    WHEN acc.pl_account_type IN ('L', 'E')      THEN -gl.signed_amount  -- revenue: credit is positive
    WHEN acc.pl_account_type IN ('M','P','S','R') THEN  gl.signed_amount  -- expense: debit is positive
    WHEN acc.pl_account_type = 'F'              THEN  gl.signed_amount  -- financial: context-dependent
    ELSE gl.signed_amount
  END AS fpa_amount
FROM silver.gl_line_item gl
JOIN silver.gl_account acc
  ON gl.gl_account       = acc.gl_account
  AND gl.chart_of_accounts = acc.chart_of_accounts
WHERE acc.is_balance_sheet = false   -- P&L accounts only
  AND CAST(gl.fiscal_period AS INT) BETWEEN 1 AND 12  -- exclude special periods
```

---

## Account Group (SKA1.KTOKS) — Common Values

Account groups are client-configured, but standard SAP uses these ranges:

| KTOKS | Typical Range | Category |
|---|---|---|
| `SAKO` | 0000000001–0099999999 | Balance sheet accounts |
| `ERLS` | 0400000000–0499999999 | Revenue accounts |
| `AUFWK` | 0600000000–0699999999 | Expense accounts |
| `ANTA` | _(asset recon)_ | Asset reconciliation |
| `DKTR` | _(customer recon)_ | Customer reconciliation |
| `KRED` | _(vendor recon)_ | Vendor reconciliation |

> Account group ranges vary by chart of accounts (e.g., CAUS, CAAP, INT). Always validate against SKA1 data.

---

## Balance Sheet Account Types (for completeness)

Balance sheet accounts (`XBILK = 'X'`) are used in cash flow, balance sheet, and AR/AP reporting but excluded from P&L:

| Category | Typical GL Range | Notes |
|---|---|---|
| Fixed Assets | 0100000000–0199999999 | Reconciliation for asset subledger |
| Current Assets / AR | 0120000000–0129999999 | Customer reconciliation |
| Bank / Cash | 0113000000–0113999999 | Liquidity reporting |
| Inventory | 0131000000–0139999999 | Material/GR-IR accounts |
| Vendor / AP | 0160000000–0169999999 | Vendor reconciliation |
| Equity | 0300000000–0399999999 | Retained earnings, capital |

---

## Fiscal Period Special Values

| Period | Type | FP&A Treatment |
|---|---|---|
| 001–012 | Normal operating periods | Include in standard FP&A |
| 013 | First special period (year-end adjustments) | Exclude from operational; include in statutory |
| 014 | Second special period | Exclude |
| 015 | Third special period | Exclude |
| 016 | Fourth special period | Exclude |

Filter: `WHERE CAST(fiscal_period AS INT) BETWEEN 1 AND 12`
