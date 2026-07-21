# AGENTS.md

**Read `GEMINI.md` first** — it contains the canonical directory structure, skill management rules, and workflow guidelines for this repo.

## Quick reference

This is a markdown-only repo of AI agent skills for Gemini CLI. No code, no build system, no tests.

### Skills

| Directory | Skill | Trigger |
|---|---|---|
| `code/hybrid-planning/` | `hybrid-planning` | `/hybrid-plan` slash command |
| `product-management/prd-spawnner/` | `prd-spawnner` | `/prd-spawnner` or PRD-related phrases |
| `product-management/prd-generator/` | `prd-generator` | `/prd-generator` or advanced PRD-related phrases |
| `product-management/sprint-planner/` | `sprint-planner` | `/sprint-plan` slash command |
| `code/vibe-prd/` | `vibe-prd` | `/vibe-prd` or PRD-related phrases |
| `code/test-strategy/` | `test-strategy` | `/test-strategy` or test planning phrases |
| `code/code-reviewer/` | `code-reviewer` | `/review` or code review phrases |

### Key conventions

- `prd-spawnner`, `prd-generator`, and `vibe-prd` are variants of PRD builders. `vibe-prd` and `prd-generator` output to `plan/prd/`, while `prd-spawnner` outputs to `/mnt/user-data/outputs/`
- `sprint-planner` takes a PRD as input and outputs a role-based, Markdown-formatted sprint schedule.
- SKILL.md descriptions must include trigger conditions so the agent knows when to activate
- Reference files (templates, tech stacks) are duplicated per skill, not shared
