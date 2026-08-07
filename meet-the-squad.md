# 🧑‍🤝‍🧑 Meet Your Squad

> Your AI development team, powered by [Squad](https://github.com/bradygaster/squad).

## The Team

This squad was cast from **The Usual Suspects** — a team of 6 specialists tailored to this repository's purpose: planning, not implementing.

| Name | Role | Specialty | How to Talk to Them |
|------|------|-----------|---------------------|
| 🏗️ Keaton | Lead / Product Analyst | Intent interpretation, scope, success criteria | `squad:keaton` label or mention in issue |
| 🏗️ McManus | Architect | Repository investigation, technical boundaries | `squad:mcmanus` label or mention in issue |
| 🔧 Fenster | Work Decomposer | Splitting intents into small, coherent child issues | `squad:fenster` label or mention in issue |
| 🧪 Hockney | Test Strategist | Completion criteria, executable evaluations | `squad:hockney` label or mention in issue |
| ⚙️ Redfoot | Dependency Reviewer | Sequencing, dependency graphs, parallel work | `squad:redfoot` label or mention in issue |
| 📝 Kobayashi | Plan Critic / Scribe | Final validation, publishing GitHub issues | `squad:kobayashi` label or mention in issue |

### Always-On Support

| Name | Role | Specialty | How to Talk to Them |
|------|------|-----------|---------------------|
| 📋 Scribe | Session Logger | Tracking all agent sessions | Automatic — never needs explicit routing |
| 🔄 Ralph | Work Monitor | Backlog health and stale work alerts | Automatic — watches for idle work |
| 🛡️ Rai | RAI Reviewer | Responsible AI and safety review | Automatic — reviews high-risk output |

## How to Work With Your Squad

### Label-Based Assignment

Apply a `squad:{name}` label to any issue or PR to route it directly to that specialist. For example, `squad:hockney` sends work to your test strategist.

### Iteration Commands

| Command | What It Does |
|---------|--------------|
| `/squad cast` | Re-cast the full team (replaces current squad) |
| `/squad cast-member <spec>` | Add or modify a single team member |
| `/squad retire <name>` | Remove a team member from the roster |
| `/squad status` | Check current team composition and health |

### Routing

Work is routed automatically via `.squad/routing.md`. Each member has a **charter** (`.squad/agents/{lowercase-name}/charter.md`) defining their expertise, boundaries, and personality.

## What Happened Here

This team was assembled based on automated analysis of your repository and the Intent Issue driving the cast (#1):

- **Repo purpose:** "A squad that plans projects and features" — a minimal, purpose-built repo with no application code, only a `Planning Squad` prompt describing an agentic planning workflow.
- **Repo structure:** Bare repository (README + `.squad/` + `.github/`), no source, no CI/CD, no tests. The substantive signal came from the Intent Issue rather than the repo tree.
- **Rationale:** The Intent Issue explicitly defines seven planning perspectives (Product Analyst, Architect, Work Decomposer, Test Strategist, Dependency Reviewer, Plan Critic, Scribe). Rather than the generic 5-role default preset (lead/reviewer/devrel/security/docs), the team was recast to mirror these planning roles one-to-one, merging Scribe's issue-publishing duty into the Plan Critic (Kobayashi) since the built-in Scribe already owns session logging. This gives every planning perspective a dedicated owner while keeping the team small (6 specialists).

---

*Cast on 2026-08-07 for bradygaster/PlanningSquad*
