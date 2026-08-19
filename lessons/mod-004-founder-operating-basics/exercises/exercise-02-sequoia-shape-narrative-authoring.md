---
module: mod-004-founder-operating-basics
exercise: exercise-02
slug: sequoia-shape-narrative-authoring
hours: 3
prereqs: [chapter-05-the-founder-narrative-sequoia]
---

# Exercise 02 — Sequoia-Shape Narrative Authoring

## Problem statement

Chapter 05 installed the ten-part Sequoia-shape narrative and the
four-audience re-frame. This exercise is where you write the
narrative for a real (or realistically-specified) startup, then
derive at least two of the four audience re-frames from it.

The exercise is deliberately memo-first: you will write the
underlying narrative as a memo, not as a deck. Chapter 05's
primary claim — the memo is the source, the deck is the derivative
— is the discipline this exercise is training.

## Requirements

### Part A — pick the startup and read the primary source (about 15 min)

Pick a **real or realistically-specified startup** at PRE-SEED or
SEED. Same three options as exercise 01: your own, one you
advise, or a well-specified hypothetical you construct. Anonymise
detail if needed.

Before writing, **read the Sequoia Capital "Writing a Business
Plan" template** (see `resources.md`). The template is short —
under 30 minutes to read. This exercise is scaffolded on the
primary source, not on chapter 05 alone.

### Part B — write the ten-part memo (about 90 min)

Write the narrative as a **memo**, one paragraph per part, in
prose. Total length: 800–1500 words. All ten parts, in order:

1. **Company purpose.** One sentence.
2. **Problem.** One paragraph in the customer's language.
3. **Solution.** One paragraph on the mechanism.
4. **Why now.** One paragraph on the specific enabling change.
5. **Market size.** One paragraph, bottom-up preferred.
6. **Competition.** One paragraph, including do-nothing and
   internal-build alternatives.
7. **Product.** One paragraph, ideally with evidence.
8. **Business model.** One paragraph on who pays, how much, on
   what cadence.
9. **Team.** One paragraph on why *these* people, plus what's
   missing.
10. **Financials.** One paragraph on current numbers and forward
    plan.

Discipline checks:
- **Purpose sentence describes the company, not the product.** If
  a pivot in the product wouldn't invalidate the purpose sentence,
  you're at the right level.
- **Problem is in the customer's language.** A specific target
  customer would recognise their own life in the sentence.
- **Why-now is a specific enabling change**, not a trend.
- **Market-size includes bottom-up**, not just top-down.
- **Competition includes do-nothing.**
- **Team is problem-fit, not resume dump.** Answer the "why these
  people for this problem?" question specifically.

### Part C — derive two audience re-frames (about 60 min)

Pick **two of the four re-frames** from chapter 05:

- The co-founder re-frame.
- The first-employee re-frame.
- The first-customer re-frame.
- The first-investor re-frame.

For each of the two you picked, produce a **half-page re-frame
memo** that:

- Keeps all ten parts of the narrative (do not drop any).
- Re-weights the depth per chapter 05's audience-emphasis table
  (the co-founder wants purpose/problem/solution/why-now/team
  deep; the first employee wants purpose/solution/product/team;
  the first customer wants problem/solution/product/business
  model; the first investor wants why-now/market-size/competition/business
  model/financials).
- Adds the *unique element* chapter 05 specified for that
  audience:
  - **Co-founder**: radical honesty about the gap between what
    is true today and what the narrative claims.
  - **First employee**: a concrete day-one-to-day-ninety picture.
  - **First customer**: evidence the product does what it claims
    (a demo, a case study, a data table, references).
  - **First investor**: the chain from market → current growth →
    KR set → runway math (may reference mod-005 founder-numbers).
- Fits in half a page (400–600 words).

Discipline check: **the two re-frames should not contradict each
other.** If your investor re-frame implies a company that a
customer wouldn't recognise from your customer re-frame, one of
the two has drifted from the underlying memo — fix the memo, not
just one re-frame.

### Part D — the two-minute verbal (about 15 min)

Compress the ten-part memo into a **two-minute verbal script** —
one sentence per part, ten sentences total. Rehearse it. If you
can, read it into a recorder or to a live person. Note where you
stumbled and update the memo if the stumble reveals a gap in the
underlying content (that is exactly what the two-minute verbal is
for).

Include the final two-minute script in the deliverable.

## Deliverable shape

A single Markdown file, `mod-004-exercise-02-sequoia-narrative.md`,
structured:

