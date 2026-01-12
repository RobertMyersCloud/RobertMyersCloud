# Monthly FinOps Close (Operating Rhythm)

![Status](https://img.shields.io/badge/Status-Active-success)
![Focus](https://img.shields.io/badge/Focus-Monthly_Close_%26_Governance-blue)
![Domain](https://img.shields.io/badge/Domain-IT_Financial_Governance-orange)
![Scope](https://img.shields.io/badge/Scope-Operating_Model-yellow)

---

## Purpose
Define a repeatable monthly rhythm for cloud cost governance that produces an executive-ready close package and a traceable decision record.

> **Scope note**
> This operating model is governance and reporting focused. It does not imply engineering authority or production enforcement.

---

## Inputs (what is reviewed)
- Budget baseline for the month
- Actual spend for the month (period-to-date and final)
- Rolling forecast (if maintained during the month)
- Allocation coverage and Unallocated exceptions
- Open variance items requiring commentary or decisions

See: [Data sources (conceptual)](../00-context/data-sources.md)

---

## Outputs (what is produced)
A monthly close package typically includes:
- variance table with governance status (monitor / investigate / escalate)
- variance commentary for investigate/escalate items
- forecast note (if updated) with rationale and date
- allocation exception list (including Unallocated)
- evidence index updates (EV / VC references)

Reference implementation:
- [Proof Pack 01 README](../01-proof-packs/finops-01-budget-variance-governance/README.md)

---

## Cadence and steps (repeatable)

### Week 1–2 (early trend control)
- Review spend trend vs baseline
- Flag anomalies and allocation gaps early
- Start commentary drafts for items trending to Investigate/Escalate

### Week 3 (pre-close stabilization)
- Confirm whether variance drivers are expected or unexpected
- Validate forecast vs baseline and update if triggers are met
- Assign owners for variance narratives and allocation fixes

### Week 4 / Close (finalization)
1. Finalize actuals
2. Calculate variance vs budget
3. Classify items by threshold (Monitor / Investigate / Escalate)
4. Complete commentary for Investigate/Escalate items
5. Record decisions (approve / re-allocate / reduce / defer)
6. Update evidence index with IDs and links
7. Publish the close package for leadership review

---

## Review meeting structure (30–45 minutes)
Recommended agenda:
- Open with top variances and allocation exceptions
- Review Investigate items (commentary required)
- Review Escalate items (decision required)
- Confirm forecast changes and rationale
- Confirm next actions and owners
- Confirm evidence references are recorded

Template:
- [Monthly cost review agenda](../03-reporting-templates/monthly-cost-review-agenda.md)

---

## Governance controls (minimum standard)
- Every Investigate/Escalate item has an owner, a recommendation, and an evidence reference
- Unallocated spend is visible and tracked as an exception
- Forecast changes are dated and explained (no silent re-baselining)
- Outputs are stored and linkable

---

## Navigation
- Repo README: [README](../README.md)
- Operating principles: [Operating principles](../00-context/operating-principles.md)
- Proof Pack 01: [Proof Pack 01 README](../01-proof-packs/finops-01-budget-variance-governance/README.md)
