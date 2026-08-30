---
module: mod-005-reading-the-numbers
exercise: exercise-06
slug: north-star-metric-selection-and-defence
hours: 3
prereqs: [chapter-06-north-star-metric]
---

# Exercise 06 — North-Star Metric Selection and Defence

## Problem statement

Chapter 06 formalised the North-Star metric — one number, chosen
deliberately, understood by everyone, defended against alternatives.
This exercise runs the full four-step selection process (draft
candidates → score against the three axes → pick and precisely
define → defend against three closest alternatives) for the same
startup used across the module's other exercises, and lands with a
North-Star row ready to drop into the founder-numbers one-pager in
exercise 07.

The exercise's actual test is the **defence against three
alternatives**. Anyone can pick a metric. The specific skill this
exercise trains is the discipline of explaining *why the runner-ups
are not the North-Star for this company at this stage*.

## Requirements

### Part A — read the primary references (about 30 min)

Read the two primary references linked in `resources.md`:

1. **Amplitude, `The North Star Playbook`** — chapters 1 and 2.
   The selection axes in chapter 06 of this module are adapted
   from the same framework.
2. **Sean Ellis's North-Star writing** — one canonical post from
   the Growth Hackers archive (or wherever the primary source is
   currently hosted).

Also skim **Eric Ries, `The Lean Startup`**, on vanity metrics
(any edition — the vanity-metrics discussion appears in the
"Learn" section). Chapter 06 argued the North-Star exists
specifically to defeat vanity metrics; the Ries framing is the
canonical source for the failure the North-Star defends against.

**Deliverable A**: one paragraph (three-to-five sentences) on
what the Amplitude and Ellis writing agree on, and one place
where chapter 06 of this module adds to or diverges from them.
This paragraph goes at the top of the exercise write-up.

### Part B — draft the candidate list (about 30 min)

For the startup you've been working against across mod-004 and
mod-005, write down **8–12 candidate metrics** that could
plausibly be the North-Star. Do not prune yet — the point of
this step is coverage, not selection. Include:

- Any cumulative totals your team currently talks about
  (registered users, total downloads, total signups). Chapter 06
  will flag these as vanity, but they belong on the draft list.
- Any revenue metrics you currently track (MRR, ARR, weekly
  bookings, GMV).
- At least two value-event-per-time counts (messages, meetings,
  transactions, deliveries — whatever the product's core
  value-delivery event is).
- At least one engaged-customer count (weekly active accounts,
  monthly active accounts, weekly active users who did X).
- At least one unit-of-value-delivered (miles, hours, loans,
  contracts — the underlying quantity of what the product
  produces).
- Any product-specific metric your team already talks about that
  doesn't fit the four canonical shapes.

**Deliverable B**: a numbered list of 8–12 candidates, each one
line. No scoring yet.

### Part C — score each candidate against the three axes (about 45 min)

For each candidate on the draft list, rate high / medium / low
on the three axes chapter 06 named:

1. **Value to the customer.** Does the metric move because the
   customer received something they came for?
2. **Value to the business.** Does the metric correlate with
   revenue over time (not necessarily *be* revenue)?
3. **Legibility across the team.** Can every person in the
   operating loop define it, name today's value, and name at
   least one lever they can pull to move it?

Produce a scoring table:

| # | Candidate | Value to customer | Value to business | Legibility | Verdict |
|---|---|---|---|---|---|
| 1 | Total registered accounts | Low | Low | High | Vanity |
| 2 | ... | ... | ... | ... | ... |

Verdict values: **Vanity** (cumulative total, top-of-funnel
without a value gate, ratio with a drifting denominator),
**Supporting** (scores well on some but not all three axes),
**Candidate** (scores well on all three), **Top candidate** (the
one you pick).

The verdict column is where the exercise's judgment lives.
Chapter 06's failure-mode section catalogues the vanity-metric
patterns; use them explicitly.

### Part D — pick and precisely define the top candidate (about 30 min)

From the Candidate / Top-candidate rows, pick one. Write the
precise definition. Chapter 06's example format:

