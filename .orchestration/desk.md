# Desk and environment facts

This project has no local development environment to describe: no services,
ports, or app to launch, and no interpreter version it depends on (confirmed:
no `tools/`, no `.github/workflows/`, no test suite; `evidence/`, `cv/`,
`linkedin/`, `jobs/`, `lake/`, `raw/`, `tasks/`, `audits/`, `drafts/` are all
plain Markdown). career-agent-hq produces documents, not running code.

The closest things to desk facts are the external, read-only sources this
project reads from, already named in `OFFICE-STATE.md`'s "Where things live"
section. This file is a pointer there, not a copy, because that section is
itself one of `.orchestration/gate.json`'s `protected_paths` (so it already
has one writer and the project's heaviest tier on any change) -- a second
copy here would be an un-protected shadow that could drift silently:
- Codex memories (read-only source): `C:\Users\carlo\.codex\memories\`
  (`MEMORY.md`, `memory_summary.md`, `rollout_summaries\`).
- Product evidence (read-only from here, never edited): `C:\Users\carlo\dev\advance-po-reader`
  (PRs, ROLES.md, gate) and `C:\Users\carlo\dev\project-notes` (workflow,
  decisions).
- Job tracker: already running in Codex (Google Sheets, workbook referenced
  from Codex memory). Not duplicated here.

Carlos's OS/shell (Windows, PowerShell, git) is the Claude Code session's own
environment, not a fact of this project specifically -- nothing in this repo
is executed, so nothing here is pinned to an interpreter version.
