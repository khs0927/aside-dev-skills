---
name: "dev-coding-workflow"
description: "Use for any software coding task: new features, bug fixes, refactoring, API design, code review, testing, or production deployment."
---
# Dev Coding Workflow

Run disciplined production-grade coding: clarify, plan, build, verify, harden, ship.

## Workflow

1. Clarify goal, inputs, outputs, and non-goals. Restate in one paragraph before coding.
2. Break work into small steps with verification per step.
3. Inspect existing code and patterns first; follow repo conventions.
4. Write minimal code with explicit error handling and no secrets in code.
5. Verify: run relevant tests, lint, typecheck, or a smoke run. Report what passed.
6. Review for quality gates: readability, edge cases, performance, backwards compatibility.
7. Harden: validate inputs, handle auth, add prompt-injection and secret-leak guards for AI-facing code.
8. Ship: summarize files changed, tests run, and remaining risks.

## Decision rules

- Prefer reusing existing utilities over new dependencies.
- Prefer explicit types and small functions over clever abstractions.
- If requirements are ambiguous, ask one targeted question and proceed with stated assumption.
- If tests are missing, add a minimal regression test for the changed behavior.

## Examples

- "Add pagination to this API": clarify page-size defaults, implement, test first/empty/last page.
- "Fix login bug": reproduce, trace auth flow, fix, verify with valid/invalid/expired credentials.
- "Review this PR": check correctness, security, tests, then suggest concrete diffs.

## References reviewed

- VoltAgent/awesome-agent-skills collection pattern for portable skills.
- DevelopersGlobal/ai-agent-skills THINK-PLAN-BUILD-TEST-REVIEW-HARDEN-SHIP gates.
- anthropics/skills document and engineering skill structure.
- coderabbitai/skills code-review workflow.





























