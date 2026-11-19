# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

Not every project needs every persona. Project teams should assign one accountable person or a clearly defined role for each applicable area, without changing the core ownership of Developers, Product Managers, or Project Managers.

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

## QA/Testing Lead

### Role Summary
Owns the test strategy, quality gates, and overall confidence in releases. This role verifies quality expectations while Developers remain responsible for implementing and testing their work.

### Responsibilities
- Define test scope, strategy, environments, entry criteria, and quality gates
- Review acceptance criteria for testability and coverage
- Coordinate functional, integration, performance, accessibility, and exploratory testing
- Track defects and recommend release or exception decisions
- Maintain test evidence and quality dashboards

### Goals
- Prevent defects from reaching production
- Make quality risks and trade-offs visible
- Establish a repeatable, proportionate release-quality process

### Typical Interactions
- **Developers:** Collaborate on acceptance criteria, testability, automation, defect reproduction, and fixes. Developers own implementation quality; QA/Testing owns independent quality strategy and validation.
- **Product Managers:** Agree on test coverage, acceptance expectations, and user-impact trade-offs. Product Managers make value and scope decisions; QA/Testing advises on quality consequences.
- **Project Managers:** Provide quality status, risks, and release-readiness evidence for schedules and go/no-go planning. Escalate unresolved quality gates or critical defects through the recorded risk process.
- **Release/DevOps Lead:** Coordinate release environments, smoke testing, rollback validation, and production evidence.

---

## UX/Design Lead

### Role Summary
Leads user research and interaction design to ensure proposed solutions are understandable, usable, and consistent.

### Responsibilities
- Define discovery needs and plan user research
- Create interaction designs, prototypes, and design specifications
- Establish usability and accessibility expectations
- Validate designs with users and delivery teams
- Maintain design constraints and relevant design-system decisions

### Goals
- Improve usability and task success
- Reduce rework caused by unclear or infeasible designs
- Ensure accessibility and consistent experiences

### Typical Interactions
- **Developers:** Collaborate on feasibility, component behavior, implementation details, and design validation. Developers own technical implementation; UX/Design owns the interaction intent.
- **Product Managers:** Partner on problem framing, research, requirements, and prioritization of usability improvements. Product Managers decide scope and priority; UX/Design recommends the experience approach.
- **Project Managers:** Communicate design dependencies, review and validation cycles, and approval needs so they can be sequenced in delivery plans.
- **Stakeholder/Customer Representative:** Incorporate business and customer context into research and validate outcomes.

### Decision Ownership and Handoff
UX/Design approves design artifacts within its scope. Significant scope, value, or priority changes remain decisions for the Product Manager, with Project Manager facilitation of timing and dependency impacts.

---

## Release/DevOps Lead

### Role Summary
Owns release planning, deployment readiness, environment and automation strategy, and operational handoff. This role does not replace Developers' responsibility for correct and supportable implementation.

### Responsibilities
- Define deployment and rollback approaches
- Maintain CI/CD pipelines and environment readiness
- Plan releases, freeze windows, approvals, and operational handoffs
- Monitor release health and coordinate incident response procedures
- Track operational dependencies and capacity constraints

### Goals
- Make releases repeatable, observable, and reversible
- Minimize deployment failures and recovery time
- Provide a clear transition from delivery to operations

### Typical Interactions
- **Developers:** Coordinate build, configuration, observability, feature flags, migration readiness, and rollback requirements. Developers own application changes; Release/DevOps owns delivery mechanisms and readiness checks.
- **Product Managers:** Align release timing and rollout scope with product milestones and customer impact. Product Managers own rollout and scope decisions.
- **Project Managers:** Provide release dates, dependencies, operational risks, and approval status for plans and stakeholder updates.
- **QA/Testing Lead:** Coordinate environment availability and release smoke testing.

### Decision Ownership and Handoff
The Release/DevOps Lead owns deployment go/no-go recommendations within established controls. Actual scope and customer-impact decisions are escalated to the Product Manager; schedule and approval coordination remains with the Project Manager.

---

## Security/Compliance Lead

### Role Summary
Defines applicable security and compliance controls, advises delivery teams on risk, and coordinates approvals or exceptions.

### Responsibilities
- Identify security, privacy, regulatory, and compliance obligations
- Review designs and implementations for required controls
- Define evidence, testing, and approval requirements
- Maintain the risk and exception process
- Advise on incident, vulnerability, and remediation priorities

