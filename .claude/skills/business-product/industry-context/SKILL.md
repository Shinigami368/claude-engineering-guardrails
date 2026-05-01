---
name: industry-context
description: "Foundation skill that captures the user's industry, business model, regulatory environment, and operational characteristics into an optional local `.claude/industry-context.md` file in the user's own setup. Use when the user mentions 'set up industry context,' 'define my industry,' 'industry profile,' 'we are a [industry] company,' 'regulatory requirements,' 'compliance needs,' 'our vertical,' or when other skills need industry-specific grounding. This is the non-SaaS counterpart to product-marketing-context."
---

# Skill: industry-context

## Purpose

Create or update optional local `.claude/industry-context.md` so downstream
skills can produce industry-aware outputs instead of defaulting to generic
assumptions.

## Trigger Conditions

Use this skill when:
- the user explicitly wants to create or update industry context
- another workflow needs industry grounding and `.claude/industry-context.md`
  does not exist yet
- the user describes their vertical, regulatory environment, or operational
  model in a way that other skills should preserve

This is a foundation-document workflow, not a broad research memo.
The file is user-owned local context, not a required repo file.

## Input Boundary

The user may provide:
- industry or sub-vertical
- business model
- company stage
- customer type
- regulatory environment
- operational model
- geographic scope
- key dependencies
- competitive landscape
- technology stack
- known pain points

Check existing context files first:
- `.claude/industry-context.md`
- `.claude/product-marketing-context.md`

## Step Order (Mandatory)

1. Check whether `.claude/industry-context.md` already exists.
2. If it exists, read it and determine whether the user wants to update or
   replace specific sections.
3. Reuse any valid industry signals from `.claude/product-marketing-context.md`
   before asking repetitive questions.
4. Gather all required fields:
   - industry or vertical
   - business model
   - company stage
   - customer type
5. Gather important context when available:
   - regulatory environment
   - operational model
   - key dependencies
   - geographic scope
   - competitive landscape
6. Draft the document in the stable repo format.
7. Present or confirm the proposed content before writing or overwriting it.
8. Update the date stamp whenever the document changes.

## Document Rules

- Keep the format stable because downstream skills read this file.
- Keep the content concise and field-oriented rather than narrative.
- Only write or update the file when the user wants reusable local context.
- Write only confirmed information.
- Mark optional sections only when the user actually provided them.

## Evidence Expectations

- State what was reused from existing context files.
- State which required fields were confirmed and which remain unknown.
- Keep regulatory or operational claims tied to user-provided information.
- Make it clear when a field is absent rather than inferring it.

## Non-Goals

- Do not invent industry, compliance, or competitive information.
- Do not overwrite an existing context file without confirmation.
- Do not turn the document into a full market research report.
- Do not destabilize the section layout that downstream skills depend on.

## Output Format

Write or update `.claude/industry-context.md` with this structure:

1. Industry Profile
2. Regulatory & Compliance
3. Operational Model
4. Competitive Landscape
5. Technology Stack
6. Industry Terminology
7. Known Pain Points

Only include the optional sections when the information exists.
