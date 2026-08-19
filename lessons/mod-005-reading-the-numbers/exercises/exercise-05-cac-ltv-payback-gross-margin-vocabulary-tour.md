---
module: mod-005-reading-the-numbers
exercise: exercise-05
slug: cac-ltv-payback-gross-margin-vocabulary-tour
hours: 3
prereqs: [chapter-05-unit-economics-vocabulary]
---

# Exercise 05 — CAC, LTV, Payback, Gross Margin: Vocabulary Tour

## Problem statement

Chapter 05 named the four unit-economic terms at the vocabulary
level and drew the boundary — depth lives in the finance-fundraising
pillar. This exercise is a *vocabulary check*, not a modelling
exercise. Its purpose is to prove that a Foundations graduate can
read a pillar-level unit-economics module without a glossary and
can already ask the right definitional follow-up questions on each
of the four terms.

The exercise is short (3 hours) on purpose. Do not spend the time
building a real CAC or LTV model — that is the pillar's job
(chapter 08's deferral, see the `startup-finance-fundraising-
curriculum` link). Spend the time defining, cross-checking, and
mapping the terms.

## Requirements

### Part A — pick the startup and the stage (about 15 min)

Use the startup from prior exercises. Note its current stage from
mod-003 (IDEA / PRE-SEED / SEED / SERIES-A / GROWTH / MATURE).

If the startup is IDEA or PRE-SEED, chapter 05's stage-gating
argument applies: none of the four terms is load-bearing yet, and
the point of this exercise is to know what will be measured *later*.
If the startup is SEED or beyond, some of the four terms should
already be at least approximately measured.

**Deliverable A**: one sentence naming the startup and its stage,
one sentence on whether the four terms are yet load-bearing per
chapter 05.

### Part B — define each term against the specific startup (about 60 min)

For each of the four terms — **CAC, LTV, payback, gross margin** —
write:

1. **The one-sentence definition** from chapter 05, in your own
   words.
2. **The specific definitional variant** you would use for this
   startup, and why:
   - For CAC: fully-loaded / paid / blended?
   - For LTV: gross margin or contribution margin? monthly
     or annual churn? discounted or undiscounted?
   - For payback: computed against which margin? measured
     against which CAC variant?
   - For gross margin: what specifically counts as COGS for
     *this* product? What variable per-customer costs (hosting,
     API calls, payment processing, direct support, per-user
     infrastructure) apply?
3. **The formula** with the specific inputs your business model
   uses.

**Deliverable B**: a four-section write-up, one per term, roughly
150–250 words each.

### Part C — the stage-gating table (about 30 min)

Fill in this table for your specific startup:

| Term | Currently measurable? | Currently load-bearing? | Approximate stage-transition when it becomes load-bearing |
|---|---|---|---|
| CAC | Y / N | Y / N | ... |
| LTV | Y / N | Y / N | ... |
| Payback | Y / N | Y / N | ... |
| Gross margin | Y / N | Y / N | ... |

"Currently measurable" means: do you have enough data over a long
enough period to compute a defensible number *if* you tried?
"Currently load-bearing" means: are you making decisions based on
the number? The two are distinct — you can have a measurable CAC
that isn't yet load-bearing because acquisition is too early to
optimise against.

Then answer, in two-to-three sentences: **which term is closest
to becoming load-bearing next for your startup?** — and what stage
transition triggers it.

### Part D — the mis-use catch (about 30 min)

Chapter 05 named the specific mis-use pattern for each term. For
each of the four, write one sentence naming a *specific example*
you have heard (in an investor pitch, a founder conversation, a
blog post, a podcast interview) or an example you can construct
that matches the pattern:

- **CAC**: someone quoting a CAC without specifying period,
  channel mix, or definition variant.
- **LTV**: someone quoting an LTV extrapolated from cohorts too
  small or too short to justify.
- **Payback**: someone quoting LTV/CAC ratio without payback.
- **Gross margin**: someone assuming SaaS-convention margins for
  a product whose variable per-customer costs are actually
  higher.

The four examples together are the exercise's actual test: if you
can spot the mis-use in the wild, you have the vocabulary.

### Part E — the pillar-module cross-reference (about 30 min)

For each of the four terms, name where in the
[`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum)
you would go for the depth. The pillar's module structure is
outside this repo, so use plausible module names based on the
term and the general shape of that curriculum. If you don't know,
write *"unit-economics module (to be authored — I would look for
X)"* and name what "X" is. This maps the deferrals from chapter
05 into concrete pillar-reading intent.

