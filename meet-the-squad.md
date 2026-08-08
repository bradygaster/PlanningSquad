# Meet the Squad

PlanningSquad is composed from the repository's own Planning Squad specification in issue #1. Its job is to turn large Intent Issues into small, ordered, independently executable GitHub issues for an agentic SDLC.

## Team Members

### product-analyst
Extracts user outcomes, scope, constraints, and success criteria from new Intent Issues.

### architect
Studies the repository and defines technical boundaries that shape decomposition.

### work-decomposer
Breaks large intent into small, coherent, independently executable units of work.

### test-strategist
Defines executable evaluations, acceptance checks, and completion criteria for every planned issue.

### dependency-reviewer
Validates sequencing, dependency edges, and opportunities for safe parallel work.

### plan-critic
Challenges oversized, vague, unnecessary, or untestable issues before they are finalized.

### issue-scribe
Creates and links the final GitHub issues from the approved plan.

## Always-On Squad Support

### Scribe
Built-in session logger that records work without needing manual routing.

### Ralph
Built-in work monitor that tracks operational flow and status.

### Rai
Built-in responsible AI reviewer for safety and policy concerns.

## How to Route Work

Use `squad:{name}` labels to route work to the right member:

- `squad:product-analyst`
- `squad:architect`
- `squad:work-decomposer`
- `squad:test-strategist`
- `squad:dependency-reviewer`
- `squad:plan-critic`
- `squad:issue-scribe`

Use the base `squad` label when a request still needs triage.

## Why These Names Are Descriptive

These members use plain descriptive names because the user explicitly requested function-based naming rather than a fictional or themed cast. The team composition is derived directly from the repository's Planning Squad specification in issue #1, with each name matching its planning role.
