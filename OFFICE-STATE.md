# Office state: Career Agent HQ

Created 2026-10-12 by Claudio · Career PM. Keep to one screen. Only the PM writes this file.

## Roles
| Who | Job | Writes |
| --- | --- | --- |
| Carlos | Decides what is public, approves every CV/LinkedIn version, applies to jobs himself | `raw/`, decisions by saying so |
| Claudio · Career PM (Claude) | Plans, task cards, verifies, keeps shared notes | shared files, `tasks/` |
| Codex · Memory Miner | Mines Codex memories and rollouts into evidence entries with source pointers | `evidence/`, `audits/codex-*` |
| Codex · Writer | Drafts CV and LinkedIn from verified evidence only | `cv/`, `linkedin/` drafts |
| Claude · Truth Reviewer | Checks every claim against evidence and repos; checks tone and ATS | `audits/review-*` |
| Claude · Market Scout | Researches agentic-engineering roles, titles, keywords, salaries | `jobs/` |

## Flow
Codex memory -> evidence bank -> (Writer drafts, Reviewer checks) -> Carlos approves -> published.
Market Scout feeds target titles and keywords into the Writer's brief.

## Where things live
- Codex memories (read-only source): `C:\Users\carlo\.codex\memories\` (`MEMORY.md`, `memory_summary.md`, `rollout_summaries\`).
- Product evidence: `C:\Users\carlo\dev\advance-po-reader` (PRs, ROLES.md, gate), `C:\Users\carlo\dev\project-notes` (workflow, decisions).
- Job tracker already running in Codex (Google Sheets, workbook in Codex memory). Do not duplicate it.

## Status (2026-10-12)
- Scaffold, T-001, T-002, T-007 done. Next: T-003 verify evidence; blocked on Carlos answers (CV in raw/, years, public-safe, employers/dates).
- Open questions for Carlos: see `tasks/queue.md`.
