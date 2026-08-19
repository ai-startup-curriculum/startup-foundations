---
module: mod-005-reading-the-numbers
exercise: exercise-03
slug: growth-rate-wow-and-mom-calculation
hours: 3
prereqs: [chapter-03-growth-as-a-rate]
---

# Exercise 03 — Growth Rate: WoW and MoM Calculation

## Problem statement

Chapter 03 installed the growth-as-a-rate mindset — WoW at early
stage, MoM at post-PMF, calibrated against Paul Graham's 5–7% WoW
yardstick. This exercise is where you compute both cadences on a
real (or realistic) 12-week series, calibrate against Graham, and
catch the specific ways rate calculations go wrong.

The exercise pairs with exercise 06 (North-Star selection) — you
need an underlying quantity before you can compute a rate. Do
exercise 06 first if you have not already picked a defensible
underlying quantity for your startup, or use a *placeholder*
quantity in this exercise and revisit once exercise 06 is
complete.

## Requirements

### Part A — pick the underlying quantity (about 15 min)

Pick one specific quantity to compute growth on. Two acceptable
options:

- **Your North-Star from exercise 06**, if you have completed it.
- **A defensible placeholder** — weekly paying customers, weekly
  active users on a strict definition, or weekly recurring
  revenue. Pick the one your startup's operating loop most
  naturally tracks. Note in the write-up that this is a
  placeholder and that exercise 06 will revisit the choice.

**Deliverable A**: one sentence naming the quantity and its
precise definition (chapter 03 and chapter 06 both stress: the
definition is the artifact).

### Part B — pull 12 consecutive weeks (about 30 min)

Pull the weekly value of the chosen quantity for the last 12
completed weeks (roughly the last three months). Use whatever
source of truth exists — your product-analytics tool, your
billing system, your CRM, a hand-count from Google Sheets if the
numbers are small enough. If real 12-week data is not available,
construct a realistic 12-week series informed by whatever you
know about the actual trajectory — but say so, and be honest
about which weeks are real and which are constructed.

The 12 weeks should be **Monday-through-Sunday** windows or
whatever week definition your operating cadence uses. Whatever
you pick, use the same definition for every week.

**Deliverable B**: a table of 12 rows — week-ending date, value —
in chronological order.

### Part C — compute WoW growth (about 30 min)

For each week from week 2 onward, compute:

```
WoW[n] = (value[n] − value[n-1]) / value[n-1]
```

Add a column to your table.

Then compute two additional summary numbers:

