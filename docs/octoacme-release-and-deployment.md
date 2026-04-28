# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Key Collaborators
- **DevOps / SRE:** Owns deployment execution, monitors production, and maintains the rollback playbook.
- **Project Manager:** Coordinates the release window, stakeholder communication, and final go/no-go decision.
- **Product Manager:** Approves release notes and communicates the release to external stakeholders.
- **Security / Compliance:** Signs off on security scans and compliance requirements before go-live.
- **Customer Support / Success:** Validates support readiness and release communications.
- **QA / Testing:** Provides final sign-off via the [QA → Release Handoff checklist](octoacme-handoff-checklists.md).

See [Roles & Personas](octoacme-roles-and-personas.md) for full role definitions.  
Use the [Handoff Checklists](octoacme-handoff-checklists.md) for QA → Release and Release → Post-Release transitions.

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
