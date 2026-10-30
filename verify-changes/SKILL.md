---
name: verify-changes
version: 1.0.0
description: Use when the user asks to test, verify, or confirm a change, or explicitly makes verification part of the requested deliverable. Choose checks that cover the affected behaviour and report their limits accurately.
---

# verify-changes

Verify the requested outcome using the project’s existing tools and the checks appropriate to the change.

- Inspect project instructions and available scripts before choosing commands. Prefer existing typechecks, builds, tests, linters, and supported manual flows over adding new test infrastructure.
- Do not add or run tests unless the user or applicable project instructions ask for testing. A request to implement alone does not imply permission to run tests.
- Match each check to a concrete claim. A successful build does not prove that a user flow works; a manual check does not prove every code path is covered.
- When UI verification is requested, check the affected flow and relevant states at realistic sizes and inputs if the environment permits.
- If a check fails, investigate failures caused by the change and fix them when in scope. Clearly separate pre-existing failures, environment blockers, and unresolved issues.
- Report the exact checks run and the result. Do not claim complete verification when some states or environments were not covered.
