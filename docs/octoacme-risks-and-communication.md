# OctoAcme — Risk Management & Communication

## Purpose
Explain how to identify, manage, and communicate risks and dependencies.

## Risk Register
Maintain a simple table with:
- ID
- Description
- Impact (High/Med/Low)
- Likelihood (High/Med/Low)
- Owner
- Mitigation plan
- Status

Review and update the Risk Register weekly during delivery syncs.

## Risk Lifecycle
- Identify: during planning and ongoing execution
- Assess: estimate impact and likelihood
- Mitigate: reduced via actions, contingency plans
- Monitor: review at weekly syncs and update status
- Resolve or Accept: document outcome and learnings

## Stakeholder Communication

### Identify Stakeholder Groups
Common stakeholder groups include:
- **Engineering/Delivery Team** — daily standups, sprint planning, PRs
- **Product & Leadership** — weekly syncs, roadmap updates, milestone reviews
- **Support & Customer Success** — impacts, workarounds, customer communications
- **Security & Compliance** — threat models, scanning results, audit trails
- **Dependent Teams** — dependency status, integration points, handoff dates
- **Customers/End Users** — release notes, feature availability, migration guidance

### Communication Strategy
- Identify stakeholder groups and communication needs
- Provide regular updates (weekly or milestone-based)
- Use a single source of truth (project README or release doc) for status
- Tailor messages to audience (technical vs. business language)
- Include "ask" or decision needed in each communication

## Communication Templates

### Weekly Status Template
```
Project: [Project Name]
Week of: [Date]
Owner: [Project Manager]

## Progress This Week
- [Completed milestone or deliverable]
- [Completed milestone or deliverable]
- [In-progress work summary]

## Next Steps
- [Planned work for next week]
- [Planned work for next week]
- [Key milestones in next 2 weeks]

## Risks & Blockers
- [Risk/Blocker]: [Impact] | [Mitigation plan] | [Owner]
- [Risk/Blocker]: [Impact] | [Mitigation plan] | [Owner]

## Metrics & Health
- Velocity: [Current] vs. [Planned]
- Success Metrics: [Key metric] is [On track / At risk / Off track]
- Quality: [Test coverage / Defect trend]

## Ask / Decisions Needed
- [Decision needed]: [Options / Context] by [Date]
- [Ask for help]: [Support needed] by [Date]
```

### Stakeholder Communication Matrix

| Stakeholder | Frequency | Content | Owner | Format |
|---|---|---|---|---|
| Engineering Team | Daily | Standups, blockers, PRs | Delivery Lead | Sync + Slack |
| Product & Leadership | Weekly | Progress, metrics, risks | Project Manager | Email + Meeting |
| Support & CS | Weekly or As-Needed | Customer impacts, workarounds | PM + CS Liaison | Email + Slack |
| Security | Per-Release | Scanning results, threat models | Security Engineer | Report + Review |
| Dependent Teams | Weekly | Status, integration points | PM + Delivery Lead | Sync + Updates |
| Customers | Per-Release | Release notes, impacts, migration | CS Liaison | Email + Release Notes |

### Incident Communication
- **Triage summary**: What happened, who is affected, severity level
- **Actions being taken**: Current response, expected timeline
- **Expected timeline**: When will it be resolved
- **Post-incident blameless retrospective**: Root cause, action items, timeline

### Release Communication
- **Release notes**: What's new, improvements, fixes, known issues
- **Customer impacts**: Who is affected, behavior changes, deprecations
- **Migration guidance**: Any required manual steps or configuration changes
- **Support readiness**: FAQ, known issues, escalation path

## Escalation Paths

### Standard Escalation (Non-Security)
1. **Team Level**: Daily standup or Delivery Lead
   - Blockers that can be resolved within team
   - Ask: Who can help? What resources needed?
   - Resolution target: 24 hours

2. **Project Level**: PM escalates to Product Lead and dependent teams
   - Blockers requiring cross-team coordination
   - Timeline impacts or scope trade-offs
   - Resource constraints
   - Resolution target: 2–3 business days

3. **Leadership/Sponsor Level**: Escalate for business-impacting issues
   - Critical delays affecting release date
   - High-risk decisions (go/no-go)
   - Significant scope changes
   - Include: context, options, recommendation

### Security Escalation
- **Critical findings**: Notify Security on-call immediately
- **Follow security incident runbook**: Security team owns response
- **Post-incident review**: Include team and process owners
- **Remediation tracking**: Security Engineer owns follow-up

## Risk Communication

Include risks in weekly status updates:
- **Identified risks**: New risks discovered this week
- **Risk status**: Track progress on mitigations
- **Resolved risks**: Document learnings and remove from register
- **Risk trends**: Highlight increasing or decreasing overall risk

Example risk communication:
```
RISK: Integration with dependent service not finalized
IMPACT: High (blocks QA testing)
MITIGATION: Daily sync with dependent team; alternative mock API ready
OWNER: Tech Lead
STATUS: In Progress (API spec due Friday)
```
