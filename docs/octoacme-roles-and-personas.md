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
UX Designers define and validate user interactions, translate requirements into wireframes and prototypes, and ensure the product delivers a high-quality user experience.

### Responsibilities
- Create wireframes, mockups, and interactive prototypes
- Conduct and synthesize usability research and testing
- Define and maintain design guidelines and component libraries
- Review implementations for design fidelity and accessibility
- Advocate for user needs in backlog prioritization and sprint planning

### Goals
- Deliver intuitive, accessible, and delightful user experiences
- Reduce design-related rework through early prototyping and validation
- Maintain a consistent visual and interaction language across the product

### Typical Communication
- Design reviews and critiques with Developers and Product Managers
- Usability test findings shared with Product Managers and Project Managers
- Async comments in design tools (e.g., Figma) and PR reviews

### Interactions
- **Product Managers**: Collaborate on feature definition, success metrics, and user research planning.
- **Developers**: Provide design specifications, review implementations, clarify interaction behavior.
- **Project Managers**: Flag design-related blockers or scope changes; participate in sprint planning.
- **QA Lead**: Align on visual/accessibility acceptance criteria so QA can validate design fidelity.

---

## QA Lead / Test Lead

### Role Summary
The QA Lead owns the overall test strategy, coordinates manual and automated quality assurance, and acts as the quality gate before releases. Aligns with QA/Testing references across OctoAcme process docs.

### Responsibilities
- Define and maintain the test strategy and test plans
- Coordinate manual and automated testing across sprints and releases
- Define and review acceptance criteria and Definition of Done
- Report test outcomes, defect trends, and quality metrics
- Drive test automation coverage improvements

### Goals
- Prevent defects from reaching production
- Reduce regression risk through reliable automated test suites
- Provide clear, timely quality signals to the team

### Typical Communication
- Sprint planning and execution sync to align test scope
- Test summary reports shared with Project Managers and Product Managers
- Defect triage with Developers; release sign-off with Release Manager

### Interactions
- **Developers**: Collaborate on testability, review test coverage, coordinate defect fixes.
- **Product Managers**: Clarify acceptance criteria; share quality metrics that inform prioritization.
- **Project Managers**: Report test status and blockers; raise quality-related schedule risks.
- **UX Designer**: Validate design fidelity and accessibility against defined criteria.
- **Release Manager**: Provide final test sign-off before each release; coordinate smoke tests.
- **DevOps Engineer**: Integrate automated tests into CI/CD pipelines; align on test environments.

---

## DevOps Engineer / Platform Engineer

### Role Summary
DevOps Engineers manage CI/CD pipelines, infrastructure, and deployment automation to enable fast, reliable, and secure delivery. They are the operational backbone of the release process.

### Responsibilities
- Design, build, and maintain CI/CD pipelines and build automation
- Manage infrastructure-as-code and cloud/platform environments
- Monitor system health, performance, and reliability
- Automate build, test, deployment, and rollback workflows
- Enforce security and compliance requirements in pipelines

### Goals
- Maximize deployment frequency while minimizing failure rate
- Ensure platform stability and observability
- Reduce manual toil through automation

### Typical Communication
- Infrastructure change notifications to Developers and Release Manager
- Pipeline and monitoring alerts to on-call and Security Representative
- Platform documentation and runbooks in the project repo

### Interactions
- **Developers**: Provide tooling, pipelines, and environments; support local dev setup.
- **Release Manager**: Execute deployments; provide rollback playbooks and environment readiness checks.
- **QA Lead**: Configure and maintain test environments; integrate automated test suites into CI.
- **Security Representative**: Implement security scanning in pipelines; remediate pipeline-level findings.
- **Project Managers**: Communicate infrastructure risks, planned maintenance windows, and capacity constraints.

---

## Release Manager

### Role Summary
The Release Manager plans and orchestrates releases, coordinates cross-functional readiness, and ensures each deployment meets quality and communication standards.

### Responsibilities
- Maintain the release calendar and coordinate release windows
- Drive pre-release readiness reviews with QA Lead, DevOps Engineer, and Product Managers
- Ensure release notes, rollback plans, and runbooks are complete
- Communicate release scope and timing to stakeholders and Customer Support
- Coordinate go/no-go decisions and post-release verification

### Goals
- Deliver predictable, low-risk releases
- Ensure all stakeholders are informed and prepared before each release
- Minimize time-to-recovery for release-related incidents

### Typical Communication
- Release readiness meetings with QA Lead, DevOps Engineer, and Product Managers
- Release announcements to stakeholders, Customer Support, and Sales
- Post-release retrospective notes shared with Project Managers

### Interactions
- **Project Managers**: Align release milestones with project schedule; escalate go/no-go decisions.
- **Product Managers**: Confirm feature scope and release notes; coordinate stakeholder communications.
- **QA Lead**: Obtain test sign-off; coordinate smoke tests and rollback triggers.
- **DevOps Engineer**: Coordinate deployment execution, environment checks, and rollback procedures.
- **Customer Support Lead**: Brief support teams on new features, known issues, and escalation paths.
- **Security Representative**: Confirm no open critical security issues before release.

---

## Security Representative

### Role Summary
The Security Representative ensures that security and compliance requirements are integrated throughout the project lifecycle, from design through deployment and incident response. Aligns with security escalation references in `octoacme-risks-and-communication.md` and `octoacme-release-and-deployment.md`.

### Responsibilities
- Participate in threat modeling and security design reviews
- Review and triage security scan results from CI/CD pipelines
- Define and maintain the security incident runbook
- Evaluate release candidates for unresolved security risks
- Advise teams on secure coding practices and compliance requirements

### Goals
- Reduce security risk across the product and infrastructure
- Ensure security issues are identified and resolved before they reach production
- Maintain clear escalation paths for security incidents

