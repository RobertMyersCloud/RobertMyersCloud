# How to Review This Repository (Recruiter / Hiring Manager Guide)

![Status](https://img.shields.io/badge/Status-Active-success)
![Focus](https://img.shields.io/badge/Focus-Reviewer_Navigation-blue)
![Audience](https://img.shields.io/badge/Audience-Recruiters_%26_Hiring_Managers-informational)
![Scope](https://img.shields.io/badge/Scope-Governance_%2F_Analysis_(No_Admin)-yellow)

---

## Purpose
Provide a fast, reliable path for reviewing this repository. This repo is designed to demonstrate **FinOps / cloud cost governance** as a financial control domain:
- budget vs actual variance governance
- rolling forecast discipline
- cost allocation exception handling
- decision logging with evidence traceability

This is **not** a cloud engineering portfolio.

---

## Recommended review path (10 minutes)

### 1) Start here (Portfolio map)
- [PORTFOLIO.md](../PORTFOLIO.md)

This is the index and the recommended reading order.

### 2) Skim the repo framing (scope + standards)
- [Operating principles](operating-principles.md)
- [FinOps maturity positioning](maturity-positioning.md)
- [Data sources (conceptual)](data-sources.md)
- [Scope boundaries](scope-boundaries.md)
- [Assumptions](assumptions.md)

This explains how decisions are made and what is intentionally excluded.

### 3) Review the primary proof pack (Proof Pack 01)
- [Proof Pack 01 README](../01-proof-packs/finops-01-budget-variance-governance/README.md)
- [Executive summary (one-page)](../01-proof-packs/finops-01-budget-variance-governance/executive-summary.md)
- [Financial logic](../01-proof-packs/finops-01-budget-variance-governance/financial-logic.md)

This shows the operating model and the logic used to govern spend.

### 4) Verify evidence discipline (traceability)
- [Evidence index (traceability register)](../01-proof-packs/finops-01-budget-variance-governance/evidence/evidence-index.md)
- [Sample variance table (sanitized)](../01-proof-packs/finops-01-budget-variance-governance/evidence/tables/sample-variance-table.md)

This confirms the repo is evidence-driven and audit-safe.

---

## What to look for (evaluation criteria)

### Governance maturity indicators
- Clear thresholds that trigger action (monitor / investigate / escalate)
- Explicit ownership and accountability
- Forecast discipline (when forecasts change and why)
- Allocation exception handling (Unallocated is visible and treated as an exception)
- Repeatable monthly close package (not ad hoc analysis)

### Audit / defensibility indicators
- Evidence artifacts are linkable
- Evidence is referenced by ID (EV / VC)
- Assumptions and scope boundaries are explicit
- No implied production access or engineering authority

---

## What this repo intentionally avoids
To prevent “tool cosplay” and over-claiming, this repo does **not** focus on:
- deep Azure configuration
- IAM protocols or security tooling deep dives
- on-call operational claims
- optimization engineering work (rightsizing/autoscaling) presented as hands-on execution

This is deliberate: the portfolio targets roles centered on **governance, analysis, controls, and executive reporting**.

---

## Navigation
- Repo README: [README](../README.md)
- Portfolio map: [PORTFOLIO.md](../PORTFOLIO.md)
- Proof Pack 01: [Proof Pack 01 README](../01-proof-packs/finops-01-budget-variance-governance/README.md)
