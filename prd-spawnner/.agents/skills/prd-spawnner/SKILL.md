---
name: prd-spawnner
description: Generate a comprehensive, professional Product Requirements Document (PRD) before the user starts building an app or software product. Triggers when the user types /prd-spawnner, or when they say things like "buatin PRD", "buat PRD dulu", "I want to create a PRD", "help me plan my app", "generate PRD", "product requirements document", "I'm about to build an app", "planning a new product", or any variant asking to plan/document a software project before development. ALWAYS use this skill when the user wants structured documentation before coding. The output is a deeply detailed .md file (minimum 800 lines) covering every aspect of the product from architecture to deployment.
---

# PRD Spawnner

A skill that produces deeply professional, engineering-grade Product Requirements Documents before a user starts building a software product. The PRD is the north star of any project — get it right, and the entire development journey becomes measurably smoother.

## Why this matters

Most bugs and scope creep originate from ambiguity at the planning stage. A thorough PRD eliminates that ambiguity. It forces product thinking before code thinking. When done well, it also becomes a living reference that the team returns to throughout development.

## Workflow

The skill runs in two phases: **Interview → Generate**.

---

## Phase 1: Interview

**Never skip this phase.** The quality of the PRD depends entirely on the information gathered here.

When triggered, immediately enter interview mode. Present all questions in a single conversational block — don't drip them one by one. Tell the user this will take 2-3 minutes and is worth it.

Use this exact opening:

```
Oke, sebelum gua generate PRD-nya, gua butuh ngerti project lo lebih dalam dulu.
Jawab semua yang bisa lo jawab — skip yang belum lo tau, nanti bisa kita isi bareng.
```

### Core Interview Questions

Group questions into sections so it feels organized, not overwhelming.

#### 🎯 Tentang Produk
1. Apa nama produk / app yang mau lo bangun?
2. Dalam 1-2 kalimat, produk ini ngapain? (elevator pitch)
3. Masalah spesifik apa yang dipecahin?
4. Siapa target user-nya? (demografi, skill level, context of use)

#### 🖥️ Platform & Scope
5. Platform apa yang dituju? (Web app / Mobile iOS / Mobile Android / Desktop / API-only / semua?)
6. Ini MVP (minimum viable product) atau full product?
7. Ada fitur yang WAJIB ada di v1? List semuanya.
8. Ada fitur nice-to-have tapi bisa nanti? List juga.

#### ⚙️ Tech & Arsitektur
9. Ada tech stack preference? (kalau gak tau, tulis "terserah" dan gua rekomendasiin)
10. Perlu integrasi dengan sistem atau third-party service lain? (payment, auth, maps, AI, dll)
11. Udah ada codebase yang jalan? Atau greenfield?
12. Perlu backend sendiri, atau serverless/BaaS (Firebase, Supabase, dll)?

#### 📊 Scale & Bisnis
13. Estimasi user di launch: berapa? 6 bulan ke depan: berapa?
14. Ada model bisnis? (freemium, subscription, marketplace, dll)
15. Ada compliance/regulasi yang perlu diperhatiin? (GDPR, HIPAA, PCI-DSS, Kominfo, dll)
16. Siapa kompetitor terdekat? Apa yang bikin produk ini beda?

#### 👥 Tim & Timeline
17. Berapa orang di tim? Apa role-nya?
18. Target launch kapan?
19. Ada budget constraint yang perlu masuk planning?

### Handling incomplete answers

The user won't always answer everything. That's fine. Use these fallback strategies:
- If platform is unknown → assume web-first, mobile-responsive
- If tech stack is unknown → recommend based on product type (see `references/tech-stacks.md`)
- If scale is unknown → assume 1K MAU at launch, 10K at 6 months
- If team is unknown → assume solo developer or small team (2-4)
- Always state your assumptions explicitly in the PRD under "Assumptions & Constraints"

### Confirming before generating

After collecting answers, give a quick summary:
```
Oke, ini yang gua tangkep dari lo:
[bullet summary of key points]

Gua mau generate PRD sekarang. Ada yang perlu diubah dulu?
```

Wait for confirmation, then proceed to Phase 2.

---

## Phase 2: PRD Generation

Generate the PRD as a single `.md` file saved to `/mnt/user-data/outputs/[product-name]-PRD.md`.

**Minimum length: 800 lines.** This is not arbitrary — professional PRDs are thorough. If a section feels thin, go deeper. Add diagrams using Mermaid syntax. Add tables. Add code examples for API contracts.

Read `references/prd-template.md` for the complete template structure and fill every section with specific, concrete content based on what the user told you. Never use generic filler text.

### Generation principles

**Be specific, not generic.** Instead of "the system should be fast", write "API endpoints must respond in < 200ms at p95 under 500 concurrent users."

**Think like a senior engineer.** Anticipate failure modes. Call out edge cases. Flag technical risks. Suggest patterns that will prevent bugs before they happen.

**Think like a product manager.** Every feature needs a WHY. Every user story maps to a business outcome. Every metric is measurable.

**Think like a security engineer.** Don't treat security as an afterthought section — weave it throughout. Mention auth strategy in the architecture section, input validation in the API section, rate limiting in the infra section.

**Think scalably.** Even for MVPs, design decisions should not create walls. Call out which decisions are "good enough for now" and what the migration path looks like.

### Mermaid diagrams to include

Always include at least these diagrams (rendered in Mermaid):
1. **System Architecture Overview** — components and how they connect
2. **Entity Relationship Diagram** — core data models
3. **Core User Flow** — the primary happy path as a flowchart
4. **API Request Lifecycle** — how a typical request flows through the system (for products with a backend)

### After generation

Present the file using `present_files`. Then say:

```
PRD udah jadi — [X] lines, siap dijadiin north star project lo.

Beberapa hal yang gua highlight dari PRD ini:
- [top 3 most important technical decisions made]
- [top risk called out]

Lo bisa langsung share ini ke tim, atau kita bisa refine bagian tertentu kalau ada yang kurang pas.
```

---

## Reference files

- `references/prd-template.md` — Full PRD template with all sections. **Read this before generating.**
- `references/tech-stacks.md` — Tech stack recommendations by product type. Read when the user hasn't specified a stack.