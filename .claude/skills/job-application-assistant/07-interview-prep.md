# Interview Preparation Guide

<!-- SETUP: STAR examples are personalized by running /setup based on your actual experience -->

## STAR Format

Structure answers as: **Situation** (context), **Task** (your responsibility), **Action** (what you did), **Result** (outcome).

Keep answers to 1-2 minutes. Be specific. End with what you learned or would do differently.

## Ready-Made STAR Examples

<!-- Built from real experience. Fill in any hard metrics before an interview (marked [add metric]). -->

### 1. OBSERVE — shipping an AI-first observability platform as a product (Product ownership / AI engineering)
**S:** Cloud-native teams were paying cardinality-billed APM (Datadog/New Relic) and still doing root-cause analysis by hand across metrics, logs, and traces.
**T:** I set out to build a self-hosted alternative that both bundles the full observability plane and automates root-cause analysis with AI.
**A:** Designed an 11-agent AI RCA swarm over a curated eBPF stack (VictoriaMetrics, ClickHouse, OTel, Beyla, Tetragon), exposed the whole plane to AI assistants via a built-in MCP server, and shipped it like a product: Helm chart published to GHCR, multi-arch images, one-command installers for EKS/GKE/AKS, and a live demo.
**R:** A working, installable platform (chart v1.3.x) with flat per-cluster pricing instead of cardinality billing. [Add metric: users/clusters/design partners if any.]
**Use for:** "Tell me about something you built end-to-end", "Describe a technically ambitious project", "How do you use AI agents in production?"

### 2. Migrating ~400 engineers to Claude Code at Taazaa (Leadership + driving adoption)
**S:** Taazaa's ~400-engineer org was on GitHub Copilot with scattered, ad-hoc AI usage, no standards, and no measurement of impact.
**T:** As Principal Architect reporting to the CTO, I owned proving out a better approach and rolling it across the whole organization.
**A:** Demonstrated the gains Claude Code's harness gives over Copilot, then drove the migration end-to-end: delivered 8 org-wide enablement sessions (Claude Code, harness engineering, loop engineering, and a head-to-head comparison of Copilot/Codex/Cursor/Claude — later open-sourced as interactive workshop field guides), plus playbooks, standards, and a multi-IDE analytics platform so leadership could see adoption and impact.
**R:** Onboarded all ~400 engineers onto Claude Code in ~1 month and measured a ~25% productivity gain against team story-point velocity. I was the pioneer who set the whole practice up.
**Use for:** "Describe leading change at scale", "How do you drive adoption?", "Convincing skeptics", "Working with executives", "Measuring impact"

### 3. Spec-Driven Development pipeline (Systems thinking / solving an AI failure mode)
**S:** As teams used AI to code, output was inconsistent — "vibe-coded." AI-generated scaffolding was often unrelated to the rest of the app and ignored surrounding context, and quality diverged when many developers used AI in parallel.
**T:** Make AI-assisted delivery consistent and tied to real requirements, not just fast.
**A:** Introduced Spec-Driven Development into the SDLC: built a pipeline that turns an epic + story into specs and acceptance criteria, then drives implementation from those specs. Paired it with custom Claude Code skills and AI-aware scaffolding for Node.js/Java/Python that bundle the right tech-stack context per app type.
**R:** Stories and acceptance criteria mapped far more tightly to shipped code, and output stayed consistent across many devs working with AI. ~15 active projects now run on the scaffolding.
**Use for:** "Tell me about a process you improved", "A hard problem with AI in production", "How do you keep quality with AI-assisted teams?"

### 4. cross-cutting — the Spring Boot SaaS accelerator (Architecture / reuse)
**S:** Every new client SaaS engagement re-built the same foundations (multi-tenancy, RBAC, audit, search, payments), burning weeks before feature work started.
**T:** Compress that bootstrap time with a reusable, production-grade platform.
**A:** Architected a Spring Boot auto-configuration library of 16 production modules (multi-tenancy, RBAC, audit, pgvector search, LiteLLM AI gateway, payments) with 264+ tests and SDKs in React/Node/Python/Java.
**R:** Engagement bootstrap dropped from ~weeks to days; a consistent, tested baseline across projects. [Add metric: engagements using it.]
**Use for:** "Describe a system you designed", "How do you think about reuse/DRY?", "Balancing speed and quality"

### 5. Panerai luxury e-commerce at AKQA (Client-facing delivery under pressure)
**S:** Richemont's Panerai brand needed a global e-commerce platform meeting exacting luxury-retail standards, with the client directly involved.
**T:** As the client-facing engineer, own architecture decisions and present them to brand-side stakeholders.
**A:** Delivered a 16-month program on AEM (OSGi/Sling/JCR) + Java 8 microservices + AWS with personalization, payment, and inventory integrations, managing the client relationship throughout.
**R:** Shipped the platform to the brand's standards; built durable client trust — the pattern I now bring to forward-deployed work.
**Use for:** "Tell me about a demanding client", "Handling high-stakes stakeholders", "Communication under pressure"

