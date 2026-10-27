# Job Evaluation Framework

<!-- SETUP: Skill match areas and career goals are personalized by running /setup -->

## Scoring Dimensions

Evaluate each job posting against these five dimensions:

### 1. Technical Skills Match (0-100)
How well do the required/preferred skills align with the candidate's capabilities?

| Score | Meaning |
|-------|---------|
| 80-100 | Core requirements are primary skills |
| 60-79 | Most requirements match, 1-2 gaps that are learnable |
| 40-59 | Partial match, significant upskilling needed |
| 0-39 | Fundamental mismatch |

**Strong match areas:** LLM application architecture, multi-agent orchestration, MCP servers, RAG (pgvector/embeddings), Java/Spring Boot microservices, AWS + Kubernetes/EKS, multi-tenant SaaS architecture, agentic SDLC (Claude Code/Copilot/Cursor), Go & TypeScript/Node, observability (OTel/eBPF)
**Moderate match areas:** Python (production-capable, not primary), evals/AI-observability tooling, front-end (React/Next.js), AI governance/compliance (EU AI Act/AIBOM), team leadership (led 12)
**Weak match areas:** Formal ML/data-science (training models, MLOps pipelines, deep-learning research), mobile development, non-JVM/Go backend ecosystems (e.g. .NET, Rails), formal people-management at scale (director/VP org design)

### 2. Experience Match (0-100)
Does work history align with what they're looking for?

| Score | Meaning |
|-------|---------|
| 80-100 | Direct experience in the same domain and role type |
| 60-79 | Related experience, transferable skills clear |
| 40-59 | Adjacent experience, would need to make the case |
| 0-39 | Unrelated experience |

**Strong:** Principal/architect-level enterprise software delivery (~12 yrs), production AI/LLM product-building, multi-tenant SaaS, client-facing/forward-deployed work, regulated domains (banking, HRMS/GDPR, luxury e-commerce), leading engineering teams
**Moderate:** Org-wide AI transformation leadership (current, ~2+ yrs), developer-productivity/analytics products, AI governance
**Entry-level:** Formal data-science/ML-research roles, pure engineering-management/director tracks, dedicated DevRel

### 3. Behavioral/Culture Fit (0-100)
Does the role and company culture match the behavioral profile?

| Score | Meaning |
|-------|---------|
| 80-100 | Culture strongly matches behavioral preferences |
| 60-79 | Mixed signals but mostly compatible |
| 40-59 | Some friction areas |
| 0-39 | Significant culture mismatch |

**Red flags to research:** Department disorganization, work dominated by maintenance over development, poor chemistry with leadership, culture mismatches. Check reviews, media coverage, LinkedIn connections, and network contacts for insider perspective.

### 4. Location & Logistics (Pass/Fail + Notes)
Shashank is location-flexible: remote-first (global) AND open to relocation. Relocation is NOT a deal-breaker.
- Remote (any timezone, or overlapping IST): PASS
- India-based (Noida/NCR/Bangalore), on-site or hybrid: PASS
- Relocation to UAE/Gulf, EU, UK, Norway, Sweden, Canada, USA: PASS
- Relocation elsewhere with sponsorship: PASS (flag for confirmation)
- On-site-only role with NO remote/relocation support in a location he can't reach: FAIL
- Visa/sponsorship note: most overseas relocations require employment visa sponsorship; UAE is Golden-Visa eligible via the AI-specialist route. FLAG postings that explicitly exclude sponsorship.

### 5. Career Alignment & Motivation (0-100)
Does this role advance career goals and contain tasks that energize?

| Score | Meaning |
|-------|---------|
| 80-100 | Strongly aligned with career direction, clear growth path |
| 60-79 | Good role but only partially aligned with long-term goals |
| 40-59 | Decent job but doesn't build toward career goals |
| 0-39 | Dead end or backwards step |

**Career goals:**
- Stay hands-on building production AI/LLM systems (agents, MCP, RAG) at a senior/principal level — not drift into pure management.
- Principal/Staff/Architect scope with real ownership and autonomy over technical direction.
- Roles that combine deep engineering with customer- or executive-facing impact (forward-deployed / applied AI / AI transformation).
- Compensation and seniority growth; access to frontier AI work.

