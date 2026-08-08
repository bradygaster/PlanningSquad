# Work Routing

How to route planning work across the PlanningSquad team.

## Routing Table

| Work Signal | Route To | Why |
|-------------|----------|-----|
| new Intent Issue | product-analyst | Starts by extracting outcomes, scope, constraints, and success criteria from the request. |
| scope/outcome extraction | product-analyst | Owns product framing and definition of what the request is really asking for. |
| repo architecture analysis | architect | Studies the repository and sets technical boundaries for decomposition. |
| issue decomposition | work-decomposer | Breaks intent into small, coherent, independently executable issues. |
| test/evaluation criteria | test-strategist | Defines executable validation and completion criteria for each issue. |
| dependency sequencing | dependency-reviewer | Validates ordering, dependency edges, and parallel work opportunities. |
| plan critique/challenge | plan-critic | Challenges oversized, vague, unnecessary, or untestable issues. |
| issue creation/linking | issue-scribe | Publishes the final approved issues and links them for traceability. |
| session logging | Scribe | Built-in silent session logger; no manual routing needed. |
| work monitoring | Ralph | Built-in monitor for progress and operational flow. |
| RAI review | Rai | Built-in reviewer for responsible AI and safety concerns. |

## Issue Routing

| Label | Action | Who |
|-------|--------|-----|
| `squad` | Triage planning request and assign the correct specialist label | Squad |
| `squad:product-analyst` | Start product framing and scope extraction | product-analyst |
| `squad:architect` | Analyze repository boundaries and architecture constraints | architect |
| `squad:work-decomposer` | Draft or refine small executable child issues | work-decomposer |
| `squad:test-strategist` | Define evaluation steps and acceptance criteria | test-strategist |
| `squad:dependency-reviewer` | Review sequencing and dependency structure | dependency-reviewer |
| `squad:plan-critic` | Critique plan quality and force sharper issue boundaries | plan-critic |
| `squad:issue-scribe` | Create and link finalized issues | issue-scribe |

## Rules

1. Route new planning requests through product framing before final decomposition whenever the intent is still ambiguous.
2. Involve the architect before freezing issue boundaries when repository structure affects execution seams.
3. Require test-strategist and dependency-reviewer input before calling a plan execution-ready.
4. Use plan-critic to challenge any issue that is oversized, vague, speculative, or not objectively verifiable.
5. Hand finalized issue sets to issue-scribe only after the plan has passed critique and sequencing review.
