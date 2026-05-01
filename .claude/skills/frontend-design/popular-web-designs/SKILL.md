---
name: popular-web-designs
description: >-
  Use contemporary web design references as inspiration while avoiding one-note visual trends.
---

# Skill: popular-web-designs

## Purpose
Use contemporary web design references as inspiration while avoiding one-note visual trends. Treat this as a narrow pattern card: use it to sharpen one decision surface quickly, then hand back to the broader workflow.

## Use When
- The active question is primarily about: use contemporary web design references as inspiration while avoiding one-note visual trends.
- A broader skill exists, but the current question is narrow enough for a fast focused review.
- You want a reusable checklist before implementation, review, or escalation continues.

## Do Not Use When
- The task needs an end-to-end workflow or multi-step implementation chain. Use `frontend-design`.
- The main risk has shifted to an adjacent concern outside this card. Use `design-review`.
- The user only wants generic best practices with no repo, product, or workflow context.

## Focus Checklist
1. Ground use contemporary web design references as inspiration while avoiding one-note visual trends in user task, readability, and responsive behavior instead of visual trend-chasing.
2. Call out contrast, motion, density, and performance constraints explicitly.
3. Tie the recommendation to one measurable UX or CRO outcome.
4. Escalate to `frontend-design` if the work turns into a full product design pass instead of a narrow style decision.

## Evidence To Collect
- current UI state or screenshots
- one proposed visual direction with known tradeoffs
- the browser or accessibility check that would validate it

## Related Skills
- Primary broader workflow: `frontend-design`
- Adjacent boundary: `design-review`
- This card stays active only while its narrow scope remains smaller than those broader lanes.

## Group
Product Design And QA

## Output Contract
```markdown
## Decision
- [recommended pattern, constraint, or next move]

## Risks
- [main failure or tradeoff]

## Evidence
- [files, commands, examples, metrics, or assumptions]

## Next Step
- [implement, escalate, or stop]
```
