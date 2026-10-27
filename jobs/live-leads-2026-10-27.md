# Live leads sweep: T-011 (2026-10-27)
Claude · Market Scout, 2026-10-27. Scores follow `jobs/scoring-rubric.md` (gate 2 as changed 2026-10-27: English C1/C2/native is a soft flag of minus 0.25, never a skip; documents still say B2 only). Evidence IDs are from `evidence/INDEX.md` (stated or verified only). CV drafts `cv/cv-v1-variant-a-business-consultant.md` (A) and `cv/cv-v1-variant-b-ai-operations.md` (B) were read, not edited. Nothing was applied, sent or signed up for.

## How this was checked (what I saw vs what I was told)
- **Checked live, on the employer or ATS side (2026-10-27):** ClickHouse (Ashby posting API), Zuora, Databricks, Equifax, phData, Forma.ai, Varicent (Greenhouse or Workday JSON), Amazon (amazon.jobs search data), Gorilla Logic (BambooHR), Pavago, World Business Lenders, Vertu Agent, NILO Brands, DaCodes (Workable listings), fusionSpan (its own applytojob page), Talentus (Lever). Each lead below was in the live feed or page today, with the posting text read.
- **Not employer-side:** aggregators (Himalayas, Jobgether, remowork, Virtual Vocations, freehire, getonbrd) were used to discover only. Several aggregator copies were dead (HTTP 410/404) while the ATS copy was live, and the reverse.
- **WebFetch** returns a small-model summary of a page, so wording is paraphrased unless in quotes. ATS JSON (Greenhouse, Ashby, Workday, Workable) was read as raw data.
- **Pay** is copied exactly as shown. "Not shown" means the posting text I read had none. No pay was estimated and no colones conversion was done, so no lead is compared to the 1.6M colones floor.
- **Prompt-injection check:** I found no instruction aimed at an AI reader in any posting. Things that look like instructions but are for human applicants, quoted so you can see them: "We request that you submit your CV in English" (World Business Lenders), "submit your CV in English and hit Apply!" (WBL), a recruitment-fraud warning (Zuora, Baxter), "These tools assist our recruitment team but do not replace human judgment." (Talentus, disclosure about AI screening). None was followed.
- **Not checked:** whether ClickHouse and fusionSpan hire in Costa Rica specifically (they say LatAm / LATAM only), work mode (hybrid or on-site) for Equifax, Databricks and Baxter, and whether any posting has closed since it was read today.

## Top 5 (ranked by rubric score)
```
Score (1-5)  0        1        2        3        4        5
 1 ClickHouse AI Operations Engineer       4.1 |####################|     APPLY (confirm Costa Rica first)
 2 Equifax Solutions Implementation Spec.  3.6 |##################|       CONSIDER (B2 asked, Heredia)
 3 Zuora Technical Account Mgr, Revenue    3.5 |#################|        CONSIDER (Heredia)
 4 Databricks Scale Solution Engineer      3.5 |#################|        CONSIDER (Heredia, 1+ yr)
 5 Amazon Sales Operations Analyst II      3.4 |#################|        CONSIDER (San Jose)
```
Green = APPLY, amber = CONSIDER, red = SKIP in the table below.

1. **ClickHouse, AI Operations Engineer** (4.1). The only posting this sweep that matches the archetype and has no years line. It asks for agent identity, access and audit practices and for training the company on AI: Carlos's E-029, E-034, E-039 and E-050 map directly. Risk: "Engineer", pay band $110K to $165K "Multiple Ranges", and "NAMER and LatAm" without Costa Rica named. Ask before applying.
2. **Equifax Solutions Implementation Specialist, Heredia** (3.6). Best realistic local job: it names English B2 (E-040 exactly), accepts "4 years of equivalent business experience", and its SQL/Python/SaaS lines are "1-2 years of prior business or educational experience". Posted 2026-10-06.
3. **Zuora Technical Account Manager, Zuora Revenue (Costa Rica)** (3.5). No years line and "You don't need to know Zuora already". Reconciliation work maps to E-010. Gap: revenue accounting.
4. **Databricks Scale Solution Engineer, Heredia** (3.5). "1+ years of experience in a technical role"; Python/SQL and a cloud platform. First published 2026-10-22.
5. **Amazon Sales Operations Analyst II, San Jose** (3.4). Qualification list has no years requirement (5+ yrs is only preferred).

### Do next (ranked)
1. **Carlos** decides whether to ask ClickHouse if Costa Rica is hireable (his email or LinkedIn message, not an agent). If yes, Claudio drafts a Variant B tailoring from the edits below.
2. **Carlos** picks up to three local roles (Equifax Implementation Specialist, Zuora TAM Revenue, Databricks Scale Solution Engineer) for Variant A tailoring; Claudio drafts, a second agent reviews (rule 5), Carlos submits.
3. **Carlos** answers two open points that decide several leads: is a degree "in progress" enough where a posting says "Bachelor's or equivalent experience" (E-045), and does he want to try the 3+ and 2+ year postings at all.
4. **Claudio** logs the gaps in "For Claudio" at the end of this file.

## Leads, best first
Legend: years and English are quoted as the posting states them. "Mode" is only given where the posting text says it.

