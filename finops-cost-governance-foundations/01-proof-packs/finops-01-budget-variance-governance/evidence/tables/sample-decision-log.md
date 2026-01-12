# Sample Decision Log (Sanitized)

![Status](https://img.shields.io/badge/Status-Sample_Data-lightgrey)
![Focus](https://img.shields.io/badge/Focus-Decision_Trail_%26_Auditability-blue)
![Domain](https://img.shields.io/badge/Domain-IT_Financial_Governance-orange)
![Scope](https://img.shields.io/badge/Scope-Evidence_Table_(Sanitized)-yellow)

---

## Purpose
Provide a sanitized example of the **decision log** produced during the monthly cost review.  
This log demonstrates:
- who owned the variance review
- what decision was made (approve / re-allocate / reduce / defer)
- the business rationale
- traceability to supporting evidence artifacts (EV) and commentary (VC)

> **Scope note**
> Entries are illustrative and sanitized. This log does not represent any employer system, tenant, or billing export.

---

## Decision log (sanitized example)

| Decision ID | Period | Cost owner | Cost center | Status trigger | Driver type | Decision | Decision summary | Effective date | Next review | Commentary Ref | Evidence Ref |
|---|---|---|---|---|---|---|---|---|---|---|---|
| DL-2026-01-001 | 2026-01 | Owner A | CC-1001 | Investigate | Usage | Re-allocate | Variance driven by expected workload increase; re-allocated funds from under-run category to maintain baseline controls. | 2026-01-15 | 2026-02 | [VC-2026-01-001](../evidence-index.md#vc-2026-01-001) | [EV-2026-01-001](../evidence-index.md#ev-2026-01-001) |
| DL-2026-01-002 | 2026-01 | Owner C | CC-3003 | Escalate | Rate / pricing | Approve increase | Approved budget increase due to pricing change; forecast updated and communicated; non-critical spend held until next review. | 2026-01-18 | 2026-02 | [VC-2026-01-003](../evidence-index.md#vc-2026-01-003) | [EV-2026-01-003](../evidence-index.md#ev-2026-01-003) |
| DL-2026-01-003 | 2026-01 | Owner D | CC-9999 | Escalate | Allocation | Correct allocation | Unallocated spend identified; assigned to correct cost center mapping; exception tracked until confirmed by next cycle. | 2026-01-20 | 2026-02 | [VC-2026-01-004](../evidence-index.md#vc-2026-01-004) | [EV-2026-01-004](../evidence-index.md#ev-2026-01-004) |

---

## Field definitions (audit-friendly)

- **Decision ID:** Unique identifier for the decision entry
- **Period:** Month being reviewed (YYYY-MM)
- **Cost owner / cost center:** Accountable owner and allocation key (sanitized)
- **Status trigger:** Monitor / Investigate / Escalate (from variance thresholds)
- **Driver type:** Primary cause category (usage / rate / allocation / scope)
- **Decision:** approve increase / re-allocate / reduce / defer / correct allocation
- **Decision summary:** Plain-language rationale suitable for leadership review
- **Effective date:** When the decision takes effect
- **Next review:** When the decision is re-checked for closure
- **Commentary Ref:** Link to the narrative entry (VC) in the evidence index
- **Evidence Ref:** Link to the supporting artifact (EV) in the evidence index

---

## Review standard (what “good” looks like)
For any **Investigate** or **Escalate** item:
- driver is stated clearly (usage / rate / allocation / scope)
- decision is explicit (not implied)
- rationale is business-first and defensible
- references exist for both commentary (VC) and evidence (EV)

---

## Navigation
- Back to Proof Pack 01: [README](../../README.md)
- Financial logic: [financial-logic](../../financial-logic.md)
- Evidence index: [evidence index](../evidence-index.md)
- Repo README: [README](../../../../README.md)
