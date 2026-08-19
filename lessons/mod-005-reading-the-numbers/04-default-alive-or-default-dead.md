# Default Alive or Default Dead — The Composite Call

## Motivation

Runway alone is a survival number in isolation. Growth alone is a
trajectory number in isolation. Neither one, on its own, tells the
founder whether the trajectory reaches profitability before the
runway ends. That is the founder's single most consequential
composite call, and Paul Graham gave it a name: **Default Alive or
Default Dead**.

Graham's 2015 essay `Default Alive or Default Dead?` argues that
almost every startup that raises money should routinely ask *"at our
current growth rate, does our current runway last long enough that
we reach profitability from our current spend plan?"* — and that too
many founders never ask the question until the answer has already
turned bad.

This chapter formalises the composite so a Foundations graduate can
make the call for their own startup in under half an hour, defend
the answer against an investor's push-back, and re-run it every time
a mod-004 decision-log entry changes one of the inputs.

## The composite in one sentence

**Default alive** is the state where, holding your current spend
plan and applying your current growth rate to your current revenue
line, the projected monthly revenue crosses the projected monthly
expense line *before your projected cash balance goes to zero*.

**Default dead** is the state where, on the same projection, the
cash balance goes to zero first.

Graham's own framing:

> A startup is *default alive* if it will become profitable before
> the runway runs out, and *default dead* if it won't, assuming its
> current expenses and growth rate.

That is the definition. Everything else in this chapter is
mechanics.

## The four inputs

The composite has exactly four inputs. All four are already available
if you have done the prior chapters and the mod-004 loop.

1. **Current cash** — from chapter 01 (the runway model input).
2. **Current net burn** — from chapter 02, ideally
   net-burn-after-variable-revenue if the two diverge, so the
   projection is honest.
3. **Current growth rate** — from chapter 03, as WoW or MoM at
   whatever cadence your stage prefers, applied to whatever
   underlying quantity is your North-Star (chapter 06). For the
   composite you need the *revenue growth rate specifically*; if
   your North-Star is not revenue, you also need a defensible
   translation from the North-Star to revenue.
4. **Current hiring / spend plan** — from chapter 01's forward plan.
   The hires and spend changes that will land in the projection
   window.

Note what is **not** on the list: fundraising expectations, hoped-for
new products, hoped-for market shifts. The composite is deliberately
run against *current* everything. Scenarios where those things change
are legitimate — chapter 04 encourages running them — but the base
case is what you have today.

## The mechanics — a projection with two lines

The composite is a single projection with two lines drawn against a
common time axis: the *revenue line* (projected forward from the
growth rate) and the *expense line* (projected forward from the
current plan). A cash line, the sum of the two, is the third element.

### Step 1 — project revenue forward

Start with current monthly recurring revenue (or the honest revenue
proxy for your business model). Apply the current growth rate month
over month:

```
revenue[m] = revenue[m-1] × (1 + monthly_growth_rate)
```

If your growth rate is WoW, compound to a monthly equivalent first —
chapter 03: `(1 + WoW)^(52/12) − 1 ≈ (1 + WoW)^4.33 − 1`. A 6% WoW
rate is roughly `(1.06)^4.33 − 1 ≈ 28%` monthly equivalent.

Project this out 18–24 months. The revenue line is what compounding
does to today's revenue at today's rate.

### Step 2 — project expense forward

Start with current monthly expense (gross burn from chapter 02).
Apply the mod-004 forward plan month by month: each hire lands as a
step-up in the month it starts; each planned non-hire change lands
as a step-up in its month. If no plan changes are pending, the
expense line is flat.

Project this out to the same horizon as revenue.

### Step 3 — compute cash forward

`cash[m] = cash[m-1] + revenue[m] − expense[m]`. This is the same
formula from chapter 01 with revenue projected forward via growth
and expense projected forward via the plan.

### Step 4 — read the two crossings

Two events matter:

- **Crossover** — the month `m_c` in which `revenue[m_c] ≥
  expense[m_c]`. Profitability.
- **Zero-cash** — the month `m_z` in which `cash[m_z] < 0`.
  Insolvency.

Then:

- **Default alive** if `m_c ≤ m_z` (profitability lands first).
- **Default dead** if `m_c > m_z` or if `m_c` never happens in the
  projection window (the money runs out first).

That is the whole composite. Two lines, a subtraction, one
comparison.

## A worked scenario

Take the same two-founder PRE-SEED SaaS from chapters 01 and 02 at
2026-01-01.

