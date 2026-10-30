---
name: ux-review-and-fix
version: 1.0.0
description: Use when reviewing a product flow for usability problems or fixing UX issues. Explain what the user experiences, why the implementation behaves that way, and make only the changes the user requested or accepted.
---

# ux-review-and-fix

Review the specified flow in the context of the existing product. Keep the review focused on user tasks and observable behaviour, not personal taste.

Review

- Inspect the relevant screen, code path, and neighbouring patterns before judging the interaction.
- Trace what happens in the states that matter, including loading, empty, error, success, keyboard, and narrow-screen states when applicable.
- For each actionable issue, explain both the technical cause and the effect on the person using the product. Distinguish confirmed defects from design recommendations and uncertain hypotheses.
- Prioritise issues by how they block or confuse the user. Avoid broad redesign proposals when a focused fix addresses the problem.

Changes

- If the user asked for a review only, report findings without editing. If they asked for fixes or accepted the findings, correct the relevant issues while preserving working behaviour and the established design language.
- Use the `think` skill for interface decisions and the `speak` skill for user-facing text when available.
- Do not introduce a new feature or alter unrelated flows as part of a UX fix.
- Verify the affected interaction when requested and when the environment permits. State what you checked and any remaining uncertainty.
