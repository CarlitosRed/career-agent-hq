# Queue (open work only; done tasks dropped 2026-10-27, history is in git and `decisions.md`)

| ID | Owner | Task | Needs |
| --- | --- | --- | --- |
| T-009 | Claude · Market Scout | Done 2026-10-27: `jobs/targets-ranked-2026-10-27.md` (top: AI ops 3.85, agent freelance 3.83; nothing at 4.0, no APPLY today). Follow-ups: English test result, one public fictional-data agent+evals sample, reconcile E-009..E-025 with the lake | Carlos picks |
| T-011 | Claude · Market Scout | Live job search sweep: real, open, CR/LATAM-eligible postings for the top role types in `jobs/targets-ranked-2026-10-27.md`; one file `jobs/live-leads-<date>.md`; Carlos applies himself | Running 2026-10-27 |
| T-004 | Writer (Claude drafts, another Claude reviews) | CV v1 drafted 2026-10-27: `cv/cv-v1-variant-a-business-consultant.md`, `cv/cv-v1-variant-b-ai-operations.md`. Needs truth review, then Carlos's picks (see "Open before this can go out" in each file) | Review + Carlos |
| T-005 | Writer (same) | Build LinkedIn from scratch: headline, About, Experience, Featured. Drafts only; Carlos creates the profile | Interview rounds done + Carlos says the "who I am" picture is ready |
| T-006 | Claude · Truth Reviewer | Review panel: 1 ATS-screen reader, 1 hiring manager, 5 persona readers (manager, other applicant, CEO, recruiter, technical lead), each alone; then one rewrite constrained to evidence IDs | T-004, T-005 |

## Interview rounds (lake in `lake/companies/`, all `stated`)
- Done: Sykes r1-3, Amadeus r1-3, VMware r1-2, Snowflake r1-2, Varicent r1-2 (employer name is Varicent; "Barisant" was misheard).
- Open after r2: a Snowflake reference; Varicent product name. "YC" dropped by Carlos 2026-10-27. Varicent is settled: Business Consultant, Aug 2025 to May 2026. E-009 and E-022 now tie to Varicent, and E-018 can move to `stated` (evidence-writer request, not edited here). Snowflake is Dec 2024 to Jul 2025.
- Rule: never write health details in the repo; they stay in git-ignored `raw/interviews/`.

## Still open for Carlos
1. Current CV example received 2026-10-27 (`raw/cv/Carlos_Redondo_TransUnion_Data_Science_Analytics_Analyst_CV.pdf`, git-ignored; it is a targeted CV for one employer, so a source to check, not proof). LinkedIn has no existing text.
   **Conflicts between the CV example and the interviews (Carlos to settle before T-004):**
   - Settled 2026-10-27 by Carlos: Snowflake Dec 2024 to Jul 2025, Spanish native, Varicent title Business Consultant (see `decisions.md`). Skills check: `audits/cv-skills-check-2026-10-27.md`; amber lines await his yes/no.
   - Snowflake tools: CV says Salesforce, Excel, SQL, Salesforce Data Loader; interviews say Snowhouse SQL, Workday, Excel, Python, notebooks, an internal partner system. No Python on the CV's Snowflake bullets.
   - CV skills the lake does not cover yet: Tableau, PostgreSQL, MySQL, SQL Server, R, Spark, AWS/Azure exposure, LEAD University degree (50%+, GPA 4.01), Cisco IT Essentials, "5+ years" summary. All need a stated/verified evidence entry before use.
2. Exact employers, titles, dates: all `stated`, several Unknown (Snowflake start month, Varicent dates and title, Amadeus months).
3. Public-safe: Varicent yes. (Sykes, Amadeus, VMware, Snowflake: see each lake file header.)
4. Which legacy tools (SQL, Python, Power BI, Salesforce, Workday...) were used professionally: now mostly covered by the lake; confirm gaps in the CV step.
5. Repo is public until about 2026-11-02, when Carlos plans to make it private (`decisions.md` 2026-10-26; exposure audit in `audits/`).
