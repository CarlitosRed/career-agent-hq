# Market scan: agentic-engineering roles (T-002)
Claude · Market Scout, 2026-10-12. Checked = I opened the employer's own page. Reported = a search snippet or article, not verified.

## 1. Title variants (reported, from postings and guides; no reliable frequency count exists)
| Title | Fit for Carlos | Why |
| --- | --- | --- |
| Agentic AI Engineer / AI Agent Engineer | Medium (stretch) | Most common label; asks for Python + LangGraph/CrewAI + production experience |
| Forward Deployed Engineer (AI) | High | Customer-facing, process discovery + build; matches BRD/process background |
| AI Solutions / Solutions Engineer (agents) | High | Same, less coding depth |
| AI Automation / Agentic Orchestration Engineer | High | Workflow + gates + agent roles = PO Reader pattern |
| AI Operations / AI Process Specialist | High | Revenue/comp ops + agents; closest to the Varicent/Snowflake past |
| MCP / AI Integration Engineer | Medium | Needs API/backend depth |
| AI Evals / Agent QA Engineer | Medium-High | Cross-vendor review, exact-head audits, class sweeps are eval-like work |
| Technical Program / Delivery role for AI teams | Medium | Orchestration of people + agents |

## 2. Keywords that recur (reported: Capgemini, CodeRoad pages, guides)
Python, multi-agent systems, tool calling, MCP, RAG, LangGraph, CrewAI, Agent SDKs, observability (LangSmith, tracing), evals/reliability testing, prompt-injection and least-privilege at the tool boundary, async APIs, cloud (AWS/Azure/GCP), explaining AI to non-technical stakeholders.
Our proof points map to: multi-agent roles and worktrees, approval gates and tiers, evals-like review rounds, fictional-data safety, document-AI with literal evidence. Gaps to close with evidence or small projects: a named framework (LangGraph or Agent SDK), MCP server, vector DB, public code sample.

## 3. Checked postings (employer pages opened 2026-10-12)
| Role | Where | Eligibility | Status |
| --- | --- | --- | --- |
| [Senior Agentic AI Engineer, CodeRoad](https://job-boards.greenhouse.io/coderoad/jobs/4110608009) | Greenhouse | 100% remote, LATAM only, USD pay | Open, no posting date shown. Needs 5+ yrs software dev, 2-3 yrs production AI. Likely too senior as written |
| Agentic AI Engineer (x2, non-senior), CodeRoad | [board](https://job-boards.greenhouse.io/coderoad) | LATAM | Listed on the board; descriptions not read yet. Best first target |
| Senior AI Product Owner (New), CodeRoad | [board](https://job-boards.greenhouse.io/coderoad) | LATAM | Listed; description not read. Possible fit (product + process) |
| Yuno "AI Agent Infrastructure" | [Lever](https://jobs.lever.co/yuno) | - | Search snippet was stale: not on the board now. Only AI roles there are Europe-based. Drop |

## 4. Reported only (not verified, do not treat as open)
Costa Rica/LATAM aggregator listings (Jobgether, Himalayas, Wellfound, Remote Rocketship) show AI engineer roles open to Costa Rica but with relative dates (9 to 12 weeks old) or hidden companies. Several US-only forward-deployed and orchestration roles (Coder, Nearform, CookUnity, Aisera) are not open to Costa Rica. Salary claims of $155K-$265K come from a staffing firm and are not usable; the one verified-style range is LATAM AI Engineer $87K-$150K on an aggregator (reported).

## 5. Recommendation
1. Target titles in this order: Forward Deployed / AI Solutions, AI Automation-Orchestration, AI Ops, then Agentic AI Engineer (non-senior).
2. Lead the CV with workflow/orchestration, review gates and document-AI results, not "ML".
3. Build one public, fictional-data sample (a small agent workflow with evals) to cover the Python/framework gap.
4. First applications to verify and read in full: CodeRoad Agentic AI Engineer (non-senior) and Senior AI Product Owner.

## For Claudio
- Add T-007: read full descriptions of the CodeRoad non-senior roles. Add question: how many years of hands-on software dev can Carlos honestly claim (decides senior vs mid)?

## 6. T-007 result: CodeRoad descriptions read in full (employer pages, 2026-10-12)
All three: 100% remote, LATAM-only, USD pay (amount not stated), advanced English mandatory, asks about US-client experience. CodeRoad is a nearshore staffing/services firm. No posting dates shown.

| Role | Link | Asks for | Carlos fit (from Codex audit) |
| --- | --- | --- | --- |
| Agentic AI Engineer (mid) | [4406476009](https://job-boards.greenhouse.io/coderoad/jobs/4406476009) | 3+ yrs software dev, advanced Python, LangGraph/CrewAI/ADK, MCP, vector DB, AWS Bedrock, LangSmith-type evals | Gap: no evidence yet of framework, vector DB, Bedrock, or years of dev |
| Agentic AI Engineer (mid-senior) | [4414020009](https://job-boards.greenhouse.io/coderoad/jobs/4414020009) | 5+ yrs Python, 2+ yrs LangGraph/LangChain agents, LangFuse, PromptFoo, M365 Agents SDK | Too far today |
| Senior AI Product Owner | [4438474009](https://job-boards.greenhouse.io/coderoad/jobs/4438474009) | 4+ yrs PO/PM with shipped LLM apps (agents, RAG, document extraction), golden datasets, release sign-off, client workshops, Jira | Best match by content (doc extraction, evidence, review gates, sign-off); blocker is "4+ yrs PO/PM" which we cannot evidence yet |

Recommendation: the Product Owner role is the best real target of the three; the mid Agentic AI Engineer is the stretch. Do not apply until Carlos confirms years and roles (queue questions 1 to 5). Frame the PO Reader as: owner of evaluation-and-sign-off process for a document-AI system, with measured accuracy marked "not measured".
