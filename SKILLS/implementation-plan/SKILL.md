---
name: implementation-plan
description: "Use this skill when the user asks for an implementation plan, development plan, step-by-step coding plan, or instructions for another model/developer to implement a requested change. This skill plans only and must not modify code."
---

# Implementation plan

Produce a complete, detailed, step-by-step plan for the requested change. Do not write or modify code.

The executor is a less capable coding model or careful junior developer. Make the plan mechanically actionable, with no missing steps, implicit architectural decisions, or avoidable follow-up questions.

## Before planning

1. Inspect the relevant codebase, architecture, conventions, naming, data flow, tests, and related files.
2. Identify every file, function, component, API, type, configuration, test, and document that needs to be created or changed.
3. Resolve ambiguity with reasonable, codebase-consistent decisions. Choose the best implementation approach and explain why rather than delegating the choice to the executor.
4. Record requirements that cannot be resolved from the codebase under "Open Questions". Identify which steps they block; do not present blocked work as ready to execute.

## Required plan structure

### 1. Objective

State the exact goal and expected user-visible or developer-visible behavior.

### 2. Current-State Analysis

Explain how the relevant code works today. Identify the files, modules, functions, components, routes, types, database tables, configuration, and tests involved, and the patterns to follow.

### 3. Desired End State

Describe the final architecture and behavior. Specify new files, functions, types, components, endpoints, database changes, environment variables, and configuration where applicable.

### 4. Implementation Steps

Provide small, numbered steps in execution order. For each, specify:

- Exactly what to change, where, and why.
- Expected names for new functions, variables, files, types, routes, tests, and constants where applicable.
- Intended logic, important edge cases, and error-handling behavior.
- Dependencies and ordering constraints.

Do not substitute vague directions such as "update the logic" or "handle errors" for concrete instructions.

### 5. Testing Plan

List all tests to add or update, with test files, cases, inputs, expected outputs, mocks, fixtures, and edge cases. Cover regressions in behavior that must remain unchanged. Include manual verification when automated tests are insufficient.

### 6. Validation Commands

Inspect repository package/configuration files and provide exact applicable commands for formatting, linting, type-checking, unit and integration tests, builds, and project-specific validation. Do not invent commands; explicitly identify validation gaps.

### 7. Risk Review

Identify likely failure modes, tricky parts, compatibility and migration risks, performance and security concerns, and UX pitfalls. Explain how the plan avoids or mitigates each.

### 8. Rollback or Recovery Notes

Explain safe reversal or recovery, including relevant data migrations, generated files, caches, and deployment concerns.

### 9. Final Execution Checklist

Provide a concise completion checklist covering code changes, tests, validation commands, and manual checks.

### 10. Open Questions

Include this section when requirements remain unresolved. State each question, why the available evidence cannot resolve it, and the decision needed to unblock affected steps.

## Constraints

- Plan only; do not implement or skip necessary steps.
- Use no vague placeholders such as "TBD", "etc.", "as needed", or "handle appropriately". Explicit open questions are not placeholders for omitted planning.
- Prefer the smallest correct change that fits the codebase.
- Preserve existing conventions unless a clear, stated reason justifies changing them.
