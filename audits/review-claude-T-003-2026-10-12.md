# T-003 review: evidence E-001 to E-008 against the repo
Claude · Truth Reviewer, 2026-10-12. Checked by me directly (git, gh, file reads), not from Codex's word.

## Verdict: all 8 hold, with 4 wording fixes
| Entry | Result | Note |
| --- | --- | --- |
| E-001 worktrees and roles | Holds | Docs and branch prefixes (claude/, codex/, chat/, integration) confirmed in `gh pr list` |
| E-002 merge gate | Holds | Commit 427be1e exists: "T-010: adopt the operating model and the merge gate (#10)", 2026-10-04. `tools/gate/` has po_gate.py, gate.json, tests |
| E-003 cross-vendor review | Holds, fix | Codex "Not approved at <head>" comments confirmed on #31 and #33. But #31 was later CLOSED unmerged at Carlos's instruction and its head changed; #33 merged 2026-10-09 |
| E-004 prompt checklist | Holds | Not re-read line by line; limits note stands (no tested gain) |
| E-005 evidence-preserving doc AI | Holds | Cited code at contracts.py and catalog.py matches the stated purpose (immutable observations, scoped retrieval, "always awaiting human review") |
| E-006 fictional/offline safety | Holds | CI workflows present; no run executed by me |
| E-007 CI lane | Holds, upgrade | 4 workflows exist and the newest runs on codex/email-e3-sender-hint all passed (checked via gh run list) |
| E-008 Windows tooling | Holds, fix | PR #26 title is "Fix Roy's Windows demo quickstart and missing private catalog error", merged 2026-10-08. Never quote the title: it names a collaborator |

## Wording fixes for the writers
1. E-002: say "Directed the design of" not "Designed". Agents built the gate under Carlos's direction.
2. E-003: do not cite PR #31 as a success; use #33 (merged) or describe the lane generically.
3. E-008: describe as "Windows quickstart for a local fictional-data demo", no PR title, no collaborator name.
4. Every bullet about code or tooling: use verbs directed, specified, orchestrated, reviewed. Not wrote, coded, engineered.

## What the repo cannot prove (attribution)
All 22 commits on main and every GitHub comment come from one shared account (CarlitosRed). The repo proves what the process produced, not who wrote it. Carlos's role is evidenced by his own decision lines ("**Carlos:** go", closing #31 at his instruction, hold/unhold rights in ROLES.md), but those use the same account too. Decision: credit as architect and director (decisions.md). Carlos should be ready to explain, in his own words, 3 decisions he made (for interviews and for LinkedIn "About").

## New evidence added
E-026 delivery scale: 41 PRs (21 merged, 16 closed, 4 open), 671 test functions, 4 CI workflows, tier labels on 19 PRs.

## Still unverified
Time span verified: first commit 2026-10-02, first PR 2026-10-03, checked 2026-10-12. Use "under two weeks". No accuracy numbers exist and none may be claimed. Not checked: E-009 to E-025 (need Carlos).

## For Codex · Writer
Add E-026 to evidence/INDEX.md (Codex owns the index). Use the four wording fixes above.

## Process findings (For Claudio · PM)
- Leak: evidence entries cite "ask Carlos" for public-safe on every entry. Fix: decisions.md now says generic is public-safe; Codex should re-tag E-001..E-008 as "generic yes, names no".