### Goals
- Reduce unacceptable security and compliance risk
- Make control obligations and exceptions explicit
- Preserve delivery progress without bypassing mandatory safeguards

### Typical Interactions
- **Developers:** Advise on threat models, secure implementation, remediation, and evidence. Developers implement controls; Security/Compliance validates whether required risk controls are met.
- **Product Managers:** Explain risk impact and feasible trade-offs so scope and launch decisions account for security and compliance constraints.
- **Project Managers:** Track approvals, exceptions, evidence, and deadlines in plans and escalation logs.
- **Release/DevOps Lead:** Coordinate deployment controls, access, audit requirements, and operational safeguards.

### Decision Ownership and Handoff
This role owns control requirements and exception recommendations within delegated authority. Final acceptance of residual risk or exceptions follows the organization's named approver; Project Managers ensure approval and timing are explicit, while Product Managers decide whether to proceed given accepted risk.

---

## Stakeholder/Customer Representative

### Role Summary
Provides business context, represents a defined stakeholder or customer group, and validates whether delivered outcomes meet real needs.

### Responsibilities
- Communicate customer or business context and constraints
- Review proposals, prototypes, outcomes, and acceptance evidence
- Surface priorities, policy needs, and impacts to affected groups
- Provide timely feedback and named approvals when delegated
- Avoid presenting personal preference as group consensus

### Goals
- Ensure solutions address representative needs
- Improve decision quality with timely context
- Keep feedback and acceptance expectations visible

### Typical Interactions
- **Developers:** Review demonstrations and technical constraints through interpretable acceptance examples. Developers own implementation feasibility and quality.
- **Product Managers:** Provide priority context, validate requirements and outcomes, and participate in discovery or feedback sessions. Product Managers remain accountable for backlog prioritization.
- **Project Managers:** Identify decision owners, communicate stakeholder impacts, and participate in agreed reviews or escalations.
- **UX/Design Lead:** Supply domain and customer context for research and validate designs.
- **Data/Analytics Lead:** Validate which outcomes matter and whether reported measures represent the intended customer or business impact.

### Decision Ownership and Handoff
This role provides evidence and approvals delegated to it. It does not replace the Product Manager's backlog decisions or the Project Manager's coordination responsibility.

---

## Data/Analytics Lead

### Role Summary
Defines measurement and reporting needs, data quality expectations, and outcome analysis for the project.

### Responsibilities
- Define success metrics, baselines, and instrumentation requirements
- Specify data definitions and reporting views
- Review data quality and interpretation
- Analyze outcomes and present actionable findings
- Identify measurement limitations and assumptions

### Goals
- Make success observable and comparable
- Connect delivery activity to customer and business outcomes
- Reduce decisions based on ambiguous or incomplete measures

### Typical Interactions
- **Developers:** Define event schemas, instrumentation, identifiers, and observability needs. Developers implement instrumentation; Data/Analytics owns metric definitions and analysis.
- **Product Managers:** Partner on success measures, experiments, and data-informed trade-offs. Product Managers own prioritization and value decisions.
- **Project Managers:** Define reporting cadence, dependencies, owners, and escalation points for missing or unreliable data.
- **Stakeholder/Customer Representative:** Confirm that reports and outcome measures reflect the stakeholder or customer perspective where applicable.

### Decision Ownership and Handoff
This role owns metric definitions and analysis interpretation within the agreed data model. It recommends changes based on evidence, but scope and priority decisions remain with the Product Manager.

---

## Cross-role Escalation and Handoffs

- The Project Manager maintains the risk, dependency, decision, and approval log and facilitates escalation when an issue crosses team boundaries or threatens agreed delivery.
- The Product Manager decides scope and prioritization trade-offs and escalates unresolved customer or business value conflicts.
- Developers own implementation decisions and technical feasibility; specialists advise and approve work only within their defined accountability.
- Specialist roles should document the evidence or criteria required for handoffs, such as test completion, design acceptance, release readiness, security approval, stakeholder acceptance, or analytics instrumentation readiness.
- Personas are assigned according to project need. One person may cover more than one role for a small project, but accountabilities and required approvals should remain explicit.

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- Teams should confirm applicable personas and named owners during project kickoff, revisiting the assignments when project scope or risk changes.