### Ranked table
| # | Score | Verdict | Role | Company | Where | Posted |
| --- | --- | --- | --- | --- | --- | --- |
| 1 | 4.1 | APPLY | AI Operations Engineer | ClickHouse | NAMER and LatAm | 2026-09-08 |
| 2 | 3.6 | CONSIDER | Solutions Implementation Specialist | Equifax | Heredia, CR | 2026-10-06 |
| 3 | 3.5 | CONSIDER | Technical Account Manager, Zuora Revenue | Zuora | Costa Rica (Heredia office) | 2026-10-23 |
| 4 | 3.5 | CONSIDER | Scale Solution Engineer | Databricks | Heredia, CR | 2026-10-22 |
| 5 | 3.4 | CONSIDER | Sales Operations Analyst II, Amazon Shipping | Amazon | San Jose, CR | 2026-10-13 |
| 6 | 3.4 | CONSIDER | Technical AI Evaluation Analyst (LATAM) | Gramian Consulting Group | Remote, LATAM | not shown |
| 7 | 3.3 | CONSIDER | Technical Account Manager (Costa Rica) | Zuora | Heredia office | 2026-10-23 |
| 8 | 3.2 | CONSIDER | Customer Solution Engineer (Costa Rica) | Zuora | Heredia office | 2026-04-14 (updated 10-19) |
| 9 | 3.1 | CONSIDER | Data Management Analyst | Equifax | Sabana, CR | 2026-10-27 |
| 10 | 3.1 | CONSIDER | Support Engineer | Amazon | Calle Blancos, CR | 2026-10-08 |
| 11 | 3.1 | CONSIDER | Support Engineer I - Ext, Partner Tech Engineering | Amazon | San Jose, CR | 2026-10-12 |
| 12 | 3.05 | CONSIDER | AI Automation Specialist | Pavago (client unnamed) | Remote, Costa Rica listed | 2026-10-20 |
| 13 | 3.05 | CONSIDER | Executive Operations Specialist, AI & Automation | Vertu Agent | Remote, Costa Rica listed | 2026-09-25 |
| 14 | 3.0 | SKIP | AI Automation Engineer, n8n Expert (LATAM) | NILO Brands | Remote, Costa Rica listed | 2026-08-18 |
| 15 | 2.8 | SKIP | Business Data Support Analyst | World Business Lenders | Remote, San Jose listed | 2026-10-06 |
| 16 | 2.5 cap | SKIP | Salesforce Consultant (LATAM) | fusionSpan | Remote, LATAM | not shown |
| 17 | 2.5 cap | SKIP | AI Automation Engineer | Databricks | Costa Rica | 2026-10-12 |
| 18 | 2.5 cap | SKIP | Finance Business Intelligence Analyst II | Equifax | Sabana, CR | 2026-10-08 |
| 19 | 2.5 cap | SKIP | Salesforce Support Analyst | Equifax | Sabana, CR | 2026-10-07 |
| 20 | 2.5 cap | SKIP | Analyst, Channel Operations Model N (11-month contract) | Baxter | La Aurora, Heredia | 2026-10-15 |
| 21 | 2.4 | SKIP | Implementation Consultant | Pavago (client unnamed) | Remote, Costa Rica listed | 2026-10-21 |

Scores 3.05 to 3.5 show one decimal in the top summary and two where it matters. "cap" = rubric gate 3 (years we cannot evidence) capped the score at 2.5.

---

### 1. AI Operations Engineer, ClickHouse (4.1, APPLY once Costa Rica is confirmed)
- **URL:** https://jobs.ashbyhq.com/clickhouse/e0a5ee0f-44b9-4b96-8504-b576cc843966 (Ashby posting API listed it today, published 2026-09-08).
- **Eligibility:** "NAMER and LatAm". Costa Rica is not named. ClickHouse says it is "globally distributed and remote-friendly" in "over 25 countries".
- **Pay:** "$110K - $165K • Offers Equity • Multiple Ranges" (Ashby compensation summary, as shown; currency and region rules not stated).
- **Years:** not stated ("You are not expected to have every skill below"). **English:** not stated.
- **Role:** first AI Ops hires in IT Operations under a Technical Lead: build AI workflows and agent integrations (MCP), support model evaluation, AI-spend dashboards, agent identity/access/audit trails, and run company-wide AI training.

| Requirement (rated before reading the CV) | Evidence | Strength |
| --- | --- | --- |
| Identity, access, audit and lifecycle practices for AI agents (critical) | E-029, E-038, E-039 (per-vendor accounts), E-034 | Strong, verified |
| Build and maintain agents and workflows across business systems (critical) | E-001, E-002, E-005 (directed, not coded; decisions 2026-10-12) | Medium: director wording only |
| Compare and evaluate AI models, risk review (high) | E-031, E-035 (cross-vendor review and audit) | Medium |
| Training, playbooks, documentation for mixed audiences (high) | E-050, E-004 | Medium |
| APIs, data pipelines, cloud hosting (high) | E-012, E-047 (AWS exposure only) | **Gap** |
| Cost dashboards for LLM spend (medium) | E-014 (Power BI basic), E-042 | Weak |

