---
name: frontend-design
description: Define a concrete frontend visual/UX contract before implementation planning.
argument-hint: "[project or page description]"
disable-model-invocation: false
---

# Skill: frontend-design

## Purpose
Produce a clear visual/UX contract that implementation workflows can execute without ambiguity.

## Trigger Conditions
Use this skill when:
- UI direction or visual system decisions are needed
- a page/app requires design decisions before build planning
- output quality must exceed boilerplate UI patterns

## Input Boundary
This skill accepts:
- product goal, audience, brand constraints
- required screens/flows
- device priorities and constraints

## Output Boundary
This skill produces:
- visual direction and style rules
- design tokens: typography, color, spacing, radius, shadows
- component state behavior spec
- responsive behavior spec
- design QA checklist

## This Skill Does Not
- produce implementation task plans
- define SEO/performance budgets
- choose framework architecture
- define backend/API contracts

## Step Order (Mandatory)
1. Extract objective, audience, and constraints.
2. Define visual direction (tone, references, anti-patterns).
3. Define design tokens with explicit values.
4. Define component state matrix: default/hover/focus/active/disabled/error/loading.
5. Define mobile/tablet/desktop behavior explicitly.
6. Define layout-stability constraints for dynamic content, long labels, and fixed-format UI.
7. Produce design QA checklist and handoff notes.

## Quality Gates (Non-skippable)
1. Specificity gate: no vague adjectives without token values.
2. Consistency gate: all components inherit the same token system.
3. Accessibility gate: focus-visible and non-color-only status signaling are defined.
4. Responsive gate: mobile-first behavior and 3 breakpoints are explicit.

## Hard Rules
1. No vague adjectives ("modern", "clean", "premium") without token-level definition.
2. Every interactive element must define focus treatment.
3. Color cannot be the only status signal.
4. Touch targets must be considered in mobile behavior.
5. Mobile-first behavior must be explicit.
6. Fixed-format controls, cards, grids, and toolbars must define stable dimensions or wrapping behavior.

## Coordination With Other Skills
If `website-build` is also active:
1. Run `frontend-design` first.
2. Hand off tokens + states + responsive rules.
3. `website-build` implements these constraints and cannot redefine them silently.

## References
- Boundary contract: `references/scope-contract.md`
- Quality checklist: `references/quality-checklist.md`

## Dry-Run Scenarios (required before claiming final quality)
1. Landing page: hero, social proof, pricing, CTA hierarchy.
2. Dashboard: dense data cards, table states, filter controls.
3. Content-heavy site: typography rhythm, reading width, toc behavior.

## Output Format
1. Visual Direction
2. Design Tokens
3. Component States
4. Responsive Rules
5. Layout Stability Rules
6. Design QA Checklist
7. Handoff Notes

## Learnings
- Design quality improves when tokens and state behavior are decided before layout polishing.
