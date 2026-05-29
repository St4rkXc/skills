# Skills Playground

This is my personal repository for developing, organizing, and managing AI agent skills. It acts as the central hub for the custom workflows, planning tools, and reference materials I use to enhance my Gemini CLI experience.

## Skills Overview

- `hybrid-plan/`: Contains skills and planning documentation for enforcing a strict, two-phase development discipline: **ARCHITECT** (planning) and **BUILDER** (execution). Use this for feature implementation, refactoring, and migrations.
- `prd-spawnner/`: Contains skills and reference materials (templates, tech stacks) for generating comprehensive, professional Product Requirement Documents (PRDs). Use this for product ideation and initial requirements definition.

## Key Files & Structures

- **`hybrid-plan/.plan/`**: Storage for active feature plan documents and the `_debt.md` log.
- **`hybrid-plan/.agents/skills/hybrid-planning/SKILL.md`**: Definitive guide on the Architect/Builder workflow.
- **`prd-spawnner/.agents/skills/prd-spawnner/SKILL.md`**: Definitive guide on the PRD generation workflow.
- **`prd-spawnner/references/`**: Contains `prd-template.md` and `tech-stacks.md` used for PRD generation.

## Skill Development & Management

To create or modify skills in this repository, follow these guidelines:

1.  **Structure**: All skills must be stored within a `.agents/skills/<skill-name>/` directory structure.
2.  **Configuration**: Each skill must include a `SKILL.md` file in its root directory. This file must follow the standard YAML frontmatter format (`name`, `description`) followed by a clear, detailed guide on usage, triggers, and protocols.
3.  **Creation**:
    - For new skills, create a new folder under `.agents/skills/`.
    - Use the `skill-creator` skill (when available) or manually define the `SKILL.md` file.
    - Ensure your `SKILL.md` includes triggers that allow the agent to know _when_ to activate the skill.
4.  **Verification**: Test new skills in a controlled environment to ensure triggers work as expected and the agent adheres to the protocols defined in your `SKILL.md`.

## Usage

Use this repository to:

1.  Manage project-specific plans using the Hybrid Planning skill.
2.  Maintain technical debt logs via `_debt.md` in active plan directories.
3.  Store and refine PRD templates and technology reference materials.
4.  Develop and experiment with new agent-based development workflows.

> **Note:** For new development tasks, always consult the respective `SKILL.md` files to ensure adherence to defined workflows and conventions.
