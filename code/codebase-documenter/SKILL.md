---
name: codebase-documenter
description: >
  Generate enterprise-grade documentation for an entire codebase. Produces
  language-idiomatic inline docblocks (JSDoc, TSDoc, phpDoc, PEP257, Javadoc,
  godoc, XML doc comments, rustdoc) and updates separate project-level docs
  (README, API reference, architecture overview, changelog). Triggers ONLY
  when the user types /doc. ALWAYS use this skill when the user wants to
  document an entire project, generate docblocks across files, or produce
  project-level documentation. Supports both generating missing docs for
  existing code and enforcing doc standards on new code. Includes Mermaid
  and PlantUML diagrams for architecture and flow visualization.
---

# Codebase Documenter Skill

An enterprise-grade documentation skill that produces language-idiomatic inline docblocks and project-level documentation for an entire codebase. It detects languages, applies the correct documentation standard, and generates both inline and standalone documentation artifacts.

## Why this matters

Undocumented codebases accumulate tribal knowledge debt. Inconsistent docblocks across languages break IDE tooling, confuse contributors, and degrade API discoverability. A single skill that enforces the correct standard per language — and produces project-level docs in one pass — eliminates the gap between code and documentation.

## Workflow

The skill runs in three phases: **Interview → Document → Feedback**.

---

## Phase 1: Context Interview

**Never skip this phase.** Documentation quality depends entirely on understanding the project scope and audience.

When triggered via `/doc`, enter interview mode. Present all questions in a single conversational block. Tell the user this will take 2-3 minutes.

Use this exact opening:

```
Alright, before I document the codebase, I need to understand the project structure and documentation goals.
Answer whatever you can — skip what you don't know, we can detect the rest.
```

### Core Interview Questions

#### Project Scope

1. **What is the project root?** (Provide path or confirm current working directory)
2. **What is the project name and purpose?** (1-2 sentences)
3. **What is the target audience for the docs?** (Internal team, external API consumers, open-source contributors, all)

#### Documentation Scope

4. **What should be documented?** Choose all that apply:
   - [ ] All source files (full codebase)
   - [ ] Specific directories or modules (specify which)
   - [ ] Public API surface only
   - [ ] Only undocumented code (fill gaps)
   - [ ] Only changed/new files (enforcement mode)
5. **Which project-level docs should be generated/updated?** Choose all that apply:
   - [ ] README.md
   - [ ] API Reference
   - [ ] Architecture Overview (with diagrams)
   - [ ] CHANGELOG.md
   - [ ] All of the above
6. **Should existing docblocks be validated and corrected, or only missing ones added?** (Validate + fill, fill only, validate only)

#### Standards & Conventions

7. **Are there project-specific documentation conventions?** (e.g., custom tags, specific formatting, company style guide)
8. **Should deprecated code be flagged?** (Yes/No)
9. **Should undocumented public APIs be flagged as warnings?** (Yes/No)

#### Diagrams

10. **Which diagrams should be included in the architecture doc?** Choose all that apply:
    - [ ] Module dependency graph (Mermaid)
    - [ ] Data flow diagram (Mermaid)
    - [ ] Class hierarchy / ER diagram (Mermaid or PlantUML)
    - [ ] Sequence diagrams for critical flows (Mermaid)
    - [ ] Deployment / infrastructure diagram (PlantUML)
    - [ ] All applicable

### Fallback Strategies

If the user doesn't answer all questions:
- Project root: Use current working directory
- Languages: Auto-detect from file extensions
- Scope: Default to all source files + all project-level docs
- Standards: Apply language-default standards (see references)
- Diagrams: Include module dependency + data flow + class hierarchy
- Audience: Default to internal team

### Confirming before documenting

After gathering context, output:

```
Alright, here is what I have gathered:
[bullet summary of key points]

Detected languages: [list]
Files to document: [count]
Project-level docs to generate: [list]

I'm ready to start documentation. Does anything need to be adjusted first?
```

Wait for confirmation, then proceed to Phase 2.

---

## Phase 2: Documentation Generation

### Step 2A: Language Detection & Standard Assignment

Scan the project for source files. Map each file extension to its documentation standard:

| Language | Extensions | Standard | Reference |
|----------|-----------|----------|-----------|
| JavaScript | `.js`, `.mjs`, `.cjs` | JSDoc | `@param`, `@returns`, `@throws`, `@example`, `@deprecated` |
| TypeScript | `.ts`, `.tsx` | TSDoc | `@param`, `@returns`, `@throws`, `@example`, `@deprecated`, `@typeParam` |
| PHP | `.php` | phpDoc (PSR-5/PSR-19) | `@param`, `@return`, `@throws`, `@example`, `@deprecated`, `@see` |
| Python | `.py` | PEP 257 / Google style | Docstrings with `Args:`, `Returns:`, `Raises:`, `Examples:` |
| Java | `.java` | Javadoc | `@param`, `@return`, `@throws`, `@see`, `@since`, `@deprecated` |
| Go | `.go` | godoc | Comment sentences above declarations, `// Example:` blocks |
| C# | `.cs` | XML Doc Comments | `<summary>`, `<param>`, `<returns>`, `<exception>`, `<example>` |
| Rust | `.rs` | rustdoc | `///` lines with `# Arguments`, `# Returns`, `# Errors`, `# Examples` |
| Ruby | `.rb` | YARD / RDoc | `@param`, `@return`, `@raise`, `@example`, `@deprecated` |
| Swift | `.swift` | Swift Markup | `- parameter:`, `- returns:`, `- throws:`, `- note:`, `- warning:` |
| Kotlin | `.kt` | KDoc | `@param`, `@return`, `@throws`, `@see`, `@sample` |
| Dart | `.dart` | dartdoc | `@param`, `@returns`, `@throws`, `@example` |

