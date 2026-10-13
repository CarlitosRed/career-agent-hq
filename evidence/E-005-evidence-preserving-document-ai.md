# E-005 Evidence-preserving document AI
- level: verified
- public-safe: ask Carlos
- skill tags: document AI, evidence preservation, structured extraction, human review, auditability
- what happened: The current project contract keeps provider observations immutable, represents uncertainty, stores deterministic parses separately, and binds source evidence to observations. Candidate retrieval is tenant/vendor scoped and returns suggestions that require human approval; review events are stored separately. No extraction-accuracy claim is supported here.
- source: C:\Users\carlo\dev\advance-po-reader\PROJECT_GOAL.md; README.md; backend\contracts.py:1, 28, 92, 273-289; backend\catalog.py:1-4, 86, 147-157, 225-240; backend\app.py:407-421
- CV-ready bullet: Specified a review-gated document AI workflow that preserves source evidence and uncertainty, scopes catalog suggestions, and records human decisions.
- how to verify: Inspect the cited contract, retrieval, and review-event code; PROJECT_GOAL.md states that accuracy remains unmeasured.
- signed: Codex · Memory Miner, 2026-10-12
