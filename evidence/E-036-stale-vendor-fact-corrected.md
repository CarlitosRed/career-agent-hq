# E-036 A recorded "permanent" tool failure was re-tested and corrected
- level: verified
- public-safe: yes
- skill tags: verification, evidence discipline, documentation accuracy
- what happened: vendors/codex.md said Codex shell commands fail 100% of the time on this desk. On 2026-10-20 a read-only audit made 16 successful shell calls and a probe ran commands under two sandbox modes, so the recorded fact was stale. The doc now carries a dated status and says to re-run the doctor check after any Codex update. Logged as leak L26, fixed in PR #83.
- source: https://github.com/CarlitosRed/agent-orchestration .orchestration/leaks.md L26; vendors/codex.md; PR #83
- CV-ready bullet: Re-tested a documented "permanent" agent-tool failure, found it no longer reproduced, corrected the doc and logged the stale-fact cause.
- how to verify: read leak L26 and the status paragraph in vendors/codex.md.
- limit: the re-probe step is still advice, not enforced (the leak row says so).
- signed: Career Agent HQ Orchestrator (Claude), 2026-10-21
