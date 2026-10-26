# E-038 A pull request cannot loosen the rules it is judged by
- level: verified
- public-safe: yes (Carlos confirmed public-safe 2026-10-26)
- skill tags: CI security, supply-chain trust, GitHub Actions, policy-as-code
- what happened: The copied workflow templates read the framework version and gate config from the PR head, so a PR could judge itself by its own edits, and the pre-review copy missed label and body edits (leak L20). PR #78 (merged 2026-10-20) changed them to read pin and config from the trusted base commit and to rerun on label and body edits. The framework repo's own live workflows already did this.
- source: https://github.com/CarlitosRed/agent-orchestration .orchestration/leaks.md L20; PR #78 "Workflow templates: pin and config from the trusted base; rerun on label and body edits"; templates/gate-pre-review.yml, templates/gate-audit.yml
- CV-ready bullet: Had CI templates changed so a pull request is judged by the base branch's rules, closing a gap where a PR could rewrite its own checks.
- how to verify: read leak L20 and the diff of PR #78.
- limit: no project had adopted the fixed templates yet (the leak row says "no project has adopted it yet").
- signed: Career Agent HQ Orchestrator (Claude), 2026-10-21
