---
module: mod-003-stages-and-what-matters-when
exercise: exercise-03
slug: do-things-that-dont-scale-annotation
hours: 2
prereqs: [chapter-04-graham-do-things-that-dont-scale]
---

# Exercise 03 — `Do Things That Don't Scale` — Annotation

## Problem statement

Paul Graham's `Do Things That Don't Scale` (July 2013) is the canonical
IDEA / PRE-SEED reconciliation of the scalability demand in the mod-001
definition with the un-scalable hand-work the earliest stages require.
Every downstream module in this repo — and every pillar repo across the
org — assumes you have read it and internalised the argument.

This exercise makes sure you have.

You will read the essay in full, produce a structured annotation, extract
the load-bearing examples, argue with a specific claim, and connect the
argument to the stage-mismatch taxonomy from chapter 03 and the
premature-scaling framing from chapter 05.

## Requirements

### Part A — read the primary essay

Read Graham's essay in full. Do not rely on chapter 04 as a substitute
— that chapter is a scaffold, not a replacement. Source:
<https://paulgraham.com/ds.html>

### Part B — structured annotation

Produce a structured annotation in Markdown with the following sections.

**1. Thesis in one sentence.** State the essay's central claim in your
own words. If it takes more than one sentence, keep trying. The
one-sentence version is a discipline.

**2. Four load-bearing examples.** The essay's argument is
example-driven. Extract **four** of the concrete examples Graham uses
(Airbnb, Stripe, YC's own recruiting, Meraki, Pinterest, etc. — the
specific list is in the essay). For each:

- **Company and activity:** one line naming what the founders did.
- **Direct quote:** 2–3 sentences maximum, verbatim from the essay.
  Cite by paragraph number since the essay is unnumbered.
- **The un-scalable move:** one line naming what specifically was
  un-scalable about it.
- **What it produced:** one line naming what learning, evidence, or
  early usage the un-scalable move produced.

**3. Graham's three reasons the un-scalable work is right.** Chapter 04
paraphrased three reasons (per-user learning, cold-start breakout,
non-linear delight returns). Read the essay carefully and either
confirm or refine those three from the primary text. If Graham's
argument decomposes differently, name your decomposition and note
where it differs from chapter 04's.

**4. When the un-scalable work should end.** Graham says less about
this than about when to do the un-scalable work. Extract whatever the
essay says (or implies) about the transition — the signal that
un-scalable becomes scalable — and compare it against chapter 04's
list of transition signals (learning rate falling, founder throughput
becoming the bottleneck, un-scalable process stabilising, most of
the week on manual work).

### Part C — argue with a specific claim

In a section titled `Disagreements and caveats`, write **at least one
substantive disagreement** with a specific claim the essay makes.
Not with the overall thesis; with a specific claim. Steelman the
claim first (state the strongest version of what Graham means), then
argue with *that* version.

Common productive disagreements:

- The essay's examples lean heavily consumer / marketplace; some
  B2B or deep-tech cases have different un-scalable-work dynamics.
- The essay understates the risk of the un-scalable phase
  *becoming permanent* — chapter 03 shape-2 mismatch. Where does
  Graham address (or fail to address) the not-letting-go failure
  mode?
- The essay is written from a venture-batch perspective (YC
  companies with 3-month rhythm); the un-scalable work has
  different dynamics in a self-funded / longer-arc startup.
- The essay's "delight" argument depends on volume being low
  enough that hand-crafting is feasible; there are markets where
  the initial-user acquisition problem forces higher volume than
  Graham's cases assume.

### Part D — connect to chapters 03 and 05

Two short cross-references, one paragraph each.

**Cross-reference with chapter 03 (mismatch taxonomy).** Name the
mismatch shape (1, 2, or 3) that the essay is *most directly
warning against*. Then name the shape that the essay is *most at
risk of causing* if a founder over-applies it. (Hint: shape 2 is
the natural over-application failure mode.)

**Cross-reference with chapter 05 (premature scaling).** Name
which Startup Genome dimension(s) the un-scalable hand-work is
specifically *keeping consistent* — i.e., which dimensions would
race ahead if the founder replaced the hand-work with scalable
infrastructure too early.

## Deliverable shape

A single Markdown file, structured as above. Approximate lengths:

```markdown
# `Do Things That Don't Scale` — Annotated Read

