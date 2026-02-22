# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

**See also:**
- [Change Control Checklist](octoacme-change-control-checklist.md)
- [Quality Gates Checklist](octoacme-quality-gates-checklist.md)

---

## Existing Roles

### Developers

#### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

#### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

#### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

#### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

### Product Managers

#### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

#### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

#### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

#### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

### Project Managers

#### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

#### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

#### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

#### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## New Roles

### Project Sponsor

#### Purpose
The Project Sponsor provides strategic direction and executive backing for the project. They ensure the initiative aligns with organizational goals and have final authority on funding, scope trade-offs, and escalated decisions.

#### Core Responsibilities
- Champion the project at the executive level and secure necessary funding
- Approve the project charter, major milestones, and scope changes
- Remove organizational blockers that are beyond the Project Manager's authority
- Review and accept key deliverables at phase gates
- Ensure strategic alignment throughout the project lifecycle

#### Key Interactions
- **Project Manager:** Receives regular status updates; consulted on escalated risks and scope changes
- **Product Manager:** Aligns product direction with business strategy
- **Stakeholder Engagement Coordinator:** Informed of stakeholder concerns requiring executive intervention
- **Change Control Manager:** Approves high-impact change requests
- **Decision points:** Go/no-go at initiation gate; approval of significant scope or budget changes

#### Inputs / Outputs / Artifacts
- **Inputs:** Project charter, risk register, milestone reports, change requests
- **Outputs:** Signed-off project charter, approved change requests, executive communications
- **Artifacts owned:** Project mandate, budget approvals

---

### Change Control Manager

#### Purpose
The Change Control Manager governs all proposed changes to project scope, schedule, cost, or quality. They ensure changes are evaluated consistently and that approvals are obtained before implementation.

#### Core Responsibilities
- Maintain and operate the change request process
- Assess impact of proposed changes on scope, time, cost, risk, and compliance
- Coordinate change review boards and obtain required approvals
- Communicate approved and rejected changes to affected stakeholders
- Update project documentation and plans to reflect approved changes
- Track change request status and SLA adherence

#### Key Interactions
- **Project Sponsor:** Escalates high-impact changes for approval
- **Project Manager:** Collaborates on schedule and resource impacts
- **Compliance Specialist:** Validates regulatory implications of changes
- **Developers:** Gathers technical impact estimates
- **Decision points:** Change approval board meetings; SLA checkpoints

#### Inputs / Outputs / Artifacts
- **Inputs:** Change proposals from any team member, project baseline documents
- **Outputs:** Approved or rejected change requests with rationale, updated project baselines
- **Artifacts owned:** Change log, [Change Control Checklist](octoacme-change-control-checklist.md)

---

### Quality Assurance Lead

#### Purpose
The Quality Assurance Lead ensures that all project deliverables meet defined quality standards before they progress to the next phase or are released to production. They establish quality gates, oversee testing activities, and facilitate process reviews.

#### Core Responsibilities
- Define quality criteria and acceptance standards for each project phase
- Plan and oversee testing activities (unit, integration, UAT, regression)
- Manage the quality gate process and sign off on phase transitions
- Identify and track defects; coordinate resolution with Developers
- Facilitate process improvement reviews to reduce recurring defects
- Report quality metrics and status to the Project Manager

#### Key Interactions
- **Developers:** Reviews test plans, works to resolve defects
- **Project Manager:** Reports quality status and gate outcomes; flags risks from quality gaps
- **Stakeholder Engagement Coordinator:** Coordinates user acceptance testing (UAT) with business stakeholders
- **Compliance Specialist:** Ensures quality processes satisfy regulatory requirements
- **Decision points:** Phase-gate sign-offs; release readiness approval

#### Inputs / Outputs / Artifacts
- **Inputs:** Acceptance criteria, test plans, defect reports, compliance requirements
- **Outputs:** Test results, quality gate decisions, defect logs, process improvement recommendations
- **Artifacts owned:** [Quality Gates Checklist](octoacme-quality-gates-checklist.md), test reports

