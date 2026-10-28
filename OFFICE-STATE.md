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

## Status (2026-10-27, evening)
- Interview lake on master: Sykes r1-3, Amadeus r1-3, VMware r1-2, Snowflake r1-2, Varicent r1-2 (all `stated`). Evidence E-001 to E-051. CV drafts A and B in `cv/`; ranked targets and first live leads in `jobs/`. Framework pin v0.9.2 with gate CI.
- Gate is in single-vendor mode (Codex lapsed): every PR needs a separate Claude subagent review plus Carlos's typed approval, then `gate.py merge` from a v0.9.2 clone. Branch must start with `claude/` and the PR needs a `tier-1` label. Revert `cross_vendor` to true when Codex returns. The gate refuses a no-owner tier with same-vendor review, so approvals stay; to cut Carlos's load, leads and application drafts go in git-ignored `work/` (decisions 2026-10-27) and source-of-truth changes are batched into one PR per work block.
- Job rerun is a daily 05:30 Windows task (decisions 2026-10-28); `work/tracker/open-tracker.bat` opens the visual tracker (Europe leads included).
- Open work: `tasks/queue.md`. Tailored CVs, cover notes, the tracker and the open/closed lead check are in `work/`; Carlos applies and sends himself.
- Handoff for the next chat: `audits/handoff-claudio-career-pm-2026-10-28.md` (checkpoint, read it first; `HANDOFF-2026-10-27-evening.md` is the earlier one).
