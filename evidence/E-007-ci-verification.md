# E-007 CI verification lane
- level: verified
- public-safe: ask Carlos
- skill tags: CI, GitHub Actions, PostgreSQL, fixed-input evaluation
- what happened: The backend-goal-checks workflow runs on pushes and pull requests with read-only repository permission, an ephemeral PostgreSQL service, backend checks, and a fixed-JSON goal suite. It preserves suite results and a scorecard as artifacts. This audit inspected the workflow definition only; it did not inspect a run result or execute tests.
- source: C:\Users\carlo\dev\advance-po-reader\.github\workflows\backend-goal-checks.yml; tools\gate\gate.json
- CV-ready bullet: Orchestrated CI checks for backend and fixed-input goal behavior with isolated PostgreSQL and retained scorecards.
- how to verify: Inspect the workflow job, permissions, service, test commands, and artifact step; retrieve a head-specific run before claiming a pass.
- signed: Codex · Memory Miner, 2026-10-12
