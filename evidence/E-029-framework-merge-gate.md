# E-029 Merge gate that refuses to merge without the right evidence
- level: verified (README read, tests run on 2026-10-21; behaviour beyond the README was not re-probed by me)
- public-safe: yes
- skill tags: merge gates, separation of duties, CI, GitHub, secrets scanning, release governance
- what happened: tools/gate/gate.py checks a tier label, required pull request body headings (Failure, Class, Fix, Proof, Affects, Rollback in .orchestration/gate.json), a signed plan, an approval from the other vendor at the exact commit, and the owner's approval line. It merges only that exact head commit. It re-reads the pull request and judges the fresh read, so a late hold blocks a merge (leak L21, fixed in #79). It scans commits for secrets and forbidden files, including UTF-16 files (L22, #79). Per-vendor GitHub-account checks were added (#73) and switched on in #87.
- source: https://github.com/CarlitosRed/agent-orchestration tools/gate/README.md, tools/gate/gate.py, tools/gate/test_gate.py, .orchestration/gate.json; PRs #73, #79, #87; .orchestration/leaks.md L21, L22
- CV-ready bullet: Directed agents to build a merge gate enforcing tiered approvals, exact-commit cross-vendor review, required PR evidence and secret scanning.
- how to verify: read tools/gate/README.md; run `python -I -m unittest discover -s tools/gate -p test_gate.py` in a clone.
- limit: the gate trusts GitHub identity only from #87 on; before that, signatures were text from one account (leak L1). The README lists what the gate cannot do. Carlos directed; agents wrote it.
- signed: Career Agent HQ Orchestrator (Claude), 2026-10-21
