---
module: mod-002-the-dependency-graph
exercise: exercise-02
slug: graph-tour-corporate-structure-branch
hours: 2
prereqs: [chapter-01-the-graph-as-the-foundations-instrument, chapter-03-corporate-structure-branch]
---

# Exercise 02 — Graph Tour: Corporate-Structure Branch

## Problem statement

Chapter 03 walked the corporate-structure branch — Incorporation → Equity /
Governance / Fundraising → Exit — and argued that the equity structure and
the governance structure gate every future round. This exercise makes you
prove you understand *why* the gating is real (not paranoia), by working
concrete failure scenarios and walking a synthetic diligence checklist.

You will (a) reconstruct the branch as a fan-out with its cross-branch
edges, (b) write short "what breaks" scenarios for four specific neglect
patterns, and (c) run a synthetic pre-Series-A diligence checklist that
covers each corporate-structure node.

## Requirements

### Part A — the branch, drawn

Draw the corporate-structure branch as an ASCII diagram in a fenced code
block. Include:

- The fan-out from Incorporation.
- The convergent endpoint at Exit.
- **Any two cross-branch edges** into the customer-facing branch or the
  economics branch (from chapter 03's coupling section).

Below the diagram, write a **two-sentence justification** for each
cross-branch edge you drew — what the coupling actually is, in your own
words.

### Part B — four neglect scenarios

For each of the four scenarios below, write a **short scenario writeup**
(4–6 sentences) covering:

- What the founder did (or didn't do) at the upstream node.
- What surfaces at the downstream gate (usually a round or an exit).
- What the fix looks like *at that late moment* — including who has to
  approve it and roughly how expensive the fix is compared to doing it
  right originally.

**Scenario 1 — the wrong entity.** A team incorporated as an LLC eighteen
months ago because it was simpler; now a lead investor has offered a
priced Series A term sheet.

**Scenario 2 — the missing consents.** A seed-stage founder issued
option grants informally, without formal board consents, for eighteen
months. A Series A lead's counsel begins diligence.

**Scenario 3 — the promised equity that isn't on the cap table.** A
founder made verbal equity commitments to two early advisors, never
documented, never issued. One advisor is now asking for the shares in
writing during Series A closing.

**Scenario 4 — the untracked SAFE stack.** A pre-seed round was raised
on 14 SAFEs at varying caps and discounts over 18 months, tracked in a
spreadsheet that has drifted from reality. A priced Series A begins,
and the pre-money dilution math must be reconstructed.

For each scenario, cite (or `<!-- needs-research: ... -->` for later
verification) at least one public founder-writeup, law-firm blog post,
or investor essay that describes the pattern. Do not fabricate legal
outcomes; if you are unsure of the mechanics, mark them for research.

### Part C — synthetic pre-Series-A diligence checklist

Produce a **10–15 item checklist** an incoming Series-A investor's
counsel would run against the corporate-structure branch. The checklist
must include at least:

- 2 Incorporation items
- 4 Equity items
- 3 Governance items
- 2 Fundraising-history items

For each item, note the graph node it belongs to and — for the items
that would most commonly be missing at real seed-stage companies — mark
"[common gap]" so the reader sees which corners founders tend to
neglect.

The checklist is synthetic — you do not need to reproduce a real
firm's diligence template. But it should be plausible enough that a
first-time founder reading it would use it as a pre-round self-audit.

## Deliverable shape

A single Markdown file, `mod-002-exercise-02-corporate-structure-tour.md`,
structured:

```markdown
# Corporate-Structure Branch — Graph Tour

## Part A — Branch diagram + cross-branch edges
<fenced ASCII diagram>

### Cross-branch edges
- Edge 1: <name> — <two-sentence justification>
- Edge 2: <name> — <two-sentence justification>

## Part B — Four neglect scenarios
### Scenario 1 — Wrong entity
...

### Scenario 2 — Missing consents
...

### Scenario 3 — Promised equity that isn't on the cap table
...

### Scenario 4 — Untracked SAFE stack
...

## Part C — Synthetic pre-Series-A diligence checklist
| # | Item | Node | Common gap? |
|---|---|---|---|
| 1 | ... | Incorporation | |
...
```

## Starter guidance

- **The scenarios are not hypothetical horror stories.** All four
  patterns show up regularly in law-firm and investor writeups on
  early-stage diligence. If your scenario writeup feels dramatic,
  that is because the reality is dramatic; do not soften it.
- **Do not invent legal mechanics.** Use the specific vocabulary from
  chapter 03 (SAFEs, option pool, board consents, protective
  provisions, cap-table hygiene). Where you don't know the exact
  mechanic, write it in plain English and mark
  `<!-- needs-research: ... -->` — that is honest and lets a future
  reader fix it.
- **For Part C, think like an investor's counsel.** They are running
  a checklist against a container they are about to invest in. Their
  job is to find the corner cases. Your job is to imagine the
  checklist so a founder can self-audit *before* they land in front
  of that counsel.
- **The "common gap" flag is the founder-facing value.** Marking
  which items are typically missing is what turns your checklist
  from a compliance list into a pre-flight briefing.

## Acceptance criteria

You have completed the exercise when:

- [ ] Part A includes an ASCII diagram with the fan-out and the
      convergent Exit endpoint, plus at least two cross-branch edges
      each with a two-sentence justification.
- [ ] Part B has all four scenarios written with the required
      structure (what the founder did / what surfaces at the gate /
      what the fix looks like at that moment).
- [ ] Each scenario cites at least one real source or marks
      `<!-- needs-research: ... -->` with a specific search hint.
- [ ] Part C has 10–15 checklist items with node tagging and at
      least two "[common gap]" flags.
- [ ] The file is committed as
      `mod-002-exercise-02-corporate-structure-tour.md`.

## Common failure modes to avoid

- Writing Part B scenarios as generic "clean up your cap table
  earlier" advice. The exercise is about the specific mechanic —
  what has to happen, by whom, at the closing gate.
- Producing a Part C checklist that is only Equity items. The whole
  branch matters; a checklist that neglects Governance or
  Incorporation misses the most common preventable gaps.
- Inventing law-firm citations. If you don't have a source, mark
  `<!-- needs-research: ... -->` and move on.

## What good looks like

A completed tour a founder about to raise a Series A could use as
their **week-before-diligence self-audit**. Every corner of the
branch is checked, every common failure mode is named, and the fixes
that need to happen *now* (not at the closing table) are surfaced
before an investor's counsel finds them.
