Do not write or modify code yet.
Your task is to produce a complete, highly detailed, step-by-step implementation plan for the requested change.
This plan will be executed later by a less capable coding model, so it must be explicit enough that a careful junior developer could follow it without needing to infer missing steps, make architectural decisions, or ask follow-up questions.
Before writing the plan:
1. Carefully inspect and understand the existing codebase, architecture, conventions, naming patterns, data flow, tests, and related files.
2. Identify all files, functions, components, APIs, types, configuration, tests, and documentation that may need to be created or changed.
3. Resolve ambiguity by making reasonable, codebase-consistent decisions. If a requirement is truly impossible to resolve from the codebase, call it out clearly under “Open Questions” instead of leaving it implicit.
The implementation plan must include:
1. Objective
   - State the exact goal of the change.
   - Describe the expected user-visible or developer-visible behavior after completion.
2. Current-State Analysis
   - Explain how the relevant existing code works today.
   - List the important files, modules, functions, components, routes, types, database tables, configs, or tests involved.
   - Mention any existing patterns that must be followed.
3. Desired End State
   - Describe the final architecture and behavior after the change.
   - Specify any new files, functions, types, components, endpoints, database changes, environment variables, or configuration.
4. Implementation Steps
   - Provide a numbered sequence of small, concrete steps.
   - Each step must say exactly what to change, where to change it, and why.
   - Include expected names for new functions, variables, files, types, routes, tests, and constants where applicable.
   - Include important edge cases and error-handling behavior.
   - Include any ordering constraints between steps.
   - Avoid vague instructions such as “update the logic” or “handle errors”; spell out the intended logic.
5. Testing Plan
   - List all tests that should be added or updated.
   - Specify test files, test cases, inputs, expected outputs, mocks, fixtures, and edge cases.
   - Include regression tests for existing behavior that must not break.
   - Include manual verification steps if automated tests are not sufficient.
6. Validation Commands
   - Provide the exact commands to run for formatting, linting, type-checking, unit tests, integration tests, builds, or other project-specific validation.
   - If the correct commands must be discovered from the repo, inspect package/config files and choose the appropriate commands.
7. Risk Review
   - Identify likely failure modes, tricky parts, compatibility concerns, migration risks, performance concerns, security concerns, and UX pitfalls.
   - For each risk, explain how the implementation plan avoids or mitigates it.
8. Rollback or Recovery Notes
   - Explain how to safely revert or recover if the implementation causes issues.
   - Mention any data migrations, generated files, caches, or deployment concerns if relevant.
9. Final Execution Checklist
   - Provide a concise checklist the executing model can follow before considering the task complete.
   - The checklist must include code changes, tests, validation commands, and manual checks.
Constraints:
- Do not implement the code.
- Do not skip steps.
- Do not leave placeholders such as “TBD”, “etc.”, “as needed”, or “handle appropriately”.
- Prefer the smallest correct change that fits the existing codebase.
- Preserve existing conventions unless there is a clear reason not to.
- If multiple implementation approaches are possible, choose the best one and explain why; do not leave the choice to the executing model.
- Be specific enough that the implementation can be performed mechanically from the plan.
