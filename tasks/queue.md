# Queue (critical path first)

| ID | Owner | Task | Needs |
| --- | --- | --- | --- |
| T-001 | Codex · Memory Miner | DONE 2026-10-12: 25 entries (8 verified project, 17 memory-only), audits/codex-memory-miner-2026-10-12.md | - |
| T-002 | Claude · Market Scout | DONE 2026-10-12: jobs/market-scan-2026-10-12.md | - |
| T-007 | Claude · Market Scout | DONE 2026-10-12: market-scan section 6 | - |
| T-003 | Claude · Truth Reviewer | DONE: audits/review-claude-T-003-2026-10-12.md; E-026 added | - |
| T-004 | Codex · Writer | Draft CV v1 (2 variants) from verified evidence | T-001, T-002, Carlos's current CV in `raw/` |
| T-005 | Writer (Codex lapsed; Claude drafts, another Claude reviews) | Build LinkedIn from scratch: headline, About, Experience, Featured | Interview rounds done + Carlos go-ahead |
| T-006 | Claude · Truth Reviewer | Review CV and LinkedIn drafts | T-004, T-005 |

## Answered 2026-10-12 (see decisions.md)
PO Reader generic only; all work types plus Upwork side income; under 1 yr dev; architect/director credit.

## Still open (re-checked 2026-10-26: no CV in `raw/` (Carlos will provide it later); LinkedIn does not exist yet; employers, titles, dates and legacy tools only partly covered by interviews in `lake/companies/`, all `stated`, some Unknown)
1. Put current CV (any format) in `raw/` (Carlos: later). LinkedIn has no existing text: it is built from scratch (T-005).
2. Exact employers, titles, dates for the Varicent and Snowflake work (Codex could not verify).
3. ANSWERED 2026-10-26: salary ideally above 1.6M colones/month or higher; English B2 (E-040) and Spanish fluent (E-041), both stated.
4. Which legacy tools (SQL, Python, Power BI, Salesforce, Workday...) were used professionally.

## New tasks
- T-008 DONE: jobs/upwork-scan-2026-10-12.md
- T-009 next (unblocked 2026-10-26): re-rank targets with scoring-rubric; target ideally above 1.6M colones/month, English B2
- T-006 upgrade: review panel = 1 ATS-screen reader, 1 hiring manager, 5 persona readers (manager, other applicant, CEO, recruiter, technical lead), each alone; then one rewrite constrained to evidence IDs.
- T-010 DONE: jobs/scoring-rubric.md
- T-011 DONE 2026-10-26: evidence E-027 to E-039 (framework work), reviewed by two separate Claude subagents (verdicts relayed in the PR #2 comments), merged as #2.
- T-005 reframed 2026-10-26: build the LinkedIn profile from scratch (no existing profile); starts after the interview rounds are done and Carlos says the "who I am" picture is ready. Drafts only; Carlos creates and edits the profile himself.
- T-004 and T-006 (CV draft and its review) stay blocked until item 1 above (current CV in `raw/`) and item 2 are answered: the Varicent and Snowflake employers and dates are still unverified, and the Amadeus, VMware and Sykes dates in the lake are `stated`, not documented.
