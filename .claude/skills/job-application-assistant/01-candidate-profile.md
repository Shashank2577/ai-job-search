# Candidate Profile

## Identity
- **Name:** Shashank Saxena
- **Location:** Noida, India
- **Phone:** +91 9899304189
- **Email:** shash2577@gmail.com
- **LinkedIn:** https://linkedin.com/in/shashank2577
- **GitHub:** https://github.com/Shashank2577
- **Portfolio:** https://shashanksaxena-info.vercel.app (product demo: https://observe.sovix.xyz)
- **Languages:** English (fluent), Hindi (native)
- **Status:** Employed (Principal Architect — AI, Taazaa Inc); open to new opportunities
- **Constraints:** Open to remote (global) and to relocation — UAE/Gulf (Golden Visa eligible via AI-specialist route), EU, UK, Norway, Sweden, Canada, USA, and India (Noida/NCR/Bangalore). Requires employment visa sponsorship for most overseas relocations.

## Education

| Degree | Period | Institution | Key Topics |
|--------|--------|-------------|------------|
| B.Tech, Mechanical Engineering (72%) | 2010–2014 | Hindustan College of Science and Technology | Mechanical Engineering (transitioned to software engineering after graduation) |

## Professional Experience

### Principal Architect — AI - Taazaa Inc (2024 - Present)
Noida, India — reporting to the CTO; ~400-engineer software-product organization
- **Led the org-wide migration of ~400 engineers from GitHub Copilot to Claude Code in ~1 month**, measuring a **~25% gain in delivery productivity** (tracked against team story-point velocity). Pioneered and owned the entire rollout end-to-end.
- Delivered **8 enablement sessions** across the organization on Claude Code, harness engineering, and loop engineering, plus a comparative evaluation of GitHub Copilot, OpenAI Codex, Cursor, and Claude Code — published as open-source interactive workshop field guides (see Independent Projects).
- **Introduced Spec-Driven Development (SDD) into the SDLC**, replacing ad-hoc "vibe-coded" AI output: built a pipeline that turns an epic + story into specs and acceptance criteria, then drives implementation from them — keeping output consistent even with many developers working with AI in parallel. Solved the core failure mode where AI-generated scaffolding was unrelated or ignored surrounding context.
- Built a **library of custom Claude Code skills and AI-aware scaffolding for Node.js, Java, and Python** (bundling the relevant tech-stack skills per app type); **~15 active projects currently run on it**.
- Built a multi-IDE AI-coding analytics platform (VS Code, IntelliJ/JetBrains, Cursor) giving leadership adoption, acceptance-rate, and impact data — the category LinearB/DX/Faros charge for, with IDE coverage they don't ship.
- Architected "cross-cutting", a Spring Boot auto-configuration accelerator: 16 production modules (multi-tenancy, RBAC, audit, pgvector search, LiteLLM AI gateway, payments) with 264+ tests and SDKs in React/Node/Python/Java, cutting SaaS engagement bootstrap from ~weeks to days.
- **Won new client business in ~6 engagements** by demonstrating AI-driven rapid prototyping — fast turnarounds that turned a scaffolding/problem demo into a signed engagement. **Named clients** include **Dale Ventures** (CRM + private notetaker), **Innago** (real estate), **Asset Strategies Group / ASG** (lease and equipment management), and a **Dublin municipality** tax-filing project.
- **Optimized a production LLM research pipeline (billionaire/individual research)** written in Python: cut runtime from 20+ minutes by **~65%** and delivered answers at **<50% of the prior cost**, while **fixing correctness/guardrail defects** — previously it researched the wrong individuals and mislabeled fiction (novels/stories a subject had written) as real-life events; those errors had surfaced in guardrails and outbound emails.
- Built/led work on **Dayko**, a Taazaa "super-app" bundling a CRM, ticketing, and 15+ SaaS apps, alongside a broader portfolio of Taazaa AI products.
- Advises CEO/CTO on AI product incubation; authored the portfolio strategy adopted by the engineering core and incubated 5 products to production grade (see Independent Projects).