**Motivation filter:** Evaluate not just whether he *can* do the tasks, but whether the tasks will *energize* him. Consider:
- Tasks that energize: shipping production AI features, architecting greenfield systems, owning a roadmap end-to-end, working directly with customers/executives, high-autonomy build work
- Tasks that drain: 100% people-management with no coding, heavy committee-driven process, legacy maintenance with no AI/greenfield
- Non-task factors: leadership style, degree of autonomy, whether the org actually ships, comp/seniority

**Life situation alignment:**
- **Security**: Currently employed (Principal Architect, Taazaa); can be selective — optimize for fit and upside, not just any move.
- **Flexibility**: Location-flexible (remote or relocation). Visa sponsorship needed for most overseas moves.
- **Professional development**: Prioritize frontier AI exposure, principal-level scope, and orgs with strong engineering cultures.

**Deal-breakers:** None hard — Shashank is open to a wide range. Treat the "friction" items above as scoring signals, not automatic rejections.

### 6. Salary Benchmark (Optional)

If the salary lookup tool is configured (`salary_data.json` exists), look up the company:
```
python salary_lookup.py "<Company Name>" --json
```

If a city is known from the posting, add `--city "<City>"` to narrow results.

Present findings as:
```
### Salary Benchmark
| Metric | Value |
|--------|-------|
| [Category] index | XX.X (+/-X.X% vs baseline) |
| Overall index | XX.X (+/-X.X% vs baseline) |
```

Interpret results relative to the baseline defined in the data file's metadata. For index-based data, higher typically means above-market compensation.

If the salary tool is not configured, skip this section.

## Output Format

Present the evaluation as:

```
## Job Fit Evaluation: [Role] at [Company]

| Dimension | Score | Notes |
|-----------|-------|-------|
| Technical Skills | XX/100 | [brief note] |
| Experience Match | XX/100 | [brief note] |
| Behavioral Fit | XX/100 | [brief note] |
| Location | PASS/FAIL | [brief note] |
| Career Alignment | XX/100 | [brief note] |

**Overall Score: XX/100** (weighted average of scored dimensions)

### Verdict: [Strong Fit / Good Fit / Moderate Fit / Weak Fit / Poor Fit]

### Key Strengths for This Role
- [bullet points]

### Gaps to Address
- [bullet points]

### Recommendation
[1-2 sentences: apply/skip/apply with caveats]

### Company Research Checklist
- [ ] Checked company website (mission, values, recent news)
- [ ] Checked review sites (Glassdoor, Jobindex, etc.)
- [ ] Checked LinkedIn for team size, recent hires, connections
- [ ] Checked media for restructuring, growth, or workplace issues
- [ ] Identified network contacts who may know the team/manager
```

## Weighting
- Technical Skills: 30%
- Experience Match: 25%
- Behavioral Fit: 15%
- Career Alignment: 30%

(Location is pass/fail, not weighted)

## Thresholds
- **Strong Fit** (75+): Definitely apply, tailor everything
- **Good Fit** (60-74): Apply, address gaps in cover letter
- **Moderate Fit** (45-59): Consider carefully, discuss with user
- **Weak Fit** (30-44): Probably skip unless strategic reasons
- **Poor Fit** (<30): Skip

## Pre-Application: Call the Employer (Best Practice)

Before writing the application, consider whether the candidate should call the contact person listed in the posting. **Only call if there are substantive questions** - never call just to "be remembered."

### When to Suggest Calling
- The posting has unclear or ambiguous requirements
- It's unclear which competencies are essential vs. nice-to-have
- The role description is vague about day-to-day tasks
- There's a named contact person who invites questions

### Good Questions to Ask
- "What are the primary challenges in this role?"
- "How is time typically divided across the listed responsibilities?"
- "Which competencies are most critical for success in this position?"
- "What does success look like in the first 6-12 months?"

### Rules for the Call
- Prepare a 30-second "elevator pitch" about your background in case they ask
- The call's purpose is **gathering information**, not delivering a pitch
- Take notes - use what you learn to tailor the application
- Reference the conversation naturally in the cover letter ("After speaking with [name], I was especially drawn to...")
