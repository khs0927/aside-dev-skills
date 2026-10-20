---
name: "dev-design-frontend"
description: "Use for UI, frontend, landing pages, dashboards, games, 3D, Figma-to-code, or design system work."
---
# Dev Design Frontend

Build repeatable, accessible, performant interfaces instead of one-off chat output.

## Workflow

1. Define screen goal, user, device, and design direction in one paragraph.
2. Select reusable pattern: layout, component, game system, or Figma mapping.
3. Implement with semantic HTML, responsive layout, and accessible states.
4. Add loading, empty, error, and mobile states by default.
5. Verify visually: check spacing, contrast, focus order, and main viewport sizes.
6. Optimize: limit dependencies, compress assets, avoid blocking resources.

## Decision rules

- Prefer design-system components over custom one-off styles.
- Prefer copy-pasteable snippets with guardrails over abstract advice.
- For Figma work: fetch node context first, map to code components, keep 1:1 fidelity.
- For Three.js/games: fix camera, controls, performance budget, and QA checklist before polish.
- Never use shadows or Mermaid placeholders as final design output.

## Examples

- "Build a dashboard": define cards, charts, filters, then implement responsive grid.
- "Figma to code": list screens, map components, implement with matching tokens.
- "Mobile Three.js game": set performance budget, controls, audio/VFX feedback, QA pass.

## References reviewed

- MengTo/Skills designer and builder workflows for UI, games, and frontend systems.
- Figma official agent skills for design-system and code implementation.
- Google Stitch design-md and enhance-prompt patterns for UI vocabulary.



























