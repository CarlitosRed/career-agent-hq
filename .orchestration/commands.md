# Commands

UNKNOWN: this project has no commands to run. There is no test suite, no CI,
no scan tool, and no app to launch (confirmed: no `tools/`, no
`.github/workflows/`; `.gitignore` only excludes `raw/`, `*.pdf`, `*.docx`,
`.env*`). `adapters/README.md` describes this file as "the exact commands for
tests, scan and the app launcher" -- none of those exist here, and inventing
placeholder commands would misrepresent a documents-only project as having
code to verify.

The nearest equivalent process is AGENTS.md's read order and `_templates/`
(`evidence-entry.md`, `task-card.md`) -- but those are file conventions, not
commands, so they stay described in AGENTS.md and are not duplicated here.

If this project ever gains a script (for example, the job-board scanner
`career-ops` flagged `PARKED` in `decisions.md`'s 2026-10-12 row, revisit only
after Carlos says yes), its command belongs here and this file stops being
UNKNOWN.

## Verification drive (`.orchestration/verify/`) -- not created
`adapters/README.md`'s verify/ spec is itself still `PROPOSED` framework-wide
(not even advance-po-reader has one yet as of this retrofit), and it assumes
a user-facing feature with a launchable surface to screenshot or record.
This project has no such surface. Its nearest equivalent -- proving a claim
is true before it reaches a CV -- already happens through `evidence/E-###`
entries (AGENTS.md rule 1), not a verify/ drive. Flagged to the Framework
Orchestrator: the adapter spec's verify/ concept may need a second shape, or
an explicit opt-out, for projects that produce documents rather than a
running app.
