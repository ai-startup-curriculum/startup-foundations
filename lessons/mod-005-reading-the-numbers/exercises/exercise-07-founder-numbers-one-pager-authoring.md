---
module: mod-005-reading-the-numbers
exercise: exercise-07
slug: founder-numbers-one-pager-authoring
hours: 3
prereqs: [chapter-07-founder-numbers-one-pager, exercise-01-build-a-runway-model-from-zero, exercise-04-default-alive-or-default-dead-scenarios, exercise-06-north-star-metric-selection-and-defence]
---

# Exercise 07 — Founder-Numbers One-Pager Authoring

## Problem statement

Chapter 07 formalised the founder-numbers one-pager — six headline
rows in a three-value grammar, one sub-line each, weekly-touched,
readable in 90 seconds, serving both the internal Monday-Wednesday-
Friday operating cadence and the external candidate-investor /
candidate-hire audience. This exercise ships the first real (or
realistically-specified) version of that one-pager for the startup
used across the module and drops it into the same folder as the
mod-004 cadence artifacts.

The exercise is the module's capstone artifact. Every earlier
chapter's teaching lands on one specific row of this page. Exercise
01 populates the cash and runway rows. Exercise 02 populates the
net-burn row (with the two sub-line variants). Exercise 03
populates the growth-rate row. Exercise 04 populates the default-
alive / default-dead row and its reason sub-line. Exercise 06
populates the North-Star row and its definition sub-line. This
exercise assembles them.

## Requirements

### Part A — check the pre-reqs are in place (about 15 min)

Confirm you have completed each of the pre-req exercises and can
locate the specific outputs each produced:

- **Exercise 01 (`Build a Runway Model from Zero`)** — you need
  the current cash balance, the current monthly net burn, the
  computed runway in months, and the calendar end date.
- **Exercise 02 (`Gross vs Net Burn Drill`)** — you need the three
  burn variants (gross, net, net-after-variable-revenue) for the
  current month.
- **Exercise 03 (`Growth Rate — WoW and MoM Calculation`)** — you
  need the current growth rate at the correct cadence for your
  stage (WoW at PRE-SEED, MoM at post-PMF).
- **Exercise 04 (`Default Alive or Default Dead — Scenarios`)** —
  you need the current default-alive / default-dead verdict with
  its one-sentence reason.
- **Exercise 06 (`North-Star Metric Selection and Defence`)** —
  you need the chosen North-Star, its current value, its
  prior-period value, its target, and its precise definition.

If any of the five pre-req outputs are missing or stale, go back
and complete or refresh that exercise first. The one-pager
cannot be assembled from placeholders on more than one row —
chapter 07's failure-mode section is explicit that a one-pager
with real numbers on some rows and placeholders on others is
worse than no one-pager, because it teaches the reader (and the
founder themselves) that some rows are optional.

**Deliverable A**: a short table listing each pre-req exercise
and the specific value or artifact it contributes. This table
belongs at the top of the exercise write-up as a provenance
audit.

### Part B — assemble the six headline rows (about 45 min)

Compose the one-pager in the shape from chapter 07:

```
Founder-Numbers One-Pager
────────────────────────────────────────────────────────────
Startup: [Company name]                  As of: [ISO date]
Stage: [PRE-SEED / SEED / ...]           Author: [founder]

Metric                | Current | Prior | Target
────────────────────────────────────────────────────────────
Cash on hand          | [$]     | [$]   | [$]
    [sub-line: source and date]

Net burn (monthly)    | [$]     | [$]   | [≤$]
    [sub-line: gross, net, net-after-variable-revenue]

Growth rate           | [%]     | [%]   | [≥%]
    [sub-line: cadence, underlying quantity, base for context]

Runway                | [~mo]   | [~mo] | [≥mo]
    [sub-line: projected end date; zone GREEN/YELLOW/RED]

Default alive/dead    | [verdict]| [verdict]| [verdict]
    [sub-line: one-sentence reason]

North-Star            | [value] | [value]| [target]
    [sub-line: precise definition from exercise 06]

Unit economics: deferred to startup-finance-fundraising-
curriculum unit-economics module (stage: SERIES-A).
Current stage: [PRE-SEED].
────────────────────────────────────────────────────────────
```

