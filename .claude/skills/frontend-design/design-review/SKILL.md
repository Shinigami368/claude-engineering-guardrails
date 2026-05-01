---
name: design-review
description: >-
  Audit implemented UI against layout, interaction, accessibility, and responsive quality gates with evidence.
---

# Skill: design-review

## Purpose
Review shipped or in-progress UI with a stricter bar than "looks okay."

## Use When
- A real interface exists and needs critique before or after implementation.
- The user asks for frontend polish, visual quality, or responsive review.
- You need to flag generic AI slop, layout instability, or inconsistent interaction patterns.

## Review Gates
1. **Hierarchy**: the primary action, reading path, and screen purpose should be obvious.
2. **Layout discipline**: spacing, alignment, and grouping should feel intentional rather than accidental.
3. **Interaction quality**: hover, focus, loading, empty, and error states should be coherent.
4. **Responsive stability**: mobile and desktop should preserve the same product story.
5. **Visual taste**: avoid default-stack, template-looking, or contradictory styling decisions.
6. **Accessibility crossover**: call out contrast, tap target, and keyboard/focus issues when visible.

## Evidence Contract
- Prefer screenshots and browser notes over general taste commentary.
- Name what is broken, what is merely weak, and what is intentionally acceptable.
- If a design system or existing site language exists, review against that language instead of inventing a new one.

## Output Requirements
```markdown
## Surface
- [page or component scope]

## Findings
- Severity: HIGH | MEDIUM | LOW
- Area: [layout, interaction, responsive, copy, accessibility]
- Issue: [concrete design problem]
- Fix direction: [smallest high-value adjustment]

## Strengths
- [what should be preserved]

## Evidence
- [screenshots, browser observations, file paths]
```

## Group
Product Design And QA
