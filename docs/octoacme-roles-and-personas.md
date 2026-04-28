# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

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

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## UX/UI Designer

### Role Summary
UX/UI Designers ensure that product features are usable, accessible, and visually consistent. They translate requirements into designs and validate solutions through user feedback.

### Responsibilities
- Create wireframes, mockups, and prototypes for new features
- Conduct user research and usability testing
- Define UX guidelines and maintain the design system
- Provide design assets and specifications to Developers
- Review implemented features against design intent

### Goals
- Deliver intuitive, accessible user experiences
- Reduce rework caused by usability issues discovered late
- Maintain visual consistency across the product

### Typical Communication
- Design reviews and handoff notes shared with Developers
- Usability findings and iteration notes shared with Product Managers
- Participation in sprint planning to size design effort

### Interactions
- **Product Managers:** Collaborate during discovery and planning to understand requirements and success criteria; review acceptance criteria together before development begins.
- **Developers:** Hand off detailed design specifications; participate in implementation reviews to ensure fidelity.
- **Project Managers:** Flag design-related risks or dependency on external assets during planning.
- **Lifecycle touchpoints:** Active during Initiation (concept sketches), Planning (wireframes and prototypes), and Execution (design QA). See also: [Handoff Checklists](octoacme-handoff-checklists.md).

---

## Tech Lead / Engineering Lead

### Role Summary
The Tech Lead sets the technical direction for a project, guides architectural decisions, and ensures engineering quality standards are upheld throughout the delivery lifecycle.

### Responsibilities
- Define and communicate technical architecture and standards
- Lead code reviews and enforce engineering best practices
- Break down complex features into implementable tasks
- Identify and mitigate technical risks and debt
- Mentor and support Developers on the team

### Goals
- Deliver a maintainable, scalable technical solution
- Keep technical debt within acceptable bounds
- Ensure the team can execute on the plan without bottlenecks

### Typical Communication
- Architecture decision records (ADRs) and technical design docs
- Code review feedback and pairing sessions
- Technical updates in weekly delivery syncs

### Interactions
- **Developers:** Provide day-to-day technical guidance; facilitate code and design reviews.
- **Product Managers:** Translate product requirements into technical feasibility constraints; negotiate scope when technical complexity arises.
- **Project Managers:** Surface technical risks and capacity constraints during planning and execution; contribute to risk register.
- **Lifecycle touchpoints:** Engaged from Planning through Execution and Release. Participates in kickoff, sprint planning, PR reviews, and pre-release readiness checks.

---

## Business Analyst

### Role Summary
Business Analysts bridge the gap between business stakeholders and the delivery team. They gather, document, and clarify requirements to ensure the team builds the right thing.

### Responsibilities
- Elicit and document business requirements and user stories
- Define and validate acceptance criteria with Product Managers
- Analyze current processes and identify improvement opportunities
- Support backlog refinement and estimation sessions
- Produce business process diagrams and data flow documentation

### Goals
- Ensure requirements are complete, unambiguous, and testable
- Reduce costly rework from misunderstood or missing requirements
- Align technical deliverables with business outcomes

### Typical Communication
- Requirements documents and user story write-ups shared with the team
- Participation in refinement and planning sessions
- Stakeholder interviews and sign-off emails

### Interactions
- **Product Managers:** Co-own requirements gathering; validate that user stories reflect the product vision and business need.
- **Developers:** Clarify acceptance criteria and answer questions during implementation; review deliverables against requirements.
- **Project Managers:** Flag scope changes or gaps that affect timeline estimates; support impact analysis.
- **Lifecycle touchpoints:** Most active during Initiation (requirements gathering) and Planning (backlog refinement), with ongoing involvement during Execution for clarification. See also: [Handoff Checklists](octoacme-handoff-checklists.md).

---

## DevOps / SRE

### Role Summary
DevOps and Site Reliability Engineers maintain the build, deployment, and production infrastructure. They keep delivery pipelines healthy and ensure services meet reliability and security standards.

### Responsibilities
- Design and maintain CI/CD pipelines and automation
- Monitor production systems and respond to incidents
- Define and enforce infrastructure security and reliability policies
- Collaborate on release planning and deployment procedures
- Conduct post-mortems and drive reliability improvements

### Goals
- Enable fast, safe, and repeatable deployments
- Maintain agreed service-level objectives (SLOs)
- Reduce toil through automation

### Typical Communication
- Pipeline and monitoring runbooks shared with Developers
- Incident reports and post-mortem summaries
- Input to release plans and deployment checklists

### Interactions
- **Developers:** Provide CI/CD tooling and deployment guidance; review infrastructure-touching code changes.
- **Product Managers:** Advise on non-functional requirements (performance, reliability, availability) during planning.
- **Project Managers:** Coordinate deployment windows and runbooks; contribute to the rollback/incident playbook.
- **Lifecycle touchpoints:** Engaged during Planning (environment setup), Execution (CI/CD maintenance, incident response), and Release (deployment execution and post-deploy verification). See also: [Handoff Checklists](octoacme-handoff-checklists.md).

---

## Security / Compliance

### Role Summary
Security and Compliance roles ensure the product meets organizational and regulatory requirements for data protection, access control, and audit readiness throughout the development lifecycle.

### Responsibilities
- Define and communicate security requirements and threat models
- Review architecture and code changes for security vulnerabilities
- Conduct or coordinate security testing (SAST, DAST, penetration testing)
- Maintain compliance documentation and evidence collection
- Drive remediation of identified vulnerabilities

### Goals
- Ship secure software that meets compliance obligations
- Shift security left to catch issues before they reach production
- Maintain audit-ready documentation

### Typical Communication
- Security review findings and remediation guidance
- Compliance checklists and sign-offs at release gates
- Threat model documents shared with engineering leads

### Interactions
- **Developers:** Provide secure coding guidance; flag vulnerabilities in code and dependency reviews.
- **Product Managers:** Define security and compliance requirements as part of feature acceptance criteria.
- **Project Managers:** Identify security-related tasks and risks in the project plan; ensure security gates are included in the release checklist.
- **Lifecycle touchpoints:** Active during Initiation (threat modeling), Planning (security requirements), Execution (security scanning in CI), and Release (compliance sign-off). See also: [Handoff Checklists](octoacme-handoff-checklists.md).

---

## Customer Support / Customer Success

### Role Summary
Customer Support and Customer Success roles are the voice of the customer within the team. They surface real-world feedback, document known issues, and ensure customers can successfully adopt new features.

### Responsibilities
- Collect and prioritize customer feedback and bug reports
- Document known issues and workarounds for the support knowledge base
- Coordinate customer communications for releases and incidents
- Validate that release notes and in-product help are accurate
- Track adoption metrics and escalate customer-impacting issues

### Goals
- Reduce customer-facing defects and friction points
- Ensure customers can successfully adopt new features
- Close the feedback loop between customers and the product team

### Typical Communication
- Support ticket summaries and customer feedback reports shared with Product Managers
- Release communication drafts reviewed with Project Managers
- Participation in retrospectives to highlight customer-impacting patterns

### Interactions
- **Product Managers:** Feed customer insights into the roadmap and backlog prioritization.
- **Developers:** Report reproducible customer bugs; verify fixes in staging before release.
- **Project Managers:** Coordinate release announcements and support readiness; flag customer-impacting risks before go-live.
- **Lifecycle touchpoints:** Consulted during Planning (customer impact assessment), active during Execution (bug triage), and key at Release (release communications, support readiness). See also: [Handoff Checklists](octoacme-handoff-checklists.md).

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

