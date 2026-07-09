---
name: code-reviewer
description: >
  Perform a structured, opinionated code review on a diff, file, PR, or
  code snippet. Triggers when the user types /review, or when they say
  things like "review this code", "review my PR", "check this diff",
  "give me a code review", "what's wrong with this code", "critique this
  implementation", or any variant asking for review or critique of code.
  ALWAYS use this skill when the user wants structured feedback on code
  quality, correctness, security, or maintainability. The output is a
  detailed review report with severity-tagged findings.
---

# Code Reviewer Skill

A skill that performs structured, engineering-grade code reviews before code is merged or shipped. It focuses on correctness, security, performance, maintainability, architecture, testing, error handling, and documentation.

## Why this matters

Code reviews are the last line of defense against bugs, security holes, and structural technical debt. A structured review checklist guarantees that code is audited against consistent criteria and gets a clear verdict before going live.

## Workflow

The skill runs in two phases: **Interview → Review**.

---

## Phase 1: Context Interview

**Never skip this phase.** The effectiveness of a code review depends entirely on understanding the context. 

When triggered, enter interview mode. Present all questions in a single conversational block. Tell the user this will take 1-2 minutes.

Use this exact opening:

```
Alright, before I review the code, I need to understand its context and the changes made.
Answer whatever you can — skip what you don't know, and we can figure it out.
```

### Core Interview Questions

1. **Where is the code?** (Provide path to files in workspace, paste the code snippet, or provide a git diff/PR description)
2. **What language and framework are used?**
3. **What is the type of change?** (e.g., New Feature, Bug Fix, Refactoring, Security Patch, Performance Tuning)
4. **What is the risk level?** (Low, Medium, High, Critical - e.g., hotfix to production vs. experimental prototype)
5. **Are there any specific concerns?** (e.g., performance issues, authentication logic, database queries, naming conventions)
6. **Are there project-specific style guides or standards to enforce?**

### Fallback Strategies for Incomplete Answers
If the user doesn't answer all questions, make reasonable assumptions and state them:
- Language/framework: Auto-detect from file extensions/content.
- Risk level: Assume Medium.
- Type of change: Auto-detect from git status/staged changes.

### Confirming before reviewing

After gathering context, output:

```
Alright, I've got the context. I'm ready to run the code review now.
Does anything need to be adjusted first?
```

Wait for confirmation, then proceed to Phase 2.

---

## Phase 2: Code Review

Apply the checklist in `references/code-review-checklist.md` to analyze the code. 

Generate the report and output it directly to the chat, and save it to `reviews/[feature-or-branch-name]-review.md` in the workspace root.

### Severity System

Every finding must be categorized under one of these severity levels:

- 🔴 **Critical:** Severe bugs, security vulnerabilities (leaked secrets, injection risks), data loss risks, or major logical flaws that will fail in production. Must be fixed before merge.
- 🟡 **Warning:** Architectural smell, bad programming practice, potential performance bottleneck, or high technical debt. Should be fixed unless explicitly justified.
- 🟢 **Suggestion:** Minor improvements, style mismatches, naming conventions, optimization tips, or simple code readability wins. Optional but recommended.
- 💬 **Discussion:** High-level design choices, structural trade-offs, or questions about the implementation details that require collaboration.

### Review Report Structure

The generated report must use this format:

```markdown
# Code Review: [Feature / PR Name]

**Date:** YYYY-MM-DD  
**Reviewer:** code-reviewer  
**Verdict:** [APPROVE | REQUEST CHANGES | NEEDS DISCUSSION]  

---

## 1. Summary of Changes
[A brief 2-3 sentence overview of what the changes cover and their scope.]

## 2. Overall Assessment
[Overall assessment of the code quality, risk, and structural integrity.]

## 3. Findings

### 🔴 Critical Findings
*None* (or list of critical findings):
- **[File name:Line number]**: [Description of issue and why it is critical]
  *Recommended Fix:* [Specific code snippet or correction]

### 🟡 Warnings
- **[File name:Line number]**: [Description of warnings and risks]
  *Recommended Fix:* [Suggested improvement]

### 🟢 Suggestions
- **[File name:Line number]**: [Description of suggestions]
  *Recommended Fix:* [Suggested code change]

### 💬 Discussions
- **[File name:Line number]**: [Topic of discussion or architectural question]

---

## 4. Checklist Compliance

| Category | Status | Notes |
| :--- | :--- | :--- |
| Correctness | Pass / Fail / N/A | |
| Security | Pass / Fail / N/A | |
| Performance | Pass / Fail / N/A | |
| Maintainability | Pass / Fail / N/A | |
| Architecture & Design | Pass / Fail / N/A | |
| Testing | Pass / Fail / N/A | |
| Error Handling | Pass / Fail / N/A | |
| Documentation | Pass / Fail / N/A | |

---

## 5. Review Verdict

| Finding Type | Count |
| :--- | :--- |
| 🔴 Critical | [Count] |
| 🟡 Warning | [Count] |
| 🟢 Suggestion | [Count] |
| 💬 Discussion | [Count] |

**Verdict: [APPROVE | REQUEST CHANGES | NEEDS DISCUSSION]**

**Top 3 priorities before merge:**
1. [Top priority fix]
2. [Second priority fix]
3. [Third priority fix]
```

---

## Reference files

- `references/code-review-checklist.md` — The comprehensive checklist applied during review. **Read this before reviewing.**
