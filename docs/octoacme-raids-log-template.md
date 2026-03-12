# OctoAcme — RAID Log Template

## Purpose
The RAID Log is a lightweight, structured tracker for **Risks, Assumptions, Issues, and Dependencies** throughout the project lifecycle. It complements the Risk Register by capturing a broader set of project factors that need monitoring and action. Review and update the RAID log at least weekly during the project sync.

---

## Definitions

| Category | Definition |
|----------|------------|
| **Risk** | An uncertain event or condition that, if it occurs, could have a negative impact on the project. Has not happened yet. |
| **Assumption** | A factor believed to be true for planning purposes. If proven false, it may affect scope, timeline, or quality. |
| **Issue** | A risk that has materialized or a problem that is actively impacting the project and requires resolution. |
| **Dependency** | An item, deliverable, or decision that the project relies on from an external team, system, or third party. |

---

## RAID Log — Risks

| ID | Description | Impact (H/M/L) | Likelihood (H/M/L) | Owner | Mitigation / Contingency | Status | Last Updated |
|----|-------------|----------------|---------------------|-------|--------------------------|--------|--------------|
| R-001 | _Example: Key backend developer unavailable during critical sprint_ | H | M | Project Manager | Cross-train a second developer; adjust sprint scope | Open | YYYY-MM-DD |
| R-002 | | | | | | | |

---

## RAID Log — Assumptions

| ID | Description | Basis / Source | Owner | Validation Method | Valid? | Last Updated |
|----|-------------|----------------|-------|-------------------|--------|--------------|
| A-001 | _Example: Third-party API will maintain current response times_ | Vendor SLA documentation | Tech Lead | Monitor API latency in staging | TBD | YYYY-MM-DD |
| A-002 | | | | | | |

---

## RAID Log — Issues

| ID | Description | Impact (H/M/L) | Owner | Resolution Actions | Target Date | Status | Last Updated |
|----|-------------|----------------|-------|--------------------|-------------|--------|--------------|
| I-001 | _Example: CI pipeline flaky tests blocking PRs_ | M | DevOps Engineer | Investigate test flakiness; add retry logic | YYYY-MM-DD | In Progress | YYYY-MM-DD |
| I-002 | | | | | | | |

---

## RAID Log — Dependencies

| ID | Description | Dependent On (Team/System) | Owner | Expected Date | Status | Notes |
|----|-------------|---------------------------|-------|---------------|--------|-------|
| D-001 | _Example: Authentication service upgrade required before login redesign_ | Platform Team | Project Manager | YYYY-MM-DD | Pending | Escalated to PM sync |
| D-002 | | | | | | |

---

## Usage Guidelines

- **Create the RAID log** at project kickoff and link it from the Project Charter.
- **Review at weekly sync**: Project Manager walks through open items; owners provide status updates.
- **Close items** promptly when resolved — do not delete them; mark Status as "Closed" and record the resolution date.
- **Escalate** unresolved high-impact items to the Sponsor or relevant stakeholder.

### Status Values
| Status | Meaning |
|--------|---------|
| Open | Identified; no mitigation or resolution in progress |
| In Progress | Mitigation or resolution actions are underway |
| Monitoring | Mitigation in place; being watched |
| Closed | Resolved, assumption validated, or dependency fulfilled |
| Accepted | Risk acknowledged and accepted (no further mitigation planned) |

---

## Roles & Responsibilities

| Role | Responsibility |
|------|----------------|
| Project Manager | Own and maintain the RAID log; facilitate weekly review |
| All team members | Raise new items as soon as identified |
| Item Owners | Keep their items updated with current status |
| Security Lead | Own security-related risks and issues |
| DevOps / Platform Engineer | Own infrastructure and pipeline-related dependencies and risks |
| Stakeholders / Sponsor | Review high-impact items; approve risk acceptance decisions |

---

## Related Documents
- [OctoAcme Roles & Personas](octoacme-roles-and-personas.md)
- [OctoAcme Risk Management & Communication](octoacme-risks-and-communication.md)
- [OctoAcme Project Planning](octoacme-project-planning.md)
- [OctoAcme Kickoff Checklist](octoacme-kickoff-checklist.md)
