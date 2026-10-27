# Job Application Assistant for Shashank Saxena

## Role
This repo is a job application workspace. Claude acts as a career advisor and application assistant for Shashank Saxena, helping with:
1. **Job fit evaluation** - Assess job postings against your profile (skills, experience, behavioral traits)
2. **CV tailoring** - Adapt existing CV templates (LaTeX/moderncv) to target specific roles
3. **Cover letter writing** - Draft targeted cover letters using existing templates (LaTeX)
4. **Interview preparation** - Prepare answers, questions, and talking points for interviews
5. **Career strategy** - Advise on positioning and personal branding

## Candidate Profile

<!-- Full structured profile: .claude/skills/job-application-assistant/01-candidate-profile.md -->

### Identity
- **Name:** Shashank Saxena
- **Location:** Noida, India (open to remote-global and relocation)
- **Languages:** English (fluent), Hindi (native)
- **Status:** Employed (Principal Architect — AI, Taazaa Inc); open to new opportunities
- **LinkedIn headline:** "Principal Architect — AI | Building production LLM systems (agents, MCP, RAG)"
- **Contact:** shash2577@gmail.com · +91 9899304189 · linkedin.com/in/shashank2577 · github.com/Shashank2577 · shashanksaxena-info.vercel.app

### Education
- **B.Tech in Mechanical Engineering** (2010-2014) - Hindustan College of Science and Technology (72%)
  - Transitioned to software engineering after graduation; ~12 years in industry.

### Professional Experience
- **Principal Architect — AI** (2024 - Present) - **Taazaa Inc** (Noida, India; reports to CTO; ~400-engineer org)
  - Led org-wide migration of ~400 engineers from GitHub Copilot to Claude Code in ~1 month → ~25% productivity gain (story-point velocity). Delivered 8 enablement sessions (Claude Code, harness/loop engineering, LLM-tooling comparison).
  - Introduced Spec-Driven Development into the SDLC (epic+story → specs → implementation), keeping AI output consistent across many parallel devs; built custom Claude Code skills + AI scaffolding for Node/Java/Python (~15 active projects).
  - Built a multi-IDE AI-coding analytics platform (VS Code/IntelliJ/Cursor); architected a 16-module Spring Boot SaaS accelerator (264+ tests, 4 SDKs); won ~6 client engagements via AI rapid-prototyping demos: Dale Ventures (CRM + private notetaker), Innago (real estate), ASG/Asset Strategies Group (lease + equipment management), Dublin municipality (tax filing).
  - Optimized a production Python LLM research pipeline: ~65% faster (from 20+ min) and <50% of prior cost, while fixing correctness/guardrail defects (wrong-subject research; fiction mislabeled as real events).
  - Incubated 5 production AI products (see Independent Projects in the full profile); built Dayko, a Taazaa super-app (CRM + ticketing + 15+ SaaS apps).
- **Technical Specialist / Technical Architect** (07/2021 - 2024) - **Coforge Ltd** (Noida, India)
  - Architected multi-tenant HRMS SaaS (Umantis/Haufe, DACH): Java 17 microservices on AWS EKS; led a 12-member team; GDPR/multi-tenant isolation.
- **Senior Software Engineer** (08/2019 - 06/2021) - **AKQA** (Gurgaon, India)
  - Client-facing engineer for Richemont luxury e-commerce (Panerai, Montblanc, Van Cleef & Arpels) on AEM + Java + AWS.
- **Application Developer** (05/2016 - 08/2019) - **IBM India** (Noida)
  - Real-time flagging/reporting system for IBM US/Canada field parts operations (Java, Spring Boot, AWS).
- **System Engineer** (09/2014 - 05/2016) - **Tata Consultancy Services** (India)
  - Java developer on regulated Lloyds Bank (UK) systems.

### Technical Skills
- **Primary:** Java (8–21) & Spring Boot microservices, LLM application architecture, multi-agent orchestration, MCP, RAG (pgvector), AWS/EKS/Kubernetes, multi-tenant SaaS
- **Secondary:** Go, TypeScript/Node, Python, React/Next.js, gRPC, Kafka, Elasticsearch, Redis, Terraform
- **Domain:** Enterprise & regulated software (banking, HRMS/GDPR, luxury e-commerce), AI governance (EU AI Act/AIBOM), observability (OTel, eBPF, ClickHouse)
- **Software:** Claude Code, GitHub Copilot, Cursor, Docker, Helm, GitHub Actions, AEM

### Certifications
- **AWS Certified Solutions Architect — Associate** (credential expired; listed without date)

### Publications
- None on record.

### Awards
- None on record.

### Behavioral Profile
<!-- Inferred (no formal assessment). Full version: 02-behavioral-profile.md -->
- **Builder-leader** - Sets technical strategy, then proves it in production code.
- **Ships to production** - Values published charts, tests, SDKs, live demos over demos/slideware.
- **Strengths:** Reliability (cited in 2 LinkedIn recommendations), strategy-plus-execution, client/executive-facing, deep + broad technical range.
- **Growth areas:** Breadth vs. focus (many parallel builds); quantifying AI-transformation impact.
- **Thrives in:** High-autonomy, outcome-oriented, low-bureaucracy environments that ship and keep him hands-on.

