# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Core Delivery Roles

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations
- Collaborate with Tech Leads on architectural decisions

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed
- Architecture review discussions

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics
- Work with UX Researchers and Data Analysts to understand customer needs

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs
- Customer feedback and metrics reviews

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication
- Track metrics (velocity, burndown, cycle time)

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation
- Escalation paths for blockers and dependencies

---

## Specialized / Cross-Cutting Roles

### Tech Lead

#### Role Summary
Tech Leads provide architectural guidance, own technical strategy, and ensure code quality and maintainability across the project.

#### Responsibilities
- Define and review architecture decisions for features and systems
- Approve significant technical changes and technology choices
- Prioritize and manage technical debt
- Mentor developers and conduct code reviews
- Identify and mitigate technical risks
- Collaborate with Release Engineers on deployment strategies

#### Interactions
- Works with Developers on design and code reviews
- Collaborates with Product Manager on feasibility and trade-offs
- Escalates architectural risks to Product Lead
- Partners with Release Engineer on deployment patterns

#### Typical Communication
- Architecture review meetings
- Technical design docs and RFC (Request for Comments)
- Code review feedback
- Sprint planning technical discussions

---

### Delivery Lead

#### Role Summary
Delivery Leads coordinate sprint-level commitments, manage day-to-day execution risks, and ensure the team stays aligned and unblocked.

#### Responsibilities
- Coordinate sprint planning and capacity management
- Manage blockers and dependencies in real-time
- Track sprint health and progress against commitments
- Liaise between PM and development team on priorities and sequencing
- Facilitate daily standups and retrospectives
- Escalate risks and blockers to PM when needed

#### Interactions
- Works with Project Manager for planning and prioritization
- Collaborates with Developers on task sequencing and blockers
- Partners with QA on acceptance gating and test scheduling
- Coordinates with Release Engineer for deployment readiness

#### Typical Communication
- Daily standups and ad-hoc synchronization
- Sprint status reports
- Risk escalations and dependency tracking

---

### Release Engineer / SRE (Site Reliability Engineer)

#### Role Summary
Release Engineers maintain deployment pipelines, own release automation, and ensure production stability and observability.

#### Responsibilities
- Design and maintain deployment pipelines and infrastructure
- Own release automation, testing, and rollback procedures
- Monitor post-release health and performance
- Establish observability and alerting standards
- Respond to production incidents
- Coordinate with Developers on deployment readiness

#### Interactions
- Works with Developers during release and for operational integration
- Collaborates with Security Engineer on security scanning and hardening
- Partners with Tech Lead on deployment architecture
- Notifies on-call and incident response teams for critical issues
- Updates Project Manager on deployment status and incidents

#### Typical Communication
- Release runbooks and playbooks
- Deployment status and incident reports
- Infrastructure and monitoring dashboards
- Post-incident retrospectives

---

### Security Engineer

#### Role Summary
Security Engineers ensure that features and systems meet security standards and identify/mitigate security risks.

#### Responsibilities
- Perform threat modeling for features and systems
- Review security implications of design and implementation
- Ensure CI security scanning (SAST, dependency scanning) is configured
- Conduct security code reviews when needed
- Manage vulnerability tracking and remediation
- Participate in incident response for security events

#### Interactions
- Works with Developers on secure coding practices and code review
- Collaborates with Release Engineer on security hardening and scanning
- Escalates critical findings to Product Lead and Security on-call
- Partners with Tech Lead on security architecture decisions

#### Typical Communication
- Security design reviews
- Threat models and risk assessments
- Security scanning reports and remediation tracking
- Security incident playbooks

---

### UX Researcher / Designer

#### Role Summary
UX Researchers and Designers validate user needs, design solutions, and ensure features are usable and meet user expectations.

#### Responsibilities
- Conduct user research and usability testing
- Create prototypes and design mockups
- Define usability acceptance criteria
- Validate design solutions with users
- Provide design feedback during development
- Document design decisions and rationale

#### Interactions
- Works with Product Manager to define success metrics and validate solutions
- Collaborates with Developers to ensure designs are implementable
- Partners with Data Analyst on measuring user experience metrics
- Influences Acceptance Criteria to include usability requirements

#### Typical Communication
- Design specs and prototypes
- User research findings and insights
- Usability testing reports
- Design review sessions

---

### Data Analyst / Product Analyst

#### Role Summary
Data Analysts define instrumentation and success metrics, analyze product data, and provide insights to guide decisions.

#### Responsibilities
- Define instrumentation needs and data collection strategy
- Analyze success metrics and feature adoption
- Produce dashboards and regular analytics reports
- Identify trends and opportunities in product data
- Collaborate on defining measurable goals
- Present insights and recommendations to leadership

#### Interactions
- Works with Product Manager to define metrics and analyze impact
- Collaborates with Developers to ensure telemetry is implemented correctly
- Partners with UX Researcher on measuring user experience
- Provides insights to inform backlog prioritization

#### Typical Communication
- Success metrics dashboards
- Analytics reports and insights
- Data-driven recommendations
- Metric review meetings

---

### Customer Success Liaison

#### Role Summary
Customer Success Liaisons surface customer feedback, coordinate beta programs, and ensure customer needs are understood and prioritized.

#### Responsibilities
- Gather and synthesize customer feedback
- Coordinate beta programs and early access initiatives
- Communicate product updates and impacts to key customers
- Escalate critical customer issues and feature requests
- Collaborate with Support teams on product issues
- Provide customer perspective in planning and prioritization

#### Interactions
- Works with Product Manager to translate customer needs into priorities
- Collaborates with Support teams on customer-impacting issues
- Provides input to acceptance criteria based on customer expectations
- Communicates product changes and impacts to customers

#### Typical Communication
- Customer feedback summaries
- Beta program updates
- Customer impact communications
- Feature request prioritization discussions

---

## How These Personas Work Together

### Planning Phase
- **Product Manager** defines the problem and success metrics
- **Project Manager** creates the timeline and identifies dependencies
- **Tech Lead** assesses technical feasibility
- **Data Analyst** defines instrumentation and success metrics
- **UX Researcher** validates user needs
- **Developers** estimate effort

### Execution Phase
- **Delivery Lead** coordinates daily work and unblocks issues
- **Developers** implement features with guidance from **Tech Lead**
- **UX Researcher/Designer** validates designs during development
- **Data Analyst** ensures telemetry is implemented
- **Project Manager** tracks progress and manages risks
- **Customer Success Liaison** gathers early feedback

### Release Phase
- **Release Engineer** manages the deployment pipeline
- **Security Engineer** ensures security scanning and hardening
- **Tech Lead** oversees architectural stability
- **Developers** handle hotfixes and troubleshooting
- **Project Manager** communicates status and impacts
- **Customer Success Liaison** notifies customers

### Post-Release Phase
- **Data Analyst** monitors success metrics and impact
- **Release Engineer** monitors production health
- **Customer Success Liaison** gathers customer feedback
- **Project Manager** captures learnings in retrospective
- **Product Manager** uses data to inform next iteration

---

## How These Personas Are Used in the Exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- When assigning work, reference the persona definitions to clarify responsibilities and escalation paths.
