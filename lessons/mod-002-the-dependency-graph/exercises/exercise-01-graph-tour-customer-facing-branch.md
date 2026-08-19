---
module: mod-002-the-dependency-graph
exercise: exercise-01
slug: graph-tour-customer-facing-branch
hours: 2
prereqs: [chapter-01-the-graph-as-the-foundations-instrument, chapter-02-customer-facing-branch]
---

# Exercise 01 — Graph Tour: Customer-Facing Branch

## Problem statement

Chapter 02 walked the customer-facing branch — Customer Discovery →
Product-Market Fit → GTM Strategy → Sales → Growth → Exit — and named,
for each node, what it produces and what the next node needs from it.
This exercise is where you prove you can walk the branch under your own
power, without the chapter open in front of you.

You will (a) reproduce the branch as a hand-off table, (b) diagnose a
skipped-upstream failure at each of the four internal hand-offs, and
(c) pick one real, publicly documented startup and map two of its known
outcomes to the correct nodes.

## Requirements

### Part A — the hand-off table (do not copy from the chapter)

Reproduce the hand-off table from memory, in the shape below. Filling in
the *breaks-if-skipped* column is the whole point — that's where the
graph earns its keep.

```markdown
| From node | To node | Hand-off (one sentence) | What breaks if skipped |
|---|---|---|---|
| Customer Discovery | Product-Market Fit | ... | ... |
| Product-Market Fit | GTM Strategy | ... | ... |
| GTM Strategy | Sales | ... | ... |
| Sales | Growth | ... | ... |
| Growth | Exit | ... | ... |
```

After you fill it in from memory, open chapter 02 and diff against the
version there. Note any differences — especially any hand-offs you
softened or dropped.

### Part B — skipped-upstream diagnosis (4 short cases)

For **each of the four internal hand-offs** in the branch (Discovery →
PMF, PMF → GTM, GTM → Sales, Sales → Growth), write a **3-sentence
diagnosis** of what a company that skipped the upstream would look like
in the wild. Concretely:

- What is the *visible symptom* an observer would see? (This is the
  downstream failure.)
- What is the *root cause* upstream that was skipped? (This is where
  the graph diagnoses to.)
- What is the *cheapest recovery move* — do the skipped upstream work
  now, or something else? (This is the founder's call.)

### Part C — real-company mapping

Pick **one real, publicly documented startup** — a well-covered one is
best (a company with a founder interview or a case study you can point
to). Identify **two concrete outcomes** you know about — a launch, a
pivot, a fundraise, a hire, a shutdown, a repositioning, a public metric
— and, for each, place the outcome on the customer-facing branch:

- Which node was the outcome *produced from*?
- Which upstream hand-off was the outcome *evidence for* — that the
  hand-off was clean, or that it was skipped?

Cite the source you drew the outcome from (a founder essay, a podcast
transcript, a press release, an S-1) with a URL or a book / episode
reference.

Do not fabricate outcomes. If you can't find two documented outcomes for
a company, pick a different company. Do not use a private / undisclosed
company you have inside information on — the exercise is about
publicly-defensible reasoning.

## Deliverable shape

A single Markdown file, `mod-002-exercise-01-customer-facing-tour.md`,
structured:

```markdown
# Customer-Facing Branch — Graph Tour

## Part A — Hand-off table (from memory)
<table>

### Diff notes (after checking against chapter 02)
- ...

## Part B — Skipped-upstream diagnoses
### Discovery → PMF
- Visible symptom: ...
- Root cause: ...
- Cheapest recovery: ...

### PMF → GTM
...

### GTM → Sales
...

### Sales → Growth
...

## Part C — Real-company mapping
- Company: ...
- Source(s): ...

### Outcome 1
- Description: ...
- Produced from node: ...
- Hand-off evidence (clean or skipped): ...

### Outcome 2
...
```

## Starter guidance

- **The hand-off table is a memory exercise on purpose.** If you copy
  it from the chapter, you get zero of the value. Write it from
  memory, then diff. The diff is where you learn.
- **The "skipped upstream" diagnoses should feel familiar.** They
  are the pattern behind most of the failure post-mortems in mod-001
  chapter 06. If your Part B diagnoses match the seven-layer taxonomy
  from that chapter, you are on the right track.
- **For Part C, prefer companies with post-mortems or founder
  essays.** They are honest sources. Avoid company-blog "here's how
  we succeeded" pieces — they are marketing, and they are
  systematically wrong about causation.
- **Do not conflate the graph with the calendar.** In Part C, an
  outcome's node placement is about *what work produced it*, not
  *when in the company's life it happened*. A Series-B company can
  still be producing Customer Discovery outcomes for a new segment.

## Acceptance criteria

You have completed the exercise when:

- [ ] Part A hand-off table has all five rows filled in from memory
      before you consulted the chapter.
- [ ] Part A diff notes list every hand-off row that was materially
      different from chapter 02, with a one-line explanation of the
      difference.
- [ ] Part B has a 3-sentence diagnosis (symptom / root / recovery)
      for each of the four internal hand-offs.
- [ ] Part C names a real company, cites at least one specific source
      (URL or book/episode reference) per outcome, and places two
      distinct outcomes on the branch with hand-off evidence.
- [ ] For every outcome in Part C, the placement identifies **both**
      the producing node **and** the hand-off it is evidence for or
      against.
- [ ] The file is committed to your notes as
      `mod-002-exercise-01-customer-facing-tour.md`.

## Common failure modes to avoid

- Turning Part A into "read the chapter, transcribe the table." The
  diff step is the exercise; skipping it defeats the purpose.
- Diagnosing every Part B case as "no PMF." PMF is often *not* the
  root even when it is the loudest symptom — the taxonomy has four
  distinct hand-offs and each has its own upstream failure mode.
- Picking a hero company for Part C and hunting for outcomes that
  make them look good. Pick a company you can be honest about; a
  well-documented pivot or failure is a better case study than an
  ambiguous success.

## What good looks like

A completed tour that another founder could read in ten minutes and
walk away with a clear working model of the customer-facing branch,
concrete failure diagnoses at each hand-off, and a real example of
graph-placement done on a real company. You should be able to hand
this file to a co-founder as the primer they read *before* their first
customer-discovery week.
