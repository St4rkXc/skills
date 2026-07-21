---
name: prd-generator
description: Generate or improve comprehensive, professional, engineering-grade Product Requirements Documents (PRDs) from scratch or by continuing/refining an existing PRD. Triggers when the user runs /prd-generator or uses phrases like "buat PRD advanced", "benerin PRD", "lanjutkan PRD", "generate advanced PRD", "improve PRD", or "advanced product requirements document". Outputs a deeply detailed English-language PRD (minimum 800 lines) with a Table of Contents and Mermaid diagrams.
---

# Advanced PRD Generator

An advanced skill designed to produce or refine deeply professional, engineering-grade Product Requirements Documents (PRDs). The PRD acts as the single source of truth and north star for a project. Getting it right eliminates ambiguity, prevents scope creep, and establishes clear contracts before any code is written.

## Why this matters

A mediocre PRD leads to architectural dead ends, misaligned expectations, and technical debt. This tool elevates the PRD to principal-engineer and lead-PM standards. By supporting **both from-scratch creation and continuous refinement/repair**, it allows PRDs to evolve dynamically alongside the product rather than remaining static drafts.

## Triggers

Activate this skill when:
- The user inputs the `/prd-generator` command.
- The user uses phrases like:
  - "buat PRD advanced", "benerin PRD", "lanjutkan PRD"
  - "generate advanced PRD", "improve existing PRD", "continue this PRD"
  - "advanced product requirements document", "help me refine my PRD"
  - "planning a complex app/system"

---

## Workflow

The skill executes in three distinct phases: **Mode Selection & Analysis → Tailored Interview → Advanced Generation**.

---

## Phase 0: Mode Selection & Analysis

First, determine if the user wants to start **from scratch** or **modify/continue/improve** an existing PRD.

### A. Greenfield (From Scratch)
If starting from scratch, skip to **Phase 1: Dynamic Interview**.

### B. Continuation & Refinement (Existing PRD)
If the user wants to continue or improve an existing PRD:
1. **Analyze the existing PRD**: Read the file carefully. Identify:
   - **Gaps**: What is missing? (e.g., missing API definitions, incomplete database schema details, handoff specs, empty sections).
   - **Ambiguities**: What needs tighter specification? (e.g., generic performance statements like "the app should be fast" instead of P95 response times; weak security definitions).
   - **Inconsistencies**: Are there contradictions between features and architectural choices?
   - **Visuals**: Are there missing or outdated Mermaid diagrams?
2. **Present the Analysis & Action Plan**: Show the user a brief, bulleted analysis of the current PRD's state and an "Action Plan" of what you propose to add, fix, or expand.
3. **Formulate tailored transition prompts**: E.g. *"I noticed the current database schema doesn't specify relations for X. I'll add that in. I also noticed the API contracts are missing error response models. I'll document those."*

---

## Phase 1: Dynamic Interview

**Never skip the interview phase.** A great PRD cannot be generated from thin air; it requires context.

Use this opening:
```
Alright, let's build/refine your advanced PRD. 
I will ask a few tailored questions to gather context or address gaps. 
Feel free to answer what you can, and we can determine/assume the rest together.
```

### Core Interview Categories

Based on the project type and current state, present a grouped set of questions (aim for 5-8 highly relevant questions to avoid questionnaire fatigue):

#### 1. 📋 Project Context & Mode
- Are we starting from scratch, or are we refactoring/extending an existing document?
- Which template style fits this project best? (Select one or let me choose):
  - **UX Research PRD** (focuses on user interviews, usability testing, and participant criteria)
  - **Mobile App UI/UX Design PRD** (focuses on mobile platforms, visual design, and screen inventory)
  - **Website Development PRD** (focuses on full-stack web, CMS, SEO, and functional requirements)
  - **Website UI Design PRD** (focuses on web visual design, design systems, and page sections)
  - *Note:* The template in `references/prd-template.md` serves as a reference guide. I will dynamically adapt the structure based on your product needs.

