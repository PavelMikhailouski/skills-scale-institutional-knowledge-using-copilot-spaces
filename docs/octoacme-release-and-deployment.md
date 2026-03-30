# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans (DevOps Engineer confirms pipeline health)
- QA Engineer has issued formal QA sign-off after full regression run
- UX Designer has reviewed release candidate for design regressions
- Release notes drafted
- Rollback / mitigation plan documented (DevOps Engineer owns rollback procedures)
- Smoke tests prepared

## Deployment Checklist
- [ ] QA sign-off received (QA → DevOps handoff)
- [ ] UX sign-off received for UX-impacting changes
- [ ] Deployment window scheduled (if needed)
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests (DevOps Engineer)
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy verifications
- [ ] Announce release to stakeholders and support (PM + PdM)

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
