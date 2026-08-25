---
name: prd-generator
description: Generate or improve comprehensive, professional, human-readable and management-focused Product Requirements Documents (PRDs) from scratch or by continuing/refining an existing PRD. Triggers when the user runs /prd-generator or uses phrases like "buat PRD advanced", "benerin PRD", "lanjutkan PRD", "generate advanced PRD", "improve PRD", or "advanced product requirements document". Outputs a deeply detailed English-language PRD (minimum 800 lines) with a Table of Contents.
---

# Advanced PRD Generator (Management & UX Focus)

An advanced skill designed to produce or refine deeply professional, human-centric, and management-focused Product Requirements Documents (PRDs). The PRD acts as the single source of truth and product alignment roadmap for all team members (clients, designers, product managers, and developers). Getting it right eliminates business alignment errors, clarifies design scope, and details user journeys before execution begins.

## Why this matters

A vague or incomplete PRD leads to misaligned client expectations, poor user experience direction, and timeline inflation. This tool raises the PRD to the standards of principal product managers and design leads. By supporting **both greenfield creation and ongoing refinement/repair**, it allows PRDs to adapt to feedback while remaining focused on user value and business outcomes.

## Triggers

Activate this skill when:
- The user inputs the `/prd-generator` command.
- The user uses phrases like:
  - "buat PRD advanced", "benerin PRD", "lanjutkan PRD"
  - "generate advanced PRD", "improve existing PRD", "continue this PRD"
  - "advanced product requirements document", "help me refine my PRD"
  - "planning a new product or application"

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
   - **Gaps**: What is missing? (e.g., missing user flows, undefined personas, empty page structures, incomplete functional requirements, or missing visual asset checklists).
   - **Ambiguities**: What needs tighter definition? (e.g., vague statements like "the site must be accessible" instead of specifying compliance targets like WCAG 2.1 AA; generic KPIs).
   - **Inconsistencies**: Are there contradictions between business goals and the proposed features/layout?
2. **Present the Analysis & Action Plan**: Show the user a brief, bulleted analysis of the current PRD's state and an "Action Plan" of what you propose to add, fix, or expand.
3. **Formulate tailored transition prompts**: E.g. *"I noticed the user personas are missing demographics and pain points. I'll define those. I also noticed the visual design guidelines lack a grid system and typography scale. I'll outline those details."*

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
  - *Note:* The templates in `references/` serve as a reference guide. I will dynamically adapt the structure based on your product needs.

#### 2. 🎯 Core Features & Scope
- What are the absolute MUST-have features for this version?
- What are the out-of-scope or nice-to-have items?

#### 3. 🖥️ Platform & Integrations
- What target platforms or environments are we deploying to? (e.g. responsive web, iOS, Android).
- What third-party service connections or CMS platforms are desired? (e.g. Stripe for payments, Sanity/WordPress for content management).

#### 4. 📈 Business Goals & KPIs
- What are the target user demographics and business success metrics?
- Are there specific compliance rules (e.g., GDPR, local privacy laws, accessibility standards)?

### Handling Incomplete or Missing Answers
If the user skips questions, apply the following senior fallbacks:
- **Scope & Platform**: Assume web-first, mobile-responsive layout.
- **KPIs**: Propose standard UX goals (e.g. increase task completion rate, reduce user friction in core flows).
- **Assumptions**: Clearly document all baseline assumptions in a dedicated "Assumptions & Constraints" section.

### Confirmation
Summarize your findings and action plan in a clean bulleted list, then ask:
```
Here is my plan for the advanced PRD:
[Bullet points of key features, design approach, and gaps to resolve]

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
   - Provide concrete, non-technical, human-readable specifications. Avoid placeholders, "TBD", or vague statements.
   - Focus on business goals, user personas, screen inventories, Visual Design guidelines (spacing, typography scale, neutral color palettes), functional requirements (user roles and CMS structures), browser/device compatibilities, accessibility checklists (alt-text rules, touch target guidelines), timelines, and RACI matrices.
   - **Strict Rule: NO code blocks, database scripts, technical deployment instructions, or Mermaid diagrams.**
4. **Dynamic Template Adaptation**:
   - Do not mindlessly copy a template. Combine or adapt the structural elements of the selected reference template dynamically to fit the project's real business and design constraints.

### Output Structure

The generated PRD must follow the exact document structure of the selected reference template. All templates share common structural elements that must always be present:

#### Required Sections (All Templates)

1. **Document Header**: `# [Template Type] PRD` followed by a bold subtitle line (`**Product Requirements Document — [Subtitle]**`)
2. **Document Information**: Metadata table with fields (Project Name, Scope, Version, Date, Prepared By, Client/Project, Platform/Type, etc.)
3. **Document Revision History**: Version tracking table with columns (Version, Date, Author, Description of Change) and at minimum 3 rows (Initial Draft, Review & Stakeholder Feedback, Final Approved Version)
4. **Executive Summary**: 2-3 paragraph overview defining the product, scope, and purpose of the document
5. **Type-Specific Body Sections**: Determined by the selected template type (see below)
6. **Stakeholders & RACI / Sign-Off**: Role-based responsibility table with name, organization, responsibility, and approval authority columns
7. **Appendix**: Supplementary content — glossary tables, reference document lists, severity scales, asset references, or revision protocols
8. **Document Footer**: Three bold lines at the end — `**Document Classification:** Confidential` / `**Last Updated:** [DD MMM YYYY]` / `**Approval Status:** Pending Stakeholder Sign-Off`

