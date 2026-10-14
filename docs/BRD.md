# Business Requirements Document (BRD)
## ReLoop — Sustainable Business Management Platform

- **Version:** 0.1 — draft based on published prototype screenshots and exported CSVs
- **Prepared:** 14 October 2026
- **Status:** Draft for validation
- **Prototype:** https://sustainable-business-fx6m.bolt.host

## 1. Executive summary
ReLoop is a web-based prototype designed to help small and medium-sized businesses review material waste, identify reuse/recycling opportunities, compare illustrative treatment costs and monitor sustainability indicators. Sustainable business and circular economy are treated as one connected operating model: preserve resource value while reducing avoidable waste and cost.

## 2. Business problem
Businesses may keep material records inconsistently, lack a consolidated view of categories and treatment outcomes, and find it difficult to compare disposal against reuse or recycling alternatives. This makes it harder to identify opportunities to preserve material value and reduce avoidable expenditure.

## 3. Business objectives
- Consolidate material and treatment records in one interface.
- Make waste, reuse, recycling and diversion indicators visible.
- Compare disposal, recycling and reuse scenarios using transparent assumptions.
- Help users discover potential surplus-material reuse opportunities.
- Provide summary and trend views/exports for review.

## 4. Stakeholders and users
- Primary: small-business owner or sustainability/operations manager.
- Secondary: operations/facilities staff recording material details.
- Potential marketplace participant: business listing or sourcing surplus material.
- Project stakeholders: product owner/project lead and tester.

## 5. Scope
### In scope in the visible prototype
- Sustainability dashboard and visual summaries.
- Material/waste record management interface.
- Search and filters.
- Circular materials marketplace with demo listings.
- Savings calculator for hypothetical quantities and cost assumptions.
- Rule-based AI Advisor demo mode.
- Sustainability report views and export controls.

### Out of scope unless implemented and verified
- Verified carbon/environmental accounting.
- Real payments, logistics, contracts or marketplace transactions.
- Live AI model integration.
- Regulatory certification or assurance.
- Enterprise access controls, audit trails and multi-tenant security.
- Guaranteed savings or environmental outcomes.

## 6. Business requirements
| ID | Requirement | Priority |
|---|---|---|
| BR-01 | Provide a consolidated view of material waste and treatment outcomes. | Must |
| BR-02 | Let users maintain material records with category, quantity, date, treatment and cost information. | Must |
| BR-03 | Compare disposal, recycling and reuse scenarios using transparent assumptions. | Must |
| BR-04 | Present potential surplus materials for reuse by other businesses. | Should |
| BR-05 | Provide data-based recommendations while disclosing whether advice is rule-based or AI-generated. | Should |
| BR-06 | Provide period-based sustainability summaries and exportable data. | Must |
| BR-07 | Distinguish sample/demo data from user-generated records and real transactions. | Must |
| BR-08 | Use consistent units and identify the currency used in calculations. | Must |

## 7. Proposed success measures (not yet measured)
- Users can add, find, edit and delete material records without assistance.
- Dashboard totals reconcile with eligible source records and documented formulas.
- Savings scenarios show inputs, assumptions and reproducible calculations.
- Report exports contain expected columns and the chosen reporting period.
- Demo listings and simulated connections are clearly labelled.
- The report/advisor helps a user identify a plausible reuse or recycling action.

## 8. Assumptions and dependencies
- Screenshots and supplied CSV exports describe the prototype as observed on 14 October 2026.
- Sample data is not proof of real operations.
- Actual savings depend on local treatment prices, material quality, transport and operational constraints.
- Source code and backend behavior still require inspection.

## 9. Risks and constraints
- Misleading KPIs if denominators, units, dates or formulas are inconsistent.
- Misleading comparisons if cost assumptions are hidden or outdated.
- Marketplace users might confuse demo listings with actual offers.
- No live AI integration is indicated in the visible advisor screen.
- Persistence, privacy and security cannot be fully assessed from screenshots alone.

## 10. Approvals
Business/Product Owner: Pending | Technical review: Pending | Test sign-off: Pending
