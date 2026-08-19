# Runway from Zero — Cash, Burn, Plan, Months

## Motivation

Ask ten pre-seed founders how much runway they have and about seven of
them will answer with a range and a hedge — *"probably eight or nine
months, maybe more if we don't hire"*. The hedge is the tell. The
founder has a *feeling* about how much time is left; they do not have
a *number*. Feelings degrade fast under stress; numbers do not.

The fix is small. A runway model is a spreadsheet with three inputs —
starting cash, monthly cash out, and a forward plan — and one output:
**months of runway**. Any founder who can subtract and divide can build
one in an afternoon. The reason so few PRE-SEED founders have one is
not difficulty; it is that nobody made them build it before the money
started running.

This chapter walks the smallest working runway model, cell by cell,
and reads the answer as a number of months against a specific
calendar month. Chapter 02 splits the burn line into gross, net, and
net-after-revenue. Chapter 04 fuses runway with growth into the
default-alive / default-dead composite. Everything downstream in the
module depends on the model this chapter builds.

## What a runway model actually is

At the founder-numbers level a runway model is a **12-to-24 row
spreadsheet** with one row per month. The columns are the same every
month; only the values change.

```
Month | Starting cash | Cash in | Cash out (gross) | Net cash flow | Ending cash | Cumulative burn
─────────────────────────────────────────────────────────────────────────────────────
2026-01 | $600,000    | $8,000  | $58,000          | -$50,000      | $550,000    | $50,000
2026-02 | $550,000    | $10,000 | $60,000          | -$50,000      | $500,000    | $100,000
2026-03 | $500,000    | $12,000 | $62,000          | -$50,000      | $450,000    | $150,000
...
```

That is the whole shape. Starting cash for month N is ending cash for
month N-1. Net cash flow is cash in minus cash out. Ending cash is
starting cash plus net cash flow. Runway is the row number at which
ending cash first crosses zero, expressed as *months from today*.

Everything else in a working PRE-SEED / SEED runway model is
**decoration on those seven columns**. Anything the model does that
cannot be traced back to those seven columns is either debug output
(fine) or scope creep (fix by moving to a separate model).

## The three inputs

The model has three inputs. Any founder who cannot name their values
for all three does not yet know their runway.

### Input 1 — starting cash

The single number on your bank account today. Not the number on your
last board slide, not the number after the next tranche is expected to
close, not the number you feel like you have. The number that would
transfer out if you wired it all today.

**Where to get it.** The current-balance line on the bank's landing
page. If you have multiple accounts (checking, savings, brokerage,
foreign-currency), sum them at today's exchange rate. If you have an
uncalled SAFE or an announced-but-uncashed round, do NOT count it as
starting cash; it is a *scenario* the model can run separately, not a
number in the base case.

**The self-deception this defends against.** Announcements-as-cash.
Many pre-seed founders treat a signed but unfunded round as money in
the bank. Every real invoice due before the wire hits is paid from
starting cash, not from the announcement. The base case runs on the
current-balance line and nothing else.

### Input 2 — monthly cash out (the burn)

Every dollar that leaves the bank in a normal month. This chapter
treats "burn" as a single line — gross cash out — and chapter 02 splits
it into the three flavours (gross, net, net-after-revenue). For the
model to work you only need one honest total.

A working PRE-SEED / SEED burn line breaks into roughly six
sub-categories. Every line is a founder call and every founder call
belongs in the mod-004 decision log:

| Category | Typical PRE-SEED items | Typical SEED items |
|---|---|---|
| **People — cash comp** | Two founders on modest / no salary, one contractor | Founders on market-ish salaries, two-to-four full-time hires |
| **People — benefits, payroll tax, PEO fees** | Small if no formal payroll | Meaningful — often 15–25% of cash comp |
| **Hosting, tools, infra** | AWS/GCP, GitHub, Notion, Linear, sundry SaaS | Same list, larger numbers, plus data / analytics stack |
| **Contractors, freelancers, professional services** | Legal for the incorporation and the SAFE round, a fractional designer | Legal for the priced round, accounting, occasional specialist contractors |
| **Marketing, sales, ads** | Very small; usually just tooling | Real number if the company is running paid experiments |
| **Rent, office, physical goods** | Often zero; sometimes coworking | Small office or dedicated coworking |

Each sub-category is one line in the model. The **total** is the
monthly cash out for the base case. Every sub-category value is
current-month reality, not aspirations.

**The self-deception this defends against.** Optimistic-average burn.
"Our burn is about $40k a month" often means "the two months we don't
pay the annual tools renewal, the two months we don't pay the
lawyer's invoice, the month we don't spin up the new sub-account, our
burn is $40k a month." A working burn line uses the *actual last three
months' average*, or if the company is too new for three months, an
honest itemised plan for next month with the annualised line items
correctly amortised.

