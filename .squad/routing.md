# Work Routing

How to decide who handles what.

## Routing Table

| Work Type | Route To | Examples |
|-----------|----------|----------|
| Intent interpretation & scope | Keaton | Extracting outcome, constraints, success criteria from an Intent Issue |
| Repo/architecture investigation | McManus | Studying existing code, conventions, boundaries, reusable implementations |
| Issue decomposition | Fenster | Splitting an intent into small, coherent child issues |
| Completion criteria & evaluations | Hockney | Writing objective, executable completion tests for child issues |
| Dependency sequencing | Redfoot | Blocked-by/blocks/parallel mapping across child issues |
| Plan critique & publishing | Kobayashi | Validating the full plan, creating and linking GitHub issues |
| Session logging | Scribe | Automatic — never needs routing |
| RAI review | Rai | Content safety, bias checks, credential detection, ethical review |

## Planning Pipeline

1. **Keaton** reads the Intent Issue, defines scope/success criteria.
2. **McManus** investigates the repo in parallel — architecture, conventions, existing implementations.
3. **Fenster** drafts child issues from Keaton's scope + McManus's findings.
4. **Hockney** adds completion criteria/evaluations to each child issue.
5. **Redfoot** validates dependency sequencing and flags parallel work.
6. **Kobayashi** runs final plan validation, creates the GitHub issues, and posts the Planning Summary on the Intent Issue.

## Issue Routing

| Label | Action | Who |
|-------|--------|-----|
| `squad` | Triage: analyze issue, assign `squad:{member}` label | Keaton |
| `squad:{name}` | Pick up issue and complete the work | Named member |

### How Issue Assignment Works

1. When a GitHub issue gets the `squad` label, **Keaton** triages it — analyzing content, assigning the right `squad:{member}` label, and commenting with triage notes.
2. When a `squad:{member}` label is applied, that member picks up the issue in their next session.
3. Members can reassign by removing their label and adding another member's label.
4. The `squad` label is the "inbox" — untriaged issues waiting for Keaton's review.

## Rules

1. **Eager by default** — spawn all agents who could usefully start work, including anticipatory downstream work (e.g., McManus investigates while Keaton scopes).
2. **Scribe always runs** after substantial work, always as `mode: "background"`. Never blocks.
3. **Quick facts → coordinator answers directly.** Don't spawn an agent for simple factual questions.
4. **When two agents could handle it**, pick the one whose domain is the primary concern.
5. **"Team, ..." → fan-out.** Spawn all relevant planning agents in parallel as `mode: "background"`.
6. **Anticipate downstream work.** While Fenster drafts issues, Hockney can begin drafting evaluation criteria from the same scope.
7. **Issue-labeled work** — when a `squad:{member}` label is applied to an issue, route to that member. Keaton handles all `squad` (base label) triage.
