---
name: test-strategy
description: >
    Generate a comprehensive, engineering-grade test strategy document from a PRD, feature spec,
    or plain-English description. Triggers when the user types /test-strategy, or when they say
    things like "create test plan", "how should I test this", "write test strategy", "test coverage plan",
    "I need a testing strategy", "plan my tests", "what should I test", or any variant asking to
    plan testing for a feature, module, or entire product. ALWAYS use this skill when the user
    wants structured test planning before or during development. The output is a deeply detailed .md
    file covering unit, integration, E2E, performance, and security testing with concrete test cases,
    tooling recommendations, and coverage targets.
---

# Test Strategy

A skill that produces a thorough, actionable test strategy document before or during development. Testing without a strategy leads to gaps, redundancy, and false confidence. A good test strategy answers: what to test, how to test it, when to test it, and who owns it.

## Why this matters

Most teams either over-test trivial paths or under-test critical ones. A test strategy forces you to think about failure modes, edge cases, and risk surfaces before writing a single test. It becomes the contract between engineering and quality — and the checklist you audit before shipping.

## Workflow

The skill runs in two phases: **Interview → Generate**.

---

## Phase 1: Interview

**Never skip this phase.** The quality of the strategy depends entirely on the information gathered here.

When triggered, immediately enter interview mode. Present all questions in a single conversational block. Tell the user this will take 2-3 minutes.

Use this exact opening:

```
Alright, before I build your test strategy, I need to understand what we're testing and what's at stake.
Answer whatever you can — skip what you don't know yet, we can fill it in later.
```

### Core Interview Questions

#### 🎯 Feature / Product Overview

1. What is the name of the feature, module, or product being tested?
2. In 1-2 sentences, what does it do?
3. What is the single most critical user flow? (the one that must never break)
4. What are the secondary flows?

#### 🧩 Scope & Boundaries

5. Is this a new feature, a refactor, or an existing system with no tests?
6. What is in scope for this strategy? (specific modules, APIs, UI flows)
7. What is explicitly out of scope?
8. Are there existing tests? If so, what coverage exists today?

#### ⚙️ Tech Stack & Tooling

9. What is the tech stack? (language, framework, backend, frontend)
10. Do you have existing test tooling? (Jest, Vitest, Pytest, Playwright, Cypress, etc.)
11. Is there a CI/CD pipeline? What runs tests today?
12. Are there any testing constraints? (no browser tests, no DB access in CI, etc.)

#### 📊 Risk & Scale

13. What are the highest-risk failure modes? (data loss, security breach, downtime, bad UX)
14. How many users / requests per day at peak?
15. Are there compliance requirements that mandate test coverage? (SOC2, HIPAA, PCI-DSS)
16. What is the cost of a bug reaching production? (reputation, revenue, safety)

#### 👥 Team & Process

17. Who writes tests? (developers, QA, both?)
18. Is there a code review process? Do tests block merges?
19. What is the release cadence? (daily, weekly, monthly)
20. Are there any past incidents or recurring bugs that should inform the strategy?

### Handling incomplete answers

The user won't always answer everything. Use these fallback strategies:

- If tech stack is unknown → recommend based on product type
- If scale is unknown → assume moderate traffic, standard SLA
- If team is unknown → assume developers own tests, no dedicated QA
- If risk is unknown → assume medium risk, standard coverage targets
- Always state your assumptions explicitly in the strategy under "Assumptions & Constraints"

### Confirming before generating

After collecting answers, give a quick summary:

```
Alright, here is what I have gathered:
[bullet summary of key points]

I'm ready to generate the test strategy. Does anything need to be changed first?
```

Wait for confirmation, then proceed to Phase 2.

---

## Phase 2: Test Strategy Generation

Generate the strategy as a single `.md` file saved to the project's `docs/` directory (or current working directory if no `docs/` exists) as `[feature-name]-test-strategy.md`.

**Minimum length: 400 lines.** Professional test strategies are thorough. If a section feels thin, go deeper. Add tables. Add concrete test case examples. Add Mermaid diagrams for test flows.

Read `references/test-strategy-template.md` for the complete template structure and fill every section with specific, concrete content based on what the user told you. Never use generic filler text.

### Generation principles

**Be specific, not generic.** Instead of "test the API", write "test POST /api/users with valid payload, missing required fields, invalid email format, and duplicate email — expect 201, 400, 400, 409 respectively."

**Think like a QA engineer.** Anticipate failure modes. Think about state, timing, concurrency, and data dependencies. Every test case needs a clear arrange-act-assert structure.

**Think like a security engineer.** Don't treat security testing as an afterthought. Weave it throughout — input validation in unit tests, auth in integration tests, penetration scenarios in E2E.

**Think about ROI.** Not everything needs 100% coverage. Prioritize tests by risk. Critical paths get exhaustive coverage. Edge cases get targeted tests. Low-risk code gets smoke tests.

**Think about maintenance.** Tests that are hard to maintain get deleted. Recommend patterns that reduce flakiness: avoid brittle selectors, use factories over fixtures, mock at boundaries not everywhere.

### Sections to include

Always include these sections (see template for full details):

1. **Executive Summary** — what this strategy covers and why
2. **Test Pyramid** — unit, integration, E2E breakdown with percentages
3. **Unit Testing** — what to test, patterns, coverage targets
4. **Integration Testing** — API, DB, service boundaries
5. **E2E / UI Testing** — critical user flows, tooling
6. **Performance Testing** — load, stress, baseline metrics
7. **Security Testing** — OWASP top 10, auth, input validation
8. **Test Data Strategy** — factories, fixtures, seeding, cleanup
9. **CI/CD Integration** — what runs when, blocking vs non-blocking
10. **Coverage Targets** — per-layer, per-module, with rationale
11. **Concrete Test Cases** — at least 20 specific test cases with expected outcomes
12. **Tooling Recommendations** — specific tools for the stack
13. **Risk Matrix** — failure modes ranked by likelihood × impact
14. **Assumptions & Constraints** — what was assumed, what limits testing

### Mermaid diagrams to include

Always include at least these diagrams (rendered in Mermaid):

1. **Test Pyramid** — visual breakdown of test layers
2. **Critical User Flow** — the primary happy path with test checkpoints marked
3. **CI Pipeline** — what tests run at each stage (PR, merge, deploy)

### After generation

Present the file. Then say:

```
The test strategy has been generated — [X] lines, ready to guide your testing effort.

Here are the highlights:
- [top 3 highest-risk areas identified]
- [recommended coverage targets]
- [most critical test cases to write first]

You can share this with your team, or we can refine specific sections if anything doesn't fit.
```

---

## Reference files

- `references/test-strategy-template.md` — Full test strategy template with all sections. **Read this before generating.**