> *"The count of meetings created in the product between Monday
> 00:00 and Sunday 23:59 (customer local timezone), divided by
> the count of accounts that had at least one user log in during
> the same window."*

The definition must name:

- **What counts as the value event** (with the specific
  qualifiers — "created," not "scheduled"; "in the product," not
  "in the customer's calendar").
- **The unit of aggregation** (per account, per user, per
  segment, or in aggregate — chapter 06 argued for
  per-active-account at PRE-SEED because aggregate hides
  per-account intensity).
- **The time window** (rolling 7 days, Monday-to-Sunday, calendar
  week — the specific window matters; different windows produce
  different numbers).
- **The customer / user filter** (paying only, active only,
  logged-in this week only — any filter must be named).

**Deliverable D**: the top-candidate metric name and its precise
one-paragraph definition.

### Part E — the defence against three alternatives (about 45 min)

Pick the **three closest runner-ups** from Part C's scoring
table (Candidate or Supporting verdicts, not Vanity). For each,
write **one paragraph** on *why the runner-up is not the
North-Star for this company at this stage*.

Each defence paragraph should name:

- **What the runner-up would optimise for.** ("Paying customer
  count would optimise for closing the next deal.")
- **What that optimisation would miss.** ("Closing more deals
  without value-per-account climbing means we're adding accounts
  that don't stick — the retention risk is a lower-priority
  problem at PRE-SEED and becomes a higher-priority problem at
  SEED.")
- **The stage transition at which the runner-up might become
  the North-Star.** ("Paying customer count is likely the right
  North-Star at mid-SEED when the customer count is high enough
  to move week to week meaningfully.")

The defence is where the reasoning becomes portable. A
North-Star chosen without a written defence is a gut call; a
North-Star chosen with three written defences against the closest
alternatives is a defensible position that can be re-visited
when the stage shifts.

### Part F — the stage-evolution note (about 15 min)

Chapter 06 named the typical stage-evolution pattern of
North-Star metrics:

- PRE-SEED / early-SEED: value-event-per-active-account rate.
- Mid-SEED to SERIES-A: paying-customer count or MRR-equivalent.
- GROWTH and beyond: segmented revenue or engaged-customer
  number by cohort.

Write **two-to-three sentences** on how you expect your chosen
North-Star to evolve as the startup moves through the next
one or two stage transitions. This is not a commitment; it is a
first-draft plan the mod-004 decision log will record when the
North-Star is actually updated.

### Part G — the one-pager row draft (about 15 min)

Draft the founder-numbers one-pager North-Star row in the
three-value grammar chapter 07 requires:

```
Metric                | Current | Prior | Target
North-Star            | [value] | [prior] | [target]
    [precise definition on the sub-line]
```

Fill in a current value (real if you have data, plausible
placeholder if you don't), the prior-week or prior-month value,
and the target. The sub-line carries the precise definition from
Part D.

This row is what will go into exercise 07's one-pager.

## Deliverable shape

A single Markdown file,
`mod-005-exercise-06-north-star.md`, structured:

```markdown
# North-Star Selection and Defence — [Startup Name]

## Primary-source read
<one paragraph — Part A>

## Candidate list
<numbered list, 8–12 items — Part B>

## Scoring table
<the four-column table — Part C>

## Top candidate
- **Metric name**: <name>
- **Precise definition**: <one paragraph — Part D>

## Defence against three alternatives

### Alternative 1: [runner-up name]
<one paragraph — Part E>

### Alternative 2: [runner-up name]
<one paragraph — Part E>

### Alternative 3: [runner-up name]
<one paragraph — Part E>

## Stage evolution note
<two-to-three sentences — Part F>

## One-pager row draft
<the three-value grammar row + sub-line — Part G>
```

Total length: 900–1400 words.

## Starter guidance

- **The defence paragraphs are the exercise.** Anyone can pick a
  metric. The three defence paragraphs are where the reasoning
  gets tested; disproportionate time on Part E is the right
  allocation.
- **Include one vanity metric in the draft list on purpose.**
  Chapter 06's failure-mode catalogue is easier to internalise
  when you have scored a candidate as Vanity and named the
  specific pattern (cumulative total, top-of-funnel without
  value gate, ratio with drifting denominator).
- **Do not pick MRR at PRE-SEED unless you can defend it.** MRR
  is often the right North-Star at SEED and beyond. At PRE-SEED
  it is usually too small and too lumpy to be a weekly signal.
  If you pick MRR at PRE-SEED, the defence against the intensity
  metric (Alternative 1) has to be honest about why the lumpiness
  is acceptable.
- **Definitions matter more than choices.** A vaguely-defined
  correct metric is worse than a precisely-defined near-miss;
  the precisely-defined near-miss can be argued about, refined,
  and updated. The vague one just gets computed differently by
  each person on the team.
- **Score against your specific product, not against the SaaS
  convention.** If your product is a marketplace, a consumer app,
  or an AI-infrastructure product, the SaaS-convention scoring
  ("MRR wins by default") may be wrong. Chapter 06's three-axis
  framework is product-agnostic.

## Acceptance criteria

You have completed the exercise when:

- [ ] The two primary references were read and the top-of-file
      paragraph names what they agree on and where chapter 06
      diverges.
- [ ] The draft candidate list has 8–12 items, covering at least
      one cumulative total, at least one revenue metric, at
      least two value-event-per-time counts, at least one
      engaged-customer count, and at least one
      unit-of-value-delivered.
- [ ] The scoring table rates every candidate against the three
      axes with a Vanity / Supporting / Candidate / Top-candidate
      verdict.
- [ ] The top-candidate metric has a one-paragraph precise
      definition that names the value event, the unit of
      aggregation, the time window, and any customer / user
      filters.
- [ ] Three defence paragraphs are present, each naming what the
      runner-up would optimise for, what that optimisation would
      miss, and the stage transition at which the runner-up
      might become the North-Star.
- [ ] The stage-evolution note is two-to-three sentences on how
      the North-Star will likely evolve at the next one or two
      stage transitions.
- [ ] The one-pager row draft is present in the three-value
      grammar with the sub-line carrying the precise definition.
- [ ] The write-up is committed as
      `mod-005-exercise-06-north-star.md`.

## Common failure modes to avoid

- **Picking the metric that grows fastest.** Chapter 06's first
  failure mode. The fastest-growing metric is often the least
  meaningful (cumulative signups, homepage traffic). Pick for
  what the metric means; the growth rate is separate.
- **Definitions that require a follow-up question.** If a
  co-founder would ask "what counts as an active account?"
  after reading your definition, the definition isn't finished.
  Add the qualifier.
- **Defence paragraphs that just restate the choice.** "Paying
  customer count isn't the North-Star because meetings-per-account
  is a better metric." That is a restatement, not a defence. The
  defence has to say *what the runner-up would optimise for* and
  *what that optimisation would miss for this company at this
  stage*.
- **Choosing the same North-Star as the last five companies you
  read about.** Every SaaS startup does not have the same
  North-Star. If your defence paragraphs read like they could be
  copy-pasted onto any competitor, the reasoning is not specific
  enough to your business.
- **Skipping the stage-evolution note.** The North-Star chosen at
  PRE-SEED is almost never the North-Star five years later. A
  first-draft evolution plan makes the current choice easier to
  update when the stage shifts, because the update was already
  anticipated.

## What good looks like

A scoring table a co-founder could read in three minutes and see
which candidates were considered and why the top one was picked.
Three defence paragraphs a candidate investor could read as the
answer to *"why this metric and not <obvious alternative>?"*
without asking a follow-up. A precise definition that a first
engineer could implement as a SQL query without asking a
question.

The most useful signal is that **the defence paragraphs teach
you something you didn't know before you wrote them**. If you
wrote a defence paragraph and thought "wait, that argument
actually applies to my top candidate too," the exercise has done
its job — it has surfaced a definitional flaw in the choice that
now needs a definition improvement or a swap.

The North-Star row you draft in Part G is the row that lands on
exercise 07's founder-numbers one-pager. The chosen metric will
also be the row the mod-004 metrics one-pager (chapter 02 of
that module) leads with. The choice and its defence are what
carry the module's growth-side view into the weekly cadence for
the rest of the founder's career at this stage.