Then, for the term that's closest to load-bearing (from Part C),
write two-to-three sentences on **when specifically you plan to
read the pillar module for that term** — the stage-transition, the
decision it will inform, and the time budget.

### Part F — the one-pager deferral line (about 15 min)

Write the one-pager deferral line for the mod-005 founder-numbers
one-pager (chapter 07) in the standard grammar. Chapter 05's
suggested language is:

> **Unit economics:** Deferred to
> [`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum)
> unit-economics module (stage: SERIES-A). Current stage: PRE-SEED.

Adjust to your startup's current stage. If your startup is SEED or
beyond, replace the deferral line with actual tracked values for
whichever of the four terms have become load-bearing per Part C.

## Deliverable shape

A single Markdown file,
`mod-005-exercise-05-unit-economics-vocabulary.md`, structured:

```markdown
# Unit Economics Vocabulary Tour — [Startup Name]

## Setup
- Startup: <one sentence>
- Stage: <PRE-SEED / SEED / ...>
- Are the four terms load-bearing yet? <one sentence>

## The four terms — defined for this startup

### CAC
- Definition: <one sentence in your words>
- Definitional variant chosen: <one-to-two sentences>
- Formula for this business:
```
CAC = ...
```

### LTV
<same shape>

### Payback
<same shape>

### Gross margin
<same shape, with the specific COGS list for your product>

## Stage-gating
| Term | Currently measurable? | Currently load-bearing? | Load-bearing transition |
|---|---|---|---|
| CAC | | | |
| LTV | | | |
| Payback | | | |
| Gross margin | | | |

Next term to become load-bearing: <one sentence, per Part C>

## Mis-use examples
- CAC: <one sentence>
- LTV: <one sentence>
- Payback: <one sentence>
- Gross margin: <one sentence>

## Pillar hand-off
- CAC depth: <pillar module>
- LTV depth: <pillar module>
- Payback depth: <pillar module>
- Gross margin depth: <pillar module>

Next pillar-reading commitment: <two-to-three sentences per Part E>

## One-pager deferral line
<the line from Part F, formatted as chapter 07 requires>
```

Total length: 700–1200 words.

## Starter guidance

- **Do not compute real CAC or LTV numbers unless you are at
  SEED or later with real data.** Chapter 05's stage-gating
  argument applies. Trying to compute a CAC on ten customers
  practices the wrong skill.
- **Do not skip the definitional-variant question.** The whole
  vocabulary-level teaching is that each of the four terms has
  more than one working definition, and knowing which variant
  you are using is what makes the number honest.
- **Use your own product's specifics when discussing gross
  margin.** SaaS-convention gross margins don't apply universally.
  A product that makes 30 LLM API calls per user session per day
  has a very different variable-cost profile from a classical
  SaaS.

## Acceptance criteria

You have completed the exercise when:

- [ ] The startup and its stage are named, with a one-sentence
      call on whether the four terms are yet load-bearing.
- [ ] Each of the four terms has a definition, a specific
      definitional variant chosen with reason, and the formula
      with the specific inputs for the business.
- [ ] The four-row stage-gating table is filled, with the "next
      term to become load-bearing" call written.
- [ ] Each of the four terms has a mis-use example in one
      sentence.
- [ ] Each of the four terms has a pillar cross-reference
      pointing at
      [`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum).
- [ ] A specific pillar-reading commitment is written for the
      term closest to load-bearing.
- [ ] The one-pager deferral line (or replacement) is drafted.
- [ ] The write-up is committed as
      `mod-005-exercise-05-unit-economics-vocabulary.md`.

## Common failure modes to avoid

- **Copy-pasting textbook definitions.** Chapter 05's own
  definitions are the reference; this exercise wants *your*
  definition, in your words, applied to your specific business.
- **Skipping the definitional variant.** The variant is where
  the honesty is. A CAC without a variant is a number without a
  meaning.
- **Building a real CAC / LTV model.** Not this exercise's
  scope. Save the modelling for the pillar-reading time budget
  in Part E.
- **Refusing to write the mis-use examples.** They are the
  exercise's actual test.

## What good looks like

A vocabulary tour that leaves you able to walk into a
pillar-level unit-economics module without stopping to look
anything up, and to ask the right definitional question the
first time each of the four terms appears in a real
conversation. The stage-gating table is what tells you *when* to
open the pillar; the definitional variants are what tell you
*how* to read it once you do.