#### Template-Specific Body Sections

Based on the selected template type from the interview, include the corresponding body sections:

**UX Research PRD** (reference: `references/ux-research-prd.md`):
- Research Background & Context (Business Context, Research Problem, Research Triggers)
- Research Objectives & Questions (Primary Objectives table, Research Questions grouped by theme)
- Research Methodology (Selected Methods table with rationale, Research Approach)
- Participant Criteria (Target Profile table, Recruitment Plan table)
- Research Plan & Timeline (Phase-by-phase timeline table)
- Research Instruments (Discussion Guide structure, Usability Task Scenarios)
- Analysis & Synthesis Framework (Qualitative Analysis, Quantitative Metrics table)
- Deliverables (Deliverables table with format, audience, due date)
- Research Ethics & Compliance (Data Privacy & Consent, Anonymization Protocol)

**Mobile App UI/UX Design PRD** (reference: `references/mobile-uiux-prd.md`):
- Project Overview (Background & Context, Problem Statement, Proposed Solution, Key Assumptions)
- Goals & Objectives (Business Goals, Design Objectives, KPIs table)
- Project Scope (In Scope, Out of Scope)
- User Personas (Primary and Secondary persona tables)
- User Flows & Screen Inventory (Critical User Journeys table, Screen Inventory table)
- Design Requirements (Visual Design table, Interaction & Motion, Accessibility Requirements table)
- Platform & Technical Specifications (Supported Devices & OS table, Design File Specifications)
- Deliverables & Milestones (Phase-based deliverables table with format, due date, reviewer)

**Website Development PRD** (reference: `references/website-dev-prd.md`):
- Project Overview (Background, Business Objectives, Success Criteria table)
- Scope of Work (In Scope, Out of Scope)
- Functional Requirements (User Authentication & Access Control table, Content Management table, Core Features)
- Non-Functional Requirements (Performance table, Security list, Browser & Device Compatibility table)
- Page & Content Structure (Site Map table)
- Integrations & Third-Party Services (Integration table with purpose, method, priority)
- Deliverables & Project Timeline (Sprint/Phase-based timeline table)

**Website UI Design PRD** (reference: `references/website-ui-design-prd.md`):
- Design Discovery & Brand Alignment (Brand Foundation table, Design Inspirations & References)
- Design System Requirements (Foundations table, Component Library Inventory table)
- Page Design Specifications (Page Inventory & Priority table, Homepage Design Requirements table)
- Interaction & Animation Requirements (Hover & Micro-Interactions table, Page Transitions & Loading)
- Accessibility & Quality Standards (Standards table with requirement and verification)
- Deliverables & Timeline (Phase-based deliverables table)

---

## Output and Handoff

Once the file is generated, call the file presentation tools to display it.
In your final chat message, present:
- A brief description of the generated/improved PRD.
- A highlight of **three major design/product decisions** made.
- The **top business or user experience risk** identified and how it's addressed.
- Next steps (e.g., moving to sprint planning or wireframing).

---

## References

- [references/ux-research-prd.md](file:///C:/Users/Jarvis/Documents/GitHub/Skills%20Playground/product-management/prd-generator/references/ux-research-prd.md) — UX Research PRD template (user interviews, usability testing, participant criteria, research ethics).
- [references/mobile-uiux-prd.md](file:///C:/Users/Jarvis/Documents/GitHub/Skills%20Playground/product-management/prd-generator/references/mobile-uiux-prd.md) — Mobile App UI/UX Design PRD template (mobile platforms, visual design, screen inventory, accessibility).
- [references/website-dev-prd.md](file:///C:/Users/Jarvis/Documents/GitHub/Skills%20Playground/product-management/prd-generator/references/website-dev-prd.md) — Website Development PRD template (full-stack web, CMS, SEO, functional & non-functional requirements, integrations).
- [references/website-ui-design-prd.md](file:///C:/Users/Jarvis/Documents/GitHub/Skills%20Playground/product-management/prd-generator/references/website-ui-design-prd.md) — Website UI Design PRD template (web visual design, design systems, component library, page design specs).
