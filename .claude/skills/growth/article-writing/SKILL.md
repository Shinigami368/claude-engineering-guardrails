---
name: article-writing
description: Produce long-form written content — articles, guides, tutorials, essays, newsletter issues — in a voice derived from supplied examples or brand references. Use when the user wants polished prose longer than a paragraph and cares about voice consistency, structure, and evidence.
---

# article-writing

Default AI long-form reads like a landing page. This skill is about making it sound like a person who actually knows the thing.

## Activation signals

- Blog post, essay, launch post, guide, tutorial, newsletter issue.
- "Turn these notes / this transcript / this research into an article."
- Voice-matching against an existing founder, operator, or brand.
- Tightening an already-written draft (pacing, evidence, structure).

## The five rules

1. **Concrete first.** Lead the section with an example, number, screenshot, code block, or anecdote. Never with a thesis statement.
2. **Explanation follows evidence**, not the other way around. The reader needs a reason to keep reading.
3. **Short sentences beat padded ones.** If a sentence has two clauses doing the same job, cut one.
4. **Cite specific numbers** when they exist and are sourced. Round numbers ("millions of users") are a trust leak.
5. **Never invent** biography, metrics, customer quotes, or outcomes. If a fact isn't supplied, ask or omit.

## Voice capture

If the user wants a specific voice, ask for samples. Any of:

- Published articles or posts.
- Past newsletters.
- X / LinkedIn writing.
- Internal memos or docs.
- A short style guide, if one exists.

Extract, in this order:

- **Rhythm** — typical sentence length, variance, paragraph size.
- **Register** — formal, conversational, operator-dry, irreverent.
- **Devices** — parentheticals, lists, fragments, rhetorical questions, em-dashes.
- **Opinion tolerance** — does this writer argue, hedge, or narrate?
- **Formatting habits** — headers, bullets, code blocks, pull quotes, inline callouts.

No samples provided → default to a direct, operator-style voice: concrete, practical, low on hype, comfortable with a one-sentence paragraph.

## Patterns to delete on sight

- "In today's rapidly evolving landscape…" and its cousins.
- "Moreover", "Furthermore", "In conclusion" — filler transitions.
- Hype adjectives: "revolutionary", "game-changing", "cutting-edge", "seamless".
- Claims without evidence — "studies show", "customers love".
- Credibility language not backed by supplied context ("as an expert in…").

If you catch yourself writing any of these, the sentence below is probably weak too. Rewrite the whole beat.

## Draft process

1. Nail down audience and purpose in one line each.
2. Sketch an outline — one clear job per section.
3. Open each section with evidence, example, or scene.
4. Expand only where the next sentence adds something the previous one didn't.
5. Kill templated or self-congratulatory sentences without mercy.

## Structure by format

### Technical guide
- Lead with the outcome the reader gets.
- Every major section has a code block, command, or concrete artifact.
- Close with takeaways, not a summary.

### Essay / opinion piece
- Open with tension, contradiction, or a sharp observation.
- One argument per section — don't stack theses.
- Earn opinions with examples, not assertions.

### Newsletter
- First screen does the heavy lifting — hook, framing, payoff.
- Mix insight with updates; skip diary filler.
- Section labels should be skimmable in 3 seconds.

## Output format

Return work in this shape:

### Article plan
- Audience
- Purpose
- Working title
- Section outline with one job per section
- Any source gaps or facts that still need confirmation

### Draft
- Full draft in the requested voice and format
- Headings, bullets, code blocks, or callouts only where they help readability

### Notes
- Voice or structure choices that matter
- Claims omitted because evidence was missing
- Optional alternate title or hook if the user is exploring directions

## Delivery gate

- [ ] Every factual claim has a source the user provided.
- [ ] No filler transitions or hype adjectives survived the last pass.
- [ ] Voice holds up against the reference samples (re-read one sample, then the draft).
- [ ] Every section earns its existence — no "for completeness" padding.
- [ ] Formatting fits the destination platform (Substack ≠ Medium ≠ personal site).