```markdown
# Sequoia-Shape Narrative — <Startup Name>

## Context
<one paragraph: startup, stage, target audience for the primary memo>

## Part 1 — the ten-part memo
### 1. Company purpose
<paragraph>
### 2. Problem
<paragraph>
### 3. Solution
<paragraph>
### 4. Why now
<paragraph>
### 5. Market size
<paragraph>
### 6. Competition
<paragraph>
### 7. Product
<paragraph>
### 8. Business model
<paragraph>
### 9. Team
<paragraph>
### 10. Financials
<paragraph>

## Part 2 — audience re-frame 1: <chosen audience>
<half-page re-frame with the audience-specific unique element>

## Part 3 — audience re-frame 2: <chosen audience>
<half-page re-frame with the audience-specific unique element>

## Part 4 — two-minute verbal
1. <sentence>
2. <sentence>
...
10. <sentence>

## Notes on the exercise
<one paragraph: what the memo-first vs. deck-first ordering
surfaced; where the two-minute rehearsal caught a gap; which
re-frame was hardest and why>
```

Total length: 1600–2400 words.

## Starter guidance

- **Write in order.** The ten parts are ordered on purpose
  (chapter 05, "why this shape"). Writing part 5 before part 4 is
  fine as a first pass; make sure the final version reads
  sequentially and each part earns its predecessor.
- **Use the customer's exact language for the problem section.**
  If you have real customer transcripts, quote them. If not, name
  a specific target customer and imagine reading the problem
  paragraph back to them; would they say "yes, that's what my
  life is like"?
- **Make the why-now specific enough to be wrong.** A why-now
  paragraph that names no specific enabling change is untestable
  and therefore useless.
- **Bottom-up market-size math beats top-down.** Even a rough
  bottom-up ("N customers × $M annual spend = $X market")
  outperforms a top-down ("$50B TAM per [analyst]") for the
  audiences this exercise cares about.
- **Do not open a deck template.** Chapter 05 was explicit: memo
  first, deck later. This exercise deliberately doesn't produce
  slides.
- **Read the Sequoia primary source.** The chapter is scaffolding
  for the primary reference, not a substitute. The primary source
  is short.

## Acceptance criteria

You have completed the exercise when:

- [ ] The ten-part memo is present, one paragraph per part, in
      the specified order, 800–1500 words total.
- [ ] Purpose sentence describes the company (not the product);
      problem uses the customer's language; why-now names a
      specific enabling change; market size includes bottom-up;
      competition includes do-nothing; team is problem-fit not
      resume dump.
- [ ] Two of the four audience re-frames are present, each
      keeping all ten parts, each 400–600 words, each including
      the audience-specific unique element from chapter 05.
- [ ] The two re-frames are internally consistent — they do not
      contradict each other on any substantive detail.
- [ ] A two-minute verbal script is present, one sentence per
      part, ten sentences total.
- [ ] A short "notes on the exercise" paragraph reflects on
      memo-first vs. deck-first, on the rehearsal, and on which
      re-frame was hardest.
- [ ] The primary Sequoia source is cited in `resources.md` form.
- [ ] The file is committed to your notes as
      `mod-004-exercise-02-sequoia-narrative.md`.

## Common failure modes to avoid

- **Marketing prose.** The memo is not a landing page. Use
  founder-honest language; avoid superlatives ("world-class,"
  "revolutionary," "seamless"). If a sentence would fit on a
  homepage, cut its adjectives.
- **Product = purpose.** The single most common shape error is
  writing the purpose sentence to describe the current product.
  Chapter 05 flagged this specifically; catch it before submitting.
- **Trend as why-now.** "AI is everywhere" is not a why-now.
  "Model inference cost dropped 90% between 2023 and 2026 and
  now sits below the threshold where our product's unit economics
  work at $20/month" is a why-now.
- **Team as bios.** Names, titles, and where people used to work
  is a slide-appendix. The team section is *why these people for
  this problem*.
- **Re-frames that lose parts.** All ten parts appear in each
  re-frame, at some depth. Dropping parts breaks the same-story
  property that makes the four re-frames coherent.

## What good looks like

A memo that, if handed to (a) a candidate co-founder, (b) a
candidate first employee, (c) a candidate first customer, and
(d) a candidate first investor, each of the four would recognise
as *the same underlying startup*, even though each of the four
audience re-frames emphasises different parts.

The strongest signal that you have the shape right is when the
two-minute verbal reads out loud without stumbling on any part.
Stumbles are where the underlying content is thin, not where the
sentence structure is bad; rewrite the memo paragraph until the
two-minute-verbal sentence for that part flows naturally.

The narrative you author here is the raw material for exercise
06 (`First Investor-Update Template`) — the investor re-frame
becomes the underlying story the update is written against. It
is also the raw material for chapter 05's future consequences
(pitch deck, marketing site, sales narrative) — none of which
this module authors, all of which will read cleanly once the
memo is right.
