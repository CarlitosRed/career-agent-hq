# Checkpoint: Claudio · Career PM, 2026-10-28 (supersedes the 2026-10-27 checkpoints where they differ)

Signed: Claudio · Career PM (Claude), 2026-10-28.

## State (checked by me)
- Master has: interview lake, evidence E-001 to E-052 (E-013, E-019 to E-021, E-025 still unverified), CV drafts A and B in `cv/`, ranked targets and first live leads in `jobs/`, decisions through 2026-10-27. PRs #19 to #32 merged; no open PRs apart from the one carrying this file.
- Gate: single-vendor mode (Codex lapsed). Every PR needs a separate subagent truth review plus Carlos's exact `**Carlos:** Approved at <full sha>`, branch `claude/...`, label `tier-1`, then `gate.py merge` from a v0.9.2 worktree (`C:\Users\carlo\.claude\jobs\3c992b80\tmp\fw`; recreate with `git -C ..\agent-orchestration worktree add <dir> v0.9.2` if gone). A new commit voids earlier approvals. The gate refuses a no-owner tier, so approvals stay.
- Low-approval-load workflow (decisions 2026-10-27): leads, tailored CVs, cover notes and outreach live in git-ignored `work/`, no PR; only source-of-truth files (evidence, lake, decisions, rules, final CV/LinkedIn files) go by PR, batched.
- Repo is public until about 2026-11-02, when Carlos makes it private himself.

## What exists in `work/` (git-ignored; `ls work/` first)
- Ready to use, each reviewed by a separate agent: CV `.docx` and `.md` for Equifax, Zuora, Sysdig, Tebra, West Monroe, with cover notes (`*-2026-10-27.md`).
- Drafts for Carlos to send: ClickHouse Costa Rica question; outreach to two ex-Snowflake contacts (v2, warmer).
- `applications-tracker.xlsx`: sheets Jobs, Wide sweep, New leads (evening), Contacts, with an "Open check 2026-10-27" column. Nothing is marked Applied yet; Carlos has not said he applied anywhere.
- Lead files: `live-leads-wide-2026-10-27.md`, `live-status-2026-10-27.md` (46 leads re-checked: 45 open, Gramian closed), `europe-jobs-2026-10-28.md` (20 leads), `europe-visas-2026-10-28.md` (visa research, not legal advice).
- Weekly rerun: Windows scheduled task `CareerAgentHQ-WeeklyRerun`, Mondays 08:07, first run 2026-11-02; script `work/run-weekly-rerun.ps1`, prompt `work/weekly-rerun-prompt.md`, logs in `work/logs/`. Tools limited, writes only under `work/`, $20 cap, never applies. Not yet run end to end: check the first log.
- `pending-batch.md`: items for the next evidence/decisions PR (below).

## Settled by Carlos (typed)
Snowflake Jan 2024 to May 2025; Varicent Business Consultant Aug 2025 to May 2026 with Varicent Designer; Spanish native, English B2 on paper (English a soft flag for postings); Power BI basic; Data Loader only VMware and Amadeus; PostgreSQL project-only; MySQL, Spark, Azure not claimed; Sykes and Amadeus cleared for the CV; Amadeus knowledge base cleared; 2+ years of analyst, operations and consulting work is OK to claim; paid freelance project Sep 2026 (prototype, investigation, logic; client unnamed; no amount); E-004 and E-005 cleared; the Equifax "4 years" wording is his call.

## Decisions not yet saved / waiting for the next PR
- Europe: Carlos has friends of his parents in Germany, Italy and Spain and asked to investigate jobs and visas there (no decision yet beyond "investigate").
- Rubric question: should data-analyst roles keep a low archetype weight? Not answered.
- The weekly rerun is now a Windows scheduled task (decision row to add).
- E-052 (support years) is in this PR.

## Not checked
- Employer pages for 10 LinkedIn/Computrabajo-only leads; Indeed, Glassdoor; big employers' own career pages (Oracle, Dell, Concentrix, Teleperformance, Deloitte, PwC, EY, KPMG and others).
- The Europe visa report's gaps: blocked official pages (Make it in Germany, Spain's Ministry of Inclusion), no official 2026 Spain visa euro figure, Germany's EUR 45,630 is the agent's computation, Costa Rica and Spain dual nationality, ETIAS start date, exchange rate from an aggregator.
- No pay was compared to the 1.6M colones floor except where the posting states colones; West Monroe's pay period is unstated.
- The scheduled task has not run for real; the .docx files were checked via their text versions.

## Carlos still owes
Apply or send when ready and say so (the tracker is updated on his word); citizenship and passport validity, ancestry (Spanish, Italian, German), criminal-record certificate; Jun-Jul 2025 gap answer; Snowflake reference; Varicent product name; data-analyst rubric weight; which Europe roles to tailor (suggested NavVis Munich, Holded Barcelona, Celonis Madrid); LinkedIn (T-005) when the "who I am" picture is ready.

## Next three actions
1. Read `work/live-status-2026-10-27.md` and `work/europe-jobs-2026-10-28.md`, then ask Carlos what he applied to; update the tracker with dates.
2. Tailor the leads Carlos picks (process in `work/sysdig-and-tebra-2026-10-27.md`: tailoring notes, cover note, separate agent review, no PR).
3. After 2026-11-02: read the first weekly-rerun log in `work/logs/`; land the next batched PR (pending-batch items).

## Paste-ready prompt for the next chat
Rooted in `C:\Users\carlo\dev\career-agent-hq`:

```
Read OFFICE-STATE.md, CONTEXT-RULES.md, AGENTS.md, audits/handoff-claudio-career-pm-2026-10-28.md, tasks/queue.md and decisions.md, in that order, then `ls work/` and open work/pending-batch.md. You are Claudio · Career PM for Career Agent HQ. Check `gh pr list`, then ask Carlos which jobs he applied to and update work/applications-tracker.xlsx. Follow the PR-landing gotchas in the checkpoint.
```
