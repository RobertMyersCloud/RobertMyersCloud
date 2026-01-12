# Data Sources (Conceptual) — Ownership, Cadence, and Controls

![Status](https://img.shields.io/badge/Status-Active-success)
![Focus](https://img.shields.io/badge/Focus-Inputs_%26_Data_Ownership-blue)
![Domain](https://img.shields.io/badge/Domain-IT_Financial_Governance-orange)
![Scope](https://img.shields.io/badge/Scope-Conceptual_(No_Platform_Admin)-yellow)

---

## Purpose
Document the conceptual data inputs required to run this repository’s FinOps governance workflows. This is written to clarify:
- what data is needed (inputs)
- who typically owns it (ownership)
- how often it is refreshed (cadence)
- what control checks ensure it is usable for review

> **Scope note**
> This document describes **conceptual** data responsibilities. It does not imply access to any employer billing system or production tenant.

---

## Data inputs required (high level)

| Data input | What it is used for | Typical owner | Cadence |
|---|---|---|---|
| Budget baseline | Budget vs actual variance calculation | Finance / IT Finance | Monthly (baseline set) |
| Actual spend (period-to-date) | Variance measurement and trend tracking | FinOps / Cloud Finance | Daily / Weekly |
| Forecast (rolling) | Month-end projection and decision support | FinOps / IT Finance | Weekly (or when triggers met) |
| Allocation mappings | Assign spend to cost centers / owners | Finance + FinOps | Monthly (or as org changes) |
| Tag / allocation coverage | Identify unallocated or misallocated spend | FinOps / Governance | Weekly / Monthly |
| Commitment records (if applicable) | Normalized cost view for management reporting | FinOps / Finance | Monthly (during close) |

---

## Conceptual source definitions (what “counts” as a source)
This repo does not require a specific vendor export format to demonstrate governance logic. Conceptually, each input can come from:

- **Budget baseline:** budget plan or approved monthly allocation sheet
- **Actual spend:** billing summary, cost management export, or invoice detail extract
- **Forecast:** maintained forecast worksheet or forecasting report
- **Allocation mappings:** cost center directory, subscription-to-owner mapping, or chargeback map
- **Tag / coverage:** allocation coverage report or governance exception list
- **Commitments:** reservation/savings plan record or equivalent commitment schedule

---

## Ownership model (RACI-style, simplified)

| Activity | Finance | FinOps / IT Finance | Cost Owner (Service/Team) |
|---|---|---|---|
| Set baseline budget | **A/R** | C | I |
| Provide actual spend inputs | I | **A/R** | I |
| Produce rolling forecast | C | **A/R** | C |
| Explain variance drivers | I | C | **A/R** |
| Decide action (approve / re-allocate / reduce / defer) | **A** | **R** | C |
| Maintain allocation mappings | **A/R** | C | I |
| Resolve unallocated exceptions | I | **R** | **A/R** (as assigned) |
| Retain evidence + index | C | **A/R** | I |

Legend:
- **A** = Accountable
- **R** = Responsible
- **C** = Consulted
- **I** = Informed

---

## Cadence (operating rhythm alignment)
This repository assumes a practical cadence aligned to a monthly close.

### Daily / Weekly (lightweight)
- Review spend trend vs baseline (spot anomalies early)
- Flag allocation gaps (Unallocated growth, missing cost owner mapping)

### Monthly (close package)
- Finalize budget vs actual variance
- Update rolling forecast and note rationale if changed
- Produce allocation exception list (including Unallocated)
- Log decisions and retain evidence references

See:
- [Monthly FinOps Close (Operating Rhythm)](../02-operating-models/monthly-finops-close.md)

---

## Control checks (data quality expectations)
To keep decisions defensible, the following checks are expected before review:

1. **Completeness:** All spend for the period is represented (no missing categories/services).
2. **Allocation coverage:** Unallocated is measurable and tracked; exceptions are visible.
3. **Consistency:** Budget, actual, and forecast use the same period definition.
4. **Normalization note (if applicable):** If commitments are normalized, the method is documented.
5. **Traceability:** Any reviewed variance item can be linked to an EV/VC reference.

Evidence linkage standard:
- [Evidence index (Proof Pack 01)](../01-proof-packs/finops-01-budget-variance-governance/evidence/evidence-index.md)

---

## Navigation
- Repo README: [README](../README.md)
- Operating principles: [Operating principles](operating-principles.md)
- Maturity positioning: [Maturity positioning](maturity-positioning.md)
- Proof Pack 01: [Proof Pack 01 README](../01-proof-packs/finops-01-budget-variance-governance/README.md)
- Portfolio map: [PORTFOLIO.md](../PORTFOLIO.md)
