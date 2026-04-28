# OctoAcme — Handoff Checklists

Standardized checklists for each stage transition in the OctoAcme delivery lifecycle. Use these to reduce ambiguity and prevent work from proceeding until prerequisites are met.

See [Roles & Personas](octoacme-roles-and-personas.md) for ownership context.

---

## Requirements → Design Handoff

**From:** Business Analyst / Product Manager  
**To:** UX/UI Designer / Tech Lead

- [ ] Problem statement and user story documented
- [ ] Acceptance criteria defined and reviewed
- [ ] Business constraints and compliance requirements noted
- [ ] Out-of-scope items explicitly listed
- [ ] Relevant existing designs or patterns identified
- [ ] Stakeholder sign-off on requirements obtained

---

## Design → Development Handoff

**From:** UX/UI Designer  
**To:** Developers / Tech Lead

- [ ] Final wireframes and/or high-fidelity mockups published in design tool
- [ ] Interactive prototype available (if applicable)
- [ ] Design assets exported and accessible
- [ ] Interaction and animation specifications documented
- [ ] Edge cases and error states designed
- [ ] Accessibility requirements noted (color contrast, ARIA hints, keyboard nav)
- [ ] Tech Lead has confirmed technical feasibility

---

## Development → QA Handoff

**From:** Developers  
**To:** QA / Testing

- [ ] Feature branch merged to integration branch (or PR ready for QA)
- [ ] All CI checks passing (tests, lint, security scans)
- [ ] PR description includes acceptance criteria and testing notes
- [ ] Known limitations or deferred items documented
- [ ] Test data / seed scripts provided if needed
- [ ] Deployment to staging environment completed
- [ ] Developer smoke test passed

---

## QA → Release Handoff

**From:** QA / Testing  
**To:** Project Manager / DevOps/SRE / Product Manager

- [ ] All acceptance criteria verified and signed off
- [ ] Regression suite executed with no blocking failures
- [ ] Security scanning completed (SAST/DAST)
- [ ] Exploratory testing completed
- [ ] Open defects triaged and dispositioned (fix vs. defer)
- [ ] Release notes reviewed for accuracy
- [ ] Support team briefed on new functionality and known issues

---

## Release → Post-Release Handoff

**From:** DevOps/SRE / Project Manager  
**To:** Customer Support/Success / Stakeholders

- [ ] Deployment to production confirmed successful
- [ ] Post-deploy smoke tests passed
- [ ] Monitoring dashboards verified (no anomalous errors or latency)
- [ ] Release announcement sent to stakeholders
- [ ] Customer-facing release notes or changelog published
- [ ] Support knowledge base updated
- [ ] On-call runbook updated if behavior changed
- [ ] Rollback/incident playbook verified and accessible

---

## How to use these checklists
- Copy the relevant checklist into the PR description, issue, or project board card for the handoff.
- Mark items complete before notifying the receiving role that work is ready.
- Raise any unchecked items as blockers and resolve them or explicitly accept the risk with the Project Manager.
- Tailor checklist items to suit the scale of the work — not every item applies to every change.
