# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies
- Weekly delivery sync — show progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review
  - Require at least one approval before merging (or team-defined policy)
  - Technical Writer reviews documentation changes in PR
  - UX Designer reviews UI implementation against designs

## Development Handoffs
- **Development → Code Review**: Developer submits PR → Peer developers review code
- **Code Review → QA**: PR merged to main/staging → QA Lead assigns test cases
- **QA → Documentation**: Feature tested and accepted → Technical Writer updates docs
- **Documentation → Release**: Docs published → Release ready for deployment

## Quality & Testing
- Unit tests for new logic
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- Security scanning in CI
- Manual QA for feature acceptance when needed

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage)

## Blocker Escalation
- **Level 1**: Team-level triage in daily standup (Scrum Master facilitates)
  - Resolve: Team members collaborate to remove blockers
  - Timeline: Within 24 hours
- **Level 2**: PM escalates to Product Lead and dependent teams
  - Resolve: Cross-team coordination, resource reallocation
  - Timeline: Within 3 days
- **Level 3**: Sponsor-level escalation for business-impacting issues
  - Resolve: Executive decision, major scope/timeline changes
  - Timeline: Within 1 week
  - **Use Risk Escalation Template** (see `octoacme-risks-and-communication.md`)

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly
- [ ] Handoff procedures documented and communicated
- [ ] QA test cases created and linked to user stories
- [ ] Documentation templates prepared by Technical Writer
- [ ] Design implementation tracked against UX specs
