# CV v1, Variant B: AI Operations / Agent Orchestration
Draft by Claudio · Career PM (Claude), 2026-10-27. Not reviewed, not approved, not sent (AGENTS.md rule 6). Every line cites its source in `[brackets]`; remove the brackets in the final file. `E-###` = `evidence/`; `L:` = `lake/companies/` (interview, `stated`). Contact details are NOT in this repo: Carlos adds them in the final copy.

## Open before this can go out
1. Truth review (T-006) is still to do. Counts and dates below came from the CV example and interviews, all `stated`.
2. Employer names (Sykes, Amadeus) are `public-safe: ask Carlos`. They are real employers on his own CV; the repo goes private about 2026-11-02.
3. Amadeus title: the CV says "Technical Support Analyst / Data Analyst"; interviews say "Technical Support Engineer, something like that" then "Data Analyst". Carlos to pick the exact wording.
4. Dates for Sykes (Jan 2020 to Apr 2021) and Amadeus (Jun 2021 to Jun 2023) come from his CV; interviews gave only "about" dates. VMware Aug 2023 to Jan 2024 is from the CV (interview said mid-2023).
5. Nothing on this page is verified by a document. A reference list (two Varicent people, a VMware manager) is held by Carlos, not in the repo.
6. Snowflake scale (about 200 to 300 requests, more than $1.5M per quarter) is rough; Carlos to confirm whether it covers his whole portfolio or one quarter's peak, and whether to keep both figures.
7. Skills-line SQL has no E entry of its own (E-011 is unverified); it rests on the Snowflake and Varicent interviews.
8. E-004 and E-005 are `public-safe: ask Carlos` (prompt checklist, document-AI workflow); the document-AI bullet is generic, but Carlos must clear both before sending. Project figures change daily (E-026 to E-034); recount.

---

# CARLOS ALBERTO REDONDO ALVARADO
AI Operations | Agent Orchestration | Process Automation | SQL, Python
Costa Rica | [email] | [phone] | [LinkedIn URL]

## Summary
Process and data professional who directs AI agents on engineering work: Program Owner of a public governance framework for multi-vendor AI agent teams (merge gate, tiered approvals, cross-vendor review, leak log). Before that, more than five years in support, partner operations, analytics and software implementation (2020 to 2026): automated a monthly partner-funds process in Python and SQL, built a team knowledge base, and validated outputs in QA/UAT. Not a software engineer: sets the review process, approves each change and keeps the evidence. [E-027, E-028, E-029, E-031, L:snowflake, L:amadeus, decisions 2026-10-12]

## Projects
**Program Owner, public AI-agent governance framework** | Oct 2026 (figures as of 2026-10-21; recount before sending)
- Directed Claude and Codex agents to build a public governance framework for multi-vendor AI agent teams: 29 rules, a merge gate, a leak log and 11 tagged releases. Agents wrote the code; Carlos set goals, made recorded decisions and gave final approval on each change. [E-027, E-028]
- Directed agents to build a merge gate enforcing tiered approvals, exact-commit cross-vendor review, required PR evidence and secret scanning. [E-029]
- Directed cross-vendor AI code review (Claude authors, Codex reviews) that caught real defects the authoring agent's own tests missed, including a silent data corruption bug and a CI trust gap. [E-031]
- Directed agents to require about 500 offline tests across 10 suites to pass in CI before any change could merge. [E-030]
- Directed agents to keep a written risk system for an AI-agent team: 29 rules each with a named enforcer and a 29-row failure log with root cause and fix. [E-034]
- Directed a multi-agent build of a document-AI order-intake system with human-review gates that preserves source evidence and uncertainty. [E-026, E-005, decisions 2026-10-12]
- Introduced a prompt-quality checklist (role, scope, source context, verification steps, output limits) for Claude and Codex tasks. [E-004]

## Experience

**Business Consultant | Varicent** | Aug 2025 to May 2026
- Investigated configuration and data discrepancies using SQL and Excel, performed root-cause analysis, reconciled results, and validated outputs during QA/UAT. [E-048]
- Built and tested imports, tables, calculation rules, and workflow components; documented expected results, testing evidence, and repeatable validation and support procedures. [E-048]
- Partnered with clients, business users, and technical teams to understand requirements, reproduce issues, communicate blockers, and align solutions with business needs. [E-048]
- Built a small demo of a client's payroll calculation in the product to confirm the requirements had been understood. [L:varicent]

**Partner Process Specialist | Snowflake** | Dec 2024 to Jul 2025
- Owned the monthly process for managing partners' cloud funds: about 200 to 300 fund requests and more than $1.5 million per quarter. [L:snowflake, stated, rough]
- Pulled data from Snowhouse (SQL) and Workday, matched and linked reports that could not be joined at source, calculated the figures and entered them in the partner information system. [L:snowflake]
- Replaced manual Excel matching, which needed updating every day through the month, with Python scripts and Snowflake notebooks that refresh the data in one run at the end of the week. [L:snowflake]
- Led meetings with partners on stuck funds, for example funds that could not be submitted until required documents were supplied; supported contract, licensing and fund approvals. [L:snowflake]
- At fiscal year end, entered the full backlog of pending fund requests in one day so the budget was less affected. [L:snowflake]

**Business Analyst (contract) | VMware** | Aug 2023 to Jan 2024
- Coordinated Data, BI, and Analytics workstreams, including requirements sessions, priorities, status reporting, and deliverable follow-up. [E-049]
- Extracted and cleansed data in Excel for mass Salesforce imports, validating data quality and reporting accuracy. [E-049]
- Checked partner contracts, found data in internal systems and granted new licenses to partners, then recorded the details in Salesforce; promoted from junior to associate level in under five months. [L:vmware]

**Data Analyst, previously Technical Support (SME) | Amadeus** | Jun 2021 to Jun 2023
- Built and maintained a team knowledge base (OneNote and SharePoint, indexed like a documentation site) after the team inherited a product with no documentation; ran weekly sessions to capture new issues and documented them. [L:amadeus]
- Proposed splitting support into subject-matter groups by strength; the manager approved it and it stayed after he left. [L:amadeus]
- Trained about four new hires in two waves and gave feedback to them and their team leads. [L:amadeus]
- Supported a Salesforce-based hospitality product: configured document templates mapped to each customer's Salesforce objects, managed user access and roles, worked with formulas, objects and flows. [L:amadeus]
- As Data Analyst, analysed case data to find why some fixes were faster, using Salesforce, Python scripts and R; documented the findings in the knowledge base. [L:amadeus]

**Customer Service Specialist / Floor Support (SME) | Sykes** | Jan 2020 to Apr 2021
- Handled support for a US financial-services client, then became subject-matter expert (about four months in): coached agents on complex calls and clarified customers' requests. [L:sykes]
- Reviewed team data while the manager was on leave, found knowledge gaps driving call escalations, and reported them. [L:sykes]
- Offered the team-lead role covering a team of 15 to 20; left for Amadeus. [L:sykes]

## Skills
Claude, Codex, multi-agent orchestration, merge gates, CI (GitHub Actions), prompt checklists, SQL, SQL Server, Python, R, Excel, Salesforce, Salesforce Data Loader, Tableau, Power BI (basic), Snowflake notebooks, Workday, Varicent, QA/UAT, data reconciliation, requirements gathering, documentation, training, AWS (coursework exposure) [E-042 to E-044, E-047, E-026 to E-034, L:*]

## Education
Data Science Engineering, LEAD University (in progress, 50%+ completed). [E-045]
Cisco Networking Academy, IT Essentials (certificate). [E-046]

## Languages
Spanish: native. English: B2. [E-041, E-040]
