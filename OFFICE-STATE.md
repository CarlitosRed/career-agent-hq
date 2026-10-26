# Office state: Career Agent HQ

Created 2026-10-12 by Claudio · Career PM. Keep to one screen. Only the PM writes this file.

**2026-10-13 (Carlos):** this project is now one of the projects run on the reusable agent orchestration framework (public repo `CarlitosRed/agent-orchestration`, made public by Carlos 2026-10-16 per E-027). "Claudio · Career PM" is this project's Orchestrator in the framework's role naming (`agent-orchestration/docs/roles-and-names.md`); the name stays as-is here for now. This chat (rooted in this repo) is this project's own Orchestrator chat and does not edit the framework repo; it logs friction in this project's own notes for the Framework Orchestrator to read later. See `agent-orchestration/docs/multi-orchestrator-model.md`.

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

## Status (2026-10-26)
- Done: scaffold, T-001, T-002, T-003, T-007, T-008, T-010, T-011. Framework pin v0.9.2 with gate CI (#3). Interview lake holds Sykes r1-2, Amadeus r1-2, VMware r1 (Amadeus r2 and VMware r1 added in #4). Evidence E-027 to E-039 on the framework work, merged in #2; Carlos's public-safe confirmation of 2026-10-26 is recorded in the entries and in `decisions.md`.
- Gate is in single-vendor mode (Codex lapsed, #5): every PR needs a separate Claude subagent review plus Carlos's typed approval, then merge with the framework's `gate.py`. Revert `cross_vendor` to true when Codex returns.
- Not started: T-004 CV draft, T-005 LinkedIn draft, T-006 review panel, T-009 re-rank. Still blocked on Carlos answers below.
- Open questions for Carlos: see `tasks/queue.md` (CV in `raw/`, employers and dates, salary floor and English level, legacy tools).
