# E-027 Public governance framework for multi-vendor AI coding agents
- level: verified (checked on GitHub and in a fresh clone on 2026-10-21; counts change daily)
- public-safe: yes (the repo is public, made public by Carlos's decision on 2026-10-16; this entry cites only the framework, no PO Reader product or customer detail)
- skill tags: multi-agent orchestration, agent governance, release governance, process design, documentation
- what happened: A framework for teams of AI coding agents from two vendors (Claude and Codex): roles, a merge gate, a review loop, a rules register (R1 to R29), a leak log (L1 to L29), templates and skills. Repo created 2026-10-13. Ten version tags v0.1.0 to v0.9.1; v0.7.0 is dated 2026-10-15, v0.8.0 and v0.9.0 2026-10-19, v0.9.1 2026-10-20. 85 pull requests merged (numbers up to #94) when checked. The repo runs under its own gate.
- source: https://github.com/CarlitosRed/agent-orchestration (README.md, STATE.md, rules/README.md, .orchestration/leaks.md, docs/decisions.md); `gh pr list --repo CarlitosRed/agent-orchestration --state merged --limit 500 --json number`; `git tag -l --format="%(refname:short) %(creatordate:short)"` in a clone
- CV-ready bullet: Directed Claude and Codex agents to build a public governance framework for multi-vendor AI agent teams: 29 rules, a merge gate, a leak log, 10 tagged releases.
- how to verify: open the repo URL; run the two commands in "source"; count rows starting `| R` in rules/README.md and `| L` in .orchestration/leaks.md.
- limit: personal framework used by one person's agents, not a team product with other users. The other two projects (advance-po-reader, career-agent-hq) pin older tags (this repo pins v0.3.0); none had adopted the latest tag on 2026-10-20. "Directed" means set goals, decided, approved (see E-028); the agents wrote the code.
- signed: Career Agent HQ Orchestrator (Claude), 2026-10-21
