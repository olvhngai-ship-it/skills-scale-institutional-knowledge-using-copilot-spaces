# OctoAcme Project Management Docs

A single landing page for teammates and stakeholders to quickly find and understand the project management processes used across OctoAcme.

## Summary of Project Management Processes

OctoAcme follows a structured, lifecycle-based approach to project delivery that emphasizes customer value, iterative execution, and clear ownership. The framework spans five phases: **Initiation**, **Planning**, **Execution**, **Release**, and **Close & Retrospective**. In the Initiation phase, teams validate business needs by creating a lightweight One-pager that defines the problem statement, measurable success metrics, stakeholders, and initial timeline. This serves as a decision gate—work only moves to planning once success metrics are clear, stakeholders align on priority, and team availability is confirmed. The Planning phase transforms the approved initiative into an actionable backlog, with work broken into shippable increments, prioritized with clear acceptance criteria, and mapped against dependencies and release milestones. This structured front-end planning reduces rework and establishes a shared understanding of scope.

Execution and delivery are coordinated through a consistent rhythm of standups, syncs, and retrospectives. Teams conduct daily 15-minute standups to surface progress and blockers, hold weekly delivery syncs to review milestones and flagged risks, and use GitHub Projects to manage workflow through columns (Backlog → Ready → In Progress → In Review → QA → Done). Pull requests are kept small (≤400 lines when possible), include issue links and acceptance criteria, and require at least one approval before merging. Quality assurance is woven throughout: unit tests for new logic, integration tests where applicable, end-to-end smoke tests for critical flows, security scanning in CI, and manual QA for feature acceptance. Teams track velocity, burndown, and success metrics from the One-pager via dashboards to remain data-informed and responsive to emerging risks.

OctoAcme defines clear roles to avoid ambiguity: **Project Managers** coordinate delivery, schedules, risks, and communications; **Product Managers** define outcomes, prioritize the backlog, and measure impact; **Developers** implement features and collaborate on design and testability; and **Stakeholders** provide inputs and approvals. Communication is multi-tiered and transparent. Weekly syncs align PM and Product Lead, twice-weekly standups keep the delivery team synchronized, monthly stakeholder updates provide visibility, and a three-level escalation path (team → PM → Product Lead → Sponsor) ensures blockers surface quickly. Risk management is continuous: teams maintain a Risk Register throughout the project, identify risks during planning and execution, assess impact and likelihood, document mitigation plans, and review status at weekly syncs. This combination of clear roles, lightweight artifacts, data-informed decision-making, and structured communication enables OctoAcme to deliver reliably while maintaining psychological safety and a culture of continuous improvement.

## Process Documents

- [Project Management Overview](octoacme-project-management-overview.md) — Concise introduction to OctoAcme's approach, roles, key artifacts, and lifecycle.
- [Project Initiation Guide](octoacme-project-initiation.md) — Steps to validate business need, align stakeholders, and create a lightweight plan.
- [Project Planning](octoacme-project-planning.md) — How to break work into shippable increments, identify dependencies, and align timelines.
- [Execution & Tracking](octoacme-execution-and-tracking.md) — Day-to-day execution guidance, team rhythm, pull request workflow, and quality practices.
- [Release & Deployment Guide](octoacme-release-and-deployment.md) — Standardized process for releasing features to production and managing rollbacks.
- [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md) — How to capture learnings and convert them into actionable improvements.
- [Risk Management & Communication](octoacme-risks-and-communication.md) — Risk register maintenance, communication strategies, and escalation paths.
- [Roles & Personas](octoacme-roles-and-personas.md) — Definitions of typical roles and responsibilities in OctoAcme projects.

## How to Use

- **New to OctoAcme?** Start here, then dive into the [Project Management Overview](octoacme-project-management-overview.md).
- **Starting a new project?** Follow the [Project Initiation Guide](octoacme-project-initiation.md) and [Project Planning](octoacme-project-planning.md).
- **Managing execution?** Reference [Execution & Tracking](octoacme-execution-and-tracking.md) and [Risk Management & Communication](octoacme-risks-and-communication.md).
- **Ready to release?** Follow the [Release & Deployment Guide](octoacme-release-and-deployment.md).
- **Wrapping up?** Use the [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md) guide to capture learnings.

## Maintaining These Docs

Use the [Add Content to Project Management Process Docs](../.github/ISSUE_TEMPLATE/add-update-content-to-process-docs.yml) issue template to propose updates or additions to these process documents.
