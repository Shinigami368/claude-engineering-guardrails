---
name: accessibility
description: >-
  Review WCAG, keyboard, focus, contrast, motion, labels, and screen-reader behavior with evidence-first gates.
---

# Skill: accessibility

## Purpose
Review implemented or planned UI against practical accessibility gates before treating it as ready.

## Use When
- The user asks for accessibility review or remediation.
- A frontend flow already exists and needs browser-visible evidence.
- A design proposal mentions keyboard flow, focus management, screen-reader support, or motion.

## Required Inputs
1. Target pages, states, or components.
2. Platform scope: desktop, mobile, or both.
3. Whether the task is review-only or includes implementation follow-up.

## Review Gates
1. **Keyboard path**: primary actions, dialogs, forms, and menus must be reachable and dismissible without pointer-only interaction.
2. **Focus behavior**: visible focus state, sensible order, no focus traps unless intentionally modal.
3. **Semantics and labels**: buttons, links, fields, error states, headings, and landmarks must expose meaning.
4. **Contrast and readability**: text, disabled states, overlays, and decorative treatments must preserve legibility.
5. **Motion and timing**: animated transitions, auto-advancing UI, and reduced-motion behavior must be called out explicitly.
6. **State announcements**: loading, validation, success, and destructive confirmations should not be invisible to assistive tech users.

## Evidence Contract
- Prefer browser evidence over abstract advice when a UI already exists.
- Reuse `browser-audit` or local project tooling when it can capture screenshots, console noise, and viewport behavior.
- Separate confirmed defects from inferred risks.

## Output Requirements
```markdown
## Scope
- [pages, states, devices]

## Findings
- Severity: HIGH | MEDIUM | LOW
- Surface: [component or flow]
- Issue: [concrete accessibility defect]
- Fix direction: [minimal implementation direction]

## Evidence
- [screenshots, file paths, commands, browser steps]

## Residual Risks
- [items not verified directly]
```

## Group
Product Design And QA
