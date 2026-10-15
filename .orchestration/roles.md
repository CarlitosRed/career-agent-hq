# Roles -- pointer, not a copy

Source of truth: `OFFICE-STATE.md`'s "Roles" table (this repo's root), kept
current by the Orchestrator (AGENTS.md rule 4 -- shared files have one
writer). Read it there directly.

Not duplicated here on purpose: `OFFICE-STATE.md` is already one of this
project's `protected_paths` (see `.orchestration/gate.json`) -- any change to
it already goes through this project's heaviest available tier. A second
copy in `.orchestration/roles.md` would be an un-protected shadow that could
drift silently, the same reasoning advance-po-reader's retrofit used for its
own `roles.md` -> `ROLES.md` pointer.

Quick orientation only (not a substitute for reading `OFFICE-STATE.md` and
`AGENTS.md` directly):
- **Carlos** (Program Owner) -- decides what is public, approves every
  CV/LinkedIn version, applies to jobs himself. Never an agent (AGENTS.md
  rule 6: "No applying, no sending").
- **Claudio · Career PM** (Claude/Anthropic) -- this project's Orchestrator.
  Plans, task cards, verifies, writes every shared file.
- **Codex · Memory Miner** and **Codex · Writer** (Codex/OpenAI) -- mine
  evidence, draft CV/LinkedIn from verified evidence only.
- **Claude · Truth Reviewer** and **Claude · Market Scout** (Claude/Anthropic)
  -- check every claim against evidence (rule 5: author never reviews own
  work -- Codex drafts, Claude reviews, and the reverse), research roles.
- No branch-prefix or launch-ceiling convention has ever been written down
  for this project (no PRs before this retrofit). **UNKNOWN** -- see
  `.orchestration/gate.json`'s own flagged fields for the same gap.