#### 2. 🎯 Core Features & Scope
- What are the absolute MUST-have features for this version?
- What are the out-of-scope or nice-to-have items?

#### 3. ⚙️ Technology & Integration
- What is your preferred tech stack? (If unsure, write "recommend" and I will consult `references/tech-stacks.md` to suggest one).
- What third-party APIs or integrations are required? (e.g., payments, auth, maps, AI/LLMs).

#### 4. 📈 Scale & Performance Requirements
- What are the target metrics? (e.g., expected page load time, concurrent users, service uptime, API latency targets).
- Are there specific compliance rules (e.g., GDPR, HIPAA, local privacy laws)?

### Handling Incomplete or Missing Answers
If the user skips questions, apply the following senior fallbacks:
- **Tech Stack**: Choose the optimal stack from [references/tech-stacks.md](file:///C:/Users/Jarvis/Documents/GitHub/Skills%20Playground/product-management/prd-generator/references/tech-stacks.md) matching their product type.
- **Scale**: Assume a standard MVP launch baseline (e.g., 1K MAU, P95 latency < 300ms).
- **Compliance**: Default to standard secure practices (OWASP Top 10, JWT auth, HTTPS) and state assumptions explicitly under a dedicated "Assumptions & Constraints" section.

### Confirmation
Summarize your findings and action plan in a clean bulleted list, then ask:
```
Here is my plan for the advanced PRD:
[Bullet points of key features, architecture choice, and gaps to resolve]

I'm ready to generate the PRD now. Does anything need to be adjusted first?
```
Once approved, proceed to Phase 2.

---

## Phase 2: Advanced PRD Generation

Generate the PRD as a single, comprehensive markdown file saved to `plan/prd/[product-name]-PRD.md`.

### Core Requirements

1. **Table of Contents (TOC)**:
   - Place a clear, clickable Table of Contents at the top of the document (right after the Document Information header).
   - Use relative anchors (e.g. `[1. Executive Summary](#1-executive-summary)`).
2. **Language**:
   - The entire document must be written in **English**.
3. **Thoroughness & Detail (Minimum 800+ lines)**:
   - Provide concrete, engineering-grade details. Avoid placeholders, "TBD", or vague statements.
   - Specify real API contracts (JSON format/REST endpoints), real database schema columns, real performance latency requirements (e.g., *p95 < 250ms under 200 RPS*), and real security controls.
4. **Mermaid Diagrams**:
   Include at least **four** functional, valid Mermaid diagrams:
   - **System Architecture Diagram**: Showing components (Frontend, Gateway, Backend, DB, Cache, External Services).
   - **Entity Relationship Diagram (ERD)**: Core data entities, fields, data types, and relationships.
   - **Core User Flow**: Flowchart of the primary user journey (happy path + primary error handling path).
   - **API Request Lifecycle / Info Architecture**: A sequence flowchart or tree diagram showing how data flows or how pages are structured.
5. **Dynamic Template Adaptation**:
   - Do not mindlessly copy a template. Combine or adapt the structural elements of [references/prd-template.md](file:///C:/Users/Jarvis/Documents/GitHub/Skills%20Playground/product-management/prd-generator/references/prd-template.md) dynamically to fit the project's real constraints.

---

## Output and Handoff

Once the file is generated, call the file presentation tools to display it.
In your final chat message, present:
- A brief description of the generated/improved PRD.
- A highlight of **three major architectural decisions** made.
- The **top technical or product risk** identified and how it's addressed.
- Next steps (e.g., moving to test planning or architectural prototyping).

---

## References

- [references/prd-template.md](file:///C:/Users/Jarvis/Documents/GitHub/Skills%20Playground/product-management/prd-generator/references/prd-template.md) — The reference template variations (UX Research, Mobile UI/UX, Web Dev, Web UI Design).
- [references/tech-stacks.md](file:///C:/Users/Jarvis/Documents/GitHub/Skills%20Playground/product-management/prd-generator/references/tech-stacks.md) — Tech stack recommendations categorized by product type.
