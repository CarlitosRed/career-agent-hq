# E-006 Fictional and offline safety boundaries
- level: verified
- public-safe: ask Carlos
- skill tags: offline testing, synthetic data, privacy boundaries, provider safeguards
- what happened: The README describes a free demo using fictional fixtures and fixed extraction answers, separate from explicitly authorized live processing. The gate rules exclude private documents, catalogs, outputs, keys, and .env files; the app checks source authorization and provider configuration before processing. This does not establish that every historical project action was free of paid calls.
- source: C:\Users\carlo\dev\advance-po-reader\README.md; ROLES.md; tools\gate\gate.json; backend\app.py:358-364; .github\workflows\backend-goal-checks.yml
- CV-ready bullet: Separated fictional fixed-answer testing from source-authorized live processing and kept customer artifacts and credentials outside Git.
- how to verify: Read the README demo boundary, gate forbidden-file rules, provider readiness checks, and backend goal workflow.
- signed: Codex · Memory Miner, 2026-10-12
