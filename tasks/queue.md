# Queue (critical path first)

| ID | Owner | Task | Needs |
| --- | --- | --- | --- |
| T-001 | Codex · Memory Miner | DONE 2026-10-12: 25 entries (8 verified project, 17 memory-only), audits/codex-memory-miner-2026-10-12.md | - |
| T-002 | Claude · Market Scout | DONE 2026-10-12: jobs/market-scan-2026-10-12.md | - |
| T-007 | Claude · Market Scout | DONE 2026-10-12: market-scan section 6 | - |
| T-003 | Claude · Truth Reviewer | DONE: audits/review-claude-T-003-2026-10-12.md; E-026 added | - |
| T-004 | Codex · Writer | Draft CV v1 (2 variants) from verified evidence | T-001, T-002, Carlos's current CV in `raw/` |
| T-005 | Codex · Writer | Draft LinkedIn headline, About, Experience, Featured | T-004 |
| T-006 | Claude · Truth Reviewer | Review CV and LinkedIn drafts | T-004, T-005 |

## Answered 2026-10-12 (see decisions.md)
PO Reader generic only; all work types plus Upwork side income; under 1 yr dev; architect/director credit.

## Still open
1. Put current CV (any format) and LinkedIn text in `raw/`.
2. Exact employers, titles, dates for the Varicent and Snowflake work (Codex could not verify).
3. Salary floor and language level (English/Spanish).
4. Which legacy tools (SQL, Python, Power BI, Salesforce, Workday...) were used professionally.

## New tasks
- T-008 DONE: jobs/upwork-scan-2026-10-12.md
- T-009 next: re-rank targets with scoring-rubric (needs Carlos: salary floor, English level)
- T-006 upgrade: review panel = 1 ATS-screen reader, 1 hiring manager, 5 persona readers (manager, other applicant, CEO, recruiter, technical lead), each alone; then one rewrite constrained to evidence IDs.
- T-010 DONE: jobs/scoring-rubric.md
