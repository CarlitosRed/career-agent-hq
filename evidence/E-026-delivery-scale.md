# E-026 Delivery scale of the agent-run project
- level: verified (counts read from GitHub and git on 2026-10-12; they change daily)
- public-safe: yes for numbers, described generically (project name stays private)
- skill tags: multi-agent orchestration, release governance, CI, testing, tiered approvals
- what happened: In the private repo, 41 pull requests were opened between 2026-10-03 and 2026-10-12: 21 merged, 16 closed unmerged, 4 open. Branches: 22 Claude-prefixed, 17 Codex-prefixed, 2 other. 19 PRs carry a tier label (13 tier-3, 5 tier-2, 1 tier-1). The repo has 671 test functions and 4 GitHub Actions workflows (Python, backend/goal, local Gate A, gate audit); the latest runs on the newest branch all passed. The landing PR #33 merged on 2026-10-09 with 168 files after a signed non-approval and a fix round. PR #31 was closed unmerged by Carlos's instruction.
- source: `gh pr list --state all --limit 200` (counts); PR #33, #31 comments; `grep "def test_"` in tests and tools/gate; `gh run list`; checked 2026-10-12 by Claude · Truth Reviewer
- CV-ready bullet: Directed a multi-agent build (Claude and Codex) of a document-AI system: 21 merged PRs, 671 tests and tiered approval gates in under two weeks (first commit 2026-10-02, first PR 2026-10-03).
- how to verify: rerun the three commands above in the repo.
- limit: all commits and comments use one shared GitHub account, so the repo proves the process and scale, not who typed what. Accuracy of extraction is unmeasured. Do not write "wrote" or "built solo".
- signed: Claude · Truth Reviewer, 2026-10-12