Row-level discipline:

- **Cash on hand.** The number is as-of a specific date and time.
  The sub-line names the source (bank balance, treasury sweep,
  operating account only, etc.). If the number is more than one
  business day stale, refresh it before writing.
- **Net burn.** The current-value column is *net* burn. The
  sub-line carries all three variants (gross, net, net-after-
  variable-revenue). Chapter 02 was explicit that a one-pager
  showing only net burn hides the two self-deceptions.
- **Growth rate.** The cadence is stage-appropriate: WoW at
  PRE-SEED / early-SEED, MoM at post-PMF. The sub-line names the
  underlying quantity (the metric the rate is computed against
  — often, but not always, the same as the North-Star). Chapter
  07 flagged the "growth rate on a different metric than the
  North-Star" failure mode; if the two do differ, the sub-line
  should explain why.
- **Runway.** All three of: months, calendar end date, and zone
  (Green / Yellow / Red). Chapter 07 was explicit that a
  months-only runway row is correct today and wrong in three
  weeks.
- **Default alive/dead.** A verdict word (ALIVE or DEAD), not
  "TBD" or blank. The sub-line is the one-sentence reason in
  the shape from chapter 04 — the same shape as a mod-004
  decision-log reason.
- **North-Star.** Current value, prior value, target. The sub-line
  is the precise definition from exercise 06.

The deferral footer for unit economics is required. It signals
to any reader — internal or external — that the one-pager is
not trying to cover the unit-economics depth, and points at the
owning pillar.

### Part C — the 90-second read test (about 15 min)

Chapter 07 named a specific acceptance test: a reader should be
able to answer six questions in 90 seconds from the one-pager
alone. Print or export your one-pager, set a 90-second timer,
and hand it to someone (a co-founder, a partner, another
Foundations learner) who has not seen the numbers before. Ask
them to answer these six questions from the page:

1. How much money does the company have?
2. How fast is that money running out?
3. Is the company growing, and how fast?
4. How much time is left?
5. Does the trajectory reach profitability first, or does the
   cash run out first?
6. What one number best measures the value being delivered?

If the reader can answer all six unaided in 90 seconds, the
one-pager passes. If any one of the six is unanswerable, the
corresponding row is broken; identify which row and fix it.

If you cannot easily recruit an outside reader, run the test
against yourself with a 24-hour cooling-off: refresh the
one-pager on day 1, set it aside, and try to answer the six
questions from it on day 2 without referring to any other
artifact. The self-test is weaker than the outside-reader test
but stronger than no test at all.

**Deliverable C**: a short note (three-to-five sentences) on the
read-test outcome — who read it (or that it was self-tested),
which of the six questions took the longest, and any row you
fixed as a result of the test.

### Part D — the six failure-mode checks (about 30 min)

Chapter 07 named a specific failure-mode check for each of the
six headline lines. Run all six against your one-pager:

1. **Cash on hand check.** Is the current number equal to the
   bank balance (or the sum across accounts) today? If it
   differs by more than a few percent, the row is stale.
2. **Net burn check.** Do gross, net, and net-after-variable-
   revenue all appear on the sub-line? If only net burn is
   visible, add the other two.
3. **Growth rate check.** Is the cadence stage-appropriate? Is
   the underlying quantity the North-Star (or, if not, is the
   difference explained in the sub-line)?
4. **Runway check.** Does the row have months, calendar end
   date, and zone — all three?
5. **Default alive/dead check.** Is there a verdict word (not
   TBD, not blank) with a one-sentence reason?
6. **North-Star check.** Is the sub-line definition specific
   enough that a new hire could compute the number without
   asking a question?

Produce a **check table** listing each of the six lines and its
verdict (Pass / Fix-required / Fixed). Do not silently fix
issues — document the check outcome and the fix.

