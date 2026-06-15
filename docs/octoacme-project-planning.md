# OctoAcme — Project Planning

## Purpose
Turn an approved initiative into an actionable plan and backlog for delivery.

## Objectives
- Break work into shippable increments
- Identify dependencies and risks
- Align timelines, releases, and responsibilities
- Define clear acceptance criteria and quality standards

## Activities
1. Kickoff meeting with stakeholders and delivery team
2. Create prioritized backlog with acceptance criteria
3. Estimate scope (T-shirt sizing or story points)
4. Define Definition of Done (DoD)
5. Identify dependencies and integration points
6. Create release plan and milestone map
7. Identify team roles and responsibilities (including specialized roles)
8. Plan instrumentation and metrics collection (with Data Analyst)

## Backlog Item Template
- Title:
- Description:
- Acceptance criteria:
- Priority:
- Estimate:
- Owner:
- Related docs/links:
- Dependencies (if any):
- Roles involved (e.g., UX Researcher, Security Engineer):

## Sprint / Iteration Planning
- Timebox planning to agreed sprint length
- Pull items that meet DoD and have clear acceptance criteria
- Ensure team capacity is respected
- Include specialized roles as needed (Tech Lead, UX Researcher, Security Engineer)
- Reserve capacity for technical debt and refactoring

## Definition of Done (DoD)

A backlog item is Done when:
- [ ] Code is implemented and peer-reviewed
- [ ] Unit tests written and passing (minimum 80% coverage for new code)
- [ ] Acceptance criteria verified by QA or Product Manager
- [ ] Technical documentation updated (README, API docs, runbooks)
- [ ] Security scanning passed (SAST, dependency checks)
- [ ] Usability validated by UX Researcher (if applicable)
- [ ] Metrics/instrumentation implemented and verified
- [ ] PR merged and deployed to staging
- [ ] Tech Lead approved architectural changes
- [ ] No open security findings or mitigations documented
- [ ] Ready for release (in the Release plan)

### Definition of Done Variations
Teams may adjust DoD based on risk and complexity:
- **High-risk items** (security, customer-facing): Add security code review, extended QA, customer validation
- **Infrastructure items**: Add monitoring/alerting, runbook documentation, rollback testing
- **User-facing items**: Add usability testing, accessibility review, translation readiness

## Risk & Dependency Management
- Capture in Risk Register:
  - ID, Description, Impact, Probability, Owner, Mitigation
- Mark cross-team dependencies in the project board and escalate during weekly syncs
- **Identify integration points**: APIs, data formats, deployment order
- **Identify resource constraints**: Specialized skills, infrastructure, tool access
- **Plan for dependencies**: Coordinate timelines, define handoff criteria

### Dependency Checklist
- [ ] All cross-team dependencies identified and documented
- [ ] Dependent teams notified and aligned on timelines
- [ ] Integration points and interfaces defined
- [ ] Testing plan includes integration testing
- [ ] Rollback plan considers dependent systems
- [ ] Escalation path clear if dependency is delayed

## Planning Checklist
- [ ] Project kickoff held (all stakeholders present)
- [ ] Backlog prioritized and estimated
- [ ] Release timeline and milestones agreed
- [ ] Definition of Done documented and agreed
- [ ] Initial test plan / QA approach drafted
- [ ] Team roles assigned (including specialized roles as needed)
- [ ] Success metrics and instrumentation planned (with Data Analyst)
- [ ] Risk register created (initial version)
- [ ] Dependency map created and shared
- [ ] Communication plan defined (stakeholders, frequency, format)
- [ ] Decision log started (track major decisions and rationale)
