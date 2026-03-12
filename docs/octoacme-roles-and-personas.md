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

## QA Engineer

### Role Summary
QA Engineers own the quality of delivered software. They design and execute test strategies, validate acceptance criteria, and ensure releases meet defined standards before reaching production.

### Responsibilities
- Design and maintain test plans (unit, integration, end-to-end, regression)
- Define and enforce acceptance criteria in collaboration with Product Managers
- Execute manual QA for feature acceptance and edge-case validation
- Automate repeatable test scenarios and integrate them into CI
- Identify, document, and track defects through to resolution
- Gate releases by confirming all tests pass and acceptance criteria are met

### Goals
- Prevent defects from reaching production
- Increase test coverage and reduce manual testing overhead over time
- Ensure consistent quality across all release types

### Typical Communication
- Sprint planning and backlog refinement (to clarify acceptance criteria)
- PR reviews and QA sign-off before merging
- Bug reports, test results, and test plan updates
- Pre-release and post-release verification sign-off

### Interactions with Existing Roles
- **Developers**: Collaborate on acceptance criteria, review PRs, and pair on reproducing/fixing defects.
- **Product Managers**: Translate feature requirements into testable acceptance criteria; escalate quality issues that affect scope.
- **Project Managers**: Report QA status and blockers during weekly syncs; flag risks that could delay release.

---

## Stakeholder / Sponsor

### Role Summary
**Stakeholders** are individuals or groups with a vested interest in the project's outcomes — including business sponsors, leadership, customers, and partner teams. A **Sponsor** is the primary executive champion who provides funding, removes organizational blockers, and approves major scope or timeline changes. Both roles are distinct from day-to-day delivery but critical for alignment and escalation.

> **Stakeholder vs. Sponsor:** Any person affected by or with influence over the project is a Stakeholder. The Sponsor is a specific Stakeholder — typically a senior leader — who has formal accountability for the project's business outcomes, provides resources, and is the ultimate decision-maker for escalations.

### Responsibilities

**All Stakeholders**
- Provide business requirements, domain expertise, and feedback
- Participate in milestone demos and checkpoint reviews
- Communicate priorities and constraints to the delivery team

**Sponsor (in addition to the above)**
- Approve the Project Charter, budget, and major scope changes
- Remove organizational blockers that the delivery team and PM cannot resolve
- Act as the ultimate escalation point for unresolved risks or issues

### Goals
- Ensure the project delivers measurable business value
- Maintain visibility into progress, risks, and decisions
- Provide timely approvals to avoid delays

### Typical Communication
- Monthly (or milestone-based) project status updates
- Charter and roadmap review sign-offs
- Executive briefings for major releases or incidents
- Escalation channels for high-priority blockers

### Interactions with Existing Roles
- **Product Managers**: Stakeholders provide business inputs and validate prioritization decisions; Sponsors approve major roadmap changes.
- **Project Managers**: Receive regular status reports and RAID log updates; engage for escalations that require sponsor-level authority.
- **Developers**: Minimal direct interaction; may participate in milestone demos or user research sessions.

---

## UX Designer

### Role Summary
UX Designers shape the user experience and interface design, ensuring that features are usable, accessible, and aligned with user needs. They bridge user research insights and engineering implementation.

### Responsibilities
- Conduct user research, usability testing, and competitive analysis
- Create wireframes, prototypes, and design specifications
- Define interaction patterns and accessibility requirements
- Collaborate in backlog refinement to ensure user needs inform acceptance criteria
- Review implemented features for design fidelity and usability
- Maintain a shared design system or component library

### Goals
- Deliver intuitive, accessible, and delightful user experiences
- Reduce design-to-development rework through clear specifications
- Advocate for the end user in every stage of the project lifecycle

### Typical Communication
- Design reviews and critique sessions with Product Managers and Developers
- Prototype walkthroughs before sprint kickoff
- Usability test results and design rationale documented in design specs
- PR reviews for UI-facing changes

### Interactions with Existing Roles
- **Developers**: Provide design specs, answer implementation questions, and review UI PRs for fidelity.
- **Product Managers**: Translate product goals into user flows and validate designs against success metrics.
- **Project Managers**: Flag design-related risks (e.g., scope creep from design changes) and coordinate design milestones.

---

## DevOps / Platform Engineer

