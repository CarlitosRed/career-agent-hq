# E-034 Rules register with named enforcers and a leak log of process failures
- level: verified
- public-safe: yes (Carlos confirmed public-safe 2026-10-26)
- skill tags: risk management, decision logging, root-cause analysis, process improvement, audit trail
- what happened: rules/README.md lists rules R1 to R29, each naming its enforcer (gate, CI, template or advice) and a status. .orchestration/leaks.md is a log of process failures L1 to L29; each row has evidence, root cause, a class, the fix and the level the fix works at, and a status (open, fixed with PR number, verified). A class seen twice must be fixed before the next PR (rule R11). docs/decisions.md records dated decisions. Nine handoff files in audits/ let a fresh session continue.
- source: https://github.com/CarlitosRed/agent-orchestration rules/README.md, .orchestration/leaks.md, docs/decisions.md, rules/leak-classes.md, audits/handoff-framework-orchestrator-*.md
- CV-ready bullet: Directed agents to keep a written risk system for an AI-agent team: 29 rules each with a named enforcer and a 29-row failure log with root cause and fix.
- how to verify: open the files; count rows. Counts were R1 to R29 and L1 to L29 on 2026-10-21.
- limit: the log is kept by the agents under Carlos's rule; he decides what is accepted. "Fixed" means a PR landed, not that recurrence was ruled out; the log marks "verified" only after a later PR shows no recurrence.
- signed: Career Agent HQ Orchestrator (Claude), 2026-10-21
