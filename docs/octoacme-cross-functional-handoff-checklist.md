# OctoAcme — Cross-Functional Handoff Checklist

## Purpose
Reduce ambiguity and dropped work items at key transition points between roles and project phases. Use this checklist at each handoff to confirm readiness before the next phase or team takes ownership.

---

## 1. Initiation → Planning (PM / PdM / BA handoff)

> **From:** Project Manager + Product Manager + Business Analyst  
> **To:** Full delivery team (Developers, UX Designer, QA Engineer, DevOps Engineer)

- [ ] Problem statement and success metrics are documented in the Project One-pager
- [ ] Business Analyst has captured initial stakeholder requirements
- [ ] Stakeholder list and communication plan are agreed
- [ ] Team roles are confirmed (UX, QA, DevOps, BA allocated)
- [ ] Go/No-Go decision has been made and recorded
- [ ] Project repo/board skeleton is created and shared with the team

---

## 2. PdM / BA → Developer (Requirements handoff)

> **From:** Product Manager + Business Analyst  
> **To:** Developers

- [ ] User stories include a clear description, acceptance criteria, and priority
- [ ] Business Analyst has facilitated a requirements walkthrough with Developers
- [ ] UX wireframes or prototypes are linked from the story/issue
- [ ] Edge cases and error scenarios are documented
- [ ] Dependencies and integration points are identified
- [ ] Story meets the **Definition of Ready**:
  - [ ] Acceptance criteria are unambiguous
  - [ ] UX designs are available
  - [ ] QA test cases are drafted
  - [ ] Estimate is agreed

---

## 3. Developer → QA Engineer (Dev-complete handoff)

> **From:** Developers  
> **To:** QA Engineer

- [ ] All acceptance criteria have been self-tested by the Developer
- [ ] Unit and integration tests are passing in CI
- [ ] PR is merged to the integration/test branch
- [ ] Build artifacts are deployed to the QA environment
- [ ] Release notes or change summary are updated
- [ ] Known limitations or areas needing special attention are noted for QA
- [ ] Linked issue/ticket is moved to **QA** status on the project board

---

## 4. QA Engineer → UX Designer (UX acceptance handoff)

> **From:** QA Engineer  
> **To:** UX Designer

- [ ] Functional tests are passing
- [ ] QA environment is stable and accessible
- [ ] UX Designer has been notified that the build is ready for UX review
- [ ] UX acceptance criteria from the original story are shared for reference
- [ ] Any known visual regressions or accessibility concerns are flagged

---

## 5. QA Engineer → DevOps Engineer (Release readiness handoff)

> **From:** QA Engineer  
> **To:** DevOps Engineer

- [ ] Full regression suite has passed in staging
- [ ] UX Designer sign-off received (for UX-impacting changes)
- [ ] Formal QA sign-off document / comment is recorded on the release issue
- [ ] Release notes are finalized and reviewed
- [ ] Rollback criteria are defined (what would trigger a rollback)
- [ ] Deployment runbook is reviewed and up to date
- [ ] Smoke test script is ready for post-deploy validation

---

## 6. DevOps Engineer → PM / PdM (Post-deploy handoff)

> **From:** DevOps Engineer  
> **To:** Project Manager + Product Manager

- [ ] Production deployment completed successfully
- [ ] Post-deploy smoke tests passed
- [ ] Monitoring and alerting confirmed active for the new release
- [ ] Any deployment issues or deviations from plan are documented
- [ ] PM / PdM notified to announce release to stakeholders and support
- [ ] Incident response on-call is aware of the new release

---

## 7. Release → Retrospective (Close & Improve handoff)

> **From:** All roles  
> **To:** PM (facilitates retrospective)

- [ ] Release outcome (success / partial / rollback) is documented
- [ ] Each role has prepared retrospective inputs:
  - [ ] Developers: code quality, technical debt, velocity observations
  - [ ] QA Engineer: defect counts, escaped bugs, test coverage gaps
  - [ ] UX Designer: usability findings, design debt
  - [ ] DevOps Engineer: deployment metrics, pipeline issues, MTTR
  - [ ] BA: requirements changes, unclear stories, stakeholder feedback
- [ ] Retrospective is scheduled within one week of release
- [ ] Action items from the previous retrospective are reviewed

---

## References
- [Roles & Personas](octoacme-roles-and-personas.md)
- [Project Management Overview](octoacme-project-management-overview.md)
- [Project Planning](octoacme-project-planning.md)
- [Execution & Tracking](octoacme-execution-and-tracking.md)
- [Release & Deployment](octoacme-release-and-deployment.md)
- [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md)
