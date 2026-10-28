# Handoff: Career Agent HQ, 2026-10-27 evening (supersedes HANDOFF-2026-10-27.md)

Signed: Claudio · Career PM (Claude), 2026-10-27.

## Where we are
- Master has: interview lake (Sykes, Amadeus, VMware, Snowflake, Varicent), evidence E-001 to E-051, two CV drafts (`cv/`), ranked targets (`jobs/targets-ranked-2026-10-27.md`), first live leads (`jobs/live-leads-2026-10-27.md`), decisions through 2026-10-27. No open PRs at the time of writing except the batch PR that carries this file.
- Settled facts (Carlos, typed): Snowflake Jan 2024 to May 2025; Varicent Business Consultant Aug 2025 to May 2026 (Varicent Designer); Spanish native, English B2 on paper (English is a soft flag, not a skip, for postings); Power BI basic; Data Loader only at VMware and Amadeus; PostgreSQL project-only; MySQL, Spark, Azure not claimed; Sykes and Amadeus cleared; 2+ years of analyst, operations and consulting work is OK to claim; paid freelance project Sep 2026 (prototype, investigation, logic; no amount, no client name).
- Open for Carlos: Jun-Jul 2025 gap answer, whether to set up a weekly job rerun, LinkedIn alerts, a Snowflake reference, Varicent product name, data-analyst archetype weight in the rubric (not answered).

## The `work/` folder (git-ignored, no PR; decisions 2026-10-27)
Leads, application drafts and CVs live in `work/` (a fresh chat must `ls work/`): tailored CV .docx and .md for Equifax, Zuora, Sysdig, Tebra; cover notes; ClickHouse question draft; outreach drafts for two LinkedIn contacts; `applications-tracker.xlsx` (sheets Jobs, Wide sweep, Contacts); `live-leads-wide-2026-10-27.md`; `live-status-2026-10-27.md` (open/closed re-check); `pending-batch.md` (items waiting for the next evidence PR). Contact details are in the .docx files, never in tracked files. Carlos applies and sends everything himself; mark statuses in the tracker when he says so.

## How a PR lands (still true)
Branch `claude/...`, label `tier-1` (the gate raises protected paths to tier-2), separate subagent truth review posted as `**Claude · Truth Reviewer:** Approved at <sha>`, Carlos's exact `**Carlos:** Approved at <full sha>`, then `python <v0.9.2 gate.py> --config .orchestration/gate.json merge N --as "Claudio · Career PM"`. Batch changes: one PR per work block. A new commit voids earlier approvals: re-review and re-approve. The v0.9.2 worktree is at `C:\Users\carlo\.claude\jobs\3c992b80\tmp\fw` (recreate with `git -C ..\agent-orchestration worktree add <dir> v0.9.2` if gone).

## Next three actions
1. Read `work/live-status-2026-10-27.md`; tell Carlos which leads are still open; tailor the best ones (same process as `work/sysdig-and-tebra-2026-10-27.md`).
2. Update the tracker with every application or message Carlos reports.
3. LinkedIn (T-005) once Carlos says the "who I am" picture is ready; repo goes private about 2026-11-02 (Carlos does it).

## Paste-ready prompt for the next chat
Rooted in `C:\Users\carlo\dev\career-agent-hq`:

```
Read OFFICE-STATE.md, CONTEXT-RULES.md, AGENTS.md, HANDOFF-2026-10-27-evening.md, tasks/queue.md and decisions.md, in that order, then `ls work/` and open work/pending-batch.md and work/live-status-2026-10-27.md. You are Claudio · Career PM for Career Agent HQ. Check `gh pr list`, then report which leads are open and ask Carlos for the next single action. Follow the PR-landing gotchas in the handoff.
```