---

### Stakeholder Engagement Coordinator

#### Purpose
The Stakeholder Engagement Coordinator manages communication plans and ensures that stakeholder needs, concerns, and feedback are actively addressed throughout the project lifecycle. They act as the bridge between the project team and its broader audience.

#### Core Responsibilities
- Identify and maintain the stakeholder register
- Develop and execute the communication plan
- Facilitate stakeholder meetings, workshops, and feedback sessions
- Escalate unresolved stakeholder concerns to the Project Sponsor or Project Manager
- Coordinate user acceptance testing (UAT) participation with business stakeholders
- Manage change communication to affected parties

#### Key Interactions
- **Project Sponsor:** Briefs on stakeholder sentiment and escalations
- **Project Manager:** Aligns communication schedule with project milestones
- **Quality Assurance Lead:** Coordinates UAT sessions and collects business feedback
- **Change Control Manager:** Communicates approved changes to stakeholders
- **Decision points:** Stakeholder sign-off on requirements; UAT exit criteria

#### Inputs / Outputs / Artifacts
- **Inputs:** Project plan, milestone schedule, change notifications, stakeholder feedback
- **Outputs:** Communication plan, stakeholder register, meeting summaries, UAT feedback reports
- **Artifacts owned:** Stakeholder register, communication plan

---

### Compliance Specialist

#### Purpose
The Compliance Specialist monitors the project for adherence to applicable regulatory, legal, and internal policy requirements. They provide guidance on compliance risks and ensure that deliverables and processes meet required standards.

#### Core Responsibilities
- Identify applicable regulatory and policy requirements at project initiation
- Review project artifacts (designs, processes, release notes) for compliance gaps
- Advise on risk mitigation strategies related to regulatory obligations
- Validate that change requests do not introduce compliance violations
- Support audits and produce compliance evidence as needed
- Stay current on regulatory changes and communicate impacts to the project team

#### Key Interactions
- **Project Sponsor:** Reports on compliance exposure and regulatory risk
- **Change Control Manager:** Reviews proposed changes for compliance implications
- **Quality Assurance Lead:** Ensures quality processes satisfy compliance requirements
- **Project Manager:** Provides compliance inputs to the risk register
- **Decision points:** Compliance review at phase gates; approval of changes with regulatory impact

#### Inputs / Outputs / Artifacts
- **Inputs:** Project scope, design documents, change requests, regulatory guidance
- **Outputs:** Compliance assessment reports, risk register inputs, audit evidence
- **Artifacts owned:** Compliance checklist, regulatory requirements log

---

## RACI — Common Project Management Activities

The table below maps each role to its level of accountability for common PM activities.

**Legend:** R = Responsible, A = Accountable, C = Consulted, I = Informed
**Column abbreviation:** "QA Lead" = Quality Assurance Lead

| Activity | Project Sponsor | Project Manager | Product Manager | Change Control Manager | QA Lead | Stakeholder Engagement Coordinator | Compliance Specialist | Developer |
|---|---|---|---|---|---|---|---|---|
| **Initiation / Charter approval** | A | R | C | I | I | C | C | I |
| **Planning (scope, schedule, resources)** | A | R | C | C | C | C | C | C |
| **Execution / Sprint delivery** | I | A | C | I | C | I | I | R |
| **Change control** | A (high impact) | C | C | R/A | C | I | C | C |
| **Release / Deployment** | I | A | R | C | R | C | C | R |
| **Retrospective / Continuous improvement** | I | R | C | I | C | C | I | C |
| **Risk escalation** | A | R | C | C | C | C | C | I |
| **Stakeholder communication** | C | R | C | I | I | R/A | I | I |
| **Compliance review** | A | C | I | C | C | I | R | I |
| **Quality gate sign-off** | I | A | C | I | R | C | C | I |

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

