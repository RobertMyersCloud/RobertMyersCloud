# Proof Pack 01: Budget vs Actuals & Variance Governance

![Status](https://img.shields.io/badge/Status-Active-success)
![Focus](https://img.shields.io/badge/Focus-Monthly_Close_%26_Forecasting-blue)
![Role](https://img.shields.io/badge/Role-Financial_Analyst-orange)
![Scope](https://img.shields.io/badge/Scope-Governance_%2F_Analysis-yellow)

---

## Goal
Demonstrate a repeatable, auditable approach for controlling cloud spend using:
- budget baselines
- variance thresholds
- forecast updates
- decision logging
- evidence retention

---

## What this proves
This proof pack shows I can operate cloud cost management as a **financial control domain**:
- define and apply variance triggers (monitor / investigate / escalate)
- separate **cash timing** from **management reporting** (cost normalization)
- run a monthly review rhythm with documented decisions
- retain traceable artifacts suitable for leadership and audit review

---

## Inputs and assumptions
This proof pack uses **sample/sanitized** tables to demonstrate methodology without implying access to any employer billing system or production tenant.

- Budget baseline is treated as fixed for the period.
- Forecast is updated monthly using a rolling forecast approach.
- Allocation uses a precedence “waterfall” to reduce unassigned spend.

See:
- [Assumptions](../../00-context/assumptions.md)
- [Scope boundaries](../../00-context/scope-boundaries.md)

---

## Core artifacts (start here)

### 1) Executive summary (one-page)
Use this if you want the business outcome quickly.

- [Executive summary](executive-summary.md)

### 2) Financial logic (how decisions are made)
Defines variance math, thresholds, forecast triggers, normalization, and allocation waterfall.

- [Financial logic](financial-logic.md)

### 3) Evidence index (traceability)
This is the audit-style index of artifacts referenced by this proof pack.

- [Evidence index](evidence/evidence-index.md)

### 4) Evidence tables (sample inputs/outputs)
Sanitized tables used to demonstrate what the review pack looks like.

- [Evidence tables](evidence/tables/)

---

## Evidence (real Azure cost data)

This proof pack includes **real Azure Cost Management evidence** captured during a live billing period and retained as traceable artifacts.

### Azure Cost Analysis screenshots
These screenshots establish budget context, isolate spend drivers, and show forecasted exposure:

- **Accumulated vs Budget (baseline context)**  
  → [EV-2026-01-005](evidence/screenshots/EV-2026-01-005_azure-cost-analysis_accumulated-vs-budget.png)

- **Group by Service (driver analysis)**  
  → [EV-2026-01-006](evidence/screenshots/EV-2026-01-006_azure-cost-analysis_group-by-service.png)

- **Forecast View (forward-looking risk)**  
  → [EV-2026-01-007](evidence/screenshots/EV-2026-01-007_cost-analysis_forecast-view.png)

### Governance outputs
- **Variance table (sanitized):** [EV-2026-01-001](evidence/tables/sample-variance-table.md)
- **Decision log (sanitized):** [EV-2026-01-008](evidence/tables/sample-decision-log.md)

All evidence artifacts are indexed and linkable:
- **Evidence index:** [evidence-index.md](evidence/evidence-index.md)

> **Control outcome**
> Spend signals → variance classification → decision → retained evidence (auditable chain).

---

## Operating workflow (how this runs monthly)

1. **Baseline budget established** for the month/period
2. **Actuals reviewed** and variance calculated
3. Variance routed by threshold:
   - **Monitor** (≤ 5%): trend tracked
   - **Investigate** (> 5% and ≤ 10%): commentary required
   - **Escalate** (> 10%): decision + evidence required
4. **Forecast updated** (rolling forecast) when triggers are met
5. **Decision logged** (approve / re-allocate / reduce / defer)
6. **Evidence retained** and referenced in the evidence index

> **Control note**
> The output is not a “dashboard screenshot.” The output is a **decision trail**: what changed, why it changed, who approved it, and what evidence supports it.

---

## Outputs produced (what a reviewer should expect)

- Variance table with commentary references
- Forecast note (date, owner, rationale)
- Allocation exception list (unallocated spend flagged)
- Decision log entries linked to evidence IDs

Templates used (repo root):
- [Variance commentary template](../../03-reporting-templates/variance-commentary-template.md)
- [Exec brief one-pager](../../03-reporting-templates/exec-brief-onepager.md)
- [Monthly cost review agenda](../../03-reporting-templates/monthly-cost-review-agenda.md)

---

## Evidence standards (audit-safe)
- Every artifact is linkable and referenced by ID in the evidence index.
- All sample data is sanitized and does not represent any employer tenant or billing export.
- The framework focuses on **governance behavior**, not platform administration.

---

## Navigation
- Back to repo: [README](../../README.md)
- Portfolio map: [PORTFOLIO.md](../../PORTFOLIO.md)
