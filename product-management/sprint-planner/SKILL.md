---
name: sprint-planner
description: Generate a structured, markdown-formatted sprint plan from an input Product Requirements Document (PRD). Triggers when the user runs /sprint-plan or asks for a sprint schedule/breakdown based on a PRD. Requires a PRD as input. Outputs sprint name headers (dates, total days, stakeholder sign-off status), sprint focus, a detailed role-activity-deliverable table (with separate rows per task), and key bare-minimum deliverables required to move to the next sprint.
---

# Sprint Planner

A skill designed to translate a Product Requirements Document (PRD) into a clear, actionable, and role-based Sprint Plan in markdown format. It maps out the development timeline, assigns responsibilities, and sets clear milestones/gates between sprints.

## Triggers

Activate this skill when:
- The user runs the `/sprint-plan` command.
- The user asks to build a sprint plan, sprint breakdown, timeline, or schedule from a PRD (e.g., "buat sprint plan dari PRD ini", "breakdown this PRD into sprints", "sprint planning based on PRD").

---

## Core Rules & Constraints

1. **Input Requirement**: **A PRD is mandatory.** If the user has not provided or referenced a PRD, halt and ask the user to provide or upload the PRD first.
2. **Language Compatibility**: Match the language of the input PRD. E.g., if the PRD is in English, output the sprint plan in English; if it is in Indonesian, output the sprint plan in Indonesian.
3. **Task Granularity**: In the tasks table, each row must contain a single, discrete task/activity. **Do not stack or bundle multiple tasks into a single row.**
4. **Stakeholder Sign-off Gate**: Explicitly mark whether a sprint requires stakeholder sign-off to proceed to the next sprint (e.g., after designs, before deployment, or at major checkpoints).

---

## Output Structure

The output must be a Markdown document structured exactly as follows for each sprint:

### 1. Sprint Header
Format: `Sprint [N] - [Start Date] to [End Date] / [Total Days] (Stakeholder Sign-off Required: Yes/No)`
- *Note:* If dates are not specified by the user, use placeholders (e.g., `YYYY-MM-DD` or `Day 1 to Day 10 / 10 Days`).

### 2. Sprint Focus
Describe the core objective and thematic focus of the sprint (e.g., "Authentication and Database setup" or "High-fidelity UI and client feedback").

### 3. Role & Tasks Breakdown Table
A table breaking down who does what and what they produce.

Columns:
- **Role** (e.g., Frontend Developer, Backend Developer, UI/UX Designer, QA Engineer, Project Manager)
- **Key Activities / Task** (must be written as separate rows for individual tasks/activities)
- **Output / Deliverable** (what is produced or verified by this task)

| Role | Key Activities / Task | Output / Deliverable |
| :--- | :--- | :--- |
| [Role Name] | [Discrete Task 1] | [Deliverable 1] |
| [Role Name] | [Discrete Task 2] | [Deliverable 2] |

### 4. Key Deliverables (Minimum Bar to Proceed)
List the absolute minimum deliverables/gates that must be fully completed and approved before the team is allowed to move to the next sprint.
- Format as a checklist (e.g., `- [ ] **[Deliverable Title]**: [Brief completion criteria]`).

---

## References

- [references/sprint-plan-template.md](file:///C:/Users/Jarvis/Documents/GitHub/Skills%20Playground/product-management/sprint-planner/references/sprint-plan-template.md) — The reference template and structure guidelines for generating sprint plans.
