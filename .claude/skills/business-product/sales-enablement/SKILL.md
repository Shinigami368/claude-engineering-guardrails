---
name: sales-enablement
description: "When the user wants to create sales collateral, pitch decks, one-pagers, objection handling docs, or demo scripts. Also use when the user mentions 'sales deck,' 'pitch deck,' 'one-pager,' 'leave-behind,' 'objection handling,' 'deal-specific ROI analysis,' 'demo script,' 'talk track,' 'sales playbook,' 'proposal template,' 'buyer persona card,' 'help my sales team,' 'sales materials,' or 'what should I give my sales reps.' Use this for any document or asset that helps a sales team close deals. For competitor comparison pages and battle cards, see competitor-alternatives. For marketing website copy, see copywriting. For cold outreach emails, see cold-email."
---

# Skill: sales-enablement

## When To Activate

Use this skill when:
- the user needs sales collateral, pitch material, or rep-facing playbooks
- the task is a deck, one-pager, proposal, objection doc, demo script, or ROI
  narrative
- the user needs materials tailored to a buyer persona, funnel stage, or deal
  type
- the current sales assets are generic, hard to use, or disconnected from proof

Use `competitor-alternatives` for public comparison pages and `cold-email` for
outbound outreach copy.

## Context Prerequisites

- Check `.claude/product-marketing-context.md` first if it exists.
- Clarify:
  - sales motion
  - deal size
  - target persona
  - funnel stage
  - asset type
  - available proof points
  - current collateral gaps
- If the request is deal-specific, clarify the buyer, the use case, and the
  next step the asset needs to support.

Use the bundled references when deeper format guidance is needed:
- [references/deck-frameworks.md](references/deck-frameworks.md)
- [references/one-pager-templates.md](references/one-pager-templates.md)
- [references/objection-library.md](references/objection-library.md)
- [references/demo-scripts.md](references/demo-scripts.md)

## Discovery Questions

- What asset is needed:
  - sales deck
  - one-pager
  - objection doc
  - demo script
  - proposal
  - playbook
  - persona card
- Who will use it:
  - SDR
  - AE
  - founder
  - champion
  - prospect
- Which persona or buying role is it for?
- What stage of the funnel does it support?
- What proof, case studies, or ROI claims can actually be defended?
- What current materials exist, and why are they failing?

## Decision Framework

- Build for a specific buyer, stage, and use case rather than generic company
  messaging.
- Keep every asset scannable enough for a rep to use live.
- Tie product claims to business outcomes and evidence, not feature lists.
- Give each asset one clear job:
  - win a meeting
  - support a demo
  - answer objections
  - move a deal forward
- Match format to context:
  - deck for narrative selling
  - one-pager for fast follow-up
  - objection doc for call support
  - proposal for deal commitment
- Keep the final CTA explicit so the asset drives the next step instead of just
  informing.

## Output Structure

1. ENABLEMENT GOAL

State the asset type, target buyer, funnel stage, and desired next step.

2. MESSAGE AND PROOF

State the core value story, differentiators, objections to address, and the
proof allowed in the asset.

3. ASSET DRAFT

Provide the requested asset in the right format, such as:
- slide-by-slide outline
- one-pager copy
- objection table
- demo script
- proposal structure
- persona card

4. USAGE NOTES

State how sales should use the asset, where to customize it, and what should
never be claimed without stronger evidence.

## Honesty And Non-Goals

- Do not invent ROI numbers, customer proof, or competitor claims.
- Do not produce generic collateral that ignores buyer role or funnel stage.
- Do not turn internal sales assets into public comparison or website copy.
- Do not overload one asset with every possible objection or persona.
- Do not write enablement material that a rep cannot scan quickly under real
  selling conditions.

## References

- Deck frameworks: [references/deck-frameworks.md](references/deck-frameworks.md)
- One-pager templates: [references/one-pager-templates.md](references/one-pager-templates.md)
- Objection library: [references/objection-library.md](references/objection-library.md)
- Demo scripts: [references/demo-scripts.md](references/demo-scripts.md)

## Related Skills

- `product-marketing-context` for shared positioning and audience context
- `pricing-strategy` for pricing and packaging decisions
- `competitor-alternatives` for comparison and battle-card adjacent work
- `copywriting` for public-facing copy
- `cold-email` for outbound outreach