### Role Summary
DevOps / Platform Engineers build and maintain the CI/CD pipelines, infrastructure, deployment tooling, and observability systems that enable teams to deliver reliably and frequently.

### Responsibilities
- Design, implement, and maintain CI/CD pipelines
- Manage cloud infrastructure, environments (dev, staging, production), and configuration management
- Implement automated deployment, rollback, and disaster-recovery mechanisms
- Integrate security scanning, dependency checks, and secrets management into pipelines
- Establish and monitor observability (logging, metrics, alerts)
- Support on-call rotation and production incident response

### Goals
- Maximize deployment frequency while minimizing change failure rate
- Ensure environment parity and reproducibility across dev, staging, and production
- Reduce time-to-restore after incidents

### Typical Communication
- Infrastructure runbooks and pipeline documentation
- Deployment and incident post-mortems
- On-call handoffs and alert triage channels
- Architecture and capacity planning discussions

### Interactions with Existing Roles
- **Developers**: Provide tooling and guidance for local environments, CI integration, and deployment workflows; review infrastructure-related PRs.
- **QA Engineers**: Support test environment provisioning and automated test integration in CI pipelines.
- **Release Manager**: Coordinate deployment windows, pipeline health, and environment readiness.
- **Security Lead**: Implement pipeline-level security controls, scanning gates, and secrets management.

---

## Security Lead

### Role Summary
The Security Lead (also referred to as Security Champion in smaller teams) ensures that security is embedded throughout the project lifecycle — from planning through deployment and incident response. They act as the primary point of accountability for security risk assessment, policy compliance, and incident coordination.

### Responsibilities
- Define and communicate security requirements and threat models
- Review architecture, design, and code changes for security implications
- Ensure security scanning tools (SAST, DAST, dependency scanning) are integrated into CI
- Maintain the security incident runbook and coordinate security on-call
- Conduct or coordinate security risk assessments and penetration testing
- Track and prioritize security vulnerabilities in the risk register
- Ensure compliance with relevant standards and policies (e.g., GDPR, SOC 2)

### Goals
- Shift security left: identify and address risks as early as possible
- Minimize the attack surface and reduce mean-time-to-remediate vulnerabilities
- Maintain a clear, actionable security posture visible to leadership

### Typical Communication
- Security review gates at architecture, code review, and pre-release stages
- Security findings reports and remediation tracking
- Incident communications and post-mortems
- Risk register updates (security-related items)

### Interactions with Existing Roles
- **Developers**: Provide security guidance, review code for vulnerabilities, and support remediation of security findings.
- **DevOps / Platform Engineers**: Define and enforce pipeline security controls, secrets management policies, and environment hardening.
- **Project Managers**: Flag security risks in the risk register; block releases if critical vulnerabilities are unresolved.
- **Product Managers**: Communicate the impact of security requirements on scope and timelines; align on risk acceptance decisions.

---

## Release Manager

### Role Summary
The Release Manager coordinates release scheduling, manages deployment logistics, and owns stakeholder communication around each release. They act as the single point of accountability for ensuring releases go out safely, predictably, and with minimal disruption.

### Responsibilities
- Maintain the release calendar and coordinate release windows with stakeholders and DevOps
- Ensure all pre-release requirements (acceptance criteria met, CI green, release notes drafted) are complete
- Facilitate go/no-go decisions before deployments
- Communicate release plans, release notes, and post-deployment status to stakeholders
- Coordinate rollback decisions during incidents and own incident communication
- Own post-release verification and close-out reporting

### Goals
- Release on schedule with minimal incidents and zero surprises to stakeholders
- Ensure each release is fully documented and verifiable
- Continuously improve the release process based on retrospective learnings

### Typical Communication
- Release announcements and release notes to stakeholders and support teams
- Go/no-go meeting agendas and sign-off records
- Post-deployment verification reports
- Rollback and incident communications during or after deployment

### Interactions with Existing Roles
- **Developers**: Confirm all PRs are merged, acceptance criteria met, and release branches are ready.
- **QA Engineers**: Obtain QA sign-off and confirm all test gates are passed before the go/no-go decision.
- **DevOps / Platform Engineers**: Coordinate deployment execution, environment health checks, and rollback readiness.
- **Project Managers**: Align on release timelines, surface blockers early, and co-own stakeholder communications.
- **Stakeholders / Sponsors**: Communicate release status, expected impact, and any scope changes before and after deployment.

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

