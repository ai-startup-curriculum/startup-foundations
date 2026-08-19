---
module: mod-002-the-dependency-graph
exercise: exercise-03
slug: graph-tour-economics-branch
hours: 2
prereqs: [chapter-01-the-graph-as-the-foundations-instrument, chapter-04-economics-branch]
---

# Exercise 03 — Graph Tour: Economics Branch

## Problem statement

Chapter 04 walked the economics branch and produced the *load-bearing
numbers compass* — a table matching each stage (IDEA → MATURE) to the
numbers that actually matter at that stage. This exercise makes you use
the compass in both directions: given a stage, name the numbers; given
a candidate activity, decide whether it is targeting the right numbers
for the stage.

You will (a) reproduce the load-bearing-numbers compass from memory,
(b) diagnose six candidate economic activities as stage-appropriate or
stage-mismatched, and (c) walk one real fundraise announcement (a
public seed or Series A announcement) and identify which economics-branch
numbers the round was priced on.

## Requirements

### Part A — the load-bearing-numbers compass (from memory)

Reproduce the compass from chapter 04 in the shape below, from memory.
Then open chapter 04 and diff — the diff is the learning move.

```markdown
| Stage | Load-bearing numbers | What is not load-bearing yet |
|---|---|---|
| IDEA | ... | ... |
| PRE-SEED | ... | ... |
| SEED | ... | ... |
| SERIES-A | ... | ... |
| GROWTH | ... | ... |
| MATURE | ... | ... |
```

Under the table, write **one sentence per stage** naming the *single
most load-bearing number* at that stage. That's the "if you can only
watch one dial" call.

### Part B — six candidate activities

For each of the six candidate activities below, decide:

- **Stage** the founder is currently at (given the description).
- **Which economics-branch node(s)** the activity targets.
- **Is the activity stage-appropriate?** (yes / no / mixed)
- **If not, what would be the stage-appropriate version of the
  activity right now?**

Write 3–4 sentences per activity.

**Activity 1.** A two-person pre-seed team, four weeks after
incorporation, spends a full week building a three-statement financial
model with cohort retention curves and channel-level CAC assumptions.

**Activity 2.** A seed-stage founder with $1.2M in cash and $80k
monthly burn is trying to decide whether to hire a second engineer or
wait three months. She opens a spreadsheet and computes runway under
each choice.

**Activity 3.** A pre-seed founder writes a one-paragraph description
of what CAC and LTV *mean*, adds no numbers yet, and pins it to the
top of her working doc.

**Activity 4.** A Series-A CEO produces a monthly board pack that
covers gross and net burn, cash-out date, cohort retention curves,
channel-level CAC, blended CAC, gross margin, and a hiring-plan
variance-to-model.

**Activity 5.** An idea-stage founder — no company yet — spends an
afternoon studying capital-allocation frameworks (BCG matrix, hurdle
rates, portfolio approaches) to prepare for eventual scale.

**Activity 6.** A growth-stage CEO with 200 people and $60M raised
insists that runway math should still be the primary board-pack
number, and dismisses channel-level unit economics as "premature."

For each Activity, cite (or `<!-- needs-research: ... -->` for later
verification) at least one primary source on the number or framework
you are naming — the Paul Graham "Default Alive or Default Dead"
essay, the OpenView / Bessemer / KeyBanc SaaS survey for SaaS
benchmarks, a specific YC or a16z essay on early-stage numbers, or a
Buffett shareholder letter for capital allocation.

### Part C — one real fundraise, priced on numbers

Pick **one publicly announced seed or Series A round** for a company
you can find real numbers on (a founder essay, a public press release
with metrics, an S-1 that later disclosed the pre-IPO numbers, a
podcast interview where the founder walked through the round). Then:

- List the economics-branch numbers that were most likely the *primary
  gating numbers* for that round. Reference the specific numbers if
  they were disclosed; reference their *category* if they were not.
- Explain in 3–4 sentences why those specific numbers were the ones
  the round was priced on, given the company's stage.
- Cite the source(s) for the round announcement and any disclosed
  numbers.

Do not invent numbers. If specific figures are not public, mark them as
"category only" (e.g., "PMF-level cohort retention — specific figures
not disclosed") and reason about the category.

## Deliverable shape

A single Markdown file, `mod-002-exercise-03-economics-tour.md`,
structured:

```markdown
# Economics Branch — Graph Tour

## Part A — Load-bearing-numbers compass (from memory)
<table>

### One-dial-per-stage
- IDEA: ...
- PRE-SEED: ...
- SEED: ...
- SERIES-A: ...
- GROWTH: ...
- MATURE: ...

### Diff notes (after checking against chapter 04)
- ...

## Part B — Six candidate activities
### Activity 1
- Stage: ...
- Node(s): ...
- Stage-appropriate? ...
- Better version: ...

### Activity 2
...

(through Activity 6)

## Part C — Real fundraise
- Round: ...
- Sources: ...
- Primary gating numbers: ...
- Reasoning: ...
```

## Starter guidance

- **Part A is a memory drill.** The compass is the single most
  reusable artifact from chapter 04; if you can't reproduce it, you
  will misuse the economics branch in every later module.
- **The Part B activities are drawn from real founder patterns.**
  Activity 1 and Activity 5 are premature-scaling patterns
  (mod-001 chapter 06); Activity 2 and Activity 4 are stage-
  appropriate; Activity 3 is a slight over-thinker but harmless;
  Activity 6 is a *late*-stage stage-mismatch (a founder who
  didn't graduate their instruments). If you find all six easy,
  swap them for six candidate activities from your own week.
- **For Part C, prefer rounds that had public founder writeups.**
  Y Combinator's Launch posts, a16z portfolio-company essays,
  founder Substacks, and S-1 filings are the reliable sources. If
  a "round announcement" is really a puff piece, look for a
  companion metrics disclosure elsewhere.
- **Do not confuse *load-bearing* with *interesting*.** Founders
  find capital allocation, three-statement models, and Rule of 40
  intellectually interesting from day one. The exercise is about
  which numbers *bear the weight of decisions* at a stage — not
  which numbers are fun to think about.

## Acceptance criteria

You have completed the exercise when:

- [ ] Part A compass is filled in for all six stages from memory,
      with a one-sentence "single most load-bearing number" per
      stage, and diff notes against chapter 04.
- [ ] Part B has all six activities diagnosed with stage /
      node(s) / stage-appropriateness / better-version fields
      populated, and at least one source or research marker per
      activity.
- [ ] Part C names a real announced round, cites sources,
      identifies the primary gating numbers (specific if
      disclosed, category-only if not), and gives a 3–4 sentence
      reasoning.
- [ ] The file is committed as
      `mod-002-exercise-03-economics-tour.md`.

## Common failure modes to avoid

- Turning Part A into a paste of chapter 04's compass. The
  memory-then-diff move is where the learning happens; if you
  paste, you learn nothing.
- Diagnosing every Part B activity by the same lens ("this is
  premature-scaling"). Some are, some aren't. Force yourself to
  distinguish.
- Inventing round numbers in Part C. If the metrics aren't
  public, say so and reason from category. Fabricated numbers
  make the whole exercise unusable as a reference.

## What good looks like

A completed tour a first-time founder could keep on her desk as the
economics-branch reference for the whole seed-to-Series-A journey.
The compass tells her which numbers to watch; the six activities
give her a taxonomy of "what is stage-mismatched-and-common"; the
real fundraise anchors it all to a concrete case.