### Part E — the mod-004 interlock (about 15 min)

Chapter 07 argued the founder-numbers one-pager is *the founder-
numbers section* of the mod-004 weekly metrics one-pager
(mod-004 chapter 02, exercise 05). This part fires that
interlock:

- **Save the founder-numbers one-pager into the same folder as
  your mod-004 cadence artifacts.** If you did mod-004
  exercise 05, that folder already exists
  (`mod-004-exercise-05-cadence/` or similar). If not, create a
  folder — `founder-cadence/` — that will hold both modules'
  weekly artifacts from this month forward.
- **Update the mod-004 metrics one-pager (or draft the first
  version if mod-004 was completed without one) so its
  founder-numbers section is the six-line block from this
  exercise.** The mod-004 metrics one-pager has three sections
  (founder-numbers, North-Star and supporting, this-week's
  watch-list); this exercise fills the first two.
- **Write two-to-three sentences in the exercise write-up** on
  what changed about the mod-004 metrics one-pager once the
  founder-numbers section became real (versus the placeholders
  that were there from mod-004 exercise 05).

If mod-004 was not completed, note that in the write-up and skip
the mod-004 side of the interlock; the founder-numbers one-pager
still gets saved to a `founder-cadence/` folder for future
integration.

### Part F — the weekly-touch discipline plan (about 15 min)

Chapter 07 named the weekly-touch discipline:

- Monday morning (5 min): read; note which lines look wrong;
  the wrong-looking lines become "decisions expected this week"
  on the mod-004 Monday plan.
- Wednesday (10 min): check the two most volatile lines
  (usually cash and growth); refresh if either jumped.
- Friday afternoon (15 min): full refresh of every headline and
  sub-line; roll "current" into "prior."

Plus the monthly reconciliation (30–60 min, last business day)
against the runway model from exercise 01.

Write a short **cadence commitment** — four-to-six sentences on:

- When (specific day and rough time) you will do the Monday,
  Wednesday, Friday, and last-business-day touches.
- Which artifact you will use as the "source of truth" for each
  line (the runway model for cash and runway; the North-Star
  data source from exercise 06 for the North-Star; the growth-
  rate calculation from exercise 03).