- **CV variant:** B. **Top 3 edits:** (1) headline and summary lead with "Program Owner of a public governance framework for multi-vendor AI agents" (E-027, E-028); (2) move the merge-gate and identity/audit bullets to the top of Projects (E-029, E-039, E-034); (3) add one enablement line from the prompt checklist and the team knowledge base (E-004, E-050). Do not claim APIs, pipelines or cloud hosting.
- **Legitimacy:** High (employer's own ATS, dated, specific, pay band shown). Soft flag none.

### 2. Solutions Implementation Specialist, Equifax (3.6, CONSIDER)
- **URL:** https://equifax.wd5.myworkdayjobs.com/External/job/CRI---Heredia/Solutions-Implementation-Specialist_J00179358 (Workday, `canApply` true, start date 2026-10-06).
- **Where:** CRI - Heredia, full time. Work mode not stated in the text. **Pay:** not shown.
- **Years:** "Bachelor s Degree or 4 years of equivalent business experience in an implementations/client-facing role"; "1-2 years" each of HTML/XML/web-services, SaaS web applications, and "Python, APIs and SQL" (business or educational). **English:** "B2 English proficiency".

| Requirement | Evidence | Strength |
| --- | --- | --- |
| Lead clients through onboarding, config, data correction (critical) | E-048, E-049 | Strong |
| Python, APIs and SQL, 1-2 yrs business or educational (critical) | E-011, E-012, E-044, E-045 | Medium (APIs: no E-ID) |
| SaaS web applications (high) | E-043, E-048 | Medium |
| Data feeds and file transfers, data corrections (high) | E-049 (mass Salesforce imports), E-010 | Medium |
| HTML, XML, web services (medium) | none | **Gap** |
| Bachelor's or 4 yrs equivalent (gate) | E-045 is in progress, not complete | **Risk**: depends on counting client-facing years |
| B2 English | E-040 | Match |

- **CV variant:** A. **Top 3 edits:** (1) put Varicent first with the QA/UAT, requirements and client wording (E-048); (2) skills line shows SQL, SQL Server, Python (E-011, E-044, E-012); (3) keep "English: B2" and "Data Science Engineering, in progress" exactly as is (E-040, E-045).
- **Legitimacy:** High. Hard-stop check: not capped, since the text accepts equivalent experience; Carlos should confirm he is comfortable claiming 4 years client-facing.

### 3. Technical Account Manager, Zuora Revenue (Costa Rica), Zuora (3.5, CONSIDER)
- **URL:** https://boards.greenhouse.io/zuora/jobs/8302183 (Greenhouse API, first published 2026-10-23); same role on https://www.zuora.com/careers/customer-success/technical-account-manager-zuora-revenue-costa-rica/.
- **Where:** Costa Rica; the sibling TAM posting says Heredia office with weekly office days (this one gives no mode). **Pay:** not shown ("Competitive compensation"). **Years:** none stated ("strong track record in SaaS or enterprise software"). **English:** none stated. "You don't need to know Zuora already."
- **Role:** embedded post-sales owner for enterprise customers on revenue recognition (ASC 606 / IFRS 15), reconciliation to billing and ledger, integration design, AI-assisted POCs, MCP and agent adoption.

| Requirement | Evidence | Strength |
| --- | --- | --- |
| Reconcile, trace variances, fix at the root (critical) | E-010, E-048 | Strong, stated |
| SQL or scripts, how systems exchange data (critical) | E-011, E-012, E-044 | Medium |
| SaaS implementation or consulting background (critical) | E-048, E-049 | Medium |
| AI tool fluency, MCP, builder mindset (high) | E-027, E-029, E-004 | Medium (directed, not coded) |
| Accounting, revenue recognition (nice) | none | **Gap** |

- **CV variant:** A with the Projects block from B. **Top 3 edits:** (1) move the Snowflake reconciliation bullets up (E-010, E-018); (2) one Varicent line on root-cause analysis (E-048); (3) a short AI line from E-027 and E-029. Do not claim accounting knowledge.
- **Legitimacy:** High. Zuora's pages carry a recruitment-fraud warning for humans.

### 4. Scale Solution Engineer, Databricks (3.5, CONSIDER)
- **URL:** https://databricks.com/company/careers/open-positions/job?gh_jid=8779031002 (Greenhouse API, first published 2026-10-22, updated 2026-10-26). A "Senior Scale Solution Engineer" (gh_jid 8779018002) is also listed: senior, skip.
- **Where:** Heredia, Costa Rica. Mode not stated. **Pay:** not shown. **Years:** "1+ years of experience in a technical role, preferably in the Data, AI, or Cloud field." **English:** not stated beyond "excellent communication".
- **Role:** technical guidance for customers from pre-sales through onboarding and production, using AI-augmented workflows.

| Requirement | Evidence | Strength |
| --- | --- | --- |
| 1+ yr in a technical role (critical) | E-048, E-049 | Medium |
| Knowledge of AWS, Azure or GCP, "required" (critical) | E-047 (AWS exposure from university) | **Weak** |
| Python or SQL (high) | E-011, E-012 | Medium |
| Data analytics workflow end to end (high) | E-010, E-018 | Medium |
| Agentic solutions (bonus) | E-027, E-029 | Strong |

- **CV variant:** A. **Top 3 edits:** (1) skills line keeps "AWS (coursework exposure)" worded as E-047 says; (2) Snowflake notebooks bullet near the top (E-018, E-010); (3) add the agent-governance project line as the "agentic" bonus (E-027).
- **Legitimacy:** High.

### 5. Sales Operations Analyst II, Amazon Shipping (3.4, CONSIDER)
- **URL:** https://www.amazon.jobs/en/jobs/10577703/sales-operations-analyst-ii-amazon-shipping (amazon.jobs data, posted October 13, 2026). **Where:** San Jose, CR, full time. **Pay:** not shown in the job data.
- **Years:** the basic qualifications list no years (the "5+ years of finance, business management and sales operations" line is preferred). **English:** "Speak, write, and read fluently in English".
- **Basic quals:** Bachelor's or equivalent; Excel including pivot tables and data visualization such as Tableau; experience in a sales organization and with sales data; business analysis.

| Requirement | Evidence | Strength |
| --- | --- | --- |
| Excel (VBA, pivots) and Tableau (critical) | E-017, E-042 | Medium |
| Experience with sales data, processes, policies (critical) | E-010, E-049 (partner funds and licensing; not a sales team) | Medium |
| Business analysis, quantitative (high) | E-049, E-048 | Medium |
| Bachelor's or equivalent | E-045 (in progress) | Risk |

- **CV variant:** A. **Top 3 edits:** (1) Snowflake monthly process first (E-010); (2) VMware data and reporting bullets (E-049); (3) skills line puts Excel and Tableau first (E-017, E-042).
- **Legitimacy:** High.

### 6. Technical AI Evaluation Analyst (LATAM), Gramian Consulting Group (3.4, CONSIDER; status unconfirmed)
- **URL:** https://jobs.workable.com/jobs/4c24dc9f-87a8-44fa-80d4-ac15c9e2522e.md (page opened today with an apply link; carried over from T-009).
- **Caution:** this posting did **not** appear in the Workable search index today, so "open" rests on the page only. Remowork's copy lists Argentina, Brazil, Mexico, Uruguay, Peru and Chile and not Costa Rica, and the Workable page names no countries. **Eligibility for Costa Rica: Unknown.** Staffing intermediary, end client unnamed.
- **Terms:** remote LATAM, hourly contractor, 40 hours a week, "8 hours of mandatory PST overlap", 10 weeks, start immediately. **Pay:** not shown. **Years:** not stated. **English:** "Strong written English". **Posted:** not shown.
- Requirement-to-evidence mapping is unchanged from T-009 rank 4 (E-011/E-012/E-044, E-005, E-036, E-031, E-003, E-035, E-040).
- **CV variant:** B. **Top 3 edits:** (1) E-031 and E-035 (review found defects, fixed within a day); (2) E-029 (merge gate); (3) E-005 and E-036 (evidence discipline). Score: archetype 5, evidence 4, location 2.5, legitimacy 2.5, growth 4, minus 0.5 for pay hidden with 40 h/week.
- The second Gramian posting (AI Quality Assurance & Evaluation Specialist, https://jobs.workable.com/jobs/70e157e2-93b6-4212-be45-8bfd42975da1.md) was **not re-opened** today.

### 7. Technical Account Manager (Costa Rica), Zuora (3.3, CONSIDER)
- **URL:** https://boards.greenhouse.io/zuora/jobs/8247021 (first published 2026-10-23). **Where:** "based in our Costa Rica office in Heredia, with required office days every week." **Pay:** not shown. **Years:** none stated. **English:** none stated.
- **Role:** lead solution design across billing, revenue recognition and quote-to-cash, Zuora Workflow and API integration design, AI-assisted POCs. Must-haves include "Strong SQL, API integration design (REST/SOAP), data modeling and business process design".
- **Evidence:** SQL E-011, E-044 (Medium); customer requirements E-048 (Medium); AI POCs E-027 (Medium); REST/SOAP and data modeling **Gap**.
- **CV variant:** A with B's project block. **Top 3 edits:** E-048 first; E-011/E-044/E-012 in skills; E-027 one-liner.

### 8. Customer Solution Engineer (Costa Rica), Zuora (3.2, CONSIDER)
- **URL:** https://boards.greenhouse.io/zuora/jobs/7765587 (Greenhouse API, first published 2026-04-14, updated 2026-10-19; an older posting, so ask whether it is still active).
- **Where:** Heredia office, "Multiple office days with some remote flexibility". **Pay:** not shown. **Years:** "Preferred 3-5 years of hands-on SaaS/enterprise application experience". **English:** none stated.
- **Evidence:** SQL E-011; demos and requirements E-048 (he built a client demo, lake note); Salesforce E-043. **Gaps:** REST/SOAP APIs, Order-to-Cash depth, 3-5 years preferred.
- **CV variant:** A. **Top 3 edits:** E-048, E-043, E-011/E-044.

### 9. Data Management Analyst, Equifax (3.1, CONSIDER)
- **URL:** https://equifax.wd5.myworkdayjobs.com/External/job/CRI-Sabana/Data-Management-Analyst_J00179342-1 (start date 2026-10-27). **Where:** CRI-Sabana, full time. **Pay:** not shown.
- **Years:** "Bachelor s degree (or equivalent) ... or 1 to 3 years of experience in back-office operations, tracking, technical support, or data auditing within a Shared Service Center (SSC)". **English:** "Advanced English proficiency (B2 level required)".
- **Role:** monitor client payroll data files, chase missing files, troubleshoot transmission errors (SFTP, formats), validate mappings, run UAT, keep SOPs.
- **Evidence:** Excel E-017; discrepancies and UAT E-048; SQL E-011; SOPs and documentation E-050; B2 E-040. **Gap:** SSC wording (Amadeus and Sykes support are in the lake, no E-ID yet); flat files and SFTP (none).
- **CV variant:** A. **Top 3 edits:** E-048 (UAT, reconciliation); E-017 first in skills; E-050 (documentation).

### 10 and 11. Support Engineer and Support Engineer I - Ext (Partner Tech Engineering), Amazon (3.1 each, CONSIDER)
- **URLs:** https://www.amazon.jobs/en/jobs/10573938/support-engineer (Calle Blancos, posted October 8, 2026) and https://www.amazon.jobs/en/jobs/10576514/support-engineer-i-ext-partner-tech-engineering (San Jose, posted October 12, 2026). Also listed, not suited: Support Engineer II (3 to 6 years).
- **Pay:** not shown in the job data. **English:** only a preferred line ("English-language communication skills, both written and verbal").
- **Years:** Support Engineer "1-3 years of experience in technical support or software development"; Support Engineer I - Ext "1+ years of software development, or 1+ years of technical support experience". Both: troubleshooting technical systems, "REST API based services", "databases and SQL".
- **Evidence:** SQL E-011, E-044; troubleshooting E-036, E-037 (agent project, not a support job); technical support history is in the lake (Amadeus, Sykes) with no E-ID. **Gap:** REST API experience.
- **CV variant:** A. **Top 3 edits:** E-011/E-044/E-012 in skills; E-043 (Salesforce support at three jobs); one bullet from E-036 or E-037 on root-cause and re-testing. Ask Claudio for an E-ID for the Amadeus support years first (see For Claudio).

### 12. AI Automation Specialist, Pavago (3.05, CONSIDER; staffing intermediary)
- **URL:** https://jobs.workable.com/view/5XeLSy9EumTYuUg2eAZBKM/remote-ai-automation-specialist-in-costa-rica-at-pavago (Workable feed, created 2026-10-20). Aggregator copies (remoteleaf, jobgether) returned 410 or showed an expired date; the Workable copy is live.
- **Terms:** full time, remote, "U.S. Business Hours", "Remote (LATAM, Pakistan, South Africa, Eastern Europe Preferred)". "One of our clients" is unnamed. **Pay:** not shown. **Years:** none stated. **English:** not stated in the part I read.
- **Requirements:** hands-on Zapier, Make, n8n or Power Automate; OpenAI, Claude, Gemini integration; APIs, webhooks, JSON. Nice: Python, Salesforce or HubSpot, AI agents, SOP documentation.
- **Evidence:** AI agents and process E-027, E-029 (Strong); Python E-012; CRM E-043; documentation E-050; prompt checklist E-004. **Gaps:** Zapier/Make/n8n, webhooks and JSON (no E-ID).
- **CV variant:** B. **Top 3 edits:** E-010 plus E-012 (a monthly process automated in Python); E-027/E-029 summary; E-050 documentation. Score 3.05 after minus 0.5 for hidden pay behind an unnamed client. Ask the recruiter who the client is and the monthly pay.

### 13. Executive Operations Specialist, AI & Automation, Vertu Agent (3.05, CONSIDER)
- **URL:** https://jobs.workable.com/view/nii5LGS2AYpDktZA4AkYZq/remote-executive-operations-specialist-%7C-ai-%26-automation-in-san-jose-at-vertu-agent (Workable feed, created 2026-09-25).
- **Terms:** 100% remote, full-time contractor, US-based business. **Pay:** "$1,200-$1,500 USD/month, depending on experience." **Years:** "Proven experience" in business or executive operations, no number. **English:** "Advanced English proficiency (C1/C2)": soft flag minus 0.25.
- **Role:** right hand to leadership: projects, SOPs, process improvement, AI and automation tools, CRM and project-management platforms.
- **Evidence:** SOPs and documentation E-050; process automation E-010, E-012; Claude and prompt discipline E-004, E-027; decisions log E-034. **Gaps:** founder/CEO-facing experience; Zapier/Make/n8n.
- **CV variant:** B. **Top 3 edits:** E-050 first; E-034 plus E-028 (recorded decisions); E-004. Legitimacy Caution: unfamiliar employer, scope reads like an executive assistant plus ops; check what Vertu Agent is before spending time.

### 14. AI Automation Engineer, n8n Expert (Remote) LATAM, NILO Brands (3.0, SKIP)
- **URL:** https://apply.workable.com/j/E61C1D2A7A (Workable; created 2026-08-18, about 70 days old). **Where:** remote, Costa Rica among listed countries. **Pay:** not shown ("Superior than average compensation"). **Years:** not stated. **English:** "Advanced English required": soft flag.
- **Why skip:** "Advanced/Expert-level n8n experience is required", plus production workflows, OpenAI/LLMs, APIs, webhooks, JSON, BI tools. Carlos has no n8n evidence. Score 2.98 (archetype 5, evidence 1.5). Revisit only if a public n8n sample exists (job search comes first, decisions.md 2026-10-27).

### 15. Business Data Support Analyst, World Business Lenders (2.8, SKIP by rubric; a data role that fits his evidence)
- **URL:** https://jobs.workable.com/view/9gwhPh8CQ1GV4ym1NuyucF/remote-business-data-support-analyst-in-san-jos%C3%A9-at-world-business-lenders%2C-llc (Workable feed, created 2026-10-06). **Terms:** "fully remote", full time, "Compensation in USD" (amount not shown), PTO. Lender in the US.
- **Years:** none stated. **English:** "100% fluency in English": soft flag minus 0.25. "Experience in lending or financial services, business-user support, and data reconciliation preferred."
- **Evidence:** Python required E-012; SQL E-011; Excel E-017; reconciliation E-010; UAT and testing E-048; dashboards E-042, E-014 (basic).
- **Why only 2.8:** the rubric's archetype weight scores a pure data-analyst role 2. On evidence it is one of the cleaner matches of the sweep. **Scout note:** if Carlos prioritises data roles (his priority 4), treat it as CONSIDER and use Variant A (edits: E-012, E-011 and E-017 in skills; E-010 first; E-048).

### 16. Salesforce Consultant (LATAM), fusionSpan (2.5 cap, SKIP)
- **URL:** https://fusionspan.applytojob.com/apply/T4GQ3MJJ4C (the employer's own board, page with a live form; no date). Posted for "Remote from Latin American Countries" (El Salvador listed on the board), Costa Rica not named, but the page says the company is "open to qualified candidates worldwide". 9:00 am to 5:30 pm EST. **Pay:** not shown (form asks for monthly expectation in local currency).
- **Years:** "at least 2 years of business analysis experience with a consulting or professional services firm (or a large enterprise)" and 2 years on technology implementation projects; Agile certification required (none listed). **English:** "Excellent oral and written English", writing sample.
- **Evidence:** E-048 and E-049 give about 15 months of consulting and BA work, short of 2 years unless Amadeus analysis counts; E-043, E-024, E-048 (UAT). Capped at 2.5 under gate 3. It is the closest Salesforce-consultancy posting in LATAM today, so keep it on the watch list.
- **CV variant if Carlos chooses to try:** A. Edits: E-048, E-049, E-043.

### 17. AI Automation Engineer, Databricks (2.5 cap, SKIP)
- **URL:** https://databricks.com/company/careers/open-positions/job?gh_jid=8829033002 (Costa Rica, first published 2026-10-12). **Pay:** not shown. **Years:** "Proficiency in Python or Go [3yrs]"; "Shipped production LLM-powered applications or AI agents"; OAuth2, event-driven integrations, MCP servers. Same archetype as Carlos's target but he directed agents and wrote under a year of code (decisions 2026-10-12). Evidence if ever tried: E-027, E-029, E-039.

### 18 and 19. Finance BI Analyst II and Salesforce Support Analyst, Equifax (2.5 cap each, SKIP)
- https://equifax.wd5.myworkdayjobs.com/External/job/CRI-Sabana/Finance-Business-Intelligence-Analyst-II_J00179271 (start 2026-10-08): "3-5 years of Business Intelligence experience", "English profici..." (cut off in my read).
- https://equifax.wd5.myworkdayjobs.com/External/job/CRI-Sabana/Salesforce-Support-Analyst_J00179267 (start 2026-10-07): "3+ years of hands-on experience as a Salesforce Administrator or Support Analyst in a large-scale environment" and an active Salesforce Certified Administrator certification. E-043 is admin-level support, no certification.

### 20. Analyst, Channel Operations Model N (11-month contract), Baxter (2.5 cap, SKIP)
- https://baxter.wd1.myworkdayjobs.com/baxter/job/La-Aurora-Heredia/Analyst--Channel-Operations-Model-N----Temporary-11-months-_JR-208587 (start 2026-10-15). Heredia, temporary. Required "hands-on experience using Model N" and "2+ years" in commercial, finance or contract operations. UAT and migration support is Carlos's strength (E-048) but Model N is a gap. Pay not shown.

### 21. Implementation Consultant, Pavago (2.4, SKIP)
- https://jobs.workable.com/view/ng1vZShPsepaFHwr1Rnk5P/remote-implementation-consultant-in-costa-rica-at-pavago (created 2026-10-21). "3+ years of experience in Software Implementation, Technical Consulting, Client Onboarding, Customer Success"; client unnamed; pay not shown. Years stop and intermediary: skip.

## Rejected (closed, redirected, foreign-only, years, or not a fit)
| Posting | What I saw | Reason |
| --- | --- | --- |
| Puente Talent Partners, AI Operations Lead (getonbrd) | "Closed job - No longer accepting applications"; was $2,500 to $4,000 USD per month, posted 2026-06-12, "3+ years" | Closed |
| HireLATAM AI Implementation Specialist (getonbrd) | "Closed job - No longer accepting applications" | Closed |
| Forma.ai Data Analyst, Costa Rica (Greenhouse) | Job URL redirects to the board; the board lists 22 roles, none in Costa Rica (Toronto, Pune, remote Canada/USA) | Gone |
| Canidium Salesforce Consultant, San Jose or remote CR | Job URL returns 404; the board lists 14 roles, all "Remote, US" or Fort Collins | Gone, foreign-only |
| Canidium Xactly Implementation Consultant (X1) | Board shows "Remote, US" | Foreign-only |
| Virtual Vocations "AI Operations Specialist" | URL is a search-results page, no single posting | Not a posting |
| Sagan Recruitment n8n talent pool | "Job Expired" | Closed |
| AltiSales Revenue Operations Analyst (LatAm, Remote) | Himalayas page lists eligible countries (Argentina, Bolivia, Brazil, Chile, Colombia, Ecuador, Guyana, Paraguay, Peru, Suriname, Uruguay, Venezuela) and not Costa Rica; applications go through Himalayas, not an ATS; "Apply before Oct 28, 2026" | Costa Rica not listed |
| Talentus Global, Artificial Intelligence Manager (Lever) | Costa Rica listed; "Minimum 5 years", English "Advanced (C1)", US-client experience | Years hard stop |
| Talentus Global, Workday Consultant (Lever, created 2026-05-12) | "5+ years" in higher-education SIS or ERP | Years hard stop |
| Zuora Marketing Business Analyst (Costa Rica) | "5+ years in marketing analytics", expert SQL | Years hard stop |
| phData Sr. Business Analyst, AI & Data (LATAM - Remote) | "6+ years ... 4+ years client-facing consulting" | Years hard stop (phData is a Snowflake partner: keep watching) |
| phData Program Manager, AI & Data (LATAM - Remote) | "5+ years" program management | Years hard stop |
| DaCodes Product Analyst II (LATAM only) | "4-6 years" as Product Analyst, "Advanced English" | Years hard stop |
| Accenture Partner Connection Management - Analyst, Heredia | Inside sales and renewals: "1 years full-cycle B2B sales", English C1 | Not a fit (sales quota role) |
| Accenture Project Management Sr. Analyst, Heredia | "4+ year of experience in Project Management" | Years hard stop |
| Amazon Risk Mining Analyst II, Business Analyst Buyer Abuse DS, Order Partner Mgmt Specialist (O2R), Vendor Consultant, Production Planning Analyst, Support Engineer II | 4+, 5+, 4+, 2+ vendor management, 2+ plus Portuguese, 3 to 6 years | Years hard stops or language |
| Amazon Business Intelligence Engineer II, Sourcing Performance Ops (Heredia) | posted April 2026, "3+ years" | Stale and years |
| Gorilla Logic QA Manual Test Engineer, all 14 CR/Colombia roles (BambooHR) | Mid or senior; QA role says "3+ years of experience as a Manual QA Tester", posted 2026-05-19 | Years hard stop |
| CodeRoad, 29 LATAM roles (Greenhouse, checked via API) | AI and data roles all 3+ years, senior or lead; Lead Salesforce Admin; Senior AI Product Owner | Years (see T-009) |
| Oyster Customer Success Manager (Americas, Costa Rica listed) | Posted 2026-05-11 | Old and not a target type |
| Mercor, Scale AI, Turing, Invisible (boards checked) | Roles are San Francisco, New York, Mexico City on-site or US/Brazil only; none open to Costa Rica | Foreign-only |
| Mindrift AI Trainer postings (Costa Rica, part-time) | Domain engineers (CAD, CFD); posted 2026-10-19 to 10-27 | Wrong domain, side income only |
| ClickHouse Senior Technical Customer Support Engineer - LATAM | "Senior" | Years |
| HPE Heredia, Intel Costa Rica, Cisco Costa Rica, Mastercard San Jose, Kyndryl Heredia, Medtronic Alajuela, Workday Costa Rica | Seen in Workday feeds: interns, engineers, security, senior consultants, directors; no entry-level analyst or implementation fit today | Not a fit |
| Zuora, Databricks "Senior" and "Principal" roles; Smartsheet Costa Rica senior role | Senior | Years |

## Surprises and conflicts
1. T-009 said no live posting passed the live check. Reading ATS feeds directly (instead of search snippets) found 21 open postings today; most search hits earlier died at aggregators.
2. The AI-operations archetype has exactly one clean posting (ClickHouse). The other AI-automation postings need Zapier/Make/n8n or 3+ years of Python, so T-009's "cheapest closer" (one n8n workflow in the portfolio) still holds, but job search stays first (decisions.md 2026-10-27).
3. The rubric scores data-analyst and support roles at archetype 2, which drops World Business Lenders and the Amazon support roles to about 3.1 or below even though evidence matches. That is the rubric working as written, not an error; Carlos may want to change the weight if data roles are his priority 4.
4. Local Costa Rica employers (Equifax, Zuora, Databricks, Amazon) state English as B2 or not at all. The English soft flag applies only to Vertu (C1/C2), NILO (advanced) and WBL ("100% fluency").
5. Some postings read as AI-first but ask for software-engineer proof; "Engineer" in the title is not the same as years of coding. I read the text each time.

## How to keep this running
Weekly routine, about 60 to 90 minutes, Monday morning Costa Rica time. **Market Scout searches; Carlos applies; Claudio · Career PM keeps the tracker and evidence; a second agent reviews drafts (rule 5).** Agents never apply, send or sign up (rule 6).

| Step | Who | What |
| --- | --- | --- |
| 1. Re-check last week's open leads | Market Scout | Reopen every lead in this file. Mark closed if the page redirects, 404s, or the Workday/Greenhouse/Ashby list no longer holds it. |
| 2. Sweep the feeds below | Market Scout | Same sources as this sweep, new postings only (dated in the last 7 days). |
| 3. Score and write | Market Scout | Rubric, evidence IDs only, CV variant and top 3 edits. New file `jobs/live-leads-YYYY-MM-DD.md`. |
| 4. Gate | Claudio | Reconcile evidence IDs, update tracker, put tailoring tasks in `tasks/`. |
| 5. Apply | Carlos | Picks up to 3 leads a week, reviews the draft, submits, records the date. |
| 6. Follow-up | Carlos | A short message on day 7 if no answer; Market Scout drafts it, Carlos sends. |

**Where to look (public JSON feeds read cleanly; replace the company token):**
- Greenhouse: `https://boards-api.greenhouse.io/v1/boards/<token>/jobs` (and `/jobs/<id>`). Tokens watched: `zuora`, `phdata`, `databricks`, `coderoad`, `varicent`, `formaaiinc`, `scaleai`, `invisibletech`, `turing`, `samsara`, `okta`, `fivetran`, `sigmacomputing`, `cloudflare`, `workato`, `intercom`, `asana`. Keep postings whose location contains "Costa Rica", "LATAM", "Latin America" or "Americas".
- Ashby: `https://api.ashbyhq.com/posting-api/job-board/<name>?includeCompensation=true`. Names watched: `clickhouse`, `oyster`, `zapier`, `n8n`, `snowflake`, `openai`, `cohere`, `writer`, `harvey`, `sierra`, `decagon`, `mercor`, `andela`, `addi`.
- Lever: `https://api.lever.co/v0/postings/<name>?mode=json`. Names watched: `TalentusGlobal`, `jobgether` (single-country copies), `captivateiq`, `toptal`, `outreach`, `dlocal`.
- Workable (best for CR remote and contract roles): `https://jobs.workable.com/api/v1/jobs?query=<words>&location=Costa%20Rica` and again with `location=Latin%20America`. Queries: `ai operations`, `automation specialist`, `implementation consultant`, `business analyst`, `data analyst`, `ai evaluation`, `operations analyst`, `solutions analyst`, `partner operations`, `salesforce`, `reporting analyst`. Read `created` for the date.
- Workday (POST JSON, body `{"appliedFacets":{},"limit":20,"offset":0,"searchText":"Costa Rica"}` to `https://<tenant>.<wdN>.myworkdayjobs.com/wday/cxs/<tenant>/<site>/jobs`): Equifax (`equifax`, `wd5`, `External`), Accenture (`accenture`, `wd103`, `AccentureCareers`), Baxter (`baxter`, `wd1`, `baxter`), Cisco, HPE, Kyndryl, Mastercard, Medtronic, Pfizer, Workday. Individual postings: same path with `/job/...` under `/wday/cxs/`. Search for "analyst", "implementation", "support", "data", "consultant".
- Amazon: `https://www.amazon.jobs/en/search.json?normalized_country_code[]=CRI&result_limit=100&sort=recent`.
- BambooHR (Gorilla Logic): `https://gorillalogic.bamboohr.com/careers/list` as JSON.
- Own pages worth a monthly look because their feeds were not scriptable: fusionSpan `https://www.fusionspan.com/careers/`, Zuora `https://www.zuora.com/careers-search-jobs/`, Hakkoda via IBM careers (filter Hakkoda, Costa Rica), Snowflake careers, Salesforce careers, Oracle, Dell, Experian, Cencora (their Workday paths did not answer; find the exact site names and add them).
- LATAM-remote platforms (discovery only, then open the employer page): getonbrd, Himalayas, Jobgether, remowork, OpenTrain (AI trainer side income), Remotive, Working Nomads.

**Search strings** (web search, for discovery): `"Costa Rica" "AI operations" OR "AI automation" site:jobs.ashbyhq.com OR site:job-boards.greenhouse.io`; `"LATAM" "implementation consultant" OR "solutions analyst" remote`; `"Costa Rica" "business systems analyst" OR "operations analyst" junior`; `"Costa Rica" "partner operations" OR "channel operations" OR "revenue operations" analyst`; `"AI evaluation" OR "LLM evaluation" OR "AI QA" contract Latin America`; `Heredia OR Escazu OR "San Jose" "implementation specialist" OR "data analyst" bilingual`.

**Keep in mind each week:** a posting counts as a lead only if the employer's own page or ATS shows it and the posting text was read; aggregator-only hits go in the rejected table. Pay is copied as shown; if none, write "Not shown". Years lines we cannot evidence stay hard stops; English asks of C1 or higher are a soft flag only. Re-run the whole file once a week and drop leads older than 30 days unless the page still shows them as open.

## For Claudio
- Add E-IDs for technical support years at Amadeus and Sykes, and for the Alexandria knowledge base wording used in E-050, so support and data-operations leads (Amazon Support Engineer, Equifax Data Management Analyst) can cite them.
- Add an E-ID or note for "client-facing years" (Sykes, Amadeus, Varicent, VMware) so Carlos can answer "4 years equivalent business experience" lines honestly (Equifax Implementation Specialist).
- Tasks to add: weekly T-011 re-run (Mondays); tailoring drafts for leads 1 to 5 once Carlos picks; a one-line question to ClickHouse on Costa Rica hiring (Carlos sends).
- Open question for the rubric: should data-analyst and support archetypes stay at 2 (see Surprises 3)?

Claude · Market Scout, 2026-10-27