### Input 3 — the forward plan

The forward plan is the month-by-month shape of *how burn will change*
because of decisions the founder has already made or is about to make.
The plan is what makes the runway model interesting; without it, the
model just extrapolates today's burn forever.

At PRE-SEED / SEED the plan has three components:

1. **Planned hires.** Each hire is a row: role, expected start month,
   monthly fully-loaded cost (base + benefits + payroll tax). Hires
   land in the burn line in the month they start.
2. **Planned non-hire spend changes.** New hosting sub-account for the
   staging environment (month 3, +$1,200/mo). New paid-ads
   experiment (month 5, +$4,000/mo). Annual legal renewal (month 8,
   one-time $6,000).
3. **Planned cash in.** A tranche of a SAFE closing in month 4
   (+$150,000 one-time). A grant landing in month 7 (+$25,000
   one-time). Do NOT include the *expected but unsigned* round —
   that is a scenario, not the base case.

Every item in the plan is *dated* to a specific month and has a
*source* — a signed offer, a signed SAFE, a signed vendor contract, or
a mod-004 decision-log entry authorising the spend. Items with no
source do not go in the base plan; they can be run as a scenario.

**The self-deception this defends against.** The "we'll hire when we
raise" plan. Founders often carry hires in their head as "conditional
on the round closing" and therefore never put them in the model. Then
the round closes and the hires all land in the same month and the burn
jumps 60%. The model catches this if the hire rows are dated to their
*plan* start month, with a note *"if round closes on time"* — the
model runs the base case without them and the scenario with them, so
the founder sees both.

## The single formula

The model has exactly one arithmetic move that isn't trivial. Every
month:

```
ending_cash[m] = ending_cash[m-1] + cash_in[m] - cash_out[m]
```

with `ending_cash[m=0] = starting_cash`.

Everything else in the model is a lookup or a rollup. If you can
express that one line as a spreadsheet formula and drag it down 24
rows, the model runs.

Runway in months is derived from ending cash:

```
runway_months = the smallest m for which ending_cash[m] < 0
```

Two variants of the same number are also useful:

- **Runway from cash / burn (constant-burn approximation)**:
  `runway_months ≈ current_cash / avg_monthly_net_burn`. Useful as
  a sanity check and as the number you can carry in your head.
- **Runway from the full model (variable-burn projection)**: the row
  number where ending cash goes negative in the actual month-by-month
  projection. This is the answer the model exists to give.

The two numbers can differ substantially when the forward plan has
step-changes — a big hire month, an annual renewal, a marketing push.
Chapter 02 explores why the two numbers diverge, but even in this
chapter the pattern is important: **the constant-burn approximation
is a check; the month-by-month projection is the answer**.

## A worked example

Take a hypothetical two-founder PRE-SEED SaaS company as of
2026-01-01.

**Starting cash**: $600,000 (from a $650,000 SAFE round closed in
2025-11; ~$50,000 spent since).

**Base monthly cash out** (average of the last three months):

- Two founders, $6,000/mo each cash: $12,000
- One contractor engineer, $8,000/mo: $8,000
- Hosting + tools + SaaS: $2,500
- Legal / accounting retainer: $1,500
- Marketing (tooling only): $500
- Rent (coworking, two seats): $1,000

Base monthly cash out: **$25,500**.

**Base monthly cash in**: three pilot customers at $2,500/mo, one
long-term ARR customer at $1,000/mo: **$8,500**.

**Base monthly net cash flow**: $8,500 − $25,500 = **−$17,000**.

**Forward plan**:

- Month 4 (2026-04): hire first full-time engineer, $12,000/mo fully
  loaded.
- Month 6 (2026-06): annual legal renewal, one-time $8,000.
- Month 7 (2026-07): move to a real 3-seat coworking, +$1,000/mo
  ongoing.
- Month 9 (2026-09): expected close of a second SAFE round —
  **NOT in base case; scenario only.**

**Constant-burn approximation**:
`$600,000 / $17,000 ≈ 35.3 months`.

**Full model projection (base case, no scenario cash in)**:

| Month | End cash | Runway remaining |
|---|---|---|
| 2026-01 | $583,000 | 34 |
| 2026-04 | $520,000 | 27 (hire lands, burn jumps to −$29,000/mo) |
| 2026-06 | $454,000 | 21 (legal renewal, one-off) |
| 2026-07 | $424,000 | 19 (coworking bump to −$30,000/mo) |
| ... | ... | ... |
| 2027-12 | ≈ −$8,000 | 0 — first month below zero |

