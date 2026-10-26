# E-033 Hygiene check that enforces a rule in CI (R29)
- level: verified for the mechanism; the effect on agent behaviour is NOT measured
- public-safe: yes (Carlos confirmed public-safe 2026-10-26)
- skill tags: policy-as-code, CI, agent instructions, prompt templates, governance
- what happened: tools/hygiene fails CI on vendor names in rules, over-long decision rows, hand-written numbers that go stale, a hashed name sweep for a public repo, and (since PR #85, merged 2026-10-21) a required sentence. .orchestration/hygiene.json lists seven files that must contain the exact "work silently, reply once, stop to ask only if truly blocked" sentence: AGENTS.md and six prompt templates (the brief said seven templates; the config shows AGENTS.md plus six). Carlos's decision (recorded 2026-10-20) was that this standing rule applies always, so it is enforced in software, not left as advice.
- source: https://github.com/CarlitosRed/agent-orchestration tools/hygiene/hygiene.py, .orchestration/hygiene.json (required_text), rules/README.md R29, docs/decisions.md row 2026-10-20 "Rule R29 (#85)", PR #85
- CV-ready bullet: Directed a standing instruction for AI agents to be enforced in CI across the agent instructions and prompt templates, rather than relying on advice.
- how to verify: read hygiene.json required_text and the R29 row; run `python tools/hygiene/hygiene.py check` in a clone.
- limit: the rules register itself says compliance can only be measured over later sessions; no tool can see what an agent writes. Rule R29's effect is not measured yet.
- signed: Career Agent HQ Orchestrator (Claude), 2026-10-21
