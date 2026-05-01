---
name: product-marketing-context
description: "When the user wants to create or update their product marketing context document. Also use when the user mentions 'product context,' 'marketing context,' 'set up context,' 'positioning,' 'who is my target audience,' 'describe my product,' 'ICP,' 'ideal customer profile,' or wants to avoid repeating foundational information across marketing tasks. Use this when the user wants a reusable shared context file for repeated marketing work — it creates an optional local `.claude/product-marketing-context.md` file in the user's own setup, which other skills can use when it exists."
---

# Skill: product-marketing-context

## When To Activate

Use this skill when:
- the user wants to create, audit, or update shared product-marketing context
- other GTM skills need a stable positioning and audience foundation first
- the user wants to avoid repeating product, audience, and messaging basics
- the task is to define ICP, positioning, differentiation, objections, or
  customer language in one reusable document

This skill owns the optional local foundation document at
`.claude/product-marketing-context.md`.

That file is generated or maintained in the user's own setup when they want
reusable context. It is not required for normal component copying and should
stay uncommitted by default.

## Context Prerequisites

- Check `.claude/product-marketing-context.md` first if it exists.
- If the current file does not exist, check legacy
  `.agents/product-marketing-context.md` only as migration source material.
- When auto-drafting, inspect the lightest useful repo evidence first:
  - README
  - landing-page copy
  - pricing page
  - about page
  - package metadata
  - existing docs
- Clarify whether the user wants to:
  - create the document
  - update specific sections
  - audit what already exists

## Discovery Questions

Capture only what materially changes the context:
- What does the product do, and what category does it belong to?
- Who buys it, who uses it, and who influences the decision?
- What problem drives customers to look for this solution?
- Which alternatives do they compare against?
- Why do customers choose this product instead?
- What objections, switching barriers, or trust gaps appear most often?
- What proof points, customer language, and goals are already known?

## Decision Framework

- Default to auto-drafting from repo evidence when no context exists, unless
  the user explicitly wants to start from scratch.
- Only write or update the file when the user wants reusable local context. For
  one-off work, return the context inline instead of assuming the file must
  exist.
- Reuse existing context and update only the sections that changed instead of
  rewriting the whole document every time.
- Capture verbatim customer language whenever available because downstream copy
  and sales work depend on it.
- Keep the document stable and field-oriented so other skills can reuse it
  predictably.
- Skip sections that genuinely do not apply instead of filling them with weak
  placeholders.
- Present the draft or proposed updates before writing when the content is
  inferred from partial evidence.

## Output Structure

Write or update `.claude/product-marketing-context.md` with these stable
sections:

1. Product Overview
2. Target Audience
3. Personas
4. Problems & Pain Points
5. Competitive Landscape
6. Differentiation
7. Objections & Anti-Personas
8. Switching Dynamics
9. Customer Language
10. Brand Voice
11. Proof Points
12. Goals

When updating an existing file:
- preserve confirmed sections that are still valid
- update only the sections affected by the new information
- refresh the date stamp if the document changes

## Honesty And Non-Goals

- Do not invent positioning, personas, proof points, or customer quotes.
- Do not overwrite an existing context document without confirming the intended
  scope of changes.
- Do not force every section onto products where it does not fit.
- Do not turn the file into a campaign brief, homepage draft, or market
  research memo.
- Do not keep using legacy `.agents` output paths as the active destination.

## Related Skills

- `market-research` for external category or competitor research
- `customer-research` for direct customer insight gathering
- `copywriting` for website and landing-page copy
- `sales-enablement` for buyer-facing collateral
- `pricing-strategy` for packaging and monetization decisions
