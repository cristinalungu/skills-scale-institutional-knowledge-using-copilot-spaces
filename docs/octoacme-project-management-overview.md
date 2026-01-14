# OctoAcme Project Management Overview

## Purpose
Provide a concise, shareable introduction to how OctoAcme runs projects so new teammates can quickly understand our approach, roles, and key artifacts.

## Scope
Applies to all cross-functional projects that deliver product features, services, or integrations.

## Principles
- Customer-first: prioritize customer value and usability.
- Iterative delivery: deliver small, testable increments.
- Clear ownership: each project has a named Project Manager (PM) and Product Lead.
- Data-informed decisions: measure impact and iterate based on evidence.
- Psychological safety: encourage feedback and learning.

## Core Roles
- Project Manager (PM): coordinates delivery, schedules, risk, communications.
- Product Manager (PdM): defines outcomes, prioritizes backlog, and measures success.
- Developers: implement features, collaborate on design and testability.
- Scrum Master: facilitates Agile ceremonies, removes impediments, coaches team.
- QA Lead: owns quality strategy, leads testing efforts, provides release signoff.
- UX Designer: researches user needs, designs interfaces, validates usability.
- Technical Writer: creates and maintains documentation, help articles, API references.
- Business Analyst: bridges business needs and technical solutions, validates requirements.
- Stakeholders: provide inputs and approvals.

## Key Artifacts
- Project Charter / One-pager
- Roadmap and Release Plan
- Sprint/Iteration Backlog
- Acceptance Criteria & Definition of Done
- Risk Register
- Retrospective notes and action items

## Lifecycle (high-level)
1. **Initiation**: problem statement, stakeholders, high-level timeline.
   - Handoff: Product Manager delivers problem statement and goals → Project Manager creates project charter
2. **Planning**: scope, resources, milestones, dependencies.
   - Handoff: Project Manager delivers project plan → Scrum Master and team begin sprint planning
3. **Design**: UX research, technical design, architecture decisions.
   - Handoff: UX Designer delivers designs → Developers begin implementation
4. **Execution**: build, test, review, iterate.
   - Handoff: Developers complete features → QA Lead begins testing
5. **QA & Validation**: comprehensive testing, acceptance validation, QA signoff.
   - Handoff: QA Lead provides signoff → Project Manager coordinates release
6. **Release**: deploy, verify, announce.
   - Handoff: Technical Writer publishes documentation → Support team begins customer assistance
7. **Close & Retrospective**: capture learnings and next steps.
   - Handoff: Scrum Master facilitates retrospective → Team documents improvements for next cycle

## Communication Cadence
### Daily
- Team standup (15 min) — led by Scrum Master, focus on progress, blockers, dependencies

### Twice-Weekly
- Design review (as needed) — UX Designer shares designs with Product and Engineering
- Documentation sync (as needed) — Technical Writer coordinates with Developers on feature docs

### Weekly
- PM + PdM sync — alignment on priorities, risks, and timeline
- Delivery team sync — show progress, demo work, flag risks
- Risk register review — Project Manager and team update risk status
- QA status update — QA Lead shares test progress and quality metrics

### Bi-Weekly (Sprint-Based)
- Sprint planning — Scrum Master facilitates, team commits to sprint goals
- Sprint review/demo — Team demonstrates completed work to stakeholders
- Sprint retrospective — Scrum Master facilitates, team identifies improvements
- Requirements refinement — Business Analyst and Product Manager clarify upcoming work

### Monthly
- Stakeholder updates — Project Manager shares progress, milestones, and decisions
- Architecture review (as needed) — Tech Lead and Developers review technical decisions
- Documentation review — Technical Writer and team validate documentation quality

### Ad-hoc
- Risk escalations — as needed per escalation checklist
- Design handoffs — UX Designer to Developers when designs are ready
- QA signoff — QA Lead when testing is complete
- Release go/no-go — decision gate before production deployment

## How to use these docs
- Keep the Project Charter updated in the project repo.
- Add process-specific docs into `.copilot/` if you want Copilot Spaces to use them as context.