Runway from the full model: **~23 months from 2026-01**, ending in
approximately 2027-12. The constant-burn approximation (35 months)
was significantly optimistic because it did not account for the
month-4 hire or the coworking bump.

That single insight — *the hire I'm planning cuts a year off my
runway* — is the reason the model exists. Nothing else in the module
matters if the founder does not see this trade-off explicitly.

## Reading the number

The runway number is the answer. Two more numbers make it
actionable.

**The date, not just the count.** Runway is more legible when
expressed as a *calendar month* (*"we run out of cash in
2027-12"*) than as a *count* (*"we have 23 months"*). Counts get
stale as time passes; dates do not. The mod-004 metrics one-pager
should carry both.

**The zone.** A working PRE-SEED / SEED convention is to bucket
runway into three zones:

- **Green** — 18 months or more. There is time for one full
  fundraise cycle and one full quarter of execution against a plan.
- **Yellow** — 9 to 18 months. Fundraise timing starts to constrain
  execution timing; a fundraise conversation has to be underway or
  very close to underway.
- **Red** — under 9 months. Every decision is now a runway decision.
  Fundraise is the only priority that isn't a fundraise. Non-critical
  hires stop. Non-critical spend stops.

The zone boundaries are not laws of physics — different founders and
different investors use slightly different lines. The important
property is that *there is a boundary at all*, and the boundary is
declared *before* the runway hits it, not after.

Chapter 04 uses the same zones inside the default-alive / default-dead
composite; this chapter is the point at which the zone is first
declared.

## Update cadence

The runway model is a **weekly-touched, monthly-reconciled** artifact:

- **Weekly (Friday, part of the mod-004 shipped-and-learned)**: read
  starting cash from the bank, update the current-month row, refresh
  the runway number on the founder-numbers one-pager.
- **Monthly (last business day)**: reconcile the actual month's cash
  in and cash out against the plan, roll the projection forward one
  month, and note any forward-plan changes since last reconciliation.
- **Per major decision**: any decision-log entry that changes hires,
  spend, or expected cash in gets reflected in the plan the day the
  decision is made. The model is one of the outputs of the mod-004
  "allocate" step.

If the model is only touched during fundraises, it is a fundraise
model, not a runway model. Runway models get looked at every week.
Fundraise models get looked at every quarter and re-built from
scratch each time.

## Common failure modes

Five failure modes are common enough to name up front.

**1. Running only the constant-burn approximation.** The
`cash / burn` heuristic is fine for a sanity check and useless as the
model of record. Any decision that step-changes burn — a hire, an
annual renewal, a paid-marketing push — is invisible to the
approximation and central to the projection.

**2. Modelling in "months from now" instead of dated months.**
"Month 6" is ambiguous the moment two weeks pass. Dated rows
(2026-01, 2026-02, ...) survive time; abstract rows do not.

**3. Counting unsigned money in the base case.** The base case
runs on money already in the account. Announcements, verbal
commits, "expected" tranches, and pipeline SAFEs run as *scenarios*
in a separate column, clearly labelled. Founders who fold the
scenario into the base case discover the difference the hard way.

**4. Ignoring the semi-annual and annual costs.** Legal renewals,
insurance premiums, annual SaaS bills, tax filings, and the
end-of-year accountant invoice do not fit inside a monthly-average
approximation. They belong as one-time entries in the specific
months they land in.

**5. Never updating the model.** A model that hasn't been touched
in six weeks is a snapshot, not a model. The weekly touch and
monthly reconciliation are what keep the runway number honest;
without them, the founder is again working from a feeling.

## Summary

- A runway model is a spreadsheet with three inputs — starting cash,
  monthly cash out, a forward plan — and one output: months of runway.
- Every row is a dated month; every value is defensible from bank
  statements, signed offers, and mod-004 decision-log entries.
- The single formula is
  `ending_cash[m] = ending_cash[m-1] + cash_in[m] - cash_out[m]`.
  Everything else is a lookup or a rollup.
- The runway number should be expressed as both a *count of months*
  and a *calendar month* — dates survive time, counts don't.
- The zone (Green / Yellow / Red) is declared before it is hit, not
  after, and it is the boundary that turns runway from a number into
  a call.
- The model is weekly-touched, monthly-reconciled, and
  per-decision-updated. A model that only gets touched during
  fundraises is a fundraise model, not a runway model.

## Homework

Exercise 01 (`Build a Runway Model from Zero`) is where this chapter
first gets exercised — build the seven-column, 24-row model for a
real (or realistic) startup, defend every input against its source,
and read the runway as both a count and a calendar month. Exercise
04 (`Default Alive or Default Dead — Scenarios`) uses the same
model with the growth-side inputs added; if the model from exercise
01 is well-built, exercise 04 is an extension rather than a
rewrite.
