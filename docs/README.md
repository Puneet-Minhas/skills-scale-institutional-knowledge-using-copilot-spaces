# OctoAcme Project Management Docs

This folder is the centralized knowledge base for OctoAcme project management processes. It is intended for use as a [GitHub Copilot Space](https://docs.github.com/en/copilot/using-github-copilot/using-copilot-spaces), giving the team quick, AI-assisted access to our shared processes, roles, and best practices.

---

## Overview

OctoAcme uses an iterative, customer-centric approach to project management with clear ownership, data-informed decisions, and well-defined roles. Every project follows a structured lifecycle from initiation through retrospective, supported by consistent tooling, communication rhythms, and quality practices.

### Project Lifecycle

| Phase | Description |
|---|---|
| **Initiation** | Define the problem, goal, and success metrics; align stakeholders; pass a decision gate before planning begins. |
| **Planning** | Hold kickoff, create a prioritized backlog with acceptance criteria and estimates, define Done, map dependencies, build a release plan, and draft an initial test plan. |
| **Execution & Tracking** | Deliver in iterations with daily standups, a weekly delivery sync, and sprint/milestone demos. Track work on a project board (Backlog → Ready → In Progress → In Review → QA → Done) using small, well-described PRs with CI checks. |
| **Release & Deployment** | Verify pre-release checklist (passing CI/security scans, release notes, rollback plan, smoke tests), deploy to staging then production, run post-deploy verification, and announce to stakeholders. |
| **Retrospective & Close** | Run a structured retro after each sprint, release, or milestone; capture 2–3 action items with owner and due date; track in the backlog and review in the weekly PM sync. |

### Key Roles

| Role | Responsibilities |
|---|---|
| **Project Manager (PM)** | Coordinates delivery, schedules, risk, and communications; facilitates planning and retros; maintains status reporting. |
| **Product Manager (PdM)** | Defines the product vision and success metrics, prioritizes the backlog, and validates solutions with data. |
| **Developers** | Implement features, write and maintain tests and docs, participate in design and code reviews. |
| **QA / Testing** | Validate acceptance criteria through unit, integration, e2e, and manual testing; run security scans in CI. |
| **Stakeholders** | Provide input, approvals, and business context; receive regular status updates. |

### Communication Cadence

- **Daily standups** — delivery team, 15 min, focus on progress and blockers.
- **Weekly delivery sync** — PM + team, show progress, surface risks.
- **Weekly PM ↔ PdM alignment** — backlog priority, roadmap, and dependencies.
- **Sprint / milestone demos** — demonstrate working software to stakeholders.
- **Monthly stakeholder updates** — high-level status, decisions, and upcoming milestones.

**Escalation path:** Team → PM → Product Lead → Sponsor. For security incidents, follow the security incident runbook and notify Security on-call.

### Quality Assurance & Release Readiness

- Unit, integration, and e2e smoke tests run in CI for every PR.
- Security scanning as part of the CI pipeline.
- Manual QA for feature acceptance when required.
- Pre-release checklist: all acceptance criteria met and PRs merged, passing CI and security scans, release notes drafted, rollback plan documented, smoke tests prepared.

### Risk Management

Maintain a risk register (ID, description, impact, likelihood, owner, mitigation, status) reviewed at every weekly sync. Risks identified during planning and execution are assessed, mitigated, and monitored continuously.

---

## Quick Links

| Document | Description |
|---|---|
| [Project Management Overview](./octoacme-project-management-overview.md) | Principles, core roles, key artifacts, and high-level lifecycle. |
| [Project Initiation Guide](./octoacme-project-initiation.md) | One-pager template, stakeholder alignment, and decision gate checklist. |
| [Project Planning](./octoacme-project-planning.md) | Backlog, estimates, Definition of Done, release plan, and planning checklist. |
| [Execution & Tracking](./octoacme-execution-and-tracking.md) | Team rhythm, project board workflow, PR conventions, quality practices. |
| [Risk Management & Communication](./octoacme-risks-and-communication.md) | Risk register, escalation paths, weekly status template, incident comms. |
| [Release & Deployment Guide](./octoacme-release-and-deployment.md) | Pre-release checklist, deployment steps, rollback playbook, release notes template. |
| [Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md) | Retro structure, action item tracking, continuous improvement culture. |
| [Roles & Personas](./octoacme-roles-and-personas.md) | Detailed responsibilities and communication patterns for each role. |

---

## How to Use These Docs

1. **Onboarding** — Start with the [Project Management Overview](./octoacme-project-management-overview.md) to understand OctoAcme's approach, then read the role that applies to you in [Roles & Personas](./octoacme-roles-and-personas.md).
2. **Starting a new project** — Follow the [Project Initiation Guide](./octoacme-project-initiation.md) and [Project Planning](./octoacme-project-planning.md) docs to stand up a new initiative correctly.
3. **Day-to-day delivery** — Reference [Execution & Tracking](./octoacme-execution-and-tracking.md) for PR conventions, board workflow, and escalation paths.
4. **Releasing** — Use the [Release & Deployment Guide](./octoacme-release-and-deployment.md) checklist before every deployment.
5. **Copilot Spaces** — Add this folder (or its contents) to your Copilot Space context so that GitHub Copilot can answer process questions directly from these documents.