## Thesis (one sentence)
<one sentence>

## Four load-bearing examples

### Example 1: <company>
- **Company and activity:** ...
- **Direct quote:** > ...
- **Location:** paragraph N
- **Un-scalable move:** ...
- **Produced:** ...

### Example 2: ...
...

## Graham's three reasons (or your revised decomposition)
1. ...
2. ...
3. ...

## When the un-scalable work should end
<one paragraph on what the essay says or implies, plus a diff against
chapter 04's transition signals>

## Disagreements and caveats

### Disagreement 1: <one-line label>
**Steelman:** <what Graham actually claims, in the strongest form>
<paragraph of push-back>

## Cross-reference with chapter 03 (mismatch taxonomy)
<paragraph>

## Cross-reference with chapter 05 (premature scaling)
<paragraph>
```

Total length: 800–1200 words.

## Starter guidance

- **Read once for surface, then once for annotation.** The examples
  are what carry the argument; you will miss the specifics on the
  first pass. Read cold, then read again with a pen.
- **Quote exactly.** Do not paraphrase inside quote marks. The
  discipline matters and citations in later mod-005 work will
  reference these quotes.
- **Steelman before you disagree.** A disagreement that
  misrepresents Graham's claim is worthless. State the strongest
  version of his claim first.
- **Do not read the essay as an argument for permanent manual
  work.** Chapter 04 was explicit that this is a common misread.
  If your annotation drifts toward "manual work is always the
  answer," you've mis-read it.
- **Prefer paragraph numbers to page numbers.** The essay is
  hosted as a web page and paragraph numbers are the reliable
  location reference. Count paragraphs from the start.

## Acceptance criteria

You have completed the exercise when:

- [ ] The primary essay has been read in full (not just chapter
      04).
- [ ] The one-sentence thesis is in your own words and is genuinely
      one sentence.
- [ ] Four load-bearing examples are extracted, each with a direct
      quote, a paragraph reference, an un-scalable-move line, and
      a produced-outcome line.
- [ ] Graham's three (or your revised) reasons are stated with the
      diff against chapter 04's version.
- [ ] The when-does-it-end section addresses both what the essay
      says and where it is silent, with the diff against chapter
      04's transition signals.
- [ ] At least one substantive, steelmanned disagreement is
      written.
- [ ] The two cross-reference paragraphs (chapter 03 and chapter
      05) are present.
- [ ] The file is committed to your notes as
      `mod-003-exercise-03-do-things-that-dont-scale-annotated.md`.

## Common failure modes to avoid

- Writing a book report. This is annotation and argument, not
  summary.
- Extracting four examples that are all the same shape (four
  marketplace / consumer cases). Force variety — B2B, consumer,
  developer-tool, marketplace all count differently.
- Skipping the disagreement section because "Graham is right."
  Even essays that are right in the core have specific claims that
  break in specific cases. Find one.
- Cross-referencing the wrong chapters. The two cross-refs are
  chapter 03 (mismatch taxonomy in this module) and chapter 05
  (premature scaling in this module). Not chapter 04 — that's the
  scaffold for the essay itself.
- Treating chapter 04's transition signals as gospel. Chapter 04
  is a scaffold. If Graham says something different (or nothing
  at all) about the transition, your annotation should say so
  honestly.

## What good looks like

An annotated read that a first-time reader could use as a working
guide alongside the primary essay. They can see the four examples
lifted out, the three reasons named with paragraph references, the
transition question addressed, and one substantive place where the
essay is contested. Your disagreement should make a reader think,
not roll their eyes.

You will reuse this annotation for exercise 04 (premature-scaling
post-mortem read), for exercise 05 (checklist application), and
across mod-004 and mod-005 whenever the "should this be
un-scalable or scalable?" question arises.
