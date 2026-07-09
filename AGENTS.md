# AGENTS.md

**Read `GEMINI.md` first** — it contains the canonical directory structure, skill management rules, and workflow guidelines for this repo.

## Quick reference

This is a markdown-only repo of AI agent skills for Gemini CLI. No code, no build system, no tests.

### Skills

| Directory | Skill | Trigger |
|---|---|---|
| `code/hybrid-planning/` | `hybrid-planning` | `/hybrid-plan` slash command |
| `code/prd-spawnner/` | `prd-spawnner` | `/prd-spawnner` or PRD-related phrases |
| `code/vibe-prd/` | `vibe-prd` | `/vibe-prd` or PRD-related phrases |
| `code/test-strategy/` | `test-strategy` | `/test-strategy` or test planning phrases |

### Key conventions

- `prd-spawnner` and `vibe-prd` are forks of the same PRD generator; `vibe-prd` outputs to `plan/prd/`, `prd-spawnner` outputs to `/mnt/user-data/outputs/`
- SKILL.md descriptions must include trigger conditions so the agent knows when to activate
- Reference files (templates, tech stacks) are duplicated per skill, not shared
