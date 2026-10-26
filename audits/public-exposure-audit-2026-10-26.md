# Public exposure audit: career-agent-hq (repo is PUBLIC)
Checked by Career Agent HQ Orchestrator (Claude) on master 14b4db9, 74 tracked files on master (75 on this branch), 2026-10-26. Method: `git ls-files`, then `git grep` for secrets, emails, phone numbers, customer/product names, and a read of the lake headers, `profile/brief.md` and the evidence `public-safe` lines. Not checked: file contents line by line, other branches, open PRs, git history (the client name from the Sykes round 1 commit is still there).

## Verdict
No secrets, keys, tokens, emails or phone numbers found. The exposure is personal and project detail, not credentials.

## Findings (ranked)
| # | Finding | Where | Rule |
|---|---|---|---|
| 1 | 25 evidence entries marked `public-safe: ask Carlos` are public today | evidence/E-001..E-025 (not E-026) | AGENTS.md rule 3 says public only with `yes` |
| 2 | Personal money situation: "income is currently zero", "about $20 a week for 4 hours" | profile/brief.md | Carlos's call |
| 3 | PO Reader repo name and details (PR numbers, file paths such as backend catalog code) in `source` lines | E-001, 002, 003, 005, 006, 007, 008, jobs/*, tasks/T-001, decisions.md | decisions.md 2026-10-12: generic only |
| 4 | Employer product name (Delphi) and employers by name (Amadeus, VMware, Sykes/Foundever, Barisant, Snowflake, Varicent) | lake/companies/amadeus.md line 10; profile/brief.md; E-009 | lake headers say "ask Carlos"; employers on a CV are normal, a product name is not |
| 5 | Salary target 1.6M colones in clear text | decisions.md, profile/brief.md, tasks/queue.md, OFFICE-STATE.md, jobs/market-scan | Carlos's call |
| 6 | Interview detail: performance termination process, manager on leave, "no recognition" | lake/companies/sykes-foundever.md | `stated`, ask Carlos |
| 7 | Local path `C:\Users\carlo\...` (Windows username) in `source` lines | 17 evidence files and 8 other files | low risk |
| 8 | README.md says "Private project (not for GitHub public)", which is false | README.md line 3 | factual error (fixed in this PR) |

## Not found
Customer names (the bank client was scrubbed in #9, still in git history), PO or catalog data, `.env*` content, credentials, emails, phone numbers.

## For Carlos to decide (nothing below was changed by this audit)
- Items 1 to 3: keep, mark each entry `yes`, or remove the detail. Recommended: make the 25 `ask Carlos` entries non-public (private repo or move them to `raw/`) until each is cleared.
- Item 2: recommend removing the money lines from brief.md.
- Item 4: recommend replacing "Delphi" with "a hospitality product built on Salesforce".
- Repo visibility: Carlos chose to keep it public on 2026-10-26; history is not rewritten.
- Carlos's answer after this audit (chat, 2026-10-26): "this is ok to be public i would make it pivate in a week so i don't care about it been public". Exposure accepted for about a week; Carlos plans to make the repo private around 2026-11-02 himself. Nothing removed. Findings 1 to 7 stay as listed; the private switch is the control.

Signed: Career Agent HQ Orchestrator (Claude), 2026-10-26
