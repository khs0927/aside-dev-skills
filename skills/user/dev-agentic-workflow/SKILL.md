---
name: "dev-agentic-workflow"
description: "Use for designing GitHub agentic workflows, multi-agent orchestration, MCP tool routing, automation playbooks, or agent eval gates."
---
# Dev Agentic Workflow

Automate repository and agent work with reasoning tasks guarded by safe outputs.

## Workflow

1. Decide deterministic vs agentic: use Actions scripts for fixed steps, agents for reasoning.
2. Define Markdown workflow with frontmatter: triggers, permissions, engine, tools.
3. Keep agent job read-only and sandboxed by default.
4. Route writes through validated safe-outputs with scoped permissions.
5. Compile and validate: gh aw compile, review generated lock file, then commit both files.
6. Add eval gate: issue triage accuracy, CI-fix success, docs freshness, or custom score.
7. Require human review for merges and permission changes.

## Decision rules

- Complement CI/CD; do not replace deterministic builds and tests.
- Least privilege first: expand network, tools, or write scope only with justification.
- One workflow does one job: triage, CI analysis, reporting, docs sync, or coverage.
- Log reasoning trace for ontology, triage, and investigation tasks.
- Review permissions, tools, and generated files before every deployment.

## Examples

- "Triage issues": label by type and priority, open ready-to-review comment.
- "Investigate CI failure": fetch logs, propose fix PR, keep original logs linked.
- "Daily repo report": summarize activity, risks, and next actions concisely.

## References reviewed

- github/gh-aw agentic workflow compile and safe-outputs architecture.
- GitHub Agentic Workflows docs for triggers, engines, and guardrails.
- CrewAI multi-agent roles and Semantic Kernel planner patterns.
- MCP server routing and tool-use workflow recipes.





























