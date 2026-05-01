---
name: investor-materials
description: Produce and keep fundraising assets consistent — decks, one-pagers, memos, financial models, use-of-funds tables, milestone plans, accelerator answers. Use when numbers or claims must stay aligned across several documents a partner will read in sequence.
---

# investor-materials

Partners read the deck, then the memo, then the model. If the numbers disagree, the raise dies quietly. Every asset this skill produces must trace back to the same canonical set of facts.

## Activation signals

- Building or revising a pitch deck.
- One-pager, memo, or application for an accelerator.
- Financial model, milestone plan, use-of-funds table.
- Reconciling assets that drifted during the raise.

## The canonical facts ("source of truth")

Before drafting anything, lock down these values in one place (conversation, doc, or spreadsheet) and don't let them shift mid-session:

- Traction: MRR / ARR, active users, growth rate, retention cohort if relevant.
- Pricing and revenue assumptions (per-unit economics).
- Raise size, instrument (SAFE / priced / note), target valuation range.
- Use of funds — hiring, runway extension, GTM, infra.
- Team bios, titles, equity splits as relevant to the doc.
- Milestones with dates tied to spending.

If two inputs conflict — e.g., deck says $18k MRR, memo says $22k — **stop and resolve before drafting**. Don't ship until it's reconciled.

## Workflow

1. Inventory canonical facts (list what we know).
2. Flag missing assumptions the asset will need.
3. Pick the asset type and its template.
4. Draft with explicit logic — every number shows the step that produced it.
5. Cross-check final draft against the canonical list. Reconcile, don't paper over.

## Asset templates

### Pitch deck — suggested order

1. Company + wedge (what you do in one line)
2. Problem
3. Solution
4. Product / demo
5. Market (TAM / SAM / SOM with stated method)
6. Business model
7. Traction
8. Team
9. Competition and why you're different
10. The ask
11. Use of funds + milestones
12. Appendix (FAQs, deep metrics)

For a web-native or interactive deck, pair with the `frontend-slides` skill.

### One-pager / memo

- One clean sentence on what the company does.
- Why now (timing, tailwind, unlock).
- Traction and proof early, not at the bottom.
- A precise ask.
- No claim the reader can't verify within two minutes.

### Financial model

Must include:

- Assumptions visible on the top sheet, not buried.
- Bear / base / bull only when the decision hinges on the band.
- Revenue logic layered cleanly (volume × price × retention, etc.).
- Expenses tied to milestones, not flat plug numbers.
- Sensitivity analysis on the one or two assumptions that move the outcome.

### Accelerator / incubator applications

- Answer the exact question; don't paste deck copy.
- Prioritize traction, insight, and team edge.
- Keep metrics identical to the deck and model — reviewers read them side by side.

## Red flags — fix before shipping

- Unverifiable claims (no source, no footnote).
- Market sizing with no method (top-down handwave).
- Inconsistent titles or roles across docs.
- Revenue math that doesn't sum cleanly.
- Confidence calibrated higher than the evidence supports.

## Pre-delivery gate

- [ ] Every number matches the canonical list.
- [ ] Use of funds sums to raise size. Revenue layers sum to topline.
- [ ] Assumptions are readable without spelunking.
- [ ] No hype language. No adjectives doing a number's job.
- [ ] You could defend every slide under partner-meeting questioning.
