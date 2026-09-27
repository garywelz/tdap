# AGENTS.md — tdap

Read by every agent that works in this repo: Claude Code (via `CLAUDE.md`), Cursor (local
and Cursor Projects), and Claude Chat. This file holds only pointers and facts specific
to this repo. **Everything shared lives in one place:**
https://raw.githubusercontent.com/garywelz/copernicus-web/main/governance/AGENT_ROLES.md

## Before you do anything

Fetch these live, with plain fetches (no cache-busters). GitHub wins over any uploaded,
remembered, or pasted copy.

- Agent roles, lanes, session rules, repo↔Space map: https://raw.githubusercontent.com/garywelz/copernicus-web/main/governance/AGENT_ROLES.md
- Constitution: https://raw.githubusercontent.com/garywelz/copernicus-web/main/governance/CONSTITUTION.md
- Bulletin (read the newest entries): https://raw.githubusercontent.com/garywelz/copernicus-web/main/governance/BULLETIN.md
- TDAP open questions: https://raw.githubusercontent.com/garywelz/tdap/main/docs/research_focus.json

Then follow the **Session rules** and your lane in `AGENT_ROLES.md`, and report in its
four-section format. If this repo has `docs/GOVERNANCE_LOCAL.md`, read it too: it may add
to or tighten the shared rules, never loosen their invariants
(`governance/ENGINE_ONBOARDING.md` §3).

## The floor — holds even if the fetch fails

1. Propose before executing; Gary approves significant changes first.
2. Never force-push or rewrite history; no autonomous or triggered run pushes to `main`.
3. Never print credential-shaped files in full; if one reaches output, say so at once.

*(Deliberately duplicated in every repo's `AGENTS.md`; canonical text is in
`AGENT_ROLES.md` → Session rules. Change it there first.)*

## This repo

- **The TDAP engine** — persistent cohomology and circular/toroidal coordinates. A
  **shared engine**: Gary is PI; the domain collaborator named in the README
  owns the research questions.
- **This repo is public.** Never commit unpublished work, data, drafts, or advisor
  correspondence — the collaborator's or anyone's.
- **If you are the collaborator's agent** (running in the collaborator's own Claude, Claude Code,
  or Cursor): the suite lanes don't apply to you; your instructions are
  `docs/project_instructions.md`. Propose changes by pull request; never push to `main`.
- **If you are a suite agent:** `research_focus.json` questions change only with
  the collaborator's confirmation — draft, don't decide. Corpus writes happen in `copernicus-web`
  tooling, not here.
