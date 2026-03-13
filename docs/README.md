# OctoAcme Project Management Documentation

Welcome to the OctoAcme Project Management Docs. This README provides a concise overview of the project management processes used by OctoAcme and quick links to each major workflow and process guide.

## Overview of OctoAcme Project Management Processes

OctoAcme runs projects with a lightweight, end-to-end lifecycle designed for iterative delivery and clear ownership. Work moves through five phases: **Initiation** (define the problem, objective, stakeholders, and success metrics), **Planning** (turn the initiative into a prioritized, estimated backlog with a Definition of Done and release plan), **Execution** (build, test, and review in small increments against acceptance criteria), **Release** (deploy with pre-release checklists, post-deploy verification, and rollback readiness), and **Close/Retrospective** (capture learnings and feed improvements back into the team's processes). Key artifacts supporting this lifecycle include a Project Charter/One-pager, sprint backlog items with acceptance criteria, a risk register, and retrospective action items.

Roles are explicitly defined to reduce ambiguity and improve decision-making speed. A named **Project Manager (PM)** coordinates delivery—managing schedules, risks, dependencies, and communications—while a **Product Manager (PdM)/Product Lead** defines outcomes, prioritizes the backlog, and measures success. **Developers** implement and test features, participate in estimation and code reviews, and surface technical risks. **QA/Testing** validates acceptance criteria and release readiness, and **Stakeholders** provide inputs and approvals at key project milestones. This clear separation of responsibilities supports both execution efficiency (PM ownership of process) and product impact (PdM ownership of outcomes).

Communication is structured around a predictable team rhythm with defined escalation paths. OctoAcme uses **daily standups** to surface progress and blockers, **weekly delivery syncs** between the PM and PdM to review progress and risks, and a **demo/review at the end of each sprint or milestone**. Status updates follow standardized templates covering progress, next steps, risks/blockers, and decisions needed. Risks and dependencies are tracked in a risk register and escalated in tiers—from team triage to PM-led cross-team resolution, and ultimately to sponsor-level escalation for business-impacting issues.

Quality assurance is embedded throughout implementation and release. The engineering workflow emphasizes **small pull requests** with clear descriptions (including issue links and acceptance criteria) and **passing CI** (tests, lint, and security scanning) before review, with at least one approval required before merging. Testing expectations scale with impact: **unit tests for new logic**, integration tests where needed, and **end-to-end smoke tests for critical flows** prior to release. Releases follow a checklist-driven approach—staging verification, production deploy via automation where possible, and post-deploy checks—with explicit rollback and incident guidance. Retrospectives close the loop by converting failures and frictions into measurable process improvements.

## Process Documents

| Document | Description |
|---|---|
| [Project Management Overview](./octoacme-project-management-overview.md) | Principles, core roles, key artifacts, and lifecycle at a glance |
| [Project Initiation Guide](./octoacme-project-initiation.md) | How to kick off a project: charter, stakeholders, problem statement |
| [Project Planning](./octoacme-project-planning.md) | Scope, backlog, milestones, risk, and dependency planning |
| [Execution & Tracking](./octoacme-execution-and-tracking.md) | Sprint workflow, PR practices, project board usage, and status reporting |
| [Risk Management & Communication](./octoacme-risks-and-communication.md) | Risk register, escalation tiers, and stakeholder communication templates |
| [Release & Deployment Guide](./octoacme-release-and-deployment.md) | Pre-release checklist, deployment steps, post-deploy verification, rollback |
| [Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md) | Retro format, action item tracking, and process improvement loop |
| [Roles & Personas](./octoacme-roles-and-personas.md) | Detailed responsibilities and goals for each role on the team |
