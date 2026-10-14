# ReLoop — Sustainable Business Management Platform

**Live demo:** https://sustainable-business-fx6m.bolt.host

ReLoop is an AI-assisted prototype exploring how businesses can track material waste, identify reuse opportunities, compare treatment-cost scenarios and review sustainability indicators. It treats sustainable business and circular economy as one integrated business problem: retaining material value while reducing waste and avoidable costs.

> **Project status:** Published prototype. Values include sample/demo data and are not independently verified business outcomes. The AI Advisor is in rule-based demo mode, and marketplace connections are simulated.

## Features
- Dashboard for waste, reuse, recycling, diversion, savings and material trends
- Waste Tracker with search/filter and add/edit/delete controls
- Circular Materials Marketplace with demo listings
- Savings Calculator with illustrative assumptions
- AI Business Advisor with rule-based recommendations (not live AI)
- Sustainability Reports with period views and CSV export controls

## Documentation
- [BRD](docs/BRD.md) — business problem, objectives, scope and success measures
- [FRD](docs/FRD.md) — functional requirements and business rules
- [RTM](docs/RTM.csv) — requirements traceability matrix
- [Agile workflow](docs/AGILE_WORKFLOW.md) — workflow, backlog and proposed sprints
- [Test plan](docs/TEST_PLAN.md) — test approach and exit criteria
- [Process flows](docs/PROCESS_FLOWS.md) — key user journeys
- [Test cases](tests/test_cases.csv) and [defect log template](tests/defect_log_template.csv)

## Validation items
1. Verify dashboard KPIs against source records and formula definitions.
2. Confirm units and currency are consistent across the dashboard, calculator and reports.
3. Verify whether records persist after refresh and across sessions.
4. Test record management, filters, scenario calculations and CSV exports.
5. Keep demo listings and simulated connections clearly disclosed.
6. Source code, backend, authentication and deployment configuration have not yet been inspected in this repository.

## Repository status
This repository holds project documentation and test artifacts. Add the application source exported from Bolt separately; never commit `.env` files, API keys or credentials.

## Workflow
Track features and defects with GitHub Issues. Use **Backlog → Ready → In Progress → Review → Testing → Done**. Mark work Done only after acceptance criteria and test evidence are recorded.

## Resume guidance
Describe this as an AI-assisted prototype and product/business analysis documentation project. Claim completed testing, verified savings, production readiness or live AI only when supported by evidence.
