# OctoAcme — Change Control Checklist

## Purpose
Provide a lightweight, repeatable process for evaluating and approving proposed changes to a project's scope, schedule, cost, or quality baseline. This checklist is owned by the [Change Control Manager](octoacme-roles-and-personas.md#change-control-manager).

**See also:** [Roles & Personas](octoacme-roles-and-personas.md) | [Quality Gates Checklist](octoacme-quality-gates-checklist.md)

---

## What Constitutes a Change

A change request is required whenever a proposed action would alter any approved project baseline. Common triggers include:

- Addition, removal, or modification of in-scope features or deliverables
- Changes to milestones, delivery dates, or sprint commitments
- Changes to the approved budget or resource allocation
- Modifications to agreed-upon technical architecture or integration points
- New or revised regulatory or compliance obligations affecting the project
- Changes to agreed acceptance criteria or definition of done

> **Not a change:** Bug fixes, minor wording corrections, and purely internal implementation decisions that do not affect the agreed baseline do not require a formal change request.

---

## Change Request — Required Information

Every change request must capture the following before it is reviewed:

- [ ] **Requestor name and role**
- [ ] **Date submitted**
- [ ] **Change title / short description** (one sentence)
- [ ] **Detailed description of the proposed change** (what is changing and why)
- [ ] **Business justification** (customer need, regulatory requirement, risk reduction, etc.)
- [ ] **Priority** (Critical / High / Medium / Low)
- [ ] **Requested implementation date** (if applicable)
- [ ] **Supporting materials attached** (design mock-ups, emails, regulatory citations, etc.)

---

## Impact Assessment

Before approval, the Change Control Manager must assess the change across the following areas. Each area should be marked as **No Impact**, **Low**, **Medium**, or **High**.

### Scope
- [ ] Are any existing deliverables added, removed, or modified?
- [ ] Does the change introduce new dependencies or third-party integrations?
- [ ] Does it affect the Definition of Done or acceptance criteria?

### Schedule / Time
- [ ] Does it require additional effort that will delay any milestones?
- [ ] Will other in-flight work need to be re-sequenced or deprioritized?
- [ ] Is the requested date achievable given current capacity?

### Cost
- [ ] Does it require additional budget (tooling, licenses, headcount, infrastructure)?
- [ ] Will it change the total cost of ownership for the delivered system?

### Risk
- [ ] Does it introduce technical, delivery, or operational risk?
- [ ] Does it reduce an existing risk (and is that trade-off acceptable)?
- [ ] Is a rollback or mitigation plan required?

### Compliance
- [ ] Does the change affect data privacy, security posture, or regulatory obligations?
- [ ] Has the [Compliance Specialist](octoacme-roles-and-personas.md#compliance-specialist) been consulted?
- [ ] Are any audit artifacts or sign-offs needed?

---

## Approval Workflow and SLAs

| Priority | Review SLA | Approver(s) |
|---|---|---|
| Critical | 24 hours | Project Sponsor + Project Manager |
| High | 3 business days | Project Manager + Change Control Manager |
| Medium | 5 business days | Change Control Manager |
| Low | Next change board meeting | Change Control Manager |

### Approval steps

1. **Submit** — Requestor submits completed change request form.
2. **Triage** — Change Control Manager validates completeness and assigns priority (within 1 business day).
3. **Impact assessment** — Change Control Manager coordinates with impacted leads (Developer, QA Lead, Compliance Specialist) to complete the impact assessment.
4. **Review board** — Change Control Manager presents to the appropriate approver(s) per the table above.
5. **Decision** — Approved, Approved with conditions, Deferred, or Rejected. Decision recorded with rationale.
6. **Notification** — Change Control Manager notifies requestor and affected stakeholders of the decision.
7. **Implementation** — If approved, Project Manager incorporates the change into the project plan and baselines.
8. **Closure** — Change Control Manager marks the request as closed in the change log once implementation is verified.

---

## Communication Steps

- [ ] Notify requestor of triage outcome within the SLA window
- [ ] Communicate decision (and conditions, if any) to requestor and all impacted parties
- [ ] Update the project plan, risk register, and other affected artifacts
- [ ] Announce approved scope changes in the next team standup or stakeholder update
- [ ] Archive approved change request in the project repository (e.g., `docs/` or project board)
- [ ] Update release notes if the change affects a pending or future release

---

## Change Log Template

Track all requests in a simple table:

| ID | Title | Requestor | Submitted | Priority | Status | Decision | Decision Date |
|---|---|---|---|---|---|---|---|
| CR-001 | _example_ | _name_ | _date_ | High | Approved | Approved with conditions | _date_ |