- One specific failure mode of the weekly touch you are most
  likely to fall into (e.g., "I will skip Wednesday when travel
  disrupts the week"), and what defence you will build in
  advance.

The cadence commitment is what turns the one-pager from a
one-time exercise into the actual weekly artifact chapter 07
argued for.

## Deliverable shape

A **folder** — `founder-cadence/` (shared with mod-004, if
present) — containing at minimum:

- `founder-numbers-one-pager.md` — the one-pager itself, in the
  shape from chapter 07.
- `mod-005-exercise-07-one-pager.md` — the exercise write-up
  containing the provenance audit (Part A), the read-test note
  (Part C), the six-failure-mode check table (Part D), the
  mod-004 interlock note (Part E), and the cadence commitment
  (Part F).

If mod-004 exercise 05 was completed, also update the mod-004
metrics one-pager per Part E; the updated file lives in the
same folder.

Total length: 800–1300 words across the exercise write-up. The
one-pager itself stays under one page (roughly 200–350 words
including all six sub-lines and the deferral footer).

## Starter guidance

- **Do not skip the provenance audit (Part A).** The one-pager
  is only as trustworthy as the exercises upstream of it. If any
  of the five pre-reqs are missing, the corresponding row
  becomes a placeholder — and chapter 07 argued that a one-pager
  with mixed real / placeholder rows is worse than none.
- **Use the runway model as the source of truth for cash and
  runway.** The one-pager is the *summary*; the model is the
  source. When they drift (they always do), snap the one-pager
  back to the model on the monthly reconciliation. Do not the
  other way around.
- **Do the outside-reader read test if at all possible.** The
  self-read test is a fallback. Ninety seconds is a tighter
  ceiling than it sounds; a reader who has not seen your
  numbers before will surface row-level failures the founder is
  too close to see.
- **The deferral footer is not optional.** Chapter 07 included
  it in the example one-pager on purpose. It signals to every
  reader that the one-pager is honestly scoped and points at
  the owning pillar for the depth it doesn't cover. Do not
  drop it.
- **Do not add rows.** Chapter 07's first failure mode is "the
  one-pager becomes a two-pager." Six headline rows plus six
  sub-lines plus the deferral footer. Anything else — CAC,
  LTV, payback, gross margin, retention rate, top customer
  concentration — belongs on a supporting artifact or in the
  underlying model, not on this page.

## Acceptance criteria

You have completed the exercise when:

- [ ] The provenance audit table names each of the five pre-req
      exercises and the specific value or artifact each
      contributed.
- [ ] The one-pager contains all six headline rows in the
      three-value grammar (current, prior, target), each with a
      populated sub-line carrying the row's key detail.
- [ ] All values are real (or realistically-specified from the
      pre-req exercises), not placeholders on more than one
      row.
- [ ] The unit-economics deferral footer is present.
- [ ] The 90-second read test was run (outside reader preferred,
      self-test acceptable) and the result is documented,
      including any row that was fixed as a result.
- [ ] The six-failure-mode check table lists each of the six
      lines with a Pass / Fix-required / Fixed verdict, and any
      fixes were documented rather than silently applied.
- [ ] The one-pager is saved into the same folder as the
      mod-004 cadence artifacts (or a new `founder-cadence/`
      folder if mod-004 was not completed).
- [ ] If mod-004 exercise 05 was completed, the mod-004 metrics
      one-pager was updated so its founder-numbers section is
      the block from this exercise.
- [ ] The cadence commitment names when the weekly and monthly
      touches will happen and one specific failure mode you
      plan for.
- [ ] The exercise write-up is committed as
      `mod-005-exercise-07-one-pager.md`.

## Common failure modes to avoid

- **Placeholders on multiple rows.** Chapter 07 was explicit —
  a one-pager with real numbers on some rows and placeholders
  on others teaches the reader some rows are optional. If more
  than one row cannot be populated from real data, go back and
  complete the missing pre-req exercise first.
- **Runway in months only.** Correct today, wrong in three
  weeks. Every runway row has months, calendar end date, and
  zone.
- **A blank or "TBD" default-alive / default-dead row.** The
  module builds to this verdict. A one-pager that skips it is
  running every other row's numbers with no summary judgment.
- **Growth rate on a different metric than the North-Star,
  without explanation.** Chapter 07 flagged this. Either the
  two match, or the sub-line explains why they don't.
- **Skipping the read test.** The 90-second read is the
  acceptance test, not a nice-to-have. A one-pager that has
  not been read against the timer might still fail the test
  the first time an actual candidate investor picks it up.
- **Skipping the cadence commitment.** The one-pager is a
  weekly-touched artifact. A one-pager authored once and never
  refreshed is a stale artifact by the second week. The cadence
  commitment is what makes the one-pager the ongoing artifact
  chapter 07 argued for.

## What good looks like

A one-pager a co-founder can read on Sunday night, a first hire
can read on their first day, and a candidate investor can read
in the first two minutes of a pitch meeting — and each of them
can answer the six chapter-07 questions unaided. The same file
survives the mod-004 weekly cadence: Monday morning the founder
opens it, notes which rows look wrong, and rolls those into the
week's plan.

The most useful signal is that **updating the one-pager on
Friday takes fifteen minutes, not an hour**. Fifteen-minute
Friday updates mean the runway model, the North-Star data
source, and the growth-rate calculation are all in place and
current. Hour-long Friday updates mean the underlying artifacts
are stale and the Friday touch is doing their work for them.

The one-pager you ship here is the same artifact you carry for
the rest of your founder career at this stage. When the stage
shifts (SEED → SERIES-A), one or more rows will change (the
North-Star will likely evolve; the growth-rate cadence will
likely shift from WoW to MoM); the *shape* stays the same. That
is the whole discipline the module has been installing.
