# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans
- Release notes drafted
- Rollback / mitigation plan documented
- Smoke tests prepared
- **QA signoff completed** (see QA Signoff Checklist below)

## QA Signoff Checklist

The QA Lead must complete and approve this checklist before a release can proceed to production:

### Test Coverage & Execution
- [ ] All planned test cases executed (manual and automated)
- [ ] Regression test suite passed on staging environment
- [ ] Integration tests passed for all affected components
- [ ] Performance tests completed (if applicable)
- [ ] Security scans completed with no critical/high issues
- [ ] Accessibility validation completed (WCAG compliance where applicable)
- [ ] Cross-browser/platform testing completed (per test matrix)
- [ ] Smoke tests prepared and validated on staging

### Defect Review
- [ ] All critical and high-priority defects resolved
- [ ] Medium-priority defects reviewed and accepted for release or deferred
- [ ] Known issues documented in release notes
- [ ] Defect trends reviewed (no concerning patterns)

### Requirements & Acceptance
- [ ] All acceptance criteria validated and met
- [ ] User stories marked as "Done" per Definition of Done
- [ ] Business Analyst and Product Manager sign-off obtained (if required)
- [ ] User Acceptance Testing (UAT) completed successfully
- [ ] Edge cases and error scenarios tested

### Documentation & Communication
- [ ] Test results documented and shared with team
- [ ] Test coverage metrics reviewed and acceptable
- [ ] Known limitations documented
- [ ] Rollback procedures tested and documented
- [ ] Support team briefed on new features and known issues

### Release Readiness Decision
**QA Lead Sign-off**:
- Name: _____________
- Date: _____________
- Decision: [ ] Approved for Release [ ] Blocked - Issues to resolve [ ] Approved with conditions

**Conditions or Blockers** (if any):
[Describe any remaining concerns, risks, or actions required before production deployment]

---

## Decision Gates

### Gate 1: Release Planning (During Sprint Planning)
**Decision**: Is the release scope well-defined and feasible?
- **Participants**: Product Manager, Project Manager, Scrum Master, Tech Lead, QA Lead
- **Criteria**: 
  - Release goals and success metrics defined
  - Features prioritized and estimated
  - Testing strategy agreed upon
  - Resources and timeline confirmed
- **Outcome**: Proceed to development or refine scope

### Gate 2: Code Complete (End of Development Sprint)
**Decision**: Is the code ready for comprehensive testing?
- **Participants**: Tech Lead, QA Lead, Scrum Master
- **Criteria**:
  - All planned features implemented
  - Code reviews completed
  - Unit tests passing
  - CI/CD pipeline green
  - Technical debt documented
- **Outcome**: Proceed to QA testing or continue development

### Gate 3: QA Signoff (After Testing Phase)
**Decision**: Is the release ready for production deployment?
- **Participants**: QA Lead, Product Manager, Project Manager, Tech Lead
- **Criteria**:
  - QA Signoff Checklist completed
  - Critical/high defects resolved
  - Acceptance criteria validated
  - Release notes finalized
- **Outcome**: Approve for staging deployment or fix remaining issues

### Gate 4: Production Go/No-Go (Pre-Deployment)
**Decision**: Deploy to production now or postpone?
- **Participants**: Product Manager, Project Manager, Tech Lead, QA Lead, On-call Engineer
- **Criteria**:
  - Staging deployment successful
  - Smoke tests passed on staging
  - Rollback plan validated
  - Deployment window scheduled
  - Support team ready
- **Outcome**: Deploy to production or postpone and reschedule

## Deployment Checklist
- [ ] Deployment window scheduled (if needed)
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy verifications
- [ ] Announce release to stakeholders and support

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Trigger incident response and notify on-call
  - Rollback to last known-good release if necessary
  - Triage root cause and capture action items

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