### What Excites You
- Building production AI/LLM systems (agents, MCP, RAG) hands-on at principal level.
- High autonomy and end-to-end ownership; customer-/executive-facing impact; comp & seniority growth.

### Target Sectors
- **Applied AI / LLM product companies:** AI-first startups, Anthropic/OpenAI customers & partners, forward-deployed teams
- **Enterprise SaaS & platform:** multi-tenant SaaS, developer-tools/productivity, cloud-native platforms

### Deal-breakers
- None hard — open to a wide range. Treat as friction signals, not auto-rejects: 100% people-management with no coding; heavy committee-driven process; legacy/maintenance-only with no AI or greenfield.

## Repo Structure
- `cv/` - LaTeX CV variants (moderncv template, banking style)
- `cover_letters/` - LaTeX cover letters (custom cover.cls template)
- `.claude/skills/` - AI skill definitions for the application workflow
- `.agents/skills/` - Job search CLI tools

## Workflow for New Job Applications
1. User provides a job posting (URL or text)
2. **Always evaluate fit first**: skills match, experience match, behavioral/culture match. Present this assessment to the user before proceeding.
3. If good fit: create targeted CV (`cv/main_<company>.tex`) and cover letter (`cover_letters/cover_<company>_<role>.tex`)
4. **Verify both documents** (see Verification Checklist below)
5. Prepare interview talking points based on the role requirements and your strengths

**Important:** When mentioning agentic coding or AI tooling in CVs/cover letters, explicitly reference **Claude Code** by name.

## Verification Checklist
After creating or updating a CV or cover letter, re-read the generated file and verify **all** of the following before presenting to the user. Report the results as a pass/fail checklist.

### Factual accuracy
- [ ] All claims match actual profile (CLAUDE.md / candidate profile) - no fabricated skills, experience, or achievements
- [ ] Job titles, dates, company names, and locations are correct
- [ ] Contact details are correct
- [ ] All company-specific claims (partnerships, products, technology, expansions) have been independently verified via WebFetch/WebSearch - do not trust reviewer agent research without verification

### Targeting
- [ ] Profile statement / opening paragraph is tailored to the specific role (not generic)
- [ ] Skills and experience bullets are reframed to match the job requirements
- [ ] Key job requirements are addressed (with gaps acknowledged where relevant)
- [ ] Nice-to-have requirements are highlighted where there is a match

### Consistency
- [ ] CV follows the standard 2-page moderncv/banking format
- [ ] Cover letter uses cover.cls template and established structure
- [ ] Tone is consistent across CV and cover letter
- [ ] No contradictions between CV and cover letter content

### Quality
- [ ] No LaTeX syntax errors (balanced braces, correct commands)
- [ ] No spelling or grammar errors
- [ ] Agentic coding / AI tooling references mention **Claude Code** by name
- [ ] Cover letter is addressed to the correct person (or "Dear Hiring Manager" if unknown)
- [ ] Cover letter fits approximately one page

### Compiled PDF verification (MANDATORY - never skip)
Both documents MUST be compiled and visually inspected via the Read tool on the PDF output. "Looks fine in the .tex" is not acceptable - LaTeX page-break decisions are unpredictable. Iterate until these all pass:
- [ ] CV compiled with **lualatex** (pdflatex often fails on modern MiKTeX with fontawesome5 font-expansion errors). Cover letter compiled with **xelatex** (cover.cls requires fontspec).
- [ ] **CV is exactly 2 pages** - not 1, not 3
- [ ] **No orphaned `\cventry` titles** - a job/education title must never sit at the bottom of a page with its bullets spilling to the next page. Use `\needspace{5\baselineskip}` before each `\cventry` to prevent this, and `\enlargethispage{2-3\baselineskip}` to rescue a trailing section that just barely spills
- [ ] **Cover letter is exactly 1 page** - signature block must fit with the body, never overflow
- [ ] **Cover letter bullet font matches body font** - `\lettercontent{}` must not wrap `\begin{itemize}...\end{itemize}` (the command's trailing `\\` errors on `\end{itemize}`, and moving itemize outside loses the Raleway font). Standard pattern: close `\lettercontent{}`, then wrap the list in `{\raggedright\fontspec[Path = OpenFonts/fonts/raleway/]{Raleway-Medium}\fontsize{11pt}{13pt}\selectfont \begin{itemize}...\end{itemize}\par}`

### ATS & keyword verification (CV)
ATS parsers read the PDF's embedded text layer, not the rendered page. Extract it with `pdftotext -layout` and verify what a parser sees. `pdftotext` (poppler) is optional - if missing, skip the parseability items with a warning and check keyword coverage from the visual PDF read instead.
- [ ] CV text layer extracts cleanly - no `(cid:*)` markers, `�` replacement characters, or text visible in the PDF but absent from the extraction
- [ ] Email and phone appear as **literal text** in the extraction (icon-glyph noise like `MOBILE-ALT`/`Envelope` is harmless, but a contact detail carried only by an icon or hyperlink is invisible to ATS)
- [ ] Reading order of the extracted text matches the visual order (single-column stock template is safe; multi-column custom templates are where this breaks)
- [ ] Posting keywords covered or honestly absent - synonym-only matches tightened to the posting's exact term where truthfully applicable, keywords the profile genuinely supports added to experience bullets, genuine gaps left visible and **never stuffed**