- Cash: $600,000.
- Current MRR: $8,500 (three pilots + one long-term customer).
- Current gross burn (before hire): $25,500.
- Current net burn: $17,000.
- Forward plan: month-4 hire (+$12,000/mo), month-7 coworking bump
  (+$1,000/mo).
- Current growth rate on paying customers: 4% WoW = ~19% MoM
  equivalent. This is honest — the pilots are new and the WoW
  number has been stable for six weeks.

**Revenue projection at 19% MoM:**

| Month | MRR |
|---|---|
| 2026-01 | $8,500 |
| 2026-06 | ~$20,300 |
| 2026-12 | ~$57,700 |
| 2027-06 | ~$163,900 |
| 2027-12 | ~$466,000 |

**Expense projection with the plan:**

| Month | Monthly expense |
|---|---|
| 2026-01 | $25,500 |
| 2026-04 | $37,500 (hire) |
| 2026-07 | $38,500 (coworking) |
| 2027-06 | $38,500 |
| 2027-12 | $38,500 |

**Crossover.** Revenue crosses expense at approximately 2026-10 to
2026-11 (revenue reaches ~$40k against expense of ~$38.5k). **m_c
≈ 10 months.**

**Zero-cash.** With the growth-driven cash flow (revenue climbing,
expense stepped), cash bottoms around late 2026 and starts recovering
as monthly revenue exceeds monthly expense. **m_z: never reached in
projection window.**

**Verdict: default alive.** Growth is on track to fund the plan
before cash runs out.

Now change one input. Suppose the WoW growth rate is 1% (Graham's
"not yet" line, ~4.3% MoM):

**Revenue projection at 4.3% MoM:**

| Month | MRR |
|---|---|
| 2026-01 | $8,500 |
| 2026-12 | ~$13,700 |
| 2027-12 | ~$22,200 |

**Expense projection** unchanged: bumps to $38,500/mo by 2026-07.

**Crossover:** never reached in projection window. Revenue is a small
fraction of expense at every month.

**Zero-cash:** approximately 2027-12 (as chapter 01's raw runway
projection).

**Verdict: default dead.** At 1% WoW, the plan does not fund itself
before the cash runs out.

Two projections. Same starting cash, same starting revenue, same
starting burn, same plan. **Only the growth rate changed** — from 4%
WoW to 1% WoW — and the composite flipped from alive to dead. That
sensitivity is exactly what Graham's essay is trying to make
inescapable.

## What each verdict actually means

### Default alive

The company can, in the base case, reach profitability from its
current spend plan against its current growth. Two things follow:

- **The fundraise conversation changes shape.** Default-alive
  companies raise from *choice* — to accelerate, to expand into an
  adjacent segment, to hire ahead of demand. They do not raise
  from *necessity*.
- **The founder's leverage in that conversation is much higher.**
  Investors distinguish sharply between "we need this money" and
  "this money would make us faster." Default-alive founders can
  price the round accordingly.

Default-alive is not a permanent state. Adding hires or expanding
spend can flip it to default-dead in a week. The composite is
re-run every time the plan changes.

### Default dead

The company will not, in the base case, reach profitability before
cash runs out. This does not mean the company is dying today. It
means: *without a change to inputs (growth rate, burn, or capital),
the current trajectory ends in insolvency*.

Graham's essay argues explicitly that being default dead is not by
itself bad — many YC companies are default dead throughout the batch
and go on to be enormously successful. What is dangerous is being
default dead and **not knowing it**. The founder who thinks they are
default alive when they are default dead makes hires and spend
commitments as if the trajectory funds them; the founder who *knows*
they are default dead makes those same commitments consciously and
against a live fundraise or a plan to change the growth rate.

The composite's real purpose is to make the state legible so the
subsequent decisions can be conscious.

## Three concrete responses to a default-dead verdict

Being default dead is a state, not a sentence. Three levers, taken
directly from the composite's inputs:

**1. Cut burn** (chapter 01 / 02 input): defer a hire, kill a
sub-scale marketing line, consolidate SaaS tooling, take a founder
paycut, move out of the office. Each move drops the expense line
and pushes `m_z` (zero-cash) further out. Founders who take this
lever seriously often discover that the reduced burn *plus* the
existing growth flips the composite back to alive.

**2. Raise growth** (chapter 03 input): change the growth rate,
usually through a product or GTM move, and re-run the composite in
6–8 weeks against the new WoW. This is the highest-leverage move
but also the slowest and least controllable — you cannot decide to
grow faster the way you can decide to defer a hire.

**3. Raise capital** (mod-004 / chapter 08 input): add to starting
cash so `m_z` moves further out and gives the growth line more
time to catch up. This is a fundraise decision and is the domain of
the finance-fundraising pillar; the composite is what tells the
founder how big a round they need and how much time it buys.

