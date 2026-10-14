# Test Plan — ReLoop

## Objective
Validate primary user flows, calculation transparency, data consistency and demo-data disclosures.

## Scope
Dashboard, waste tracker, marketplace, savings calculator, AI Advisor demo mode, reports and CSV exports.

## Approach
- Manually test primary flows on the published prototype.
- Test invalid/boundary inputs in forms and calculator.
- Reconcile dashboard KPIs with exports and written formula rules.
- Inspect downloaded CSV headers, row counts and date ranges.
- Check responsive layout and keyboard accessibility.
- Record each result as Not Run, Pass, Fail or Blocked. Never mark Pass before execution.

## Entry criteria
Prototype accessible; test records identified; browser downloads enabled.

## Proposed exit criteria
All Must-priority cases executed; no unresolved critical defect; failures logged; KPI formulas, currency and unit policies documented.

## Risks
- Exported summary metrics may need formula clarification.
- Records may mix units; direct summation may be invalid.
- Savings may depend on assumed rates rather than actual costs.
- Persistence behavior has not been verified.
