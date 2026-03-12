# OctoAcme — Project Kickoff Checklist

## Purpose
Ensure every project starts with a well-structured kickoff that aligns the team, confirms roles, and surfaces early risks. Use this checklist to prepare for and conduct the kickoff meeting, and to verify all pre-conditions are in place before execution begins.

---

## Pre-Kickoff Preparation (Project Manager)

- [ ] Project Charter / One-pager drafted and shared with attendees at least 48 hours before the meeting
- [ ] Attendee list confirmed (see Required Attendance below)
- [ ] Meeting invite sent with agenda attached
- [ ] Communication channels set up (e.g., Slack channel, mailing list)
- [ ] Project board / repository created and accessible to the team
- [ ] Initial backlog items drafted (or at minimum, epics / high-level scope captured)
- [ ] RAID log created from the [RAID Log Template](octoacme-raids-log-template.md) with initial known risks

---

## Required Attendance

| Role | Required? | Notes |
|------|-----------|-------|
| Project Manager | ✅ Required | Facilitates the meeting |
| Product Manager | ✅ Required | Presents product vision and outcomes |
| Tech Lead / Developers (representative) | ✅ Required | Confirms technical feasibility and initial estimates |
| QA Engineer | ✅ Required | Reviews acceptance and quality approach |
| Sponsor / Key Stakeholders | ✅ Required | Provides business context and approves charter |
| UX Designer | ⬜ If applicable | Required if UX work is in scope |
| DevOps / Platform Engineer | ⬜ If applicable | Required if infrastructure setup is in scope |
| Security Lead | ⬜ If applicable | Required if security requirements are in scope |
| Release Manager | ⬜ If applicable | Required if release planning is discussed |

---

## Kickoff Agenda (suggested 60–90 minutes)

1. **Welcome & Introductions** (5 min)
   - Brief introductions if the group is new to each other

2. **Project Overview** (10 min) — Product Manager
   - Problem statement and customer context
   - Business goals and success metrics
   - High-level scope (in scope / out of scope)

3. **Roles & Responsibilities** (10 min) — Project Manager
   - Confirm who owns what using the [Roles & Personas](octoacme-roles-and-personas.md) guide
   - Clarify escalation paths and decision-making authority

4. **Timeline & Milestones** (10 min) — Project Manager
   - High-level release plan and key milestones
   - Sprint cadence and demo schedule
   - Hard deadlines or external constraints

5. **Technical Approach & Feasibility** (15 min) — Tech Lead
   - Architecture overview (if new)
   - Integration points and dependencies
   - Initial technical risks

6. **Quality & Security Expectations** (10 min) — QA Engineer / Security Lead
   - Definition of Done overview (see [DoD & Acceptance Criteria](octoacme-definition-of-done-and-acceptance-criteria.md))
   - Test strategy overview
   - Security requirements (if applicable)

7. **Risks, Assumptions & Dependencies** (10 min) — All
   - Walk through initial RAID log (see [RAID Log Template](octoacme-raids-log-template.md))
   - Open floor for the team to raise early concerns

8. **Communication & Process** (5 min) — Project Manager
   - Meeting cadence (standups, weekly sync, demos)
   - Communication channels and escalation path
   - Documentation conventions and where to find things

9. **Q&A and Next Steps** (5 min)
   - Open questions
   - Confirm action items and owners with due dates

---

## Post-Kickoff Actions (Project Manager)

- [ ] Meeting notes published to the team within 24 hours
- [ ] Action items captured with owners and due dates
- [ ] RAID log updated with items raised during the meeting
- [ ] Project Charter finalized and signed off by Sponsor
- [ ] Team added to all relevant tools (project board, repo, communication channels)
- [ ] Sprint planning meeting scheduled

---

## Related Documents
- [OctoAcme Roles & Personas](octoacme-roles-and-personas.md)
- [OctoAcme Project Planning](octoacme-project-planning.md)
- [OctoAcme Definition of Done & Acceptance Criteria](octoacme-definition-of-done-and-acceptance-criteria.md)
- [OctoAcme RAID Log Template](octoacme-raids-log-template.md)
- [OctoAcme Project Initiation](octoacme-project-initiation.md)