### Typical Communication
- Security findings shared with Developers and DevOps Engineers
- Risk assessments and sign-offs communicated to Release Manager and Project Managers
- Incident notifications to stakeholders per the incident communication plan

### Interactions
- **Developers**: Provide secure coding guidance; review and help remediate security findings.
- **DevOps Engineer**: Integrate and tune security scanning tools in CI/CD; review infrastructure security.
- **Release Manager**: Provide security sign-off for each release; flag open critical findings.
- **Project Managers**: Raise security-related risks and dependencies; participate in risk register reviews.
- **Product Managers**: Advise on compliance and privacy requirements that affect feature design.

---

## Customer Support Lead

### Role Summary
The Customer Support Lead ensures the support team is prepared to handle user inquiries, escalations, and known issues associated with each release. They act as the voice of the customer in release and risk discussions.

### Responsibilities
- Review release notes and known issues before each deployment
- Brief the support team on new features, changes, and known issues
- Escalate customer-reported production issues to engineering teams
- Contribute customer feedback and issue trends to Product Managers
- Maintain support runbooks and FAQ documentation

### Goals
- Minimize customer-facing impact of releases and incidents
- Ensure support teams can respond quickly and accurately to post-release inquiries
- Surface recurring customer pain points to drive product improvements

### Typical Communication
- Pre-release briefings from the Release Manager
- Issue escalations to Project Managers and Developers
- Customer feedback summaries shared with Product Managers

### Interactions
- **Release Manager**: Receive release briefings; flag support-readiness concerns before go/no-go.
- **Product Managers**: Share customer feedback and pain points; influence backlog prioritization.
- **Project Managers**: Escalate high-impact customer issues; receive status updates during incidents.
- **Developers**: Collaborate on reproducing and resolving customer-reported defects.
- **Technical Writer**: Review and improve user-facing help content aligned with each release.

---

## Data Analyst / Analytics

### Role Summary
Data Analysts define, track, and interpret the success metrics that guide product decisions. They are the bridge between raw data and actionable product insights. Aligns with success metrics references in `octoacme-project-initiation.md` and `octoacme-project-management-overview.md`.

### Responsibilities
- Define and instrument success metrics in collaboration with Product Managers
- Build and maintain dashboards and data pipelines for project KPIs
- Analyze post-release data to evaluate feature impact
- Provide data-driven insights to inform backlog prioritization and roadmap decisions
- Surface anomalies and trends to relevant stakeholders

### Goals
- Enable data-informed product decisions
- Reduce time to insight for success metric review
- Ensure metrics are accurate, reliable, and actionable

### Typical Communication
- Metric review sessions with Product Managers and Project Managers
- Dashboard links and analysis summaries in project status updates
- Ad-hoc analysis requests from Product and Engineering teams

### Interactions
- **Product Managers**: Co-define success metrics; deliver post-release impact analysis.
- **Project Managers**: Provide data to support milestone reporting and risk assessments.
- **Developers**: Coordinate on instrumentation and data collection requirements.
- **DevOps Engineer**: Align on data pipeline reliability and observability infrastructure.

---

## Technical Writer

### Role Summary
Technical Writers create and maintain clear, accurate documentation for internal teams and end users. They ensure that documentation keeps pace with product changes and supports onboarding, support, and compliance needs. Aligns with documentation expectations referenced across OctoAcme process docs.

### Responsibilities
- Author and maintain user guides, API docs, runbooks, and release notes
- Review and improve existing process documentation for clarity and accuracy
- Coordinate doc reviews with Developers, Product Managers, and QA Lead
- Ensure documentation is updated as part of the Definition of Done
- Develop and maintain documentation templates and style guides

### Goals
- Reduce support load through high-quality, self-service documentation
- Ensure every release includes complete and accurate documentation
- Maintain a consistent documentation style and structure across the project

### Typical Communication
- Doc review requests to Developers and Product Managers for new features
- Release documentation delivered to Release Manager before each deployment
- Style guide and template updates shared with the broader team

### Interactions
- **Developers**: Gather technical details; conduct peer reviews of technical accuracy.
- **Product Managers**: Align on user-facing messaging and feature descriptions.
- **Release Manager**: Deliver finalized release notes and updated docs before release.
- **Customer Support Lead**: Collaborate on help content, FAQs, and support runbooks.
- **QA Lead**: Verify that documentation updates are included in the Definition of Done and tested.

---

## Stakeholder Groups

### Role Summary
Stakeholder Groups are functional teams or individuals — such as Sales, Legal/Compliance, and Executive Leadership — who have an interest in project outcomes and provide domain-specific inputs or approvals at key decision gates.

### Responsibilities
- Review project milestones and deliverables from a domain-specific perspective
- Provide timely feedback and approvals at defined decision gates
- Communicate business requirements, constraints, or blockers to the project team
- Receive and act on release communications relevant to their function

### Goals
- Ensure project outcomes align with business, legal, and customer objectives
- Enable timely decision-making to avoid project delays
- Maintain awareness of product changes that affect their function

### Typical Communication
- Monthly stakeholder updates from Project Managers
- Targeted briefings at major milestones (e.g., release readiness, go-live)
- Escalation paths for domain-specific concerns to Project or Product Managers

### Interactions
- **Product Managers**: Provide domain requirements; receive roadmap updates and trade-off explanations.
- **Project Managers**: Receive status updates; provide approvals at decision gates; surface blockers.
- **Release Manager**: Receive release scope and timing communications; provide domain go/no-go input.
- **Security Representative**: Engage on compliance and regulatory requirements.

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- For role interaction and accountability planning, use the [OctoAcme RACI & Role Handoff guide](./octoacme-raci-and-role-handoff.md).

