# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies
- Weekly delivery sync — show progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone
- Cross-team sync (when needed) — coordinate dependencies with other teams

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review
  - Require at least one approval before merging (or team-defined policy)
  - Request review from Tech Lead for significant architectural changes

## Quality & Testing
- Unit tests for new logic
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- Security scanning in CI (SAST, dependency scanning)
- Manual QA for feature acceptance when needed
- Usability testing by UX Researcher when applicable

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage)
- Review metrics weekly with Data Analyst
- Communicate progress in weekly status updates

## Blocker Escalation
- Level 1: Team-level triage in daily standup
  - Delivery Lead owns unblocking within 24 hours
  - Ask: Who owns this? What resources are needed?
- Level 2: PM escalates to Product Lead and dependent teams
  - Coordinate cross-team dependencies
  - Adjust priorities or timelines if needed
- Level 3: Sponsor-level escalation for business-impacting issues
  - Follows Risk Management escalation path
  - Includes mitigation plan and timeline

## Cross-Team Coordination
When work depends on other teams:
- **Identify dependencies early** — during Planning phase
- **Mark dependencies in project board** — use labels or custom fields
- **Communicate status weekly** — include dependent teams in syncs
- **Adjust timelines collaboratively** — avoid surprises
- **Escalate delays immediately** — don't wait for weekly sync

### Dependency Checklist
- [ ] Dependencies identified and documented in backlog items
- [ ] Dependent teams notified and aligned on timelines
- [ ] Integration points defined (APIs, data formats, interfaces)
- [ ] Testing plan includes integration testing with dependencies
- [ ] Rollback plan considers dependent systems
- [ ] Weekly sync includes dependent team representatives

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests, lint, and security scanning
- [ ] Regular demos scheduled with stakeholders
- [ ] Risk register updated weekly
- [ ] Project board actively maintained (columns, labels, assignments)
- [ ] Metrics dashboard created and monitored
- [ ] Cross-team dependencies tracked and communicated
- [ ] Delivery Lead assigned to manage day-to-day execution
