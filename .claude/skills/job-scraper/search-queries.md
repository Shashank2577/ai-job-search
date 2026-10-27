# Search Queries for Job Scraper

<!-- Personalized for Shashank Saxena via /setup. Update with `/setup --section search`. -->

> **Note on portals:** This framework ships CLI tools for Danish job boards (Jobindex, Jobbank,
> Jobdanmark, Jobnet). Shashank is based in India and targeting global-remote + relocation, so
> those CLIs don't apply. These queries lean on LinkedIn, Google `site:` searches, and
> remote-first boards instead. You can scaffold a new portal with `/add-portal` if needed.

## Search Sites

Primary:
- **linkedin.com/jobs** — filter by "Remote", and by target countries (UAE, UK, Germany, Netherlands, Sweden, Norway, Canada, USA, India)
- **wellfound.com** (AngelList Talent) — startup/AI roles, remote-friendly
- **weworkremotely.com**, **remoteok.com**, **remote.io** — remote-first boards
- **ycombinator.com/jobs** (Work at a Startup) — AI-heavy, forward-deployed roles common
- **naukri.com** / **instahyre.com** / **cutshort.io** — India market

Secondary (company career pages via Google):
- Direct Google searches with `site:` filters for AI-first companies (Anthropic, OpenAI, and their customers/partners; applied-AI startups)

## Query Categories

Queries are grouped by priority. Add a location term (`remote`, or a target country) where the site supports it.

### Priority 1: Forward Deployed / Applied AI Engineer

Strongest, most desired direction — customer-facing AI product building.

```
site:linkedin.com/jobs "Forward Deployed Engineer" (AI OR LLM) remote
site:linkedin.com/jobs "Applied AI Engineer" remote
site:linkedin.com/jobs "Solutions Engineer" (LLM OR "generative AI") remote
"forward deployed engineer" AI startup careers
site:ycombinator.com "forward deployed" OR "applied AI"
```

### Priority 2: Principal / AI Architect & AI Engineering

Core AI/LLM architecture and engineering.

```
site:linkedin.com/jobs "Principal AI Architect" remote
site:linkedin.com/jobs "AI Architect" (LLM OR "multi-agent" OR RAG) remote
site:linkedin.com/jobs "Principal AI Engineer" remote
site:linkedin.com/jobs ("LLM" OR "generative AI") architect (UAE OR Dubai OR "United Kingdom" OR Germany OR remote)
site:linkedin.com/jobs "MCP" OR "agentic" engineer remote
```

### Priority 3: Staff / Principal Backend & Platform

Enterprise-Java core — Spring Boot, microservices, Kubernetes, multi-tenant SaaS.

```
site:linkedin.com/jobs "Staff Engineer" (Java OR "Spring Boot") (Kubernetes OR AWS) remote
site:linkedin.com/jobs "Principal Engineer" microservices (Java OR Go) remote
site:linkedin.com/jobs "Platform Architect" (Kubernetes OR EKS) "multi-tenant" remote
site:linkedin.com/jobs "Software Architect" (Java OR Go) SaaS (UAE OR EU OR remote)
```

### Priority 4: Engineering Leadership / AI Transformation

Player-coach and AI-transformation leadership (must keep a hands-on component).

```
site:linkedin.com/jobs "Engineering Manager" AI remote
site:linkedin.com/jobs "Head of AI" OR "AI transformation" (engineering OR platform) remote
site:linkedin.com/jobs "AI Engineering Lead" remote
site:linkedin.com/jobs "Director of Engineering" (AI OR LLM) "hands-on" remote
```

## Location Filter

Shashank is remote-first and relocation-open, so "location" is about eligibility, not commute:
- **Ideal:** Fully remote (global, or IST-overlapping)
- **Acceptable (relocation, sponsorship OK):** UAE/Dubai (Golden-Visa eligible), UK, Germany, Netherlands, Sweden, Norway, Canada, USA
- **Acceptable (local):** India — Noida/NCR, Bangalore, Gurgaon, remote-India
- **Borderline:** On-site roles in countries requiring sponsorship the employer won't provide (flag)
- **Too far / FAIL:** On-site-only with no remote or relocation support in a location he can't reach

## Date Filter

Only include jobs posted within the last 14 days, or with an application deadline that has not yet passed. If a posting date cannot be determined, include it but flag as "date unknown".

## Adapting Queries

If the user specifies a focus area, select queries from the matching category and also generate 2-3 custom queries for that focus. For example:
- "/scrape forward deployed" -> Priority 1 queries + custom FDE-specific queries
- "/scrape uae" -> add `(UAE OR Dubai OR "Abu Dhabi")` to the top queries across categories
