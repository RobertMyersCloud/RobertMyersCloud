# Sample Variance Table (Sanitized)

![Status](https://img.shields.io/badge/Status-Sample_Data-lightgrey)
![Focus](https://img.shields.io/badge/Focus-Variance_%26_Forecast_Triage-blue)
![Domain](https://img.shields.io/badge/Domain-IT_Financial_Governance-orange)
![Scope](https://img.shields.io/badge/Scope-Evidence_Table_(Sanitized)-yellow)

---

## Purpose
Provide a sanitized example of the variance table used in the monthly close package. This table supports:
- budget vs actual comparison
- variance classification (monitor / investigate / escalate)
- forecast view and commentary references
- evidence traceability (IDs link back to the evidence index)

> **Scope note**
> Values are illustrative. This table does not represent any employer billing export or production tenant.

---

## Table (sanitized example — monthly close view)

> **Viewing note:** This table is wide by design. Use the horizontal scroll bar to view all columns.

| Billing period | Cost owner | Cost center | Service / Category | Budget (USD) | Actual (USD) | Variance (USD) | Variance (%) | Status | Forecast (USD) | Commentary Ref | Evidence Ref |
|---|---|---|---|---:|---:|---:|---:|---|---:|---|---|
| 2026-01 | Owner A | CC-1001 | Compute | 10,000 | 10,650 | 650 | 6.5% | Investigate | 10,900 | VC-2026-01-001 | EV-2026-01-001 |
| 2026-01 | Owner B | CC-2002 | Storage | 4,500 | 4,420 | -80 | -1.8% | Monitor | 4,520 | VC-2026-01-002 | EV-2026-01-002 |
| 2026-01 | Owner C | CC-3003 | Networking | 2,000 | 2,320 | 320 | 16.0% | Escalate | 2,450 | VC-2026-01-003 | EV-2026-01-003 |
| 2026-01 | Owner D | CC-9999 | Unallocated | 0 | 740 | 740 | N/A | Escalate | 740 | VC-2026-01-004 | EV-2026-01-004 |

---

## Column definitions (audit-friendly)

- **Billing period:** Month being reviewed (YYYY-MM)
- **Cost owner:** Accountable individual or team alias (sanitized)
- **Cost center:** Financial allocation key (sanitized)
- **Service / Category:** Spend grouping for investigation and reporting
- **Budget / Actual:** Period baseline vs observed spend
- **Variance (USD):** `Actual - Budget`
- **Variance (%):** `(Actual - Budget) / Budget` (when Budget > 0)
- **Status:** Governance routing based on thresholds (Monitor / Investigate / Escalate)
- **Forecast (USD):** Rolling forecast for period close
- **Commentary Ref:** Linkable ID for the variance narrative
- **Evidence Ref:** Linkable ID recorded in the evidence index

---

## Governance notes
- **Investigate:** Commentary required (driver + expected duration)
- **Escalate:** Commentary + decision required (approve / re-allocate / reduce / defer) with evidence references
- **Unallocated:** Treated as a governance exception requiring resolution within the next review cycle

---

## Navigation
- Back to Proof Pack 01: [README](../../README.md)
- Financial logic: [Financial logic](../../financial-logic.md)
- Evidence index: [Evidence index](../evidence-index.md)
- Repo README: [README](../../../../README.md)