### 6. Fixing a production LLM research pipeline (Python / correctness + cost + latency)
**S:** A production Python pipeline doing research on individuals (billionaires) took 20+ minutes per run and had correctness defects that had surfaced in guardrails and outbound emails — it sometimes researched the wrong person, and mislabeled fiction (novels/stories a subject had authored) as real-life events.
**T:** Make it correct, faster, and cheaper without losing answer quality.
**A:** Reworked the pipeline: fixed the retrieval/grounding and guardrail logic that caused wrong-subject and fiction-as-fact errors, and restructured the LLM calls/infrastructure for efficiency.
**R:** Cut runtime by ~65% (from 20+ minutes), delivered answers at <50% of the prior cost, and closed the correctness defects that had been flagged repeatedly.
**Use for:** "Show me hands-on LLM/Python work", "A production AI reliability problem", "How do you handle hallucination / evals / cost?", "Optimizing an AI system"

<!-- Additional anchors available: Prompture (AI governance/EU AI Act), Spreix Notetaker (multi-tenant SaaS + 35 agents),
     Coforge Umantis (leading a 12-member team, GDPR/multi-tenant isolation), IBM real-time flagging system. -->

## Common Tough Questions

### "Why are you looking to move from Taazaa?"
> I've had a great run here — I built the org's AI practice from scratch and shipped several production platforms. I'm looking for a role where I can go deeper on frontier AI product work at a bigger scale, with strong engineers around me, rather than being the one person defining the practice. It's about the next level of challenge, not away from anything. [Adapt to the specific company.]

### "You don't have formal ML / data-science background."
> That's fair — I'm not training models from scratch, and I don't claim to be. My strength is building production LLM *systems*: multi-agent orchestration, MCP servers, RAG pipelines, evals, and the platform/observability layer around them. I've shipped 5 of these to production. For a role that needs applied AI in real products, that's exactly the profile; where deep ML research is core, I'd partner with specialists.

### "Where do you see yourself in 5 years?"
> Still hands-on with AI systems, but at the level where I'm shaping a company's core AI product and the engineering approach around it — principal/architect scope with real ownership. I deliberately want to keep building, not become a manager who's three layers from the code.

### "What's your biggest weakness?"
> I tend to build broadly — I've shipped a lot of products in parallel, which can spread focus. I've learned to counter it by ruthlessly picking the two or three that matter and going deep, and by shipping to production (tests, charts, SDKs) so nothing stays a half-finished prototype.

### "Why this company specifically?"
> Customize per company. Must reference: specific projects, company values, market position, or team structure. Never give a generic answer.

## Questions You Should Ask Interviewers

### About the Role
- "What does a typical week look like in this role?"
- "What would success look like in the first 6 months?"
- "What's the biggest challenge the team is facing right now?"

### About the Team
- "How big is the team, and how do you divide work?"
- "What does the development/project lifecycle look like, from idea to production?"
- "How do you onboard new team members?"

### About Tech & Growth
- "What's your current tech stack for [relevant area]?"
- "Is there room to grow into more architectural or strategic decisions?"
- "How does the team stay current with new tools and methods?"

### About Culture (use these to prevent disappointment)
- "How would you describe the team culture?"
- "What does professional development look like here?"
- "Is there flexibility for remote/hybrid work?"
- "What's the balance between development/new projects and maintenance work?"
- "How would you describe the leadership style in this team?"
- "What do people who thrive here have in common?"

## Phone/Video Interview Tips
- Have STAR examples written out (use this file)
- Keep a glass of water nearby
- Smile when speaking (it changes your tone)
- Ask for clarification if a question is vague
- It's OK to take 5 seconds to think before answering
- End with: "Is there anything else you'd like to know about my background?"

## After the Application (Best Practice)

### Follow-Up Etiquette
- **Don't call to "stand out"** or to learn more about the role post-submission - this risks a negative impression
- If the employer specified a timeline, respect it and wait
- If no timeline was given and significant time has passed (2+ weeks), a brief call to ask about status is acceptable
- If you have genuinely new, relevant information to share, a short follow-up is fine

### Thank-You Notes
- When you receive any update (interview invitation, rejection, or status update), send a brief thank-you message
- Express appreciation for their time and the process
- Keep it short (2-3 sentences)

## Roleplay Guidelines
When the user asks for interview practice:
1. Ask which role/company to simulate
2. Start with easy warm-up questions ("Tell me about yourself")
3. Progress to role-specific technical questions
4. Include 1-2 behavioral questions using the competencies from the job posting
5. End with a tough question or curveball
6. After each answer, give brief feedback: what worked, what to sharpen
7. Suggest which STAR example would work best for each question
