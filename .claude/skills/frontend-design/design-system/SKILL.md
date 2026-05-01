---
name: design-system
description: >-
  Define or critique a project-appropriate design system with palette, typography, component, and anti-pattern rules.
---

# Skill: design-system

## Purpose
Turn vague visual direction into a repeatable system a maintainer can actually use.

## Use When
- A project needs a visual language before UI implementation scales.
- A UI already exists but tokens, typography, or components feel inconsistent.
- The user wants a stronger look without collapsing into generic template aesthetics.

## System Contract
1. Define the brand mood and the product contexts it must serve.
2. Choose a palette with semantic roles, not just raw colors.
3. Define typography, density, spacing rhythm, and corner/motion preferences.
4. Identify canonical components and the states each one must support.
5. List visual anti-patterns that should be rejected during implementation.

## Required Outputs
- palette tokens with intended roles
- typography stack and usage hierarchy
- spacing and layout rhythm
- component state rules
- anti-pattern list tied to this repo's aesthetic direction

## Evidence And Reuse
- Reuse existing style guides or CSS variables when the project already has them.
- If the repo is greenfield, produce a small system that can be implemented directly.
- Point to `frontend-design` references when deeper visual QA guidance is needed.

## Output Requirements
```markdown
## System Direction
- [mood, constraints, target surfaces]

## Tokens
- [palette, typography, spacing, motion]

## Components
- [canonical components and required states]

## Anti-Patterns
- [what must not happen]

## Adoption Notes
- [how this system should be applied incrementally]
```

## Group
Product Design And QA
