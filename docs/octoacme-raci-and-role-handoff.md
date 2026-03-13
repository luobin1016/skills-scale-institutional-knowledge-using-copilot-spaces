# OctoAcme — RACI & Role Handoff Guide

This document provides a RACI-lite template for project accountability and a role handoff checklist for release readiness. Use it alongside [`octoacme-roles-and-personas.md`](./octoacme-roles-and-personas.md).

---

## RACI-Lite Template

Use this template to assign accountability for key activities in your project. Populate one row per major activity or phase.

**Key:**
- **R** = Responsible (does the work)
- **A** = Accountable (owns the outcome; final decision-maker)
- **C** = Consulted (provides input before decision/action)
- **I** = Informed (notified of outcome)

| Activity / Phase | Project Mgr | Product Mgr | Developer | UX Designer | QA Lead | DevOps Eng | Release Mgr | Security Rep | Support Lead | Data Analyst | Tech Writer | Stakeholders |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| Project initiation & charter | A | C | I | I | I | I | I | C | I | C | I | C |
| Requirements & backlog definition | C | A | C | C | I | I | I | C | C | C | I | C |
| UX design & prototyping | I | C | C | A | C | I | I | I | I | I | I | I |
| Sprint planning | A | C | R | C | C | I | I | I | I | I | I | I |
| Feature development | I | I | A | C | C | C | I | C | I | I | I | I |
| Test planning & execution | I | C | C | C | A | C | I | C | I | I | I | I |
| Security review | C | C | C | I | C | C | C | A | I | I | I | I |
| Release planning | A | C | I | I | C | C | R | C | C | I | C | I |
| Deployment execution | I | I | C | I | C | R | A | C | I | I | I | I |
| Release communication | C | C | I | I | I | I | A | I | R | I | R | I |
| Post-release metrics review | C | A | I | I | I | I | I | I | C | R | I | I |
| Retrospective facilitation | A | C | R | R | R | R | R | C | C | C | C | I |

> **How to use:** Copy this table into your project's documentation, adjust roles to match your team composition, and fill in R/A/C/I for each activity. Ensure every row has exactly one **A**.

---

## Release Readiness Handoff Checklist

Use this checklist before each release to ensure all roles have completed their responsibilities and handed off to the next. Reference the [Release & Deployment Guide](./octoacme-release-and-deployment.md) for deployment steps.

### Development Sign-off (Developers)
- [ ] All planned features and fixes are merged to the release branch
- [ ] Code reviewed and approved per PR policy
- [ ] Unit and integration tests passing in CI
- [ ] No known critical defects pending

### Design Sign-off (UX Designer)
- [ ] Implemented features reviewed against design specifications
- [ ] Accessibility requirements validated
- [ ] Any design deviations documented and accepted by Product Manager

### Quality Sign-off (QA Lead)
- [ ] Test plan executed; results documented
- [ ] All critical and high-priority defects resolved or formally accepted
- [ ] Acceptance criteria verified for all in-scope features
- [ ] Regression suite passing
- [ ] Smoke test scripts prepared for post-deploy verification

### Security Sign-off (Security Representative)
- [ ] Security scans complete with no unresolved critical findings
- [ ] Threat model reviewed for new features (if applicable)
- [ ] Compliance requirements confirmed as met
- [ ] Incident runbook updated if new attack surfaces introduced

### Infrastructure Sign-off (DevOps Engineer)
- [ ] Deployment pipeline tested and ready
- [ ] Target environments (staging, production) verified and healthy
- [ ] Rollback procedure documented and tested
- [ ] Monitoring and alerting configured for new features

### Documentation Sign-off (Technical Writer)
- [ ] Release notes drafted and reviewed
- [ ] User-facing documentation updated for all new or changed features
- [ ] Support runbooks updated as needed
- [ ] Documentation included in Definition of Done review

### Support Readiness (Customer Support Lead)
- [ ] Support team briefed on new features, changes, and known issues
- [ ] Help articles and FAQs updated or queued for publish
- [ ] Escalation paths confirmed with engineering team
- [ ] Support tooling (tags, categories) updated for new features

### Release Go/No-Go (Release Manager)
- [ ] All sign-off items above are complete
- [ ] Release notes finalized and approved by Product Manager
- [ ] Deployment window confirmed with DevOps Engineer
- [ ] Stakeholder communication drafted and scheduled
- [ ] Go/No-Go decision recorded with attendees, date, and outcome

---

## Role Interaction Summary

The following summarizes key handoff points across roles during a typical project lifecycle. For full role definitions, see [`octoacme-roles-and-personas.md`](./octoacme-roles-and-personas.md).

| From | To | Handoff / Trigger |
|---|---|---|
| Product Manager | UX Designer | Approved feature brief / user story |
| UX Designer | Developer | Final design spec and assets |
| Developer | QA Lead | Feature branch / PR ready for testing |
| QA Lead | Release Manager | Test sign-off / go recommendation |
| DevOps Engineer | Release Manager | Environment readiness confirmation |
| Security Representative | Release Manager | Security sign-off |
| Technical Writer | Release Manager | Final release notes and updated docs |
| Release Manager | Customer Support Lead | Pre-release briefing |
| Release Manager | Stakeholders | Release announcement |
| Data Analyst | Product Manager | Post-release impact analysis |
