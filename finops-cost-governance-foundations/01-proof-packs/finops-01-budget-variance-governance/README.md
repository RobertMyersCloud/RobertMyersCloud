# Proof Pack 01: Budget vs Actuals & Variance Governance

![Status](https://img.shields.io/badge/Status-Stable_v1.0-success)
![Focus](https://img.shields.io/badge/Focus-Monthly_Close_%26_Forecasting-blue)
![Role](https://img.shields.io/badge/Role-Financial_Analyst-orange)
![Scope](https://img.shields.io/badge/Scope-Governance_%2F_Analysis-yellow)

> **Status:** Stable (v1.0)  
> **Change policy:** Content is version-locked. Enhancements or alternate approaches will be demonstrated in subsequent proof packs.

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
This proof pack uses **sample/sanitized** tables and lab-generated evidence to demonstrate methodology without implying access to any employer billing system or production tenant.

- Budget baseline is treated as fixed for the period.
- Forecast is updated monthly using a rolling forecast approach.
- Allocation uses a precedence “waterfall” to reduce unassigned spend.

See:
- [Assumptions](../../00-context/assumptions.md)
- [Scope boundaries](../../00-context/scope-boundaries.md)

---

## Core artifacts (start here)

### 1) Executive summary (one-page)
- [Executive summary](executive-summary.md)

### 2) Financial logic (how decisions are made)
- [Financial logic](financial-logic.md)

### 3) Evidence index (traceability)
- [Evidence index](evidence/evidence-index.md)

### 4) Evidence tables (sample inputs/outputs)
- [Evidence tables](evidence/tables/)

---

## Evidence (real Azure cost data)

This proof pack includes **real Azure Cost Management evidence** captured during a live billing period and retained as traceable artifacts.

### Azure Cost Analysis screenshots
- **Accumulated vs Budget (baseline context)**  
  → [EV-2026-01-005](evidence/screenshots/EV-2026-01-005_azure-cost-analysis_accumulated-vs-budget.png)

- **Group by Service (driver analysis)**  
  → [EV-2026-01-006](evidence/screenshots/EV-2026-01-006_azure-cost-analysis_group-by-service.png)

- **Forecast View (forward-looking risk)**  
  → [EV-2026-01-007](evidence/screenshots/EV-2026-01-007_cost-analysis_forecast-view.png)

### Governance outputs
- **Variance table (sanitized):** [EV-2026-01-001](evidence/tables/sample-variance-table.md)
- **Decision log (sanitized):** [EV-2026-01-008](evidence/tables/sample-decision-log.md)

> **Control outcome**  
> Spend signals → variance classification → decision → retained evidence (auditable chain).

---

## Operating workflow (monthly rhythm)

1. Baseline budget established
2. Actuals reviewed and variance calculated
3. Variance routed by threshold:
   - **Monitor** (≤ 5%)
   - **Investigate** (> 5% and ≤ 10%)
   - **Escalate** (> 10%)
4. Forecast updated when triggers are met
5. Decision logged (approve / re-allocate / reduce / defer)
6. Evidence retained and indexed

---

## Evidence standards (audit-safe)
- All artifacts are linkable and referenced by ID
- Sample data only; no employer billing exports
- Governance behavior is demonstrated, not platform administration

---

## Navigation
- Back to repo: [README](../../README.md)
- Portfolio map: [PORTFOLIO.md](../../PORTFOLIO.md)
