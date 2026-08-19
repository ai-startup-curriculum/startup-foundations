---
module: mod-002-the-dependency-graph
exercise: exercise-05
slug: lean-canvas-vs-business-model-canvas-drill
hours: 3
prereqs: [chapter-06-lean-canvas-vs-business-model-canvas]
---

# Exercise 05 — Lean Canvas vs Business Model Canvas Drill

## Problem statement

Chapter 06 named two working canvases for the assumption set under a
startup — the **Business Model Canvas** (Osterwalder / Pigneur, 2010)
and the **Lean Canvas** (Ash Maurya, 2010) — and gave you the choice
rule: Lean for validating hypotheses under uncertainty, BMC for
describing a known or mostly-known model. This exercise makes you
draw *both* canvases against *one* startup and defend the
stage-appropriate choice, so the rule stops being abstract.

You will (a) draw a full Lean Canvas and a full BMC for the same
chosen startup, (b) diff the two canvases block-by-block to see
where they diverge, and (c) write a short defense of which canvas
is the right primary instrument at the startup's current stage.

## Requirements

### Part A — pick one startup

Pick **one startup** as the subject. Options, in order of
preference:

1. Your own current startup (best — highest signal).
2. A startup you have detailed public knowledge of (founder
   interviews, S-1 filings, ProductHunt launches, YC Launch posts).
3. A synthetic startup you invent for the exercise, with a
   deliberately specified stage and enough context to draw the
   canvases (a target segment, a rough product idea, a rough
   business-model shape).

Whichever you pick, state **explicitly at the top of the
deliverable**:

- The startup's name (or a synthetic name).
- The stage it is currently at (from `STARTUP_STAGES.md`).
- The evidence for the stage claim.
- Two sentences on what the startup does.

### Part B — draw a Lean Canvas

Draw the Lean Canvas as a 9-cell table (or as a fenced-code ASCII
grid). Fill in each block honestly. The nine blocks:

1. Problem
2. Customer Segments (name early adopters explicitly)
3. Unique Value Proposition
4. Solution
5. Channels
6. Revenue Streams
7. Cost Structure
8. Key Metrics
9. Unfair Advantage

For each block, add a **confidence tag** — `validated`, `assumed`,
or `unknown` — reflecting how much real evidence backs the block
today. Empty and `unknown` are both honest answers if you don't
know; `assumed` is what you're guessing.

### Part C — draw a Business Model Canvas

Draw the BMC as a 9-cell table for the same startup. Blocks:

1. Customer Segments
2. Value Propositions
3. Channels
4. Customer Relationships
5. Revenue Streams
6. Key Resources
7. Key Activities
8. Key Partnerships
9. Cost Structure

Same confidence-tag discipline as Part B.

<!-- needs-research: verify the canonical BMC block naming at strategyzer.com and align the labels above with the primary source before publishing worked examples. -->

### Part D — the block-by-block diff

Produce a short table showing which cells differ between the two
canvases for your startup:

```markdown
| Cell | Lean Canvas content | BMC content | Same / different / not-in-both |
|---|---|---|---|
| ... | ... | ... | ... |
```

The five shared blocks (Customer Segments, Value Proposition,
Channels, Revenue, Cost) should be either "same" or "different"
(if you filled them in differently); the four Lean-only blocks
(Problem, Solution, Key Metrics, Unfair Advantage) and the four
BMC-only blocks (Customer Relationships, Key Resources, Key
Activities, Key Partnerships) should be "not-in-both."

### Part E — the choice defense

Write a **300–500 word defense** of which canvas is the *primary
instrument* for this startup at its current stage. Cover:

- Which canvas is primary and why (apply the chapter-06 rule
  explicitly).
- Which specific Lean-only or BMC-only blocks are doing the
  most work for this startup right now, and why.
- At what future stage — and by what evidence — you would
  expect to switch from one canvas to the other.
- One concrete piece of evidence you would go collect *this
  week* against a block currently tagged `assumed` or
  `unknown` on the primary canvas.

Cite the primary sources for either canvas (*Business Model
Generation*, *Running Lean*, strategyzer.com, leanstack.com,
etc.) at least once each — the exercise is a canonical-canvas
drill and the citations should be to the canonical books.

## Deliverable shape

A single Markdown file, `mod-002-exercise-05-canvas-drill.md`,
structured:

```markdown
# Lean Canvas vs Business Model Canvas — <startup name>

## Part A — Startup
- Name: ...
- Stage: ...
- Evidence for stage: ...
- What it does: ...

## Part B — Lean Canvas
<9-cell filled canvas with confidence tags>

## Part C — Business Model Canvas
<9-cell filled canvas with confidence tags>

## Part D — Block-by-block diff
<table>

## Part E — Choice defense
<300–500 word defense with citations>
```

## Starter guidance

- **Honest is better than complete.** A Lean Canvas with three
  blocks tagged `assumed` and four tagged `unknown` is more
  useful than one with plausible-sounding fiction in every cell.
  The whole point is to see what you don't yet know.
- **Draw both canvases *before* writing the defense.** If you
  decide which canvas is primary first, you'll fill the
  non-primary one in weakly to make your choice look obvious. The
  defense should follow from the drawing, not drive it.
- **The five shared blocks should be identical across the two
  canvases** for the same startup, unless you have a real reason
  they should differ. If they differ, name why in the diff table.
- **The confidence tags are the exercise's memory.** When you
  come back to this file in six weeks after some evidence has
  landed, the tags tell you which cells to revise. Choose them
  carefully.

## Acceptance criteria

You have completed the exercise when:

- [ ] Part A states the startup name, stage, evidence for the
      stage claim, and a two-sentence description.
- [ ] Part B has all nine Lean Canvas blocks filled or explicitly
      tagged `unknown`, each with a confidence tag.
- [ ] Part C has all nine BMC blocks filled or tagged, each with
      a confidence tag.
- [ ] Part D has a diff table covering all 13 unique blocks
      across the two canvases.
- [ ] Part E is a 300–500 word defense that applies the chapter
      06 choice rule explicitly, names which specific blocks are
      doing the most work, states the future-switch condition,
      and names one piece of evidence to collect this week.
- [ ] Part E cites *Running Lean* or leanstack.com **and**
      *Business Model Generation* or strategyzer.com at least once
      each.
- [ ] The file is committed as
      `mod-002-exercise-05-canvas-drill.md`.

## Common failure modes to avoid

- Drawing only one canvas and hand-waving the other. Both
  canvases must be fully drawn; that's what makes the diff
  meaningful.
- Filling every block in both canvases with confident-sounding
  copy. If you have no evidence, tag `assumed` or `unknown` and
  move on.
- Defending your canvas choice with "I like this one better."
  The defense must apply the chapter-06 rule; personal
  preference is not the criterion.
- Skipping the confidence tags. Tags are the artifact's most
  reusable feature.

## What good looks like

A completed drill you can hand to a co-founder along with the
question *"tell me the three assumptions we most need to test
this month."* The primary canvas plus its confidence tags should
make the answer obvious in under two minutes. The choice defense
should read like an operating brief, not a canvas-tool essay.
