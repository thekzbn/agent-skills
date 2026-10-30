---
name: project-feature-work
version: 1.0.0
description: Use when implementing a feature or substantial change in an existing project. Inspect the current code and project instructions, preserve useful behaviour and architecture, and keep the work within the requested scope.
---

# project-feature-work

Use this skill to carry a requested change through an established project without losing the decisions and working behaviour already there.

Before changing code

- Read the repository instructions and inspect the implementation around the requested change. Check related routes, components, data flows, and tests where relevant.
- Identify existing patterns and use them unless the task calls for a change or there is a concrete problem to solve.
- Separate the requested outcome from suggestions, future ideas, and explicit exclusions. A discussion request is not permission to implement.

Implementation

- Make the smallest coherent change that fulfils the requested outcome. Preserve unrelated behaviour and avoid adding features, dependencies, abstractions, or redesigns without a clear need.
- Follow the project’s terminology, visual language, architecture, and conventions. For interface work, use the `think` skill when available.
- Carry changes through connected parts of the product when the feature requires it, such as navigation, persistence, settings, empty and error states, documentation, or version references. Do not update unrelated files just because they are nearby.
- For user-facing copy or substantial prose, follow the `speak` skill when available. Keep product-specific terminology and explicit project writing rules.
- If an assumption could change the product direction or data behaviour, surface it before relying on it. Otherwise make a reasonable, reversible choice and continue.

Before handing back

- Review the diff for scope, consistency, and accidental changes.
- Run checks only when requested or required by the task instructions. Report what changed and what was actually verified; do not imply checks passed if they were not run.
