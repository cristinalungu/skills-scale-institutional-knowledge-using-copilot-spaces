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

## Risk Lifecycle
- Identify: during planning and ongoing execution
- Assess: estimate impact and likelihood
- Mitigate: reduced via actions, contingency plans
- Monitor: review at weekly syncs and update status

## Stakeholder Communication
- Identify stakeholder groups and communication needs (e.g., engineering, sales, support)
- Provide regular updates (weekly or milestone-based)
- Use a single source of truth (project README or release doc) for status
- Follow the communication cadence defined in the Project Management Overview

## Cross-Role Communication Patterns
- **Scrum Master ↔ Project Manager**: Daily blocker updates, weekly velocity and team health sync
- **QA Lead ↔ Developers**: Defect triage, testability reviews, quality metrics
- **UX Designer ↔ Product Manager**: User research findings, design validation, usability feedback
- **Technical Writer ↔ Developers**: Documentation reviews, feature walkthroughs, API changes
- **Business Analyst ↔ Product Manager**: Requirements refinement, stakeholder feedback, UAT coordination

## Communication Templates
Weekly Status Template:
- Progress this week:
- Next steps:
- Risks & blockers:
- Ask / decisions needed:

Incident Communication
- Triage summary
- Actions being taken
- Expected timeline
- Post-incident blameless retrospective scheduled

## Escalation Paths
- Team-level -> PM -> Product Lead -> Sponsor
- For security incidents, follow the security incident runbook and notify Security on-call

## Risk Escalation Template

Use this template when escalating a risk that requires management attention or cross-team coordination:

**Risk ID**: [From Risk Register]
**Escalated By**: [Name, Role]
**Escalation Date**: [YYYY-MM-DD]
**Escalation Level**: [Level 1: PM | Level 2: Product Lead | Level 3: Sponsor]

**Risk Summary**: 
[One-sentence description of the risk]

**Impact Assessment**:
- **Business Impact**: [e.g., Revenue loss, customer satisfaction, compliance]
- **Timeline Impact**: [e.g., Milestone delay, release postponement]
- **Resource Impact**: [e.g., Additional team members needed, budget increase]

**Current Mitigation Status**:
- Actions taken so far:
- Why escalation is needed:
- What is blocked:

**Decision/Action Needed**:
- [ ] Approve additional resources
- [ ] Adjust timeline/scope
- [ ] Accept risk and proceed
- [ ] Escalate to next level
- [ ] Other: [specify]

**Proposed Resolution Options**:
1. [Option 1 with trade-offs]
2. [Option 2 with trade-offs]
3. [Option 3 with trade-offs]

**Urgency**: [Critical (24h) | High (3 days) | Medium (1 week)]

**Next Steps if Approved**: 
[Specific actions and owners]

---

## Escalation Checklist

Before escalating a risk, ensure you have:
- [ ] Updated the Risk Register with latest status
- [ ] Documented attempts to mitigate at current level
- [ ] Identified specific decisions or resources needed
- [ ] Prepared concrete resolution options with trade-offs
- [ ] Determined appropriate escalation level and stakeholders
- [ ] Set clear urgency and response timeframe
- [ ] Prepared impact assessment (business, timeline, resources)
- [ ] Notified the PM or Scrum Master of the escalation
