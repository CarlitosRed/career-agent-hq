# E-032 Review-relay tool that checks its own post
- level: verified
- public-safe: yes
- skill tags: tooling, process automation, Python, audit trail
- what happened: tools/review-relay/relay.py posts a vendor's review into the pull request. It refuses to post a review with no finding text and reads the posted comment back by its URL (leak L16, fixed in #77). It was used to relay the reviews on #77 to #79 and the read-back passed each time (leaks.md L16 status). Later work added posting as the vendor's own login (#92).
- source: https://github.com/CarlitosRed/agent-orchestration tools/review-relay/relay.py, tools/review-relay/test_relay.py; PRs #77, #92; .orchestration/leaks.md L16
- CV-ready bullet: Directed a tool that relays AI reviewer findings into pull requests, refuses empty reviews and verifies the posted comment, with 14 tests.
- how to verify: read relay.py and its tests; read leak L16. The "14" is from the PR #77 Codex comment ("14 new review-relay tests"); recount with the test file before quoting.
- limit: actual GitHub posting was not exercised in the #77 review (Codex said so); later use passed read-back per the leak log.
- signed: Career Agent HQ Orchestrator (Claude), 2026-10-21