### Technical Specialist / Technical Architect - Coforge Ltd (07/2021 - 2024)
Noida, India — Product: Umantis (Haufe Group), multi-tenant talent-management HRMS SaaS for the DACH market
- Architected and evolved a multi-tenant HRMS SaaS: Java 17 microservices on AWS EKS with gRPC, Eureka, circuit breakers, Kafka & ActiveMQ, Elasticsearch, MySQL/PostgreSQL (Flyway), Redis.
- Led a 12-member engineering team — solution design, code-review culture, POC evaluation, performance optimization, mentoring.
- Implemented security and GDPR-compliance practices for multi-tenant data isolation across DACH enterprise customers.
- Worked directly with product stakeholders and clients to translate business requirements into architecture.
- Ran hands-on "designing with AI" enablement sessions for engineering teams (a practice he later scaled org-wide at Taazaa).

### Senior Software Engineer - AKQA (08/2019 - 06/2021)
Gurgaon, India — Product: E-commerce for Richemont luxury brands (Panerai, Montblanc, Van Cleef & Arpels)
- Client-facing engineer for luxury e-commerce builds on AEM (OSGi/Sling/JCR) + Java 8 microservices + AWS; owned architecture decisions and presented directly to brand-side stakeholders under exacting luxury-retail standards.
- Delivered the Panerai global e-commerce platform (16-month program): personalization, payments, and inventory integrations.

### Application Developer - IBM India (05/2016 - 08/2019)
Noida, India — Product: IBM US/Canada Parts Administration (ERP for field engineers)
- Built the real-time flagging and reporting system used daily by IBM field engineers across US/Canada parts operations — turnaround-time calculation and cost-loss tracking (Java, Spring Boot, Spring MVC, Hibernate, AWS, MySQL, REST).

### System Engineer - Tata Consultancy Services (09/2014 - 05/2016)
India — Client: Lloyds Bank (UK)
- Java developer on regulated UK retail-banking systems — first exposure to compliance-grade delivery.

## Independent Projects
<!-- Production AI products built and shipped; live and on GitHub (github.com/Shashank2577, 40 public repos) -->
- **OBSERVE** (observe.sovix.xyz): Self-hosted, AI-first Kubernetes observability platform. One Helm install bundles metrics/logs/traces/eBPF (Beyla, Tetragon; VictoriaMetrics, ClickHouse, OTel) with an 11-agent AI root-cause-analysis swarm and a built-in MCP server. Helm chart published to GHCR (multi-arch amd64/arm64), one-command installers for EKS/GKE/AKS. *~20 developers using OBSERVE/Prompture.*
- **Prompture** (prompture.sovix.xyz): AI prompt capture & governance platform (AIBOM for the EU AI Act). Go platform (~1,200+ source files, ~32% test ratio) capturing prompts across CLI/IDE/web and matching them to git commits via a six-signal engine; OPA policies, KMS, SSO/RBAC, Python + TypeScript SDKs, MCP server.
- **Spreix Notetaker** (spreix.cloud): Multi-tenant AI meeting-intelligence SaaS. Bots join Google Meet/Microsoft Teams/Zoom, transcribe and extract decisions/actions; 35+ context-aware agents, MCP server, multi-tenant Prisma schema, 18 Playwright E2E suites, Helm on AWS EKS. *A version is deployed internally at Taazaa with ~400 active users.*
- **cross-cutting** + **custom Claude Code skills / AI scaffolding**: Spring Boot starter bundling 16 production modules (multi-tenancy, RBAC, audit, search, AI gateway, payments); 264+ tests, 4 SDKs. Paired with AI-aware scaffolding for Node.js/Java/Python — *~15 active Taazaa projects run on it.*
- **ClosePilot**: Autonomous inbound-sales agent chain with human-in-the-loop gates. Scout→Prep→Scribe→Proposal→Chase agents over Gmail + CRM (HubSpot/Salesforce/Pipedrive); MCP server exposing 50+ tools; pgvector, BullMQ, OTel.
- **Copilot Analytics Platform**: Multi-IDE AI-coding telemetry (VS Code, JetBrains, Cursor) — adoption, acceptance rates, impact.
- **UI Generator**: Multi-library AI UI generator with an MCP server that exports React across 5 component libraries.

