# E-030 Offline test suites required in CI before merge
- level: verified (I ran the suites myself on 2026-10-21)
- public-safe: yes
- skill tags: testing, CI, GitHub Actions, Python, quality gates
- what happened: 10 test suites under tools/, all offline. At v0.9.1 the count was about 480 (the building session reported that Codex counted 476 in PR #77; hygiene tests were added later). On main at commit 8e9f132 on 2026-10-21 I ran all ten with `python -I -m unittest` and got 509 tests, all passing. .orchestration/gate.json requires the check named "tests" to pass before merge.
- source: https://github.com/CarlitosRed/agent-orchestration tools/*/test_*.py; .orchestration/gate.json (required_checks: ["tests"]); my run on 2026-10-21 at commit 8e9f132; PR #77 Codex relay ("All 476 tests across the 10 offline tool suites passed")
- CV-ready bullet: Required about 500 offline tests across 10 suites to pass in CI before any change could merge, in a framework directed through AI agents.
- how to verify: clone the repo; for each tools/*/test_*.py run `python -I -m unittest discover -s <dir> -p <file>`; sum the "Ran N tests" lines.
- limit: the number moves with every PR; always re-count before quoting. Agents wrote the tests.
- signed: Career Agent HQ Orchestrator (Claude), 2026-10-21
