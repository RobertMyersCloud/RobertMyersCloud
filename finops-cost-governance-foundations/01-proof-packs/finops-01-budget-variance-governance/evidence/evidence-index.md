# Proof Pack 01 — Evidence Index (Traceability Register)

![Status](https://img.shields.io/badge/Status-Active-success)
![Focus](https://img.shields.io/badge/Focus-Evidence_%26_Traceability-blue)
![Domain](https://img.shields.io/badge/Domain-IT_Financial_Governance-orange)
![Scope](https://img.shields.io/badge/Scope-Audit_Safe-yellow)

---

## Purpose
Provide an audit-style register of evidence artifacts referenced by **Proof Pack 01**.

Each entry:
- has a unique reference ID (EV / VC)
- links directly to the supporting artifact
- states what governance control or decision it supports

> **Scope note**
> All artifacts are sample or lab-generated. No employer billing exports or production tenant access is implied.

---

## Reference ID conventions

- **EV-YYYY-MM-XXX** — Evidence artifact (tables, screenshots, supporting files)
- **VC-YYYY-MM-XXX** — Variance commentary or decision narrative

---

## Evidence register (sample / sanitized)

| Ref ID | Type | Artifact | What it proves | Location |
|---|---|---|---|---|
| EV-2026-01-001 | EV | Sample variance table (sanitized) | Budget vs actual comparison with variance classification | [sample-variance-table.md](tables/sample-variance-table.md) |
| EV-2026-01-005 | EV | Azure Cost Analysis – Accumulated vs Budget | Baseline budget context and actual spend position vs monthly budget | [EV-2026-01-005](screenshots/EV-2026-01-005_azure-cost-analysis_accumulated-vs-budget.png) |
| EV-2026-01-006 | EV | Azure Cost Analysis – Group by Service | Identification of primary spend drivers by service/category | [EV-2026-01-006](screenshots/EV-2026-01-006_azure-cost-analysis_group-by-service.png) |
| EV-2026-01-007 | EV | Azure Cost Analysis – Forecast View | Forecasted month-end exposure and forward-looking variance risk | [EV-2026-01-007](screenshots/EV-2026-01-007_cost-analysis_forecast-view.png) |
| EV-2026-01-008 | EV | Sample decision log (sanitized) | Conversion of variance signals into accountable governance decisions | [sample-decision-log.md](tables/sample-decision-log.md) |

---

## Variance commentary references (placeholders)

| Ref ID | Type | Artifact | What it supports | Location |
|---|---|---|---|---|
| VC-2026-01-001 | VC | Variance commentary (Compute) | Driver explanation and forecast rationale | (to be created) |
| VC-2026-01-002 | VC | Variance commentary (Storage) | Monitor classification justification | (to be created) |
| VC-2026-01-003 | VC | Variance commentary (Networking) | Escalation rationale and decision | (to be created) |
| VC-2026-01-004 | VC | Variance commentary (Unallocated) | Allocation exception handling | (to be created) |

---

## How this index is used (review standard)

During monthly close, any item classified as **Investigate** or **Escalate** must:
- reference one or more **EV** artifacts
- produce a **VC** commentary or decision
- be traceable end-to-end through this index

> **Control note**
> This index enables independent review of *what changed, why it changed, who decided, and what evidence supports the decision*.

---

## Navigation
- Back to Proof Pack 01: [README](../README.md)
- Financial logic: [financial-logic.md](../financial-logic.md)
- Executive summary: [executive-summary.md](../executive-summary.md)
- Repo README: [README](../../../README.md)
