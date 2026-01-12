# Proof Pack 01 — Evidence Index (Traceability Register)

![Status](https://img.shields.io/badge/Status-Active-success)
![Focus](https://img.shields.io/badge/Focus-Evidence_%26_Traceability-blue)
![Domain](https://img.shields.io/badge/Domain-IT_Financial_Governance-orange)
![Scope](https://img.shields.io/badge/Scope-Audit_Ready_Index-yellow)

---

## Purpose
Provide an audit-style register of evidence artifacts referenced by **Proof Pack 01**. Each entry:
- has a unique reference ID (EV = evidence artifact, VC = variance commentary)
- links to the exact artifact location
- states what it supports and how it is used in governance review

> **Scope note**
> This proof pack uses sample/sanitized artifacts. No entries imply access to an employer billing system or production tenant.

---

## Reference ID conventions
- **EV-YYYY-MM-###** = Evidence artifact (table, screenshot, export, supporting file)
- **VC-YYYY-MM-###** = Variance commentary (narrative record tied to a variance item)

---

## Evidence register (sample / sanitized)

| Ref ID | Type | Artifact | What it supports | Location |
|---|---|---|---|---|
| EV-2026-01-001 | EV | Variance table row (Compute) | Investigate classification + forecast view for monthly close | [Sample variance table](tables/sample-variance-table.md) |
| EV-2026-01-002 | EV | Variance table row (Storage) | Monitor classification + trend tracking | [Sample variance table](tables/sample-variance-table.md) |
| EV-2026-01-003 | EV | Variance table row (Networking) | Escalate classification + decision requirement | [Sample variance table](tables/sample-variance-table.md) |
| EV-2026-01-004 | EV | Variance table row (Unallocated) | Allocation exception handling + escalation trigger | [Sample variance table](tables/sample-variance-table.md) |
| VC-2026-01-001 | VC | Variance commentary (placeholder) | Driver + impact horizon for Investigate item | (To be created) |
| VC-2026-01-002 | VC | Variance commentary (placeholder) | Rationale for Monitor item (optional) | (To be created) |
| VC-2026-01-003 | VC | Variance commentary (placeholder) | Driver + recommendation + decision for Escalate item | (To be created) |
| VC-2026-01-004 | VC | Variance commentary (placeholder) | Root cause + allocation resolution plan for Unallocated exception | (To be created) |

---

## How this index is used (review standard)
During monthly close, any item classified as **Investigate** or **Escalate** must:
- reference a **VC-** entry for narrative rationale, and
- reference an **EV-** entry for supporting evidence

> **Control note**
> The index exists to prove the decision trail is repeatable and reviewable: what changed, why it changed, and what evidence supports the conclusion.

---

## Navigation
- Back to Proof Pack 01: [README](../README.md)
- Executive summary: [Executive summary](../executive-summary.md)
- Financial logic: [Financial logic](../financial-logic.md)
- Evidence tables: [Evidence tables](tables/)
- Repo README: [README](../../../README.md)
