# Codex memory miner audit — 2026-10-12

## What I checked
- Career Agent HQ task card, AGENTS.md, OFFICE-STATE.md, and evidence-entry template. The profile brief is absent.
- C:\Users\carlo\dev\AGENT-WORKFLOW.md; project-notes\CONTEXT-RULES.md, prompt checklist, and prompting playbook.
- Advance PO Reader local main checkout at 49d9dbd, which reported one commit behind origin when checked; ROLES.md, tools\gate\README.md, gate.json, README.md, PROJECT_GOAL.md, selected backend source, and the backend-goal-checks workflow.
- Read-only GitHub PR list and signed issue-comment headers for PRs #31 and #33. PRs show Codex-signed non-approval comments on Claude-prefixed branches. ROLES.md says the account is shared, so these comments do not prove the human author. No PR or review-round totals are stated in the evidence entries.
- Codex memory registry and the 2026-09-10 job-search rollout summary. That summary says the candidate profile came from the user's request because the workspace had no résumé or other source files.

## Memory claims not independently verified
- The role phrases “Snowflake Partner Process Specialist” and “Varicent Business Consultant” and the listed tools are memory-only. Exact employers, titles, dates, assignments, proficiency, and outcomes are Unknown.
- Exact personal contributions to code, CI, Windows tooling, and the document-AI implementation cannot be separated from agent contributions using a shared GitHub account. The verified entries establish project artifacts and documented responsibilities, not individual commit authorship.
- The prompt checklist is a real document, but the playbook says it was not tested against a live model and that some earlier prompts exceeded its length target. No improvement metric is available.
- The project documentation explicitly says extraction accuracy is unmeasured. This audit did not inspect a CI run result or execute tests.

## Gaps a hiring manager would ask about
- Employment history with exact employers, titles, locations, dates, and responsibilities.
- Concrete examples showing the candidate's personal role in requirements, architecture, code, agent orchestration, review, and release decisions.
- Measured business or engineering results: users, volume, time saved, quality, reliability, cost, or adoption, each with a source.
- Demonstrated proficiency and work samples for each legacy tool claim, especially SQL, Python/Spark, Power BI, Salesforce, Workday, and Varicent.
- Education, certifications, portfolio links, and which project details Carlos permits for public use.
- For the document-AI project, an approved evaluation set and measured accuracy are not evidenced here; do not present the demo as validated production performance.

## Questions for Carlos
1. What were the exact employers, titles, dates, and client/product context for the Snowflake and Varicent experience?
2. Which of SQL, Python, Spark/PySpark, Power BI, Salesforce, Workday, Excel, Snowflake notebooks, Linux/shell, Git/regex, Varicent Designer, PostgreSQL, BRD/process discovery, and Visio were used professionally, and what sanitized work samples can support them?
3. For the agentic-engineering project artifacts, which decisions and outcomes were yours, and which implementation, review, CI, or Windows work should be attributed to Codex or Claude?
4. Which generic workflow or project details may be marked public-safe, and which details must remain private?
5. What source-backed results can you provide for scope and impact, such as users, workload, time saved, quality, reliability, cost, or adoption?

- signed: Codex · Memory Miner, 2026-10-12