Read `references/docblock-standards.md` for the complete specification per language before generating any docblocks.

### Step 2B: Inline Docblock Generation

For each source file, generate docblocks following these rules:

#### What to document

1. **All public/ exported functions, methods, classes, interfaces, traits, enums**
2. **All public properties and fields**
3. **All modules/packages** (module-level docblock at top of file)
4. **Complex private/internal functions** (when logic is non-obvious)
5. **Type definitions, interfaces, and structs**

#### Docblock content requirements

Every docblock must include:

1. **Summary line** — one sentence describing what the entity does (not how)
2. **Description** (if needed) — additional context, behavior notes, side effects
3. **Parameter docs** — name, type, description, default value if optional
4. **Return value** — type and description
5. **Throws/Raises** — every exception/error type with condition
6. **Examples** — at least one runnable example for non-trivial functions
7. **Deprecated notice** — with replacement if applicable
8. **See also** — cross-references to related functions/classes

#### Docblock quality rules

- Summary must be imperative for functions ("Calculate the total...") or declarative for classes ("Represents a user session...")
- No redundant docs that merely restate the name (`/** Returns the name */` for `getName()` is forbidden)
- Types must match actual code types, not be vague (`string` not `mixed`)
- Examples must be syntactically valid and runnable
- `@throws` must list actual exceptions the function can raise, not generic "throws errors"

### Step 2C: Project-Level Documentation

Generate the selected project-level docs. Read `references/project-docs-template.md` for the complete template structure.

#### README.md

Must include:
- Project name, badge area, one-line description
- Table of contents
- Features / capabilities list
- Quick start (installation + minimal usage)
- Architecture overview (with Mermaid diagram)
- API summary (link to full API reference)
- Configuration reference
- Contributing guidelines
- License

#### API Reference

Must include:
- Module/package index
- Per-module: exported entities with full signatures, docblock content, examples
- Type definitions and interfaces
- Error/exception reference
- Constants and enums

#### Architecture Overview

Must include:
- System context diagram (Mermaid)
- Module dependency graph (Mermaid)
- Data flow diagram (Mermaid)
- Class/entity hierarchy (Mermaid or PlantUML)
- Key design decisions and rationale
- Technology stack summary
- Directory structure with purpose of each directory

#### CHANGELOG.md

Must follow [Keep a Changelog](https://keepachangelog.com/) format:
- `[Unreleased]` section
- Categories: Added, Changed, Deprecated, Removed, Fixed, Security
- Date-stamped version entries
- Link to comparison diffs

### Output Locations

| Document | Path |
|----------|------|
| Inline docblocks | Written directly into source files |
| README.md | `[project-root]/README.md` (update existing) |
| API Reference | `[project-root]/docs/api-reference.md` |
| Architecture | `[project-root]/docs/architecture.md` |
| CHANGELOG | `[project-root]/CHANGELOG.md` (update existing) |

---

## Phase 3: Documentation Feedback Report

After generation, produce a feedback report saved to `docs/documentation-report.md`.

### Report Structure

```markdown
# Documentation Report

**Date:** YYYY-MM-DD
**Project:** [project name]
**Documenter:** codebase-documenter

---

## 1. Coverage Summary

| Language | Total Files | Documented | Undocumented | Coverage % |
|----------|------------|------------|--------------|------------|
| [lang]   | [n]        | [n]        | [n]          | [%]        |

**Overall coverage:** [X]%

## 2. Documentation Quality Score

| Category | Score | Notes |
|----------|-------|-------|
| Completeness | [1-10] | [notes] |
| Accuracy | [1-10] | [notes] |
| Consistency | [1-10] | [notes] |
| Example coverage | [1-10] | [notes] |
| Standard compliance | [1-10] | [notes] |

**Overall quality:** [X]/10

## 3. Code Feedback

### Documentation Anti-Patterns Found

- **[File:Line]**: [Anti-pattern description and fix]
  - Example: Redundant docblock that restates function name
  - Example: Missing `@throws` for function that raises exceptions
  - Example: Vague type annotation (`mixed` instead of specific type)

### Missing Documentation Warnings

- **[File:Line]**: [Public entity without docblock]

### Suggestions

- [Improvement suggestion with rationale]

## 4. Generated Artifacts

| Document | Path | Status |
|----------|------|--------|
| [doc name] | [path] | Created / Updated |

## 5. Diagrams Generated

| Diagram | Type | Location |
|---------|------|----------|
| [name] | Mermaid/PlantUML | [file:section] |
```

### After generation

Present the report summary to the user:

```
Documentation complete.

Coverage: [X]% across [N] files ([language list])
Quality score: [X]/10
Project docs generated: [list]
Diagrams created: [count]
Warnings: [count] undocumented public APIs

Full report: docs/documentation-report.md

Top 3 recommendations:
1. [Highest priority documentation gap]
2. [Second priority]
3. [Third priority]
```

---

## Reference files

- `references/docblock-standards.md` — Complete docblock specifications per language. **Read this before generating any inline docblocks.**
- `references/project-docs-template.md` — Templates for README, API reference, architecture overview, and CHANGELOG. **Read this before generating project-level docs.**
