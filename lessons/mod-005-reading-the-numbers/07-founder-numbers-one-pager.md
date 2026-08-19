# The Founder-Numbers One-Pager

## Motivation

Everything in chapters 01–06 is upstream of one artifact: a **single
page**, readable in **90 seconds**, that answers every founder-
numbers question a co-founder, a first employee, or a candidate
investor could ask this week. Not a dashboard. Not a spreadsheet.
Not a deck. One page.

The one-pager is what turns the module's concepts into a habit. A
founder who has read the module but doesn't ship the one-pager
still can't answer *"how much runway do you have?"* in one number.
A founder who ships the one-pager and updates it every Friday can
answer the question — and every follow-up — from memory, because
the shape of the answer is fixed.

This chapter formalises the one-pager: what rows go on it, what
each row means, how it interlocks with the mod-004 metrics
one-pager, and the specific ways one-pagers go bad.

## The six headline lines

A working founder-numbers one-pager has exactly six headline lines.
Each corresponds to one prior chapter.

| # | Headline line | Chapter |
|---|---|---|
| 1 | **Cash on hand** (as of a specific date) | 01 |
| 2 | **Net burn** (monthly, current) | 02 |
| 3 | **Growth rate** (WoW or MoM at stage) | 03 |
| 4 | **Runway** (months + calendar date + zone) | 01 |
| 5 | **Default alive / Default dead** (verdict) | 04 |
| 6 | **North-Star metric** (name + current value + last-week + target) | 06 |

Six lines. Every line is one row. Every row is populated by a real
number, not a placeholder. The whole page fits on one screen
without scrolling.

## The row grammar

Each of the six headline lines uses the same three-value grammar
that mod-004's metrics one-pager uses:

```
<Metric name> | <current value> | <last-week / last-month value> | <target for this week / month>
```

- **Metric name** — the short label. Not the full definition; the
  definition lives on a separate line at the bottom of the sheet.
- **Current value** — the number as of the reading date (Friday
  afternoon for the weekly update).
- **Last-week or last-month value** — the same number, one period
  ago. The comparison is what makes movement visible.
- **Target** — what the founder committed on Monday (or the first of
  the month) the value should be at the end of the period. Missing
  targets and hitting targets are both signals.

The three-value grammar is intentional. A one-pager with only the
current value hides all movement; a one-pager with only movement
hides the level. Three values per row is the smallest shape that
carries both.

## The sub-line detail

Below each of the six headline lines is one indented **sub-line**
carrying the important detail the headline abstracted away. Six
sub-lines total — one per headline row. Together they turn six
numbers into a fully-defensible picture without spilling into a
second page.

**Cash on hand — sub-line**: the source of the number and the date
it was read. *"Bank balance across two accounts, USD equivalent, as
of 2026-01-31 4:00pm."*

**Net burn — sub-line**: gross burn *and* net-burn-after-variable-
revenue, so the reader can see the delta from chapter 02. *"Gross
burn $37.5k, net burn $17k, net burn after variable revenue $29k
(one-off R&D rebate this month)."*

**Growth rate — sub-line**: the cadence (WoW / MoM), the underlying
metric, and the base for context. *"WoW on paying customers; 26
this week vs 22 last week."*

**Runway — sub-line**: the calendar date runway ends and the zone
(Green / Yellow / Red). *"~23 months, projected end 2027-12,
zone: GREEN."*

**Default alive / Default dead — sub-line**: the one-sentence
reason for the verdict, written the same way as a mod-004 decision-
log reason. *"DEFAULT ALIVE — at 4% WoW growth on paying customers,
projected MRR crosses monthly expense at ~month 10, before cash
runs out at ~month 23."*

**North-Star — sub-line**: the precise definition. *"Meetings
scheduled per week per active account, distinct accounts with ≥1
user login in Mon–Sun window."*

## An example one-pager

