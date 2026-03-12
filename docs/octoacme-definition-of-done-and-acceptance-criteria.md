# OctoAcme — Definition of Done & Acceptance Criteria

## Purpose
Provide a shared, reusable standard for when work is "done" and how to write clear, testable acceptance criteria. Consistent DoD and AC reduce ambiguity, prevent rework, and make quality expectations explicit across all roles.

---

## Definition of Done (DoD)

The Definition of Done is a team-level checklist that every work item must satisfy before it is considered complete. It applies to all user stories, features, and bug fixes unless a specific item is explicitly waived with justification.

### Default DoD Checklist

**Code Quality**
- [ ] Code implemented and peer-reviewed (minimum one approval on the PR)
- [ ] PR description includes a link to the related issue and a summary of changes
- [ ] No unresolved review comments before merge

**Testing**
- [ ] Unit tests written for new logic (minimum coverage threshold met per repo policy)
- [ ] Integration tests updated or added where applicable
- [ ] End-to-end / smoke tests pass for affected critical flows
- [ ] All automated tests passing in CI (no skipped tests without justification)

**Security**
- [ ] Security scan (SAST / dependency scan) passed in CI with no new critical or high findings
- [ ] No secrets or credentials committed to the repository

**Documentation**
- [ ] Inline code comments added for non-obvious logic
- [ ] Public API changes reflected in relevant documentation
- [ ] Changelog or release notes entry drafted (if applicable)

**QA Sign-off**
- [ ] Manual QA completed for user-facing features (QA Engineer sign-off)
- [ ] All acceptance criteria verified and checked off

**Deployment Readiness**
- [ ] Feature flag or rollout strategy documented (if applicable)
- [ ] Dependent services or migrations identified and coordinated

---

## Acceptance Criteria (AC) Guidelines

Acceptance Criteria are conditions that a specific work item must meet to be accepted by the Product Manager and QA Engineer. They should be written **before** development begins.

### AC Format

Use **Given / When / Then** (Gherkin-style) or a **bulleted list of conditions** — choose the format that is clearest for the work item.

**Gherkin-style example:**
```
Given a logged-in user on the dashboard
When they click "Export Report"
Then a CSV file is downloaded containing all items from the current filtered view
And the download completes within 5 seconds
```

**Bulleted-list example:**
```
- The export button is visible only to users with the "Editor" role or higher.
- Exported CSV includes columns: ID, Title, Status, Owner, Created Date.
- If no items match the filter, an empty CSV with headers is downloaded (not an error).
- Button is disabled and shows a loading spinner during export.
```

### AC Writing Checklist
- [ ] Criteria are **testable** — a tester can verify pass/fail without ambiguity
- [ ] Criteria address the **happy path** (expected behavior)
- [ ] Criteria address **edge cases** and error states where relevant
- [ ] Criteria are **independent** — each condition can be verified separately
- [ ] Criteria are agreed upon by **Product Manager, Developer, and QA Engineer** before sprint start
- [ ] Criteria are included in the **PR description** and referenced in the related issue

---

## Roles & Responsibilities for DoD / AC

| Role | Responsibility |
|------|----------------|
| Product Manager | Author initial acceptance criteria; approve final AC |
| QA Engineer | Review AC for testability; verify all AC met before sign-off |
| Developer | Implement to AC; self-verify DoD checklist before requesting review |
| Project Manager | Ensure DoD and AC are defined before work enters sprint |
| UX Designer | Contribute AC for UX/accessibility requirements on UI-facing work |

---

## Related Documents
- [OctoAcme Roles & Personas](octoacme-roles-and-personas.md)
- [OctoAcme Project Planning](octoacme-project-planning.md)
- [OctoAcme Execution & Tracking](octoacme-execution-and-tracking.md)
- [OctoAcme Release & Deployment Guide](octoacme-release-and-deployment.md)
