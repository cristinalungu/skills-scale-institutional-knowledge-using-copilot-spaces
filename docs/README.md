# OctoAcme Project Management Docs

Welcome to the OctoAcme Project Management documentation. This guide centralizes all key processes and team practices, providing clear, repeatable workflows for project teams and faster onboarding for new members.

## Overview of Project Management Processes

OctoAcme organizes work around a clear project lifecycle—Initiation, Planning, Execution, Release, and Close—with lightweight artifacts that drive decisions and alignment. Projects start with a Project One-pager (problem, goal, success metrics, stakeholders, timeline) and a decision gate that confirms success metrics, stakeholder buy-in, and team availability before moving into planning. Planning breaks approved initiatives into a prioritized backlog using a standard backlog-item template (title, description, acceptance criteria, priority, estimate, owner) and a Definition of Done. Teams estimate scope, identify dependencies and risks, run a kickoff, and produce a release/milestone plan before executing.

Day-to-day work follows standard agile workflows and branching/PR conventions. Work is tracked on a project board with columns like Backlog, Ready, In Progress, In Review, QA, and Done. Pull requests are expected to be small when possible, include issue links and acceptance criteria, and run CI linters/tests before review; at least one approval is required prior to merging. The planning and execution checklists (kickoff held, backlog prioritized, CI configured, demos scheduled, risk register updated) are used to keep projects on track and ensure handoffs and expectations are clear.

Roles and responsibilities are explicit: Project Managers coordinate delivery, schedules, risks, and cross-team communication; Product Managers (PdMs) own outcomes, prioritize the backlog, and validate success through metrics; Developers implement code and tests; QA/testing validate acceptance criteria; and stakeholders provide input and approvals. This role clarity shows up in artifacts (one-pager, roadmaps, acceptance criteria, risk register) and routines—e.g., weekly PM+PdM syncs, daily standups focused on progress and blockers, weekly delivery syncs for progress and flagged risks, and monthly stakeholder updates—to maintain alignment and transparency.

Quality and risk management are embedded into CI/CD and release practices. The QA stack includes unit tests, integration tests where applicable, end-to-end smoke tests for critical flows, security scanning in CI, and manual QA for feature acceptance when needed. Releases follow a standardized checklist (pre-release checks, staging smoke tests, automated production deploys when possible, post-deploy verifications) and include rollback/incident playbooks and a release-notes template. Risks are tracked in a simple register (ID, impact, likelihood, owner, mitigation, status) with a three-level escalation path (team → PM → Product Lead → Sponsor) and regular review at weekly syncs. Continuous improvement is captured via retrospectives that produce prioritized action items tracked back into the backlog.

## Docs Index

- [Project Management Overview](octoacme-project-management-overview.md)
- [Project Initiation Guide](octoacme-project-initiation.md)
- [Project Planning](octoacme-project-planning.md)
- [Execution & Tracking](octoacme-execution-and-tracking.md)
- [Risk Management & Communication](octoacme-risks-and-communication.md)
- [Release & Deployment Guide](octoacme-release-and-deployment.md)
- [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md)
- [Roles and Personas](octoacme-roles-and-personas.md)
