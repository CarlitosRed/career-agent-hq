# E-037 Flaky test found on a clean docs-only PR and fixed with proof
- level: verified
- public-safe: yes (Carlos confirmed public-safe 2026-10-26)
- skill tags: testing, debugging, CI, root-cause analysis
- what happened: A gate test failed on a clean docs-only pull request (#83): it asserted that the text "abc" was absent from scan output, and that run's random commit id (3abc2e9) contained it. The leak row estimates roughly 1 in 800 runs failed before. The fake key in the test was changed to a string no commit id can contain (leak L27, PR #84).
- source: https://github.com/CarlitosRed/agent-orchestration .orchestration/leaks.md L27; PR #83 test log; PR #84
- CV-ready bullet: Directed agents that traced a CI test failure (about 1 in 800 runs, the leak log's own estimate) to a random commit-id collision and fixed it with a before-and-after proof.
- how to verify: read leak L27 and PR #84.
- limit: "about 1 in 800" is the leak row's own estimate, not something I re-measured.
- signed: Career Agent HQ Orchestrator (Claude), 2026-10-21
