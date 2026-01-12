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

## Foundational context (how this proof pack should be evaluated)

This proof pack is governed by repository-level standards that define **how evidence is evaluated**, **what claims are allowed**, and **what is intentionally out of scope**.

It should be reviewed as a **financial governance capability demonstration**, not as a technical implementation walkthrough.

### Governing standards
This proof pack explicitly adheres to:
- [Operating principles (repo standards)](../../00-context/operating-principles.md)
- [How to review this repository](../../00-context/how-to-review.md)
- [Data sources (conceptual ownership & cadence)](../../00-context/data-sources.md)
- [Scope boundaries](../../00-context/scope-boundaries.md)
- [Assumptions](../../00-context/assumptions.md)

### Evidence philosophy (important)
This proof pack emphasizes **decision governance**, not tooling screenshots.

What is being demonstrated:
- how variance thresholds trigger action
- how forecasts are adjusted and documented
- how decisions are logged and retained
- how evidence is indexed for traceability

What is intentionally *not* demonstrated in this proof pack:
- live billing exports
- platform configuration screenshots
- enforcement actions inside a tenant

> **Why this matters**
> In real organizations, cost governance failures are rarely caused by missing dashboards.
> They are caused by missing ownership, inconsistent decisions, and lack of retained rationale.
>
> This proof pack demonstrates the **control layer** that must exist *before* tooling screenshots are meaningful.

### Evidence maturity note
Proof Pack 01 represents an early-stage governance control:
- establishes standards
- defines decision logic
- proves review discipline

Subsequent proof packs may introduce:
- tool-generated artifacts
- screenshots
- exports

—but only after governance standards are established.

This sequencing is intentional and reflects how mature FinOps programs are built.

---

## Core artifacts (start here)

### 1) Executive summary (one-page)
Use this if you want the business outcome quickly.
- [Executive summary](executive-summary.md)

### 2) Financial logic (how decisions are made)
Defines variance math, thresholds, forecast triggers, normalization, and allocation waterfall.
- [Financial logic](financial-logic.md)

### 3) Evidence index (traceability)
Audit-style index of artifacts referenced by this proof pack.
- [Evidence index](evidence/evidence-index.md)

### 4) Evidence tables (sample inputs/outputs)
Sanitized tables used to demonstrate what the review pack looks like.
- [Sample variance table](evidence/tables/sample-variance-table.md)
- [Sample decision log](evidence/tables/sample-decision-log.md)

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
