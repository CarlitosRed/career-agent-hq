# Leak log

New with this retrofit (2026-10-15) -- this project has never kept one
before (confirmed: no file resembling a leak or incident log exists under
`audits/`, `tasks/`, or anywhere else in this repo, unlike advance-po-reader's
`project-notes\tasks\process-leaks.md`, which already existed before its own
retrofit). Unlike `desk.md` and `roles.md` above, there is nothing elsewhere
to point to, so entries go directly in this file from now on, in the shape
`adapters/README.md` asks for: what went wrong, evidence, root cause, fix.

| Date | What went wrong | Evidence | Root cause | Fix |
| --- | --- | --- | --- | --- |
| 2026-10-22 | This repo carried a tracked root `CLAUDE.md` alongside `AGENTS.md`. Claude Code silently prefers a project `CLAUDE.md` over `AGENTS.md`, so Codex sessions (which read `AGENTS.md`) and Claude sessions (which read `CLAUDE.md`) could in principle see different rules -- the exact anti-pattern agent-orchestration's own hygiene tool later added a check for (PR #106, not yet in the `v0.9.2` pin this repo runs). | `CLAUDE.md` (1 line, pointer to `AGENTS.md`/`OFFICE-STATE.md` plus a visuals instruction not in `AGENTS.md`); agent-orchestration `tools/hygiene/hygiene.py` PR #106 description | A Claude-only file was created as a shortcut pointer instead of writing its one real instruction straight into the vendor-neutral `AGENTS.md`. | Merged the one unique instruction (explain with visuals) into `AGENTS.md` rule 9, deleted `CLAUDE.md`, removed it from `.orchestration/gate.json`'s `protected_paths` (same PR that upgraded the framework pin to `v0.9.2`). |
