# Framework evidence intake: fit check, new entries, open questions
Career Agent HQ Orchestrator (Claude), 2026-10-21. Source brief: `what-we-built-for-career-evidence.md` (Framework Orchestrator session). Checked by me against the public repo https://github.com/CarlitosRed/agent-orchestration (fresh clone at commit 8e9f132, `gh` for PRs and tags, my own test run).

## 1. Does this repo fit the goal?
Yes, with one gap. The evidence bank (`E-###`, levels, "no entry, no claim"), the gate and the Truth Reviewer step are exactly what a job hunt built on AI-agent work needs, because the risk is overclaiming. The gap: no current CV or LinkedIn text exists here (`raw/` has only the 2026-10-12 vision dump and three interview transcripts; `cv/`, `linkedin/`, `drafts/` are empty), and the target roles in `decisions.md` and `jobs/` were set on 2026-10-12, before the framework existed, so they need a re-rank (T-009).

## 2. What I added
Evidence entries E-027 to E-039 in `evidence/` (index updated). One claim each, each with a source a reader can open.

| ID | Claim | Level |
| --- | --- | --- |
| E-027 | Public framework, 29 rules, 29 leak rows, 10 tags, 85 merged PRs | verified |
| E-028 | Carlos's exact role: Program Owner (goals, decisions, approval lines) | **stated** |
| E-029 | Merge gate | verified |
| E-030 | 10 offline suites, 509 tests pass (I ran them) | verified |
| E-031 | Cross-vendor review found real defects | verified |
| E-032 | Review-relay tool | verified |
| E-033 | Hygiene check enforcing R29 | verified (effect unmeasured) |
| E-034 | Rules register and leak log | verified |
| E-035 | Second-vendor audit, fixes merged within a day | verified / stated |
| E-036 | Stale tool-failure fact re-tested and corrected | verified |
| E-037 | Flaky test found and fixed | verified |
| E-038 | PR cannot loosen the rules it is judged by | verified |
| E-039 | Per-vendor GitHub accounts | verified / stated |

## 3. Where I differ from the brief (checked, not assumed)
- **PRs #77 to #86 were not all merged on 2026-10-20.** #77 to #80 merged 2026-10-20; #81 to #86 merged 2026-10-21 (UTC). Entries use the real dates.
- **R29 sits in `AGENTS.md` plus six templates, not seven templates** (`.orchestration/hygiene.json`, one `required_text` entry, seven paths).
- **Test count:** the brief says about 480 (Codex counted 476 on #77). Today on main I counted 509 in the same 10 suites. E-030 gives both with dates; re-count before quoting.
- **The "11-item" audit list is not in the repo** (the handoff file says it lived in a notes folder). E-035 proves the fixes through leak rows and merge dates and tells the Writer not to quote "11".
- **Not verified by me:** "17 PRs merged in the previous session" (reported by that session's handoff; there are 69 merged PRs numbered below #77, so I did not use the figure), the launcher scripts, and Carlos's chat instructions of 2026-10-20/21 (kept in E-028 as "reported, no artifact").
- **The repo moves fast.** It was at PR #88 when I started and #94 an hour later; entries carry check dates.

## 4. The honest limit that matters most
Until PR #87 (2026-10-21) every comment on the repo, including "Program Owner: Approved at <commit>", was posted from one GitHub account (leak L1). GitHub therefore proves the process and its scale, not who typed what. That is why E-028 is `stated`, not `verified`. Any CV line must say "directed, decided, approved", never "wrote" or "built". The same limit already sits in E-026.
Also kept in the entries: personal framework with one user, other projects pin older tags, R29 effect unmeasured, no token or cost numbers.

## 5. Not done on purpose
No CV, LinkedIn or cover-letter text (rule 1: entries first; the Writer drafts only after Carlos approves these entries and the Truth Reviewer, a different agent from me, checks them, rule 5). Carlos has not yet confirmed `public-safe: yes` for E-027 to E-039; AGENTS.md rule 3 makes that his call.

## 6. Questions for Carlos (only what I cannot derive)
1. Target roles: stay with "AI ops / solutions / process / product-owner / freelance" from `decisions.md`, or add agent-governance and agentic-engineering process roles? (Dev experience is under 1 year per `decisions.md`; the evidence supports process and oversight, not coding.)
2. Location and remote: Costa Rica on-site/hybrid plus LATAM-remote, as in `decisions.md`, or global remote?
3. Deadline: when do you need the offer or the first income?
4. Are your current CV and LinkedIn text in `raw/`? They are not there now. Paste them (or give the file) and I will store them verbatim.
5. Do you confirm E-027 to E-039 as public-safe and E-028 as your role statement?
