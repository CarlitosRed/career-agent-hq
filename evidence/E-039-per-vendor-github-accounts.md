# E-039 Per-vendor GitHub accounts so signatures become provable
- level: verified for the config change; stated for Carlos creating the accounts
- public-safe: yes
- skill tags: identity, audit trail, separation of duties, governance
- what happened: The Orchestrator's own self-review (audit dated 2026-10-19) found every actor posted as one GitHub account, so "Independent Reviewer · Codex" was text anyone could type (leak L1). The need came from that self-review, not from Carlos. PR #87 (merged 2026-10-21) set per-vendor logins, owner_logins and distinct_accounts in the gate config, after Carlos created the accounts (PR #87 body). Rolling out needed a separate posting path; PR #92 added posting as the vendor's login.
- source: https://github.com/CarlitosRed/agent-orchestration .orchestration/leaks.md L1, L13; docs/vendor-accounts.md; PRs #87, #92; audits/framework-self-review-2026-10-19.md
- CV-ready bullet: Decided to create one GitHub account per AI vendor so agent approvals are tied to identity, after a self-review showed they were only typed text.
- how to verify: read leak L1, PR #87's body, and its diff of .orchestration/gate.json.
- limit: PR #87's own proof says the first real test of the account checks is the next PR after it merged. Carlos's part: deciding and creating the accounts; the diagnosis and code were the agents'.
- signed: Career Agent HQ Orchestrator (Claude), 2026-10-21
