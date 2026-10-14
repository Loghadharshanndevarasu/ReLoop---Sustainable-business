# Agile Workflow — ReLoop

## Working approach
Use a lightweight Scrum-inspired planning cycle and a Kanban board for daily visibility. The sprint plan below is proposed and does not claim these sprints have already occurred.

## Workflow
**Backlog → Ready → In Progress → Review → Testing → Done**

Move a card to Done only when acceptance criteria are met, tests have been executed, and evidence/notes are attached. Record a blocker note for blocked work.

## Suggested roles
- Product Owner: prioritizes value and accepts stories.
- Builder/Developer: implements and documents features.
- Tester: executes test cases and records outcomes.
- Stakeholder: reviews usability and validates assumptions.
For a solo project, one person may perform multiple roles; state that transparently.

## Definition of Ready
- User story states user, need and value.
- Acceptance criteria are testable.
- Assumptions and dependencies are identified.
- Story is small enough for a sprint.

## Definition of Done
- Acceptance criteria are met.
- Happy path, invalid-input path and relevant empty state are tested.
- No unresolved critical defect remains.
- Documentation and RTM are updated.
- Demo data and limitations are disclosed.
- Test evidence is recorded.

## Proposed product backlog
| ID | User story | Priority | Acceptance criteria summary |
|---|---|---|---|
| US-01 | As a manager, I want sustainability KPIs to understand performance. | Must | Values, units and formulas are clear and reconcile. |
| US-02 | As an operations user, I want to maintain waste records. | Must | Add/edit/delete and validation behave correctly. |
| US-03 | As an operations user, I want search and filters to find records. | Must | Search/filter combinations work and can be cleared. |
| US-04 | As a manager, I want to compare treatment costs. | Must | Outputs update using documented assumptions. |
| US-05 | As a business, I want to list surplus materials for reuse. | Should | Required details validate; demo status is clear. |
| US-06 | As a sourcing user, I want to find surplus materials. | Should | Search and filters return expected listings. |
| US-07 | As a manager, I want recommendations based on records. | Should | Advice explains data patterns and discloses rule-based demo mode. |
| US-08 | As a manager, I want period reports and exports. | Must | Views and exports match the selected period. |
| US-09 | As a reviewer, I want requirements linked to tests. | Must | Each requirement maps to relevant test cases. |
| US-10 | As a portfolio reviewer, I want setup and project documentation. | Should | README describes verified state and limitations. |

## Proposed sprint plan
### Sprint 1 — Data visibility and record management
Goal: validate KPI definitions and core waste-record flows. Candidate stories: US-01, US-02, US-03, US-09. Deliverables: KPI definitions, record workflow evidence and updated RTM.

### Sprint 2 — Circular value and decision support
Goal: test reuse discovery and transparent scenario comparisons. Candidate stories: US-04, US-05, US-06. Deliverables: calculator arithmetic checks, listing workflow evidence and documented limitations.

### Sprint 3 — Recommendations, reporting and portfolio readiness
Goal: verify advisor transparency, exports and end-to-end consistency. Candidate stories: US-07, US-08, US-10. Deliverables: export checks, advisor tests and portfolio walkthrough.

## Ceremonies
- Sprint Planning: set a Sprint Goal and select work based on capacity.
- Daily check-in: record progress, next steps and blockers.
- Sprint Review: demonstrate completed behavior and gather feedback.
- Retrospective: record what worked, what did not and one improvement for next cycle.

## Suggested GitHub setup
Labels: `type:feature`, `type:bug`, `type:documentation`, `priority:must`, `priority:should`, `status:blocked`. Use GitHub Issues for stories/defects and Projects for the board. Close issues only when acceptance criteria and test evidence are recorded.
