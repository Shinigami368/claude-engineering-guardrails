---
name: website-build
description: Turn an approved frontend design contract into implementation-ready website architecture and delivery gates.
argument-hint: "[project or page description]"
disable-model-invocation: false
---

# Skill: website-build

## Purpose
Translate design intent into executable website build plans and acceptance gates.

## Trigger Conditions
Use this skill when:
- visual decisions exist and implementation planning is needed
- page architecture and component breakdown are required
- delivery quality needs explicit a11y/perf/SEO gates

## Input Boundary
This skill accepts:
- frontend design contract (tokens, states, responsive rules)
- feature/page requirements
- stack and runtime constraints

If design contract is missing:
- infer only a minimal provisional contract
- mark it clearly as `PROVISIONAL`
- keep it temporary and do not expand into full design exploration

## Output Boundary
This skill produces:
- information architecture (IA)
- page/section breakdown
- component contracts (template-defined)
- accessibility/performance/SEO gates
- engineering handoff checklist with acceptance criteria

## This Skill Does Not
- redefine design language unless hard constraints force a change
- perform pure art-direction exploration
- define backend domain/infrastructure architecture

## Step Order (Mandatory)
1. Validate design contract completeness.
2. Build IA: routes, page goals, navigation model.
3. Decompose pages into named sections and reusable components.
4. Write component contracts using the required template.
5. Define measurable accessibility/performance/SEO gates.
6. Define browser evidence preset for visual or responsive changes.
7. Produce phased handoff checklist with test-ready acceptance criteria.

## Quality Gates (Non-skippable)
1. Contract gate: every page maps to named sections; every section maps to named components.
2. Accessibility gate: keyboard support, focus states, semantics, and form errors are specified.
3. Performance gate: include LCP target, image strategy, loading strategy, and render strategy.
4. SEO gate: include title/meta rules, heading hierarchy, canonical/crawlability, and structured data plan.
5. Traceability gate: every acceptance criterion links to page + section + component.
6. Browser evidence gate: browser-visible changes name Quick, Standard, or Exhaustive `browser-audit` evidence.

## Hard Rules
1. Every page must map to named sections.
2. Every section must map to named components.
3. Every interactive component must define keyboard behavior.
4. Performance decisions must include image/loading/render strategy.
5. Any deviation from design contract must be explicitly justified with impact.

## Component Contract Template (Required)
For each component, provide:
1. `Name`
2. `Purpose`
3. `Used In` (page/section)
4. `Inputs` (props/data)
5. `States` (default/hover/focus/disabled/error/loading)
6. `Events` (user/system triggers)
7. `Accessibility` (role/label/keyboard/focus)
8. `Performance Notes` (lazy-load, memoization, render cost)
9. `SEO Notes` (if content-bearing)
10. `Acceptance Checks`

Acceptance checks must include the relevant `browser-audit` preset when visual, responsive, navigation, or content rendering behavior changes.

## Coordination With Other Skills
If `frontend-design` is active:
1. `frontend-design` runs first.
2. Import its tokens/states/responsive rules as fixed constraints.
3. Only propose deviations with explicit rationale + impact.

## References
- Boundary contract: `references/scope-contract.md`

## Dry-Run Scenarios (required before claiming final quality)
1. Landing page: conversion path + SEO metadata plan.
2. Dashboard: authenticated IA + stateful components + perf constraints.
3. Content-heavy site: taxonomy, navigation depth, and rendering strategy.

## Output Format
1. Input Validation Notes
2. Information Architecture
3. Page & Section Breakdown
4. Component Contracts
5. A11y/Performance/SEO Gates
6. Browser Evidence Plan
7. Handoff Checklist
8. Risks & Tradeoffs

## Learnings
- Build quality improves when component contracts and acceptance gates are explicit before coding.
