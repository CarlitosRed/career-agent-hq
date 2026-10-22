# AGENTS.md: Career Agent HQ (rules for every agent, Codex and Claude)

Goal: get Carlos a job in agentic engineering (building, orchestrating and reviewing AI-agent systems) by improving his CV and LinkedIn with true, provable claims. Costa Rica based, remote-compatible roles.

Read in this order: `OFFICE-STATE.md`, `CONTEXT-RULES.md`, `profile/brief.md` (if it exists), then your own task card in `tasks/`.

## Hard rules
1. **Evidence first.** Every claim on a CV, LinkedIn or cover letter must trace to an entry in `evidence/` (E-###). No entry, no claim. Never invent numbers, titles, employers, dates or tools.
2. **Claim levels.** Each evidence entry is `verified` (checked against a repo, PR, file or document), `stated` (Carlos said it, no artifact yet) or `unverified` (memory only). Only `verified` and `stated` may be used; `unverified` needs a check first.
3. **Confidentiality.** No customer names, PO/catalog data, keys, tokens or `.env*`. Advance PO Reader details go public only as `public-safe: yes` in the entry. Carlos decides. Real customer data stays out of this folder.
4. **One writer per file.** Shared files (`OFFICE-STATE.md`, `CONTEXT-RULES.md`, `profile/brief.md`, `decisions.md`, `tasks/`, `_templates/`) are written only by Claudio · Career PM. Everyone else writes their own file in `evidence/`, `audits/` or `drafts/` and puts requests under "For Claudio".
5. **Author never reviews own work.** Codex mines and drafts, Claude reviews truth, and the reverse.
6. **No applying, no sending.** Agents never submit applications, send messages or edit LinkedIn directly. They produce drafts; Carlos presses the button.
7. **Never guess.** Unknown stays `Unknown`. Report what you checked vs what you were told.
8. Sign every file with the chat name and date.
9. **Explain with visuals.** When explaining findings, code paths, comparisons, plans or task handoffs to Carlos, draw an inline visual (diagram or widget) next to the text rather than relying on prose alone (Carlos's own global preference, carried in here since a project CLAUDE.md would otherwise shadow this file for Claude Code specifically -- see `.orchestration/leaks.md` 2026-10-22 and agent-orchestration's hygiene check for why).
