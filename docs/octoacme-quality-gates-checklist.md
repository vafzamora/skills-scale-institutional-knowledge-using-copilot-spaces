# OctoAcme — Quality Gates Checklist

## Purpose
Define the quality criteria, testing expectations, and sign-off requirements that must be satisfied before a project advances from one phase to the next. This checklist is owned by the [Quality Assurance Lead](octoacme-roles-and-personas.md#quality-assurance-lead).

**See also:** [Roles & Personas](octoacme-roles-and-personas.md) | [Change Control Checklist](octoacme-change-control-checklist.md)

---

## Gate 1 — Initiation → Planning

**Purpose:** Confirm that the project is sufficiently defined to begin detailed planning.

### Quality Criteria
- [ ] Project one-pager is complete (problem statement, goals, success metrics)
- [ ] Primary stakeholders identified and initial communication plan drafted
- [ ] High-level timeline and milestones defined
- [ ] Initial risk list documented
- [ ] Resource needs and team roles identified

### Validation
- [ ] Product Manager or Project Sponsor has reviewed and accepted the one-pager
- [ ] No blocking dependencies unresolved

### Sign-off Required
| Role | Sign-off |
|---|---|
| Project Sponsor | ☐ |
| Project Manager | ☐ |
| Product Manager | ☐ |

---

## Gate 2 — Planning → Execution

**Purpose:** Confirm that planning is complete and the team is ready to begin building.

### Quality Criteria
- [ ] Detailed project plan with milestones approved
- [ ] Scope, acceptance criteria, and Definition of Done documented
- [ ] Risks assessed and mitigation plans in place
- [ ] Architecture and technical design reviewed and accepted
- [ ] Test plan drafted (unit, integration, UAT, regression)
- [ ] Compliance requirements identified and incorporated into plan

### Validation
- [ ] QA Lead has reviewed and accepted the test plan
- [ ] Compliance Specialist has confirmed no outstanding regulatory blockers
- [ ] All critical dependencies resolved or tracked with mitigation

### Sign-off Required
| Role | Sign-off |
|---|---|
| Project Manager | ☐ |
| QA Lead | ☐ |
| Compliance Specialist | ☐ |

---

## Gate 3 — Execution Milestone Reviews (per sprint/iteration)

**Purpose:** Validate incremental quality at regular intervals during execution.

### Quality Criteria
- [ ] All committed user stories or tasks meet the Definition of Done
- [ ] No open critical or high-severity defects
- [ ] Test coverage meets or exceeds agreed threshold
- [ ] Code review completed for all merged changes
- [ ] Updated acceptance criteria validated by Product Manager or QA Lead

### Testing / Validation Expectations
- [ ] Unit tests pass with adequate coverage
- [ ] Integration tests pass for affected modules
- [ ] Regression suite passes (or regressions are tracked with resolution plan)
- [ ] Performance benchmarks met (if applicable)
- [ ] Security scan shows no new critical or high findings

### Sign-off Required
| Role | Sign-off |
|---|---|
| QA Lead | ☐ |
| Project Manager | ☐ |

---

## Gate 4 — Execution → Release (Pre-Release Readiness)

**Purpose:** Confirm the release candidate meets all quality, compliance, and operational standards before deployment to production.

### Quality Criteria
- [ ] All acceptance criteria for release scope met and verified
- [ ] No open critical defects; all high-severity defects resolved or deferred by agreement
- [ ] Full regression suite passes
- [ ] User acceptance testing (UAT) completed with business stakeholder sign-off
- [ ] Performance and load testing completed (if applicable)
- [ ] Security review completed with no unmitigated critical findings
- [ ] Release notes drafted and reviewed

### Testing / Validation Expectations
- [ ] Staging environment deployment successful
- [ ] Smoke tests pass in staging
- [ ] All automated pipelines (CI/CD) green
- [ ] Rollback plan documented and validated
- [ ] Monitoring and alerting configured for new features or changes

### Compliance Validation
- [ ] Compliance Specialist has confirmed all regulatory requirements are satisfied
- [ ] Required audit artifacts or evidence collected and stored
- [ ] Data privacy review completed (if applicable)

### Sign-off Required
| Role | Sign-off |
|---|---|
| QA Lead | ☐ |
| Compliance Specialist | ☐ |
| Project Manager | ☐ |
| Product Manager | ☐ |
| Stakeholder Engagement Coordinator (UAT exit) | ☐ |

---

## Gate 5 — Post-Release Verification

**Purpose:** Confirm the release was successful and the system is stable in production.

### Quality Criteria
- [ ] Post-deploy smoke tests pass in production
- [ ] Key metrics and monitoring dashboards show expected behavior
- [ ] No critical production incidents triggered by the release within agreed stabilization window
- [ ] Release announcement sent to stakeholders

### Validation
- [ ] QA Lead confirms post-deploy validation complete
- [ ] Project Manager confirms stakeholder communication sent

### Sign-off Required
| Role | Sign-off |
|---|---|
| QA Lead | ☐ |
| Project Manager | ☐ |

---

## Gate 6 — Retrospective / Close

**Purpose:** Validate that the project is formally closed and learnings are captured.

### Quality Criteria
- [ ] Retrospective held and action items documented
- [ ] All open defects triaged (resolved, deferred, or accepted as known issues)
- [ ] Final project documentation archived
- [ ] Lessons learned shared with relevant teams
- [ ] Process improvement items logged in backlog or improvement tracker

### Sign-off Required
| Role | Sign-off |
|---|---|
| Project Manager | ☐ |
| QA Lead | ☐ |

---

## Defect Severity Definitions

| Severity | Definition | Max Open Allowed at Release Gate |
|---|---|---|
| Critical | System unavailable or data loss/corruption | 0 |
| High | Major feature broken with no workaround | 0 |
| Medium | Feature degraded; workaround exists | Tracked with mitigation |
| Low | Minor cosmetic or usability issue | Tracked |
