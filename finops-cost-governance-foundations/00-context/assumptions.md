# Assumptions (Framework Constraints)

![Status](https://img.shields.io/badge/Status-Active-success)
![Focus](https://img.shields.io/badge/Focus-Assumptions_%26_Constraints-blue)
![Domain](https://img.shields.io/badge/Domain-IT_Financial_Governance-orange)
![Scope](https://img.shields.io/badge/Scope-Recruiter_%26_Audit_Safe-yellow)

---

## Purpose
Make assumptions explicit so reviewers can evaluate the framework without inferring access, authority, or tooling that is not demonstrated in this repository.

---

## Governance assumptions
- Cloud spend governance is treated as a **financial control domain** with consistent review rhythms.
- Ownership is required for effective governance (cost owner + cost center mapping).
- Variance thresholds trigger defined actions (monitor / investigate / escalate).
- Decisions are logged and supported by evidence references (EV / VC).

---

## Data assumptions (conceptual)
- Budgets exist as an approved baseline for the period (monthly or annual plan broken into months).
- Actual spend is available at least monthly, ideally weekly/daily for trend detection.
- Forecasts are updated on a rolling basis when triggers occur.
- Allocation mappings exist or can be maintained (subscription/resource group defaults when needed).

See: [Data sources (conceptual)](data-sources.md)

---

## Reporting assumptions
- Executive reporting must be readable without deep technical context.
- Variance explanations include driver, duration (one-time vs recurring), and recommendation.
- Unallocated spend is measurable and treated as an exception requiring resolution.

---

## Portfolio safety assumptions
- Sample/sanitized artifacts are used unless real data is explicitly available and sanitized.
- No claims are made about production enforcement or automation unless evidence exists in-repo.
- Metrics and outcomes are not stated unless supported by artifacts.

---

## Navigation
- Repo README: [README](../README.md)
- Scope boundaries: [Scope boundaries](scope-boundaries.md)
- Operating principles: [Operating principles](operating-principles.md)
- Proof Pack 01: [Proof Pack 01 README](../01-proof-packs/finops-01-budget-variance-governance/README.md)
