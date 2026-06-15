# OctoAcme — Cross-Team Coordination

## Purpose
Provide guidance for managing dependencies, coordinating handoffs, and ensuring alignment across teams working on related projects or features.

## When Cross-Team Coordination Is Needed
- Features depend on APIs or services from another team
- Work requires shared infrastructure or resources
- Release coordination is required (one team must ship before another)
- Multiple teams contribute to the same user-facing feature
- Data or integration points require synchronization

## Dependency Identification

### Types of Dependencies
1. **Technical Dependencies**: Code, APIs, libraries, infrastructure
2. **Data Dependencies**: Shared data models, analytics, integration formats
3. **Temporal Dependencies**: One feature must ship before another
4. **Resource Dependencies**: Shared people, infrastructure, tools
5. **Process Dependencies**: Security reviews, compliance approval, legal review

### Dependency Documentation
For each dependency, document:
- **Description**: What is needed and why
- **Dependent Team(s)**: Who owns the dependency
- **Integration Point**: How teams will integrate (API, data format, event, etc.)
- **Timeline**: When is it needed (date, milestone)
- **Success Criteria**: How will we know it's ready
- **Backup Plan**: What if dependency is delayed

## Coordination Rhythm

### Dependency Identification (Planning Phase)
- Identify dependencies during project planning
- **Notify dependent teams immediately** — don't wait for weekly syncs
- Document integration points and APIs early
- Schedule initial sync with dependent teams

### Weekly Dependency Sync
- **Frequency**: Weekly (or twice-weekly for high-risk dependencies)
- **Attendees**: Project Manager, Delivery Lead, Tech Lead from both teams
- **Agenda**:
  - Status of each dependency (on track, at risk, blocked)
  - Any changes to timeline or interface
  - Blockers or concerns
  - Next steps and decision points

### Integration Testing
- **Plan early**: Define test strategy during planning
- **Coordinate timing**: Ensure both teams have features ready for integration testing
- **Dedicated environment**: Use staging or test environment for integration tests
- **Clear ownership**: Who is responsible for writing/maintaining integration tests

### Handoff Criteria
Define clear criteria for when work is ready to hand off:
- Code is merged to main branch
- Automated tests passing (unit + integration)
- API/interface is stable and documented
- Security scanning and code review completed
- Metrics/instrumentation implemented and verified
- Performance meets requirements
- Backward compatibility considered (if applicable)

## Communication Plan

### Stakeholder Matrix

| Role | Frequency | Content | Format |
|---|---|---|---|
| Project Manager (both teams) | Weekly | Status, risks, decisions | Meeting + Email |
| Delivery Lead (both teams) | 2–3x/week | Day-to-day blockers, updates | Slack + Ad-hoc |
| Tech Lead (both teams) | Weekly | Architecture, API changes, risks | Design review + Email |
| Developers (as needed) | As-needed | Technical details, API questions | Slack + Pairing |

### Status Update Template
```
Dependency: [API name / Feature name]
Team: [Team A] depends on [Team B]
Status: [On Track / At Risk / Blocked]

## Progress
- [What was completed this week]
- [What is planned for next week]

## Risks & Blockers
- [Risk/Blocker]: [Impact] | [Owner] | [Timeline]

## Interface Changes
- [Any changes to API, data format, or integration point]
- [Changes to timeline or release date]

## Next Milestones
- [Milestone name]: [Target date]
- [Milestone name]: [Target date]
```

## Escalation Path

### Dependency On Track
- Weekly status updates sufficient
- Proceed with planned integration

### Dependency At Risk
- **Trigger**: Estimate slipped by 1+ week or critical uncertainty
- **Action**: Schedule sync with both teams + Product Leads
- **Goal**: Identify mitigation (adjust timeline, reduce scope, parallel work)
- **Timeline**: Escalate within 2 business days

### Dependency Blocked
- **Trigger**: Work cannot proceed without resolution
- **Action**: Escalate immediately to Project Managers + Product Leads
- **Goal**: Resolve within 24–48 hours
- **Options**: De-scope dependent work, find workaround, reassign resources

## Risk Mitigation Strategies

### API/Integration Risk
- **Mitigation**: Define API contract early, use API mocks for parallel development
- **Testing**: Integration tests in staging environment
- **Fallback**: Document API compatibility, support multiple versions

### Timeline Risk
- **Mitigation**: Identify critical path, schedule dependent work with buffer
- **Fallback**: De-scope or delay dependent feature, create phased rollout plan

### Resource Risk
- **Mitigation**: Identify key people, cross-train backup
- **Fallback**: Reassign work, extend timeline, pairing/documentation

### Technical Risk
- **Mitigation**: Architecture review early, proof-of-concept for complex integrations
- **Fallback**: Alternative approach, vendor solution, phased rollout

## Integration Testing Strategy

### Test Levels
1. **Unit Tests**: Each team tests their own code
2. **Integration Tests**: Both teams test interaction points
3. **End-to-End Tests**: Full user flow across teams
4. **Smoke Tests**: Critical paths before release

### Test Environment Setup
- **Staging**: Deployed versions of both systems
- **Test Data**: Realistic data that exercises integration points
- **Monitoring**: Logs, metrics, error tracking
- **Rollback**: Ability to roll back one or both systems

### Ownership
- **Who writes integration tests?** Both teams or dedicated QA
- **Where are tests stored?** Shared repo or separate with references
- **How are tests run?** Manual before release, automated in CI

## Handoff Checklist

Before handing off to dependent team:
- [ ] Code merged and deployed to staging
- [ ] API/interface documentation complete
- [ ] Integration tests passing
- [ ] Performance testing completed (if applicable)
- [ ] Security scanning passed
- [ ] Backward compatibility documented (if applicable)
- [ ] Runbook/operations documentation complete
- [ ] Both teams agree "ready for integration"
- [ ] Agreed timeline for next steps
- [ ] Escalation path clear if issues arise

## Retrospective & Learnings

After release or integration, capture learnings:
- **What went well?** Smooth integrations, clear communication, etc.
- **What could improve?** API changes, timeline accuracy, communication frequency
- **Action items**: Process improvements, documentation updates, tooling

Share learnings with both teams and update this guide based on feedback.