```
Founder-Numbers One-Pager
────────────────────────────────────────────────────────────
Startup: [Company name]                  As of: 2026-01-31
Stage: PRE-SEED                          Author: [founder]

Metric                | Current | Prior | Target
────────────────────────────────────────────────────────────
Cash on hand          | $600k   | $625k | $600k
    Bank balance across two accounts, USD equivalent,
    as of 2026-01-31 16:00.

Net burn (monthly)    | $17k    | $18k  | ≤$25k
    Gross burn $37.5k, net burn $17k, net burn after
    variable revenue $29k (one-off R&D rebate this month).

Growth rate           | 4% WoW  | 3% WoW| ≥5% WoW
    WoW on paying customers; 26 this week vs 22 last week
    (below Graham 5–7% band but trending up).

Runway                | ~23mo   | ~24mo | ≥18mo
    Projected end 2027-12; zone: GREEN.

Default alive/dead    | ALIVE   | ALIVE | ALIVE
    At 4% WoW growth on paying customers, projected MRR
    crosses monthly expense at ~month 10, before cash runs
    out at ~month 23.

North-Star            | 3.2     | 2.9   | ≥4.0
    Meetings scheduled per week per active account
    (accounts with ≥1 user login, Mon–Sun window).

Unit economics: deferred to startup-finance-fundraising-
curriculum unit-economics module (stage: SERIES-A).
Current stage: PRE-SEED.
────────────────────────────────────────────────────────────
```

That is the whole page. A reader who cannot answer *"how are the
numbers?"* from those six rows in 90 seconds is looking at a
one-pager that broke somewhere.

## The 90-second read test

The name "one-pager readable in 90 seconds" is not a slogan; it is
the acceptance test. The specific things a reader should be able to
answer, unaided, after 90 seconds with the page:

1. How much money does the company have?
2. How fast is that money running out?
3. Is the company growing, and how fast?
4. How much time is left?
5. Does the trajectory reach profitability first, or does the cash
   run out first?
6. What one number best measures the value being delivered?

If any of the six is unanswerable in 90 seconds, the corresponding
row is broken. Common breakage patterns are listed under Common
failure modes below.

## Where the one-pager sits in the mod-004 cadence

The founder-numbers one-pager is *the founder-numbers section* of
the mod-004 weekly metrics one-pager (mod-004 chapter 02). Mod-004
chapter 02 formalises a three-section metrics one-pager: (1)
founder-numbers, (2) North-Star and supporting numbers, (3)
this-week's watch-list. Mod-005's one-pager fills sections 1 and 2
with the specific rows in this chapter.

Concretely:

- The **six headline rows** map to sections 1 and 2 of the mod-004
  metrics one-pager.
- The **sub-lines** are the mod-004 definition rows.
- The **watch-list** (mod-004 section 3) is populated by whichever
  quarterly OKR key-result the current week is advancing (mod-004
  chapter 04); it is not owned by mod-005.

The interlock is intentional. A founder running the mod-004 cadence
already reads a metrics one-pager on Wednesday and updates it on
Friday. Mod-005's job is not to add a second artifact to that
cadence; it is to give the top two sections of that artifact
defensible content.

## Update discipline

The one-pager is a **weekly-touched** artifact:

- **Monday morning (5 minutes)** — read; note which lines look
  wrong; the wrong-looking lines go into the mod-004 Monday plan
  as "decisions expected this week."
- **Wednesday (10 minutes)** — check the two most volatile lines
  (usually growth rate and cash on hand); refresh if either
  jumped.
- **Friday afternoon (15 minutes)** — full refresh. Update every
  headline value and sub-line. Compute the new WoW growth rate.
  Re-run the default-alive / default-dead call if any input
  materially changed. Move the "prior" column to what "current"
  was last Friday, and put the new number in "current."

Once a month (last business day), do a longer reconciliation
(30–60 minutes) against the runway model — see chapter 01. The
one-pager is the *summary*; the model is the *source of truth*. The
one-pager can drift from the model between reconciliations, but
the monthly close snaps it back.

## The six failure-mode checks

Each of the six headline lines has a specific failure mode. Running
them once a month as an honesty check catches most drift.

**Cash on hand — the check.** Is the number today equal to the
current bank balance (or the current balance summed across
accounts)? If it differs from the bank by more than a few percent,
something is stale. Update.

**Net burn — the check.** Do gross, net, and net-after-variable-
revenue all appear? If only net burn is visible, the founder is at
risk of the chapter-02 self-deception. Add the other two.

