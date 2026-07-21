# Skills Playground

Welcome to my **Skills Playground**! 🚀

This repository is my personal lab for designing, testing, and refining custom AI agent skills for the [Gemini CLI](https://github.com/google/gemini-cli). Here, I explore how structured workflows, rigorous planning, and automated documentation can transform LLM interactions from simple chat into highly reliable, engineering-grade assistance.

## Available Skills

| Skill             | Version | Description                                                                      |
| :---------------- | :------ | :------------------------------------------------------------------------------- |
| `hybrid-planning` | 1.1.0   | Enforces a strict, two-phase ARCHITECT/BUILDER workflow.                         |
| `prd-spawnner`    | 1.0.0   | Automates professional PRD generation via structured interviews.                 |
| `prd-generator`   | 1.0.0   | Advanced PRD generator supporting scratch & continuation workflows.            |
| `sprint-planner`  | 1.0.0   | Generates role-based sprint plan breakdowns from an input PRD.                 |
| `vibe-prd`        | 1.0.3   | Vibe-Coded-Ready-PRD generator with an interview process.                        |
| `test-strategy`   | 1.0.0   | Generates comprehensive, engineering-grade test strategy documents.              |
| `code-reviewer`   | 1.0.0   | Structured, severity-tagged code reviews with APPROVE/REQUEST CHANGES verdicts.  |

## What's Inside

This repo acts as the home for my experimental workflows under the `code/` and `product-management/` folders:

- **`code/hybrid-planning/`**: Implementation of a strict, two-phase development discipline. It forces a clear separation between **ARCHITECT** (theory/planning) and **BUILDER** (code execution).
- **`product-management/prd-spawnner/`**: A toolset designed to solve the "blank page problem" by automating the generation of professional PRDs.
- **`product-management/prd-generator/`**: An advanced PRD generator supporting greenfield creation, dynamic reference templates, and continuous improvement/refinement of existing PRDs.
- **`product-management/sprint-planner/`**: A toolset that parses a PRD to construct organized, role-based sprint plans with milestone gates.
- **`code/vibe-prd/`**: A refined version of PRD generation with an English-first approach and outputs saved to `plan/prd/`.
- **`code/test-strategy/`**: A toolset for generating comprehensive, engineering-grade test strategy documents from a PRD or feature spec.
- **`code/code-reviewer/`**: A structured code review skill that interviews for context, applies an opinionated checklist, and delivers severity-tagged findings with a clear verdict.

## Why I Built This

I believe that the true power of AI agents is unlocked not by _more_ code, but by _better_ processes. By formalizing my interactions into reusable skills, I can:

1.  **Reduce Ambiguity:** Ensure every feature has a well-defined contract before implementation.
2.  **Improve Reliability:** Maintain rigorous standards for planning, documentation, and technical debt management.
3.  **Share & Iterate:** Treat my development workflow as code, allowing me to version, refine, and improve how I build software.

## Contributing & Exploration

Feel free to explore the contents. While this is primarily my personal workspace, I'm sharing it to contribute to the growing ecosystem of agentic workflows.

- **Found a workflow you like?** Feel free to adapt it for your own projects.
- **Have ideas for improvement?** Feel free to open an issue or submit a PR if you have suggestions for refining these skills.

---

_Built for the Gemini CLI ecosystem._
