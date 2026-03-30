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

## UX Designer

### Role Summary
UX Designers ensure that features are intuitive, accessible, and aligned with user needs. They bridge the gap between product requirements and implementation by producing research insights, design artifacts, and usability validation.

### Responsibilities
- Conduct user research, interviews, and usability testing
- Create wireframes, prototypes, and design specifications
- Collaborate with PdM to translate business requirements into user flows
- Review implemented features against design specs and accessibility standards
- Contribute to the Definition of Done by validating UX acceptance criteria

### Goals
- Deliver user-centric experiences that reduce friction and increase adoption
- Ensure accessibility (WCAG compliance) across all product surfaces
- Maintain a shared design system and component library

### Typical Communication
- Design reviews and critique sessions with Developers and PdM
- Usability test readouts shared with the full delivery team
- Handoff notes in design tools (e.g., Figma) linked from relevant issues/PRs

### Interaction Points & Handoffs
- **Initiation:** Partners with PdM to understand problem space; contributes user research and personas to the Project One-pager.
- **Planning:** Provides design estimates; reviews acceptance criteria for UX completeness; delivers wireframes or prototypes before development begins (PdM → UX handoff).
- **Execution:** Participates in developer syncs; reviews PRs for UI/UX fidelity; flags deviations from design specs.
- **QA/Testing:** Collaborates with QA Engineer to define usability test cases; reviews QA sign-off for UX acceptance criteria.
- **Release:** Reviews release-candidate build for design regressions; signs off on UX readiness.
- **Retrospective:** Shares usability findings and design debt items for continuous improvement.

---

## QA Engineer

### Role Summary
QA Engineers own test planning, test execution, and quality gates throughout the delivery lifecycle. They ensure that features meet acceptance criteria, are free of regressions, and are safe to release.

### Responsibilities
- Define test strategies, test plans, and acceptance test cases
- Execute manual and automated test suites (unit, integration, end-to-end)
- Manage defect tracking, triage, and resolution follow-up
- Maintain the Definition of Done quality criteria
- Sign off on release readiness after successful test cycles
- Collaborate with DevOps to ensure CI pipelines include adequate automated coverage

### Goals
- Prevent defect leakage into production
- Increase automated test coverage and reduce manual regression effort
- Provide clear quality signals to the delivery team at every stage

### Typical Communication
- Test plans and test reports shared in the project repo or issue tracker
- Bug reports linked to relevant issues/PRs with reproducible steps
- Go/No-Go quality verdict shared with PM and PdM before each release

### Interaction Points & Handoffs
- **Initiation:** Reviews proposed success metrics to identify testability requirements.
- **Planning:** Contributes QA estimates and acceptance criteria to backlog items; drafts initial test plan (Developer → QA handoff: "Definition of Ready" includes test cases).
- **Execution:** Executes tests on completed features; raises defects; collaborates with Developers on fixes.
- **Release:** Runs final regression suite and smoke tests; issues formal QA sign-off (QA → Release handoff).
- **Retrospective:** Reports on defect trends, escaped bugs, and test coverage gaps for improvement.

---

## DevOps Engineer

### Role Summary
DevOps Engineers own the build, deployment, and operational infrastructure that enables the team to deliver software reliably and at pace. They design and maintain CI/CD pipelines, environments, and observability tooling.

### Responsibilities
- Design, build, and maintain CI/CD pipelines and deployment automation
- Manage cloud/infrastructure resources and environment configurations
- Implement monitoring, alerting, and logging infrastructure
- Ensure security and compliance requirements are met in the deployment process
- Support the team with environment provisioning for development, staging, and production
- Own rollback procedures and incident response runbooks

### Goals
- Enable fast, safe, and repeatable deployments
- Minimize mean time to recovery (MTTR) for production incidents
- Reduce toil through automation and self-service tooling

### Typical Communication
- Infrastructure-as-code (IaC) PRs and deployment runbooks
- Incident post-mortems and action items
- Release schedule coordination with PM and QA

### Interaction Points & Handoffs
- **Initiation:** Advises on infrastructure feasibility and operational requirements for the project.
- **Planning:** Provides environment and pipeline estimates; documents deployment constraints and dependencies.
- **Execution:** Maintains CI pipelines and developer tooling; unblocks environment issues; collaborates with QA on automated test integration.
- **Release:** Executes deployments per the agreed release plan; validates post-deploy health checks; owns rollback if needed (QA → DevOps handoff: QA sign-off triggers production deployment).
- **Retrospective:** Shares deployment metrics, incident learnings, and pipeline improvement opportunities.

---

## Business Analyst

### Role Summary
Business Analysts translate business needs into clear, actionable requirements. They bridge the gap between stakeholders and the delivery team, ensuring that what is built maps to measurable business outcomes.

### Responsibilities
- Elicit and document business and functional requirements
- Facilitate backlog refinement and requirements workshops
- Create user stories, use cases, and process flow diagrams
- Validate that delivered features satisfy business requirements
- Maintain requirements traceability and documentation throughout the project
- Support change management by documenting scope changes and their impact

### Goals
- Ensure the delivery team has unambiguous, well-scoped requirements before work begins
- Reduce rework caused by misunderstood or missing requirements
- Keep stakeholder expectations aligned with delivery reality

### Typical Communication
- Requirements documentation and feature briefs shared with PdM and Developers
- Backlog refinement facilitation with PM, PdM, and Developers
- Stakeholder meeting notes and decision logs

### Interaction Points & Handoffs
- **Initiation:** Facilitates stakeholder interviews; drafts the problem statement and success metrics for the Project One-pager.
- **Planning:** Leads requirements workshops; writes and refines user stories with acceptance criteria (BA → Developer handoff: stories are "Definition of Ready" before sprint entry).
- **Execution:** Available to clarify requirements during development; reviews in-progress work against requirements.
- **Release:** Validates release notes reflect delivered scope; supports stakeholder communication on feature changes.
- **Retrospective:** Reviews which requirements were unclear or changed; proposes improvements to the requirements process.

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- When working across phases (initiation → planning → execution → release → retro), refer to the **Interaction Points & Handoffs** section for each role to clarify ownership and cross-functional responsibilities.
- See [`octoacme-cross-functional-handoff-checklist.md`](octoacme-cross-functional-handoff-checklist.md) for a practical checklist of key handoffs between roles.