The three levers are *not* mutually exclusive. A well-run
default-dead → default-alive transition often uses all three: a
20% burn cut, a growth-rate improvement from a shipped
product change, and a small bridge SAFE to buy time for both.

## The composite over time

The composite is not a one-shot call. It is a rolling reading. The
right cadence is:

- **Every mod-004 metrics one-pager (weekly)** — the *verdict*
  (Default Alive / Default Dead) is one of the six headline lines on
  the founder-numbers one-pager (chapter 07). It changes whenever
  the inputs change enough to flip the underlying comparison.
- **Every mod-004 monthly investor update** — the verdict, and the
  reason it did or didn't change since last month, is a standard
  section of the update.
- **Every mod-004 decision-log entry that changes an input** — hire
  a person, defer a hire, ship a growth-changing product change,
  close a SAFE — the composite is re-run and the new verdict
  recorded.

The point is that the verdict is a *live* signal. Founders who read
Graham's essay, run the composite once, get "default alive," and
never re-run it have missed the essay's argument.

## Common failure modes

Five failure modes are worth calling out.

**1. Using an aspirational growth rate.** The composite has to be
run against the *current, measured* growth rate — the number from
chapter 03's actual series — not the number the founder is aiming
for. A default-alive verdict computed off a 20% MoM aspiration when
the measured rate is 5% MoM is worse than not running the composite
at all; it institutionalises the self-deception.

**2. Using net burn when net-burn-after-variable-revenue is
higher.** Chapter 02's warning applies here: if the two burns
diverge because of one-offs, the honest projection uses the higher
number. A default-alive verdict computed on the flattering burn
number is a well-timed inheritance away from being wrong.

**3. Ignoring the forward plan.** Founders sometimes compute the
composite against the *current-today* burn and forget that a hire
lands in three months. The whole point of the runway model in
chapter 01 is the forward plan; the composite has to project the
plan, not just the current line item.

**4. Treating "default alive" as permanent.** A default-alive
verdict is only stable if the inputs are stable. A single new hire
can push m_z closer than m_c and flip the verdict. The composite is
re-run per decision-log entry, not per quarter.

**5. Never actually running the composite.** The most common
failure mode. The founder understands the concept, agrees it is
important, and does not sit down and compute the two lines. Graham's
essay closes with an appeal on exactly this point: the founders
who run the composite consciously make different decisions from the
founders who don't. Exercise 04 exists to make sure you have run
it at least once for real.

## Boundaries and hand-offs

The composite as taught here is the founder-numbers version — four
inputs, two lines, one verdict. Two directions of depth are
deliberately *out of scope*:

- **Sensitivity analysis** — running the projection across a full
  distribution of growth rates, burn rates, and capital-raising
  timing — is finance-pillar work
  ([`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum)).
  Chapter 08 (this module) draws the boundary; the pillar owns the
  depth.
- **The three-statement financial model** (income statement, balance
  sheet, cash-flow statement) that Graham's argument sits on top of
  at a large company is also pillar work, and not needed to run the
  composite at PRE-SEED / SEED. This module's model has one
  statement (cash flow) and it is enough.

The composite is deliberately the *simplest possible thing that
makes the survival call*. That simplicity is why every PRE-SEED
founder can and should run it; the pillar depth is what a
CFO-level operator layers on later.

## Summary

- **Default Alive** if projected revenue at current growth crosses
  projected expense before projected cash goes to zero. **Default
  Dead** otherwise.
- Four inputs, from prior chapters and mod-004: current cash,
  current net burn, current growth rate, current forward plan.
- Two lines, one comparison. If revenue ≥ expense before cash < 0,
  alive; else dead.
- Default alive is not permanent; default dead is not fatal. Both
  are *states* that make subsequent decisions conscious.
- Three levers for flipping default dead → alive: cut burn, raise
  growth, raise capital. Usually a combination.
- Re-run the composite every week (metrics one-pager), every month
  (investor update), and every time a decision-log entry changes an
  input.
- Sensitivity analysis and full financial modelling are pillar
  depth; the founder-numbers composite is what fits on the
  one-pager.

## Homework

Exercise 04 (`Default Alive or Default Dead — Scenarios`) requires
you to run the composite against a specific real (or realistic)
startup at three input variations — the base case, a
growth-rate-cut scenario, and a burn-cut scenario — and read the
verdict for each. Exercise 07 (`Founder-Numbers One-Pager
Authoring`) puts the verdict on the one-pager alongside cash, burn,
growth, and runway.