### Open Source (github.com/Shashank2577 — 40 public repos)
- **hesoyam-for-claude-code** (11★, 3 forks): One-install orchestration, config, memory, knowledge & ecosystem-discovery tooling for Claude Code — his most-starred project.
- **Claude Code / Copilot / Cursor workshop field guides** (`awesome-*-walkthrough`): interactive 2-hour workshop guides + presenter scripts + handouts — the published form of his enablement sessions and comparative LLM/tooling evaluation. Live:
  - Claude Code: https://shashank2577.github.io/awesome-claude-code-walkthrough/
  - Copilot: https://shashank2577.github.io/awesome-copilot-walkthrough/
  - Cursor: https://shashank2577.github.io/awesome-cursor-walkthrough/
  - Taazaa Copilot Playbook: https://taazaainc.github.io/TZ-Copilot-Playbook
- **brain**: a framework for building agent-native applications.
- **java-microservices-framework**: Java 21 + Spring Boot 3.4 + Postgres + Kafka microservices framework.
- **demopilot** / **OpenMontage**: open-source agentic video-production tooling. **marvin-template**: AI Chief-of-Staff template for Claude Code. **prompture-cli**: AI audit trail for engineering teams.

## Technical Skills

### Programming & AI/LLM
- **Java (8–21)** (expert): Spring Boot microservices, gRPC, Hibernate
- **Go** (proficient), **TypeScript/Node.js** (proficient), **Python** (proficient), **SQL**
- **AI/LLM engineering:** LLM application architecture, multi-agent orchestration (35+ agents in production), MCP (6 servers shipped), RAG (pgvector, embeddings, HNSW, hybrid retrieval), prompt engineering & governance (AIBOM, EU AI Act), evals & AI observability
- **AI platforms & SDKs:** Anthropic / OpenAI / Gemini APIs, LangGraph, Vercel AI SDK, LiteLLM
- **Agentic SDLC:** Claude Code, GitHub Copilot, Cursor, autonomous agents (Jules)

### Domain Expertise
- Enterprise & multi-tenant SaaS architecture
- Regulated domains (UK banking, DACH HRMS/GDPR, luxury e-commerce)
- Cloud & platform: AWS (EKS, Lambda, SQS/SNS, DynamoDB, Step Functions, S3, API Gateway, CloudWatch, X-Ray), Kubernetes & Helm, Docker, Terraform, GitHub Actions
- Observability: OTel, eBPF (Beyla, Tetragon), Prometheus, ClickHouse, VictoriaMetrics
- Data & messaging: PostgreSQL, MySQL, Elasticsearch, Redis, Kafka, ActiveMQ, BullMQ
- Security: OAuth/SSO, RBAC, OPA, KMS

### Software & Tools
- React, Next.js, Tailwind CSS, Framer Motion
- AEM (OSGi/Sling/JCR)
- Git, GitHub Actions

## Publications
<!-- None on record -->
- N/A

## Awards
<!-- None on record -->
- N/A

## References
- **Tibor Gémes** — LinkedIn recommendation praising reliability, sharp technical work, POC development, and team-leadership ability.
- **Lucas Cairella** — LinkedIn recommendation highlighting collaborative spirit, reliability, and positive team contributions.

More references available upon request.

## Interests
- Cricket, Chess, Photography (portfolio photographer; Sony A7IV/A7RIII, DJI Mavic 3)
