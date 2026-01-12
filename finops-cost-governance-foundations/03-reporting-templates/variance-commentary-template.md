# Variance Commentary (Template)

![Status](https://img.shields.io/badge/Status-Template-lightgrey)
![Focus](https://img.shields.io/badge/Focus-Variance_Commentary_%26_Decisions-blue)
![Domain](https://img.shields.io/badge/Domain-IT_Financial_Governance-orange)
![Scope](https://img.shields.io/badge/Scope-Governance_Record-yellow)

---

## Purpose
Standardize variance commentary so Investigate/Escalate items are documented consistently and defensibly. This template produces a review-ready narrative that:
- explains the driver in business terms
- states whether the variance is one-time or recurring
- recommends an action (approve / re-allocate / reduce / defer)
- references evidence artifacts (EV / VC IDs)

> **Usage note**
> Keep the narrative concise. Link to evidence rather than embedding long detail.

---

## Variance record
- **Reference ID (VC):** VC-YYYY-MM-###
- **Billing period:** YYYY-MM
- **Cost owner:** (Name / Team alias)
- **Cost center:** (CC-####)
- **Service / Category:** (Compute / Storage / Networking / Shared / Unallocated)
- **Status:** Monitor / Investigate / Escalate
- **Prepared by:** (Name / Role)
- **Date prepared:** YYYY-MM-DD

---

## Summary (2–3 sentences)
State what changed and why it matters.

(Example) Actual spend finished 6.5% above budget due to increased compute hours supporting an approved scope change. The variance is expected to normalize next month as the workload stabilizes.

---

## Driver classification
Select one primary driver (add secondary if needed):
- Scope change (new workload / environment)
- Usage increase (consumption)
- Rate change (pricing / commitment change)
- Allocation change (mapping / tagging K gaps)
- One-time event (project / incident / migration)
- Unknown (requires investigation)

**Primary driver:**  
**Secondary driver (if any):**

---

## Duration and impact horizon
- **One-time or recurring:** One-time / Recurring / Unknown
- **Expected duration:** (e.g., 2 weeks / 1 month / ongoing)
- **Forecast impact:** +/– $X (if known)

---

## Financial view
- **Budget (USD):** $
- **Actual (USD):** $
- **Variance (USD):** $
- **Variance (%):** %

---

## Recommendation (required for Investigate/Escalate)
Choose one:
- Approve increase (document rationale)
- Re-allocate budget (identify source)
- Reduce usage (targeted action)
- Defer / pause non-critical spend
- Correct allocation (fix mapping and re-assign costs)

**Recommended action:**  
**Rationale (1–2 lines):**

---

## Decision (required for Escalate)
- **Decision:** Approve / Re-allocate / Reduce / Defer / Correct allocation
- **Decision owner:** (Name / Role)
- **Decision date:** YYYY-MM-DD
- **Due date (if action required):** YYYY-MM-DD

---

## Evidence references (linkable)
List the evidence artifacts supporting this commentary.

- **EV references:** EV-YYYY-MM-###, EV-YYYY-MM-###
- **Links:** (paste links to tables/screenshots/notes as applicable)

> **Minimum standard**
> Every Investigate/Escalate item must reference at least one EV artifact and must be recorded in the Evidence Index.

---

## Notes (optional)
Add any constraints, risks, or dependencies that leadership should be aware of.

---

## Navigation
- Repo README: [README](../README.md)
- Monthly FinOps Close: [Monthly FinOps Close](../02-operating-models/monthly-finops-close.md)
- Proof Pack 01: [Proof Pack 01 README](../01-proof-packs/finops-01-budget-variance-governance/README.md)
