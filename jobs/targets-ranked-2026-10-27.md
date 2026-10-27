# Targets ranked: T-009 re-rank (2026-10-27)
Claude · Market Scout, 2026-10-27. Supersedes the "best target" calls in `market-scan-2026-10-12.md` section 6 where they conflict (see Surprises).

How to read this file
- **Checked live** = I opened the employer's own page (WebFetch, which returns a small-model summary of the page, so wording is paraphrased unless in quotes). **Reported** = search snippet or aggregator, not opened on the employer's side. **Inferred** = my judgement from patterns, no posting behind it.
- Scores follow `jobs/scoring-rubric.md` (archetype 30%, evidence 25%, location and terms 15%, legitimacy 15%, growth 15%; soft red flag minus 0.5). A role TYPE with no live posting is scored on typical content and its legitimacy is capped at 2, because rubric gate 1 needs a live employer page. Type scores are provisional until a posting exists.
- Carlos facts used (all `stated` except E-026..E-039 `verified`): CR based, remote or local CR, ideally above 1.6M colones/month gross, English B2 (E-040), Spanish native (E-041), under 1 year hands-on dev (decisions.md 2026-10-12).
- Pay is copied exactly as shown. "Not shown" means the page showed none. No pay was invented or estimated. Colones-to-dollar conversion not checked, so no posting could be compared to the 1.6M floor.
- Evidence note: `evidence/INDEX.md` still lists E-009 to E-025 as `unverified`, but `lake/companies/*.md` records Snowflake, Varicent, SQL, Python and Salesforce items as `stated`, and E-042 to E-049 are `stated`. Where I cite E-009..E-025 below I mark it "(index: unverified, lake: stated)". Claudio to reconcile.
- Prompt-injection check: every employer page I opened was read for instructions aimed at an AI reader. None found. (One page, Varicent's careers, carries a recruitment-scam warning for humans; not an instruction to me.)

## Verdict at a glance
```
Score (1-5)   0        1        2        3        4        5
 1 AI ops / automation specialist       3.85 |#######################|  CONSIDER (type, no live posting)
 2 Agent freelance / workflow setup     3.83 |#######################|  CONSIDER (type; Upwork page blocked)
 3 AI governance / program ownership    3.50 |#####################|    CONSIDER (type, nothing found)
 4 AI evaluation analyst (Gramian x2)   3.43 |####################|     CONSIDER (live page, status unconfirmed)
 5 Snowflake-partner associate consult  3.25 |###################|      CONSIDER when a posting is live
 6 Implementation consultant (Varicent) 3.15 |###################|      CONSIDER when a posting is live
 7 Partner / business-ops analyst       3.00 |##################|       CONSIDER (borderline)
 8 Salesforce / business systems analyst 2.80 |################|        SKIP today
 9 AI trainer / expert contractor       2.65 |###############|          SKIP (side income only)
10 Data / BI analyst, Costa Rica        2.60 |###############|          SKIP today
```
Colour key for the table below: green = go, amber = conditional, red = skip/gate fail.

| Rank | Role type | Score | Live-checked posting | Verdict |
| --- | --- | --- | --- | --- |
| 1 | AI operations / automation specialist | 3.85 | none (one aggregator lead, unopened) | AMBER consider |
| 2 | Agent freelance / AI workflow setup | 3.83 | none (Upwork returned 403) | AMBER consider |
| 3 | AI governance / program-owner roles | 3.50 | none found | AMBER consider |
| 4 | AI evaluation / agent QA analyst | 3.43 | Gramian x2, page opened, no date | AMBER consider |
| 5 | Snowflake-partner associate consultant | 3.25 | none open (old postings expired) | AMBER watch |
| 6 | SaaS implementation / business consultant | 3.15 | none open at Varicent in Costa Rica | AMBER watch |
| 7 | Partner / revenue / business ops analyst | 3.00 | none eligible | AMBER borderline |
| 8 | Salesforce / business systems analyst | 2.80 | none live | RED skip today |
| 9 | AI trainer / expert contractor | 2.65 | none opened | RED skip (side income) |
| 10 | Data / BI analyst, Costa Rica | 2.60 | none live (one 404, one hard stop) | RED skip today |

Nothing reaches 4.0, so there is no APPLY today. The honest picture: Carlos's evidence is strong for the roles at the top, but the market for juniors who are CR/LATAM-eligible, B2 English and under 1 year of dev is thin on live employer pages.

## Main gap (applies to almost every row)
1. **Years and a named stack.** Roles that say "AI engineer" ask 3+ yrs software dev, LangGraph/CrewAI, MCP, vector DB. Hard stop (cap 2.5). Fix: one public fictional-data sample (agent workflow with evals) plus the public framework repo (E-027).
2. **English B2.** Two roles I opened need C1+ or C2 (CodeRoad Senior AI Product Owner "C1+ English fluency"; Entrepreneur Cooperative "near-native English (C2)", reported). Under rubric gate 2 those are SKIP. A recognised English test result would let us test this gate honestly (E-040 stays `stated`).
3. **No numbers anywhere** in the lake (Carlos: "idk"). Roles that screen on metrics will score him low; roles that screen on process, documentation and judgment will not.

---

## 1. AI operations / automation specialist (score 3.85, type)
Status: **inferred type**; one lead found, **reported only** (Virtual Vocations aggregator, "AI Operations Specialist", part-time contract, remote within Latin America, requires 1+ yr low-code automation (Zapier) and SQL, compensation "to be discussed"). I could not open the employer's own page (the Virtual Vocations URL returned a search-results page), so gate 1 is not passed for that lead.
Scores: archetype 5, evidence 4, location/terms 3, legitimacy 2 (cap), growth 4.

| Requirement (typical + the lead) | Evidence | Strength |
| --- | --- | --- |
| Automate a recurring manual data process | E-010, E-012 (Snowflake Excel-to-Python, index: unverified, lake: stated) | Medium (no hour counts, nothing to show) |
| SQL | E-011, E-044 (SQL Server, Snowflake; SQL at Varicent E-048) | Medium |
| Low-code tools (Zapier, n8n, Make) | none | **Gap** |
| Knowledge capture, documentation for teams | Alexandria (Amadeus lake note; no E-ID yet, stated only in lake) | Medium, no E-ID: Claudio to add |
| Agents with gates and review | E-001, E-002, E-003, E-029 (verified) | Strong |
| Remote async across time zones | VMware lake note (stated; no E-ID) | Medium |

Gaps: Zapier/n8n/Make, dashboards, any metric. Verdict: **CONSIDER**. Cheapest closer: one n8n workflow in the portfolio sample (also serves rank 2). Do not apply to the unopened lead until its employer page is read.

## 2. Agent freelance / AI workflow and agent-team setup (score 3.83, type)
Status: **reported + inferred**. Upwork listing pages exist (n8n / Make / AI-agent postings turned up in search) but my fetch of one returned HTTP 403, so none was checked live. Rates seen in search, **reported, not verified**: one vendor blog "roughly $40 to $100 per hour" for n8n experts; one posting snippet showed "$5.00 to $20.00" hourly. Costa Rica eligibility and withdrawal options for Upwork: **Unknown** (not found).
Scores: archetype 5, evidence 3, location/terms 3 (no gate, but income unproven vs the 1.6M floor), legitimacy 2.5, growth 5.

| Requirement | Evidence | Strength |
| --- | --- | --- |
| Design agent roles, rules, approval gates | E-001, E-002, E-004, E-029 (verified); E-028 Program Owner (stated) | Strong, uncommon |
| Document-to-data workflow with human review | E-005 (verified; generic wording only) | Strong, no public sample yet |
| Cross-vendor QA, audits, flaky-test fixes | E-003, E-031, E-035, E-037 (verified) | Strong |
| Python for scripts | E-012 (index: unverified, lake: stated) | Medium |
| n8n, Make, Zapier, CRM integration | none | **Gap** |
| Client communication, scoping | E-048 (Varicent requirements), E-049 | Medium |

Gaps: no finished client project, no reviews, no public portfolio, low-code tools. Verdict: **CONSIDER**, as the parallel track the 2026-10-12 Upwork scan already recommends. It is the only type where years of dev and English level are not gates. Income claim: Unknown until 3 to 5 gigs close.

## 3. AI governance / program-owner / delivery-for-AI-teams (score 3.50, type)
Status: **inferred**. No posting for this exact title found open to Costa Rica today. It maps Carlos's strongest verified material (E-026..E-039: public governance framework, merge gate, audits). Keep as a positioning target and as the headline for LinkedIn and CV, and watch for "AI program manager", "AI delivery lead", "AI risk/controls analyst" titles.
Scores: archetype 4, evidence 4.5, location/terms 2.5 (unknown), legitimacy 1.5 (nothing found), growth 4.

| Requirement (typical) | Evidence | Strength |
| --- | --- | --- |
| Own process and decisions for agent work | E-028 (stated), E-027 (verified) | Strong |
| Controls, audit trail, separation of duties | E-029, E-032, E-034, E-038, E-039 | Strong, verified |
| Defects found by independent review | E-031, E-035 | Strong |
| Years in program/project management | none | **Gap** (not a hard stop only if text accepts project proof) |
| Stakeholder reporting | E-049 (VMware status reporting, stated) | Medium |

Verdict: **CONSIDER as positioning, not a search lane yet**. Needs a live posting to score above 3.5.

## 4. AI evaluation / agent QA analyst (score 3.43, type with live pages)
**Checked live (employer-hosted pages opened 2026-10-27, no posting date, status not confirmable):**
- [Technical AI Evaluation Analyst (LATAM), Gramian Consulting Group](https://jobs.workable.com/jobs/4c24dc9f-87a8-44fa-80d4-ac15c9e2522e.md). Remote, Latin America, hourly contractor, 40 hours per week, "8 hours of mandatory PST overlap", 10 weeks, start immediately. Years: not stated. Pay: not shown.
- [AI Quality Assurance & Evaluation Specialist, Gramian Consulting Group](https://jobs.workable.com/jobs/70e157e2-93b6-4212-be45-8bfd42975da1.md). "Remote — Latin America (LATAM)", hourly contractor, 40 hours per week, no overlap stated. Years: not stated. Pay: not shown. Duration: not stated.
Both pages show an apply link but no date or "closed" notice; the page header and body name the company inconsistently ("Gramian Consulting Group" vs "Gramian Consultancy"): treat as a staffing intermediary and verify the end client before any application.
Scores (Technical AI Evaluation Analyst): archetype 5, evidence 4, location/terms 3, legitimacy 2.5, growth 4, minus 0.5 (pay hidden with 40 h/week) = **3.43**. Legitimacy tier: **Caution**.

| Requirement (posting, importance rated first) | Evidence | Strength |
| --- | --- | --- |
| Read Python, SQL, shell scripts, structured data, execution logs (critical) | E-011/E-012 (index: unverified, lake: stated), E-044; shell E-019 unverified | Medium |
| Verify calculations, reconcile conflicting evidence (critical) | E-005 (literal-evidence document AI), E-036 (re-tested a stale claim), E-031 | Strong |
| Assess correctness and completeness of technical deliverables (critical) | E-003, E-035 (cross-vendor and second-vendor audits) | Strong |
| Strong written English, reproducible feedback (high) | E-040 (B2, stated); feedback habit: E-032 review relay | Medium (B2 is a risk, posting says "strong written English") |
| Review AI agent traces, tool calls, deliverables (high, from search snippet of the same posting) | E-001, E-029 (agent workflow he directed) | Strong, but he directed, not wrote |
| 8 hours PST overlap (terms) | none needed; Costa Rica is Central time, overlap is workable (inferred, Costa Rica has no DST: check) | Terms |

Gaps: pay unknown (cannot test the 1.6M floor), 10-week contract is not a permanent job, no eval-framework tool named. Top CV lines, evidence IDs only: E-031 and E-035 (review found defects, audit fixed in a day), E-029 (merge gate), E-005 plus E-036 (evidence discipline). Verdict: **CONSIDER**. Cheapest tailored draft; ask for the rate in the first message. Contract work like this also builds the "AI evals / agent QA" line the 2026-10-12 scan rated Medium-High.

## 5. Snowflake-partner associate consultant (score 3.25, type)
Status: **reported only**; nothing open found. Hakkoda (Snowflake partner, Costa Rica delivery center) Associate Consultant, Data Engineering, Heredia postings were marked removed in 2025 (reported). The posting text then asked for "at least two years of practical project work and/or relevant education" (reported), which is the kind of phrase that lets education plus project proof count. Hakkoda's own careers page, opened today, lists no roles and links to an IBM careers search filtered to Hakkoda (checked live); I did not open that search. Snowflake's own Costa Rica opening seen in search is a Senior Cloud Support Engineer in Santa Ana (reported, senior).
Scores: archetype 3, evidence 4, location/terms 3.5, legitimacy 2 (cap), growth 3.5.

| Requirement (typical) | Evidence | Strength |
| --- | --- | --- |
| Snowflake, SQL, notebooks | E-010, E-011, E-018, E-044 (index: unverified, lake: stated for E-010/E-018) | Medium |
| Python scripting | E-012 | Medium |
| Cloud basics (AWS/Azure/GCP) | E-047 (AWS exposure only) | Weak |
| Data engineering tools (Matillion, Fivetran, dbt) | none | **Gap** |
| Degree in progress | E-045 (LEAD, in progress) | Medium |
| Client requirements work | E-048 | Medium |

Verdict: **CONSIDER when a live posting exists**; set an alert on IBM/Hakkoda and Snowflake partner firms. Gap closer: one dbt or Snowflake-trial project in the portfolio.

## 6. SaaS implementation / business consultant, Varicent-type (score 3.15, type)
**Checked live (employer board, 2026-10-27):** [Varicent's Greenhouse board](https://job-boards.greenhouse.io/varicent) lists 22 openings; **no Costa Rica role**, and no business-consultant or implementation role at all. The three Varicent postings that search returned (business consultant, technical consultant, technical account manager; Greenhouse IDs 4680842008, 5198581008, 5030346008) now show only the board index (closed or redirected: SKIP under gate 1). The only LATAM role is [Cloud Operations Engineer, Mexico, remote](https://job-boards.greenhouse.io/varicent/jobs/5464150008), "2 to 4 years of professional experience in a DevOps role", pay "the estimated annual base salary range is between $450,900.00 - $591,700.00 MXN." Costa Rica is not mentioned: **SKIP** (years hard stop, DevOps depth, Mexico).
Scores for the type: archetype 3, evidence 4.5, location/terms 3, legitimacy 2 (cap), growth 2.5.

| Requirement (typical) | Evidence | Strength |
| --- | --- | --- |
| Gather client requirements, demo to confirm | E-048 (stated), E-024 BRD (index: unverified) | Strong, stated |
| SQL and ETL/ELT workflows | E-048, E-011 | Medium |
| Weekly client and internal meetings | E-048 | Medium |
| Implementation tool expertise (Varicent Designer) | E-022 (index: unverified, lake: stated) | Medium, product name unknown |
| Consulting seniority | none; lake says never claim it | **Gap** |

Verdict: **CONSIDER only when a Costa Rica posting is live**. Carlos has references at Varicent (names stay with him); a referral to a future opening is his call, not an agent action.

## 7. Partner / revenue / business operations analyst (score 3.00, type)
Status: **reported + inferred**. The one posting that surfaced, [Senior Business Operations Specialist, The Entrepreneur Cooperative](https://www.jobtarget.com/jobs/jt-q8h8n0w49o/senior-business-operations-specialist), returned HTTP 404 on its JobTarget URL (gate 1 fails). Reported by search: "$2,000 to $3,000 USD per month", full-time, remote LATAM, "near-native English (C2)" and US Eastern hours. **C2 fails the English gate (E-040 B2) and "Senior" implies years: SKIP.** Varicent's Payroll & Benefits Specialist is Toronto only (checked live): SKIP.
Scores for the type: archetype 3, evidence 4.5, location/terms 2.5, legitimacy 2 (cap), growth 2.

| Requirement (typical) | Evidence | Strength |
| --- | --- | --- |
| Run a recurring monthly data and approval cycle | E-010 (Snowflake funds process, stated) | Strong, stated |
| Pull SQL and Workday data, reconcile, enter in system | E-010, E-011, E-016 (Workday, index: unverified) | Medium |
| Contracts, licensing, partner meetings | E-049 (VMware partner licensing, stated), E-010 | Medium |
| Excel and reporting | E-049, E-042 (Tableau) | Medium |

Verdict: **CONSIDER, borderline**: strong on evidence, weak on live roles and AI archetype. Best used as the "ops with agents" angle in rank 1.

## 8. Salesforce / business systems analyst, junior (score 2.80, type)
Status: **reported**. Cisco's Salesforce Business Systems Analyst link redirected to the Cisco careers home (gate 1: SKIP). CodeRoad's [Lead Salesforce Admin](https://job-boards.greenhouse.io/coderoad/jobs/4459152009) is open (checked live): LATAM only, contractor, 9 months, "Senior or Lead Salesforce Administrator", 1,000+ asset report migration, "Fluent/Advanced English", pay "Competitive Pay (USD)": **SKIP** (lead level vs E-043 admin-level support, stated). A "Junior Level Business Analyst" Salesforce remote contract (1+ yr, location not Costa Rica specific) appeared on an aggregator only (reported).
Scores: archetype 2.5, evidence 4, location/terms 3, legitimacy 2, growth 2.

| Requirement | Evidence | Strength |
| --- | --- | --- |
| Salesforce user roles, access, formulas, objects | E-043 (stated, 3 jobs) | Medium (not current; flows need refresher per lake) |
| Data Loader | E-043 (VMware, Amadeus) | Medium |
| Requirements and user stories | E-048, E-049 | Medium |

Verdict: **SKIP today**; reconsider if a junior CR posting appears.

## 9. AI trainer / expert contractor (score 2.65, type)
Status: **reported only**. Aggregators (OpenTrain, aitrainer.work, remowork.life) show Costa Rica-filtered AI evaluation gigs with spreads from "$20 to $40 per hour" up to "$60 to $100 per hour" and one "AI Expert - Operations" contract "$80/hour". Not opened on the employer or platform side; eligibility per role not verified; rates depend on an assessment (reported). Not a career target, but fast side income and AI-eval practice.
Scores: archetype 3, evidence 2.5, location/terms 3.5, legitimacy 2, growth 2.
Gaps: domain-expert requirements, no assessment result. Evidence to cite if he tries: E-031, E-035 (review judgment). Verdict: **SKIP as target; optional side income** after Carlos reads each platform's terms.

## 10. Data / BI analyst, Costa Rica hybrid (score 2.60, type)
Status: **reported + partly checked**. Johnson Controls BI Analyst (San José) URL: 404 (SKIP). CRG "Analista de Datos" (Teamtailor, hybrid) asks "3+ años de experiencia" in data analysis (reported snippet; hard stop). Golabs and Experian roles are Senior (reported). Aggregator Heredia data-analyst roles asked 3 to 4+ years (reported).
Scores: archetype 2, evidence 3.5, location/terms 3.5, legitimacy 2, growth 2.

| Requirement (typical) | Evidence | Strength |
| --- | --- | --- |
| SQL, Excel | E-011, E-044, E-049 | Medium |
| Tableau / Power BI | E-042 (Tableau stated); Power BI E-014 (index: unverified, lake: stated for VMware) | Medium |
| Python or R | E-012; R only from Amadeus (lake, stated) | Medium |
| 3+ yrs data analysis | Amadeus Data Analyst about 1 yr plus others, but total unclear | **Gap / hard stop** |

Verdict: **SKIP today**; LEAD University progress (E-045) helps in 1 to 2 years.

---

## Checked and skipped (live pages, for the record)
| Posting | What I saw | Why skipped |
| --- | --- | --- |
| [CodeRoad Senior AI Product Owner](https://job-boards.greenhouse.io/coderoad/jobs/4438474009) | Open form, LATAM only, "4+ years of product ownership experience", "C1+ English fluency", pay "Competitive Pay (USD)" | Gate 2 (English C1+ vs B2) and hard stop (4+ yrs). **Reverses the 2026-10-12 "best target" call.** |
| [CodeRoad Agentic AI Engineer (mid)](https://job-boards.greenhouse.io/coderoad/jobs/4406476009) | Open form, "3+ years" software dev with LLM/RAG/agentic apps; project-proof equivalent not mentioned; pay "Competitive Pay (USD)" | Years hard stop, cap 2.5 |
| [CodeRoad Data Scientist](https://job-boards.greenhouse.io/coderoad/jobs/4458093009) | Open form, "1-3 years" data science/ML, pandas, scikit-learn, Azure ML; pay "Competitive Pay (USD)" | No ML evidence in the lake; years stop |
| [CodeRoad Lead Salesforce Admin](https://job-boards.greenhouse.io/coderoad/jobs/4459152009) | See rank 8 | Lead level |
| Varicent Cloud Operations Engineer (Mexico) | See rank 6 | Years, DevOps, Mexico |
| Nexxa.ai QA Engineer (AI Systems) | Aggregator copy dated 27 August 2026, "5+ years"; employer Ashby link returned 404 | Closed and years |
| NTT DATA Business Support Analyst, Heredia | "Sorry, this position has been filled." | Closed |
| Simeio Junior IT Support & Business Systems Analyst, Heredia | Simeio's careers page and job board list no Costa Rica roles | Not on employer page |
| Customer Times SF Business Analyst/Consultant, Modsquad, Johnson Controls, Cisco | 404 or redirect | Gate 1 |
| HireLATAM AI Implementation Specialist | Search result said closed | Closed |
CodeRoad's board (29 roles, checked live) is the only employer board I found with many LATAM-only AI/data roles; none of its AI roles fits Carlos today (all are 3+ yrs, senior or lead).

## Surprises and conflicts
1. The 2026-10-12 scan called the CodeRoad Senior AI Product Owner "best match by content" with the blocker as years only. Reading the page today adds a second hard blocker: "C1+ English fluency" against E-040 B2.
2. Varicent, Carlos's former employer, has no Costa Rica openings today, and the earlier Costa Rica consultant postings are gone.
3. Rubric gate 1 is strict, so most search leads died at "page not found". Aggregator dates were unreliable (relative "x weeks ago" or hidden companies).
4. WebFetch summarises pages with a small model: any "no instructions to AI found" claim is that summary's statement, so a hostile line could be missed. I treated everything as data.

## Do next (ranked)
1. **Carlos decides** whether to try the two Gramian contract roles (rank 4) and ask the pay in the first message; Claude writes a one-page draft from E-029, E-031, E-035, E-005, E-036. He sends it.
2. **Build the one public fictional-data sample** (agent workflow with evals plus an n8n or Make automation): closes the gap in ranks 1, 2 and 5. Adds a sample-link line to the CV (E-ID needed once it exists).
3. **Claudio** reconciles the evidence index with the lake (E-009..E-025 rows) and adds E-IDs for Alexandria and VMware remote work, so tables above can cite them.
4. **Alerts, not applications:** Varicent Greenhouse board, IBM/Hakkoda careers, CodeRoad board. Re-run T-009 in 2 weeks.
5. **Open question for Carlos:** is a 10-week LATAM-only hourly contract acceptable while seeking the full-time role, and what hourly rate equals the 1.6M colones/month floor for him?

## For Claudio
- Update index rows for E-009 to E-025 against the lake notes; add a decision on whether C1+ English roles are permanently out until a test result exists.
- Add T-011 (re-run, 2 weeks) and a task for the portfolio sample.

Claude · Market Scout, 2026-10-27
