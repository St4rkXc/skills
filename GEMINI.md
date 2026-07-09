# Skills Playground

This is my personal repository for developing, organizing, and managing AI agent skills. It acts as the central hub for the custom workflows, planning tools, and reference materials I use to enhance my Gemini CLI experience.

## Directory Overview

- `code/hybrid-planning/`: Contains skills and planning documentation for enforcing a strict, two-phase development discipline: **ARCHITECT** (planning) and **BUILDER** (execution). Use this for feature implementation, refactoring, and migrations.
- `code/prd-spawnner/`: Contains skills and reference materials (templates, tech stacks) for generating comprehensive, professional Product Requirement Documents (PRDs). Use this for product ideation and initial requirements definition.
- `code/vibe-prd/`: A refined version of PRD generation with an English-first approach and outputs saved to `plan/prd/`.
- `code/test-strategy/`: Contains skills and reference materials for generating comprehensive, engineering-grade test strategy documents from a PRD, feature spec, or plain-English description. Use this for test planning before or during development.

## Key Files & Structures

- **`code/hybrid-planning/.plan/`**: Storage for active feature plan documents and the `_debt.md` log.
- **`code/hybrid-planning/SKILL.md`**: Definitive guide on the Architect/Builder workflow.
- **`code/prd-spawnner/SKILL.md`**: Definitive guide on the PRD generation workflow.
- **`code/prd-spawnner/references/`**: Contains `prd-template.md` and `tech-stacks.md` used for PRD generation.
- **`code/vibe-prd/SKILL.md`**: Definitive guide on the vibe-prd workflow.
- **`code/vibe-prd/references/`**: Contains `prd-template.md` and `tech-stacks.md` used for vibe-prd generation.
- **`code/test-strategy/SKILL.md`**: Definitive guide on the test strategy generation workflow.
- **`code/test-strategy/references/`**: Contains `test-strategy-template.md` used for test strategy generation.

## Skill Development & Management

To create or modify skills in this repository, follow these guidelines:

1.  **Structure**: All skills must be stored directly within a `code/<skill-name>/` directory structure.
2.  **Configuration**: Each skill must include a `SKILL.md` file in its root directory. This file must follow the standard YAML frontmatter format (`name`, `description`) followed by a clear, detailed guide on usage, triggers, and protocols.
3.  **Creation**:
    - For new skills, create a new folder under `code/`.
    - Use the `skill-creator` skill (when available) or manually define the `SKILL.md` file.
    - Ensure your `SKILL.md` includes triggers that allow the agent to know _when_ to activate the skill.
4.  **Verification**: Test new skills in a controlled environment to ensure triggers work as expected and the agent adheres to the protocols defined in your `SKILL.md`.

## Usage

Use this repository to:

1.  Manage project-specific plans using the Hybrid Planning skill.
2.  Maintain technical debt logs via `_debt.md` in active plan directories.
3.  Store and refine PRD templates and technology reference materials.
4.  Generate test strategies from PRDs or feature specs using the Test Strategy skill.
5.  Develop and experiment with new agent-based development workflows.

> **Note:** For new development tasks, always consult the respective `SKILL.md` files to ensure adherence to defined workflows and conventions.