**Growth rate — the check.** Is the cadence appropriate to the
stage (WoW at PRE-SEED, MoM at post-PMF)? Is the underlying quantity
the North-Star? If the growth-rate row is measured on a metric
different from the North-Star row, one of the two is not really
the primary metric.

**Runway — the check.** Is the number in months, the calendar end
date, *and* the zone (Green / Yellow / Red)? All three, always.

**Default alive / dead — the check.** Is a verdict actually
present, with a reason? A one-pager that reads "TBD" or is blank
on this row has skipped the composite call that is the reason the
one-pager exists.

**North-Star — the check.** Is the definition on the sub-line
detailed enough that a new hire could compute the number without
asking a question? If not, the definition needs work (chapter 06).

## Two audiences the one-pager is designed for

The one-pager is a single artifact serving two different audiences.
The row shape has to work for both.

### The internal audience — you, your co-founder, the first hire

The Monday-Wednesday-Friday cadence is the internal use. The
one-pager tells the operator team where the week stands on the six
things that matter most for survival and growth. It sits alongside
the mod-004 Monday plan and Friday shipped-and-learned. Nobody
outside the operating team ever needs to see it for this use.

### The external audience — a candidate co-founder, a candidate first employee, a candidate investor

The one-pager is also the artifact you hand over when someone
outside the company asks "what does the numbers picture look like?"
The advantage of the same one-pager serving both audiences is that
you never have to build a "just for external eyes" version and
therefore never have to keep two copies in sync. The disadvantage
is that the one-pager cannot include anything you would not want an
outside candidate investor to see; the mod-004 decision log and
other private context stay in their own files.

If the one-pager is honest for the internal use, it is
appropriate for the external use. Any place where those two
requirements diverge is a signal that the internal artifact is
carrying self-serving language.

## Common failure modes

Six failure modes worth naming.

**1. The one-pager becomes a two-pager.** More lines seem more
useful; they are not. The 90-second read is the property that
distinguishes this artifact from a dashboard. Six headline lines,
six sub-lines. Anything more goes into the underlying model.

**2. Values without units, dates, or scope.** *"Cash: 600"* is
useless. *"$600,000, USD, as of 2026-01-31 16:00, two accounts
summed"* is what the sub-line is for. Every number has units, a
date, and a scope.

**3. No target column.** Two-value one-pagers (current + prior)
hide the plan-vs-actual gap. Three-value one-pagers (current +
prior + target) make it visible on the page.

**4. Growth rate on a different metric than the North-Star.** If
line 3 (growth rate) is computed on paying customers and line 6
(North-Star) is meetings-per-account, one of them is the primary
metric and the other is a supporting metric — pick one and demote
the other. Chapter 06 has the argument.

**5. Runway in months but no calendar date.** *"~23 months"* is
correct today and wrong in three weeks (it is now ~20 months and
nobody updated the row). Calendar dates survive time; month-counts
don't.

**6. A blank or "TBD" default-alive / default-dead line.** The
whole module builds to this call. A one-pager that skips it is
carrying every other row's numbers with no summary judgment; that
is the pattern chapter 04 is arguing against.

## Summary

- The founder-numbers one-pager has **six headline lines** and one
  sub-line each: cash, net burn, growth rate, runway,
  default-alive/dead, North-Star.
- Each row uses the same three-value grammar: current, prior,
  target.
- The 90-second read test is the acceptance criterion — a reader
  can answer six specific questions in 90 seconds.
- The one-pager is the founder-numbers section of the mod-004
  weekly metrics one-pager; it lives in the same cadence.
- Weekly touch, monthly reconciliation against the runway model.
- The same one-pager serves the internal (Monday-Wednesday-Friday
  operating) and external (candidate co-founder / hire / investor)
  audiences — if it works for the first, it works for the second.

## Homework

Exercise 07 (`Founder-Numbers One-Pager Authoring`) ships the
first real version of the one-pager against the startup used in
prior exercises. The one-pager from exercise 07 goes into the same
folder as the mod-004 cadence artifacts — the two integrate as one
weekly cadence from then on.
