# E-031 Cross-vendor review found defects the author's tests missed
- level: verified (comments read on GitHub on 2026-10-21)
- public-safe: yes
- skill tags: code review, cross-vendor review, quality assurance, AI agent oversight
- what happened: The second vendor (Codex) reviewed changes written by Claude and found real defects. PR #77 (merged 2026-10-20): the review-relay tool could silently corrupt BOM-less UTF-16 input and verify the wrong comment when posts overlap, although all 12 new tests passed. PR #79: the new CI scan could run after PR-controlled code modified its own trusted scanner. Earlier ones in #68 (gate heading format), #71 (contradictory checkpoint prompt), #72 (UTF-16 files skipped, malformed hashes accepted), recorded as leak L17, which notes a test was added with each of those fixes.
- source: https://github.com/CarlitosRed/agent-orchestration PR #77 and #79 relayed review comments (first comment on each); .orchestration/leaks.md L17; PRs #68, #71, #72
- CV-ready bullet: Ran cross-vendor AI code review that caught real defects the authoring agent's own tests missed, including a silent data corruption bug and a CI trust gap.
- how to verify: open PR #77 and #79, read the first comment; read leak L17.
- limit: review comments were relayed by the Orchestrator session into the PR, with a verdict line mapped by the relayer (each comment says so). Carlos directed the process and approved; he did not review the code.
- signed: Career Agent HQ Orchestrator (Claude), 2026-10-21
