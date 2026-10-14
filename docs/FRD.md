# Functional Requirements Document (FRD)
## ReLoop — Sustainable Business Management Platform

- **Version:** 0.1 — draft
- **Prepared:** 14 October 2026
- **Basis:** Published prototype screenshots and exported CSVs
- **Prototype:** https://sustainable-business-fx6m.bolt.host

## 1. Purpose
Define expected user-visible behavior. Reconcile these draft requirements against source code and executed tests before treating them as final.

## 2. User roles
- Business/operations user (assumed)
- Marketplace listing creator (assumed)
- Dashboard/report viewer (assumed)

Authentication and permissions were not evidenced in the supplied screenshots and remain to be verified.

## 3. Functional requirements
| ID | Module | Requirement | Acceptance criteria |
|---|---|---|---|
| FR-01 | Dashboard | Display total waste, material reused, recycling rate, savings and diversion rate. | KPI value, unit and calculation rule are clear. |
| FR-02 | Dashboard | Show treatment trends and category distribution. | Labels, periods, categories and legend are readable; chart values reconcile. |
| FR-03 | Waste Tracker | Add a material record. | Required fields are validated; valid record appears and dependent metrics update. |
| FR-04 | Waste Tracker | Edit/delete a material record. | Change/removal is reflected consistently in dependent views. |
| FR-05 | Waste Tracker | Search and filter by material/category/treatment. | Results respect query and filters; clearing filters restores the full list. |
| FR-06 | Marketplace | Display and filter surplus-material listings. | Cards show supplied category, description, quantity/unit, condition, location and price. |
| FR-07 | Marketplace | Create listing and initiate a connection request. | Listing validation works; sample listings and simulated connections are labelled. |
| FR-08 | Savings Calculator | Compare disposal, recycling and reuse scenarios. | Outputs update based on quantity and cost assumptions; formula/currency are visible. |
| FR-09 | AI Advisor | Analyze records and provide recommendations. | Demo mode discloses rule-based logic and does not imply a live AI connection. |
| FR-10 | Reports | Switch monthly/yearly views. | Metrics and trends correspond consistently to the selected period. |
| FR-11 | Reports | Export records, summary and trends. | Each export contains expected columns and data for the selected period. |
| FR-12 | Data quality | Handle missing/invalid inputs and empty records. | Clear feedback is shown; invalid values do not silently corrupt KPIs. |
| FR-13 | Transparency | Disclose demo data, assumptions and measured values. | Simulated transactions and illustrative assumptions are visibly distinguished. |
| FR-14 | Consistency | Maintain consistent units and currency. | Conversion rules are explicit; unlike units are not added without conversion. |

## 4. Business rules to validate
- BRL-01: Define eligible records, units and period used for Total Waste.
- BRL-02: Define denominators for reuse/recycling rates and make labels match formulas.
- BRL-03: Define diversion rate, e.g. reused + recycled quantity divided by total eligible waste.
- BRL-04: Avoid double-counting savings; distinguish actual outcomes from scenario estimates.
- BRL-05: Do not aggregate incompatible units without conversion.
- BRL-06: Period comparisons use equivalent date windows and handle periods with no data.
- BRL-07: Simulated marketplace connections are not actual transactions.
- BRL-08: Advisor stays labelled as rule-based demo mode until live integration is configured and tested.

## 5. Proposed non-functional requirements
- Usability: responsive layout, understandable labels and keyboard-accessible forms.
- Reliability: invalid records must not crash dashboard/report views.
- Security/privacy: do not commit secrets; validate inputs; assess access control before using real business data.
- Maintainability: document and test calculations.
- Accessibility: readable contrast, visible focus, labelled inputs and semantic controls.
- Performance: common interactions remain responsive on typical broadband.

## 6. Dependencies and interfaces
- Browser-based interface and CSV export actions.
- Live AI integration is not present in the supplied advisor screenshot; any future integration requires secure server-side secret handling.
- Frontend stack, persistence provider, authentication and backend: pending source-code inspection.

## 7. Open questions
1. Which records are seeded sample data versus user-entered records?
2. Does record data persist after refresh and across devices?
3. Is the intended currency USD, INR or configurable?
4. What exact formulas produce each dashboard KPI and savings figure?
5. Does monthly/yearly selection affect every card/chart/export?
6. What validation and delete-confirmation behavior is implemented?
