# Financial Logic: Budget Variance, Forecasting, and Cost Normalization

This document defines the financial logic used in **Proof Pack 01**. It is written to be auditable, repeatable, and business-first.

> **Scope note**
> This is a governance and analysis framework. It does not imply production access, engineering authority, or the ability to enforce technical actions.

---

## 1) Core variance calculation (Budget vs Actual)

**Monthly variance ($):**  
`VarianceUSD = ActualSpend - BudgetedSpend`

**Monthly variance (%):**  
`VariancePct = (ActualSpend - BudgetedSpend) / BudgetedSpend`

### Thresholds and required actions (governance triggers)

| Variance band (vs budget) | Status | Required governance action |
|---:|---|---|
| ≤ 5% | Monitor | Optional commentary; track trend. |
| > 5% and ≤ 10% | Investigate | Commentary required (driver + impact horizon). |
| > 10% | Escalate | Commentary + decision required (approve / re-allocate / reduce / defer) with evidence references. |

**Output artifact:** Variance table and commentary reference IDs  
- See: [Evidence index](evidence/evidence-index.md)

---

## 2) Cost normalization (upfront commitments)

Cloud costs can include **upfront commitments** (e.g., reservations or savings plans) that create a cash spike. For **management reporting** and variance analysis, spend can be normalized to avoid misleading month-to-month variance.

**Example (illustrative):**
- Upfront payment: $12,000  
- Term: 12 months  
- Normalized monthly view: $1,000 per month  

> **Policy (for this framework)**
> Variance reporting uses a **normalized / amortized view** for commitments when available, so budget performance reflects consumption patterns rather than one-time payment timing.

**Evidence expectation (when implemented with real data):**
- Retain the commitment record and the normalization method used (inputs + outputs).

---

## 3) Forecast adjustment logic (rolling forecast)

Budgets are typically set annually; forecasts are updated on a rolling basis.

**Simple rolling forecast (illustrative):**  
`NewForecast = (AvgDailySpend * RemainingDaysInMonth) + MonthToDateSpend`

### Forecast update triggers (governance)

A forecast update is required when one of the following occurs:
- Current forecast exceeds baseline budget by **> 10%** and the condition persists for **3 consecutive days**, or
- A known scope change is approved (new workload, new environment, contract change), or
- Allocation changes materially shift costs between owners or cost centers.

**Output artifact:** Forecast note / commentary (business rationale + date + owner)  
- Recommended template: [Variance commentary template](../../03-reporting-templates/variance-commentary-template.md)

---

## 4) Cost allocation waterfall (ensure 100% allocation)

Allocation is applied in order of precedence to minimize “unassigned” spend.

1. **Direct attribution:** Resource-level assignment (e.g., `CostCenter`).
2. **Group inheritance:** Resource group-level assignment.
3. **Subscription default mapping:** Subscription-to-owner or cost center mapping.
4. **Unallocated bucket:** Any remainder assigned to a shared or central bucket for follow-up.

> **Control note**
> Any spend landing in **Unallocated** is a governance exception that requires investigation and resolution within the next review cycle.

**Output artifact:** Allocation exception list (count, $ amount, owners impacted)  
- Evidence reference should be recorded in the [Evidence index](evidence/evidence-index.md)

---

## 5) Decision logging standard (what “good” looks like)

For any item in **Investigate** or **Escalate**:
- State the driver (scope / usage / rate / allocation)
- State whether it is one-time or recurring
- Provide a recommendation (approve / re-allocate / reduce / defer)
- Reference evidence IDs that support the conclusion

Recommended output format:
- [Exec brief one-pager](../../03-reporting-templates/exec-brief-onepager.md)
