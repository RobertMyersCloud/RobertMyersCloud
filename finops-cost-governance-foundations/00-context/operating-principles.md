# Operating Principles (Repo Standards)

![Status](https://img.shields.io/badge/Status-Active-success)
![Focus](https://img.shields.io/badge/Focus-Governance_%26_Decision_Discipline-blue)
![Domain](https://img.shields.io/badge/Domain-IT_Financial_Governance-orange)
![Scope](https://img.shields.io/badge/Scope-Repo_Level_Standard-yellow)

---

## Purpose
Define the operating principles used across this repository. These principles ensure the work is:
- business-first and decision-oriented
- defensible for leadership, finance, and audit review
- repeatable without relying on deep platform administration

---

## Principle 1: Governance over tooling
Cloud cost management is treated as a **financial control domain**, not a tool exercise.

- The objective is consistent decisions, not perfect dashboards.
- The output is a **decision trail**: what changed, why it changed, who approved it, and what evidence supports it.

---

## Principle 2: Evidence before conclusions
Every material conclusion must be supported by linkable evidence artifacts.

- Evidence is indexed and referenced by ID (EV / VC).
- Assertions are avoided when they cannot be traced to an artifact.

---

## Principle 3: Explicit assumptions and scope boundaries
This repository is designed to be recruiter-safe and audit-safe.

- Sample / sanitized data is used where real billing exports are not available.
- Scope boundaries are explicit to avoid implying engineering authority or tenant access.

See:
- [Scope boundaries](scope-boundaries.md)
- [Assumptions](assumptions.md)

---

## Principle 4: Ownership and accountability
Governance requires clear ownership.

- Every review item should map to a **cost owner** and **cost center** (or a defined allocation default).
- “Unallocated” spend is treated as an exception that must be resolved within the next review cycle.

---

## Principle 5: Thresholds trigger action
Variance and exceptions are not “interesting information.” They are triggers for action.

- Monitor / Investigate / Escalate thresholds define the required governance response.
- Investigation produces commentary; escalation produces a decision.

See:
- [Financial logic (Proof Pack 01)](../01-proof-packs/finops-01-budget-variance-governance/financial-logic.md)

---

## Principle 6: Normalize where finance requires it
Financial reporting should reflect consumption patterns, not cash timing.

- Upfront commitments (if present) are normalized for management reporting when available.
- The method used is documented and retained as evidence.

---

## Principle 7: Repeatability over complexity
Frameworks that cannot be repeated do not scale.

- The operating rhythm is designed to run monthly with a consistent package of outputs.
- Templates exist to standardize inputs and reduce ambiguity.

See:
- [Monthly FinOps Close (Operating Rhythm)](../02-operating-models/monthly-finops-close.md)
- [Reporting templates](../03-reporting-templates/)

---

## Navigation
- Repo README: [README](../README.md)
- Portfolio map: [PORTFOLIO.md](../PORTFOLIO.md)
- Proof Pack 01: [Proof Pack 01 README](../01-proof-packs/finops-01-budget-variance-governance/README.md)