- **Trailing-four-week average WoW rate.** Average of the last
  four weekly WoW rates. Note that this is a smoothed number, not
  a growth rate for a specific week (chapter 03's warning).
- **Compound-annualised equivalent.** `(1 + trailing_four_week_avg)^52 − 1`,
  expressed as a multiplier. E.g., a trailing four-week average
  of 5% WoW is `(1.05)^52 ≈ 12.6×` per year.

### Part D — compute MoM equivalent (about 30 min)

Bucket the 12 weeks into three roughly-monthly periods (weeks
1-4, weeks 5-8, weeks 9-12). Compute the sum (for count-based
quantities) or the average (for rate-based quantities like MRR)
for each period. Then compute:

```
MoM_month_2_vs_month_1 = (period_2 − period_1) / period_1
MoM_month_3_vs_month_2 = (period_3 − period_2) / period_2
```

Also compute a *WoW-to-MoM check*: convert your trailing-four-week
WoW to a monthly-equivalent (`(1 + WoW)^4.33 − 1`) and compare
against the actual MoM you computed. They should be close but not
identical; big divergences (>3-5 percentage points) usually mean
the underlying quantity is noisy at weekly scale.

### Part E — the yardstick calibration (about 20 min)

Compare your trailing-four-week WoW against Paul Graham's
`Startup = Growth` bands:

- **<1% WoW** — Graham's "not yet figured out what you're doing"
  line.
- **1–5% WoW** — sub-YC-median; the company is working but not
  at the compounding rate.
- **5–7% WoW** — Graham's "good YC-batch" band.
- **7–10% WoW** — above-band; exceptional.
- **>10% WoW** — Graham's exceptional line; usually a small-
  numbers artefact or a real breakout — the next 2-3 weeks tell
  you which.

Write, in one paragraph:

- Which band your trailing four-week WoW falls into.
- Whether the *level* of the underlying quantity is small enough
  that the rate might be noise, and what you'd have to see over
  the next 2–3 weeks to confirm the reading.
- Whether the stage of your startup makes WoW the right cadence.
  If your natural sales cycle or product-value-delivery cycle is
  longer than a week, MoM may be the more honest signal (chapter
  03 has the argument).

### Part F — the failure-mode audit (about 30 min)

Run the six chapter-03 failure-mode checks against your 12-week
series and your rate calculations. For each check, answer in one
sentence: **did you avoid the failure mode, or did you fall into
it?**

1. **Cherry-picking the base week?** Is every WoW rate against
   the immediately-preceding week, or did you compare across
   weeks?
2. **Trailing average presented as "our growth rate"?** Have you
   labelled the trailing four-week number correctly, or is it
   being reported as *the* rate?
3. **Definition change mid-series?** Did the underlying quantity's
   definition change during the 12 weeks (a new counting rule,
   an expanded scope, a bug fix)? If yes, is the change dated and
   the series broken visibly at the change?
4. **Wrong cadence for the cycle?** Is your natural cycle time
   weekly-or-shorter (making WoW honest), or longer (making WoW
   noisy)? If MoM is the honest cadence at your stage, note it.
5. **Ignoring churn?** If your underlying quantity is a
   customer or subscriber count, is churn subtracted? Did you
   report *net* growth or *new* growth?
6. **One massive week extending the trend?** Any single week
   contributing an outsized share of the trailing average? If
   yes, was it a repeatable event or a one-off?

### Part G — the one-line update (about 15 min)

Write the growth-rate line for the mod-005 founder-numbers
one-pager (chapter 07) in the standard three-value grammar:

```
Growth rate | <this-week WoW> | <last-week WoW> | <target this week>
    Sub-line: WoW on <underlying quantity>; <this week value> vs
    <last week value> (<band relative to Graham>).
```

This is one of the six headline rows on the one-pager exercise 07
will ship. Getting the phrasing right here saves work there.

## Deliverable shape

A single Markdown file, `mod-005-exercise-03-growth-rate.md`,
structured:

```markdown
# Growth Rate — WoW and MoM Calculation — [Startup Name]

## Setup
- Underlying quantity: <name and definition>
- Data source: <where the 12-week series came from>
- Real vs. constructed weeks: <if applicable>

## The 12-week series
| Week ending | Value | WoW rate |
|---|---|---|
| YYYY-MM-DD | ... | — |
| ... | ... | ... % |

Trailing four-week average WoW: X%
Compound-annualised equivalent: N.N×

## Monthly view (weeks bucketed)
| Period | Total / average | MoM rate |
|---|---|---|
| Month 1 (weeks 1-4) | ... | — |
| Month 2 (weeks 5-8) | ... | ... % |
| Month 3 (weeks 9-12) | ... | ... % |

WoW→MoM conversion check: <one sentence>

## Yardstick calibration
<one paragraph, per Part E>

## Failure-mode audit
1. Cherry-picking the base week? <one sentence>
2. Trailing average presented as "the rate"? <one sentence>
3. Definition change mid-series? <one sentence>
4. Wrong cadence for the cycle? <one sentence>
5. Ignoring churn? <one sentence>
6. Massive week extending the trend? <one sentence>

## One-pager row
Growth rate | <this-week WoW> | <last-week WoW> | <target>
Sub-line: <definition and calibration>

## What surprised me
<two to four sentences>
```

Total length: 600–1000 words plus the tables.

## Starter guidance

- **Compute the rates by hand for at least the first two weeks
  before dragging the spreadsheet formula down.** The muscle
  memory matters more than the automation. Chapter 03's failure
  modes almost all come from copy-paste calculations that
  quietly misalign.
- **If the numbers are small (single-digit or low-tens),
  suppress the impulse to skip the exercise.** Small numbers are
  exactly where rate is most useful — 2 new customers on a base
  of 10 is 20% WoW, right on the exceptional line. Chapter 03's
  argument.
- **Do not smooth or hand-tune the series to make it match
  Graham's band.** The exercise's whole point is the honest
  reading. A 2% WoW reading in the "sub-YC-median" band is a
  useful diagnostic, not a failure.

## Acceptance criteria

You have completed the exercise when:

- [ ] The underlying quantity and its precise definition are
      recorded.
- [ ] A 12-week table of values is captured with the source
      documented (and real-vs-constructed labelled honestly).
- [ ] The WoW rate column is populated correctly.
- [ ] The trailing four-week average WoW and the compound-
      annualised equivalent are computed.
- [ ] The three-period monthly view is computed with MoM rates.
- [ ] The WoW→MoM conversion check is run and any material
      divergence noted.
- [ ] The one-paragraph Graham-yardstick calibration is written.
- [ ] All six failure-mode checks are answered in one sentence
      each.
- [ ] The one-pager row (chapter 07 grammar) is drafted.
- [ ] The write-up is committed as
      `mod-005-exercise-03-growth-rate.md`.

## Common failure modes to avoid

- **Computing the rate on the wrong denominator.** WoW is against
  the immediately-preceding week — always. Trailing averages are
  a separate number.
- **Reporting the compound-annualised multiplier and pretending
  it's the growth rate.** The 12.6× annual number is a
  visualisation of what 5% WoW compounds to; it is not "we grow
  1260% per year."
- **Skipping the failure-mode audit.** The audit is where the
  exercise's actual teaching lands. Skipping it turns the
  exercise into arithmetic.

## What good looks like

A 12-week series with real numbers, a WoW column that catches at
least one week the founder wouldn't have noticed otherwise, a
trailing-four-week average that lands honestly against Graham's
band, and a failure-mode audit that names at least one thing to
fix in the tracking. The one-pager row that comes out of Part G
is a real deliverable — it goes on chapter 07's artifact
unchanged.
