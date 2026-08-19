# Growth as a Rate — WoW, MoM, and the 5–7% Yardstick

## Motivation

Chapters 01 and 02 built the *cash-side* view. This chapter builds
the *growth-side* view. The two together are everything the
default-alive / default-dead composite in chapter 04 needs.

Founders talk about growth in three broadly different registers.
Some talk about it as an *event* — "we tripled last month!" Some
talk about it as a *total* — "we're at $40k MRR." A smaller number
talk about it as a *rate* — "we grew 6% week over week last week and
5% the week before." Only the third register lets you compare this
week to last, this quarter to last, and yourself to any other
startup at any other point in history.

Paul Graham's `Startup = Growth` is the canonical treatment: the
best startups at YC grow **5–7% per week** at the seed stage, the
extraordinary ones grow 10% per week, and 1% per week means the
company isn't really working yet. This chapter installs the rate
mindset, walks the two cadences that matter (WoW and MoM), calibrates
against Graham's yardstick, and names the specific ways rate
calculations go wrong.

## Rate, not total, not delta

Three different sentences describe the same growth in different
registers:

- **Total.** *"We're at 1,240 weekly active users."* Tells you the
  size. Useless for prediction — a company at 100,000 users growing
  0.5% a week and a company at 1,240 users growing 8% a week are
  incomparable on the total.
- **Delta.** *"We added 92 weekly active users last week."* Tells
  you the amount added. Slightly more useful, but still bakes the
  size in — 92 net-adds on 1,240 is a very different signal from
  92 net-adds on 100,000.
- **Rate.** *"We grew 7.4% week over week last week."* Tells you
  the *percentage change* of the underlying quantity. Size falls
  out; comparability arrives.

The rate is the register that matters at PRE-SEED and SEED. The
total and the delta are legitimate secondary metrics; the rate is
the primary one, and it is the one that goes on the founder-numbers
one-pager (chapter 07).

## The two cadences

Which cadence to compute growth on depends on stage. Two rules of
thumb cover almost every case.

### Week-over-week (WoW) — early stage

**When to use.** IDEA through mid-SEED. Small numbers, short
feedback cycles, everything volatile enough that a month is too
coarse to see what changed.

**Formula.**

```
WoW_growth = (this_week − last_week) / last_week
```

That is it. If the North-Star is signups and there were 210 last
week and 224 this week, WoW is `(224 − 210) / 210 = 6.7%`.

**Cadence.** Computed every Monday morning as part of the mod-004
weekly cadence, on the previous seven completed days. The
comparison is *week-to-week*, not "this Monday vs. last Monday" —
the whole week's total (or average) compared to the previous
whole week's total.

**Why weekly at early stage.** A pre-seed / early-seed startup
often has small enough underlying numbers that a single good day
distorts a monthly figure. Weekly aggregation smooths the
day-to-day noise; monthly aggregation over-smooths and hides the
short-cycle information the founder needs to decide *this week*.
Weekly is also the cadence that matches the mod-004 operating
loop — the growth rate is one of the numbers on the metrics
one-pager (chapter 02 of mod-004) and it belongs at the same
cadence as the artifact it lives on.

### Month-over-month (MoM) — post-PMF

**When to use.** Late SEED through GROWTH. The absolute numbers
are big enough that a single week's noise no longer moves the
signal, and the reporting audience (a board, an investor list)
naturally operates at the monthly cadence.

**Formula.**

```
MoM_growth = (this_month − last_month) / last_month
```

**Cadence.** Computed on the first business day of each month
against the fully closed prior month.

**Why monthly at later stage.** A post-PMF company with sales
cycles measured in weeks has enough natural month-to-month
smoothing that MoM is a stable signal. WoW at that scale often
picks up the calendar noise (holidays, month-end pushes) more
than the underlying trend.

### Both cadences at the transition

At the SEED-to-SERIES-A transition it is normal to run *both*
WoW and MoM in parallel for a few months. WoW is the operating
signal (weekly cadence, catches the short-cycle information); MoM
is the reporting signal (monthly cadence, matches the update
audience). When MoM has been stable and defensible for several
consecutive months, WoW starts to drop off the one-pager and MoM
takes over as the primary.

The `stage` tag in the mod-004 metrics one-pager (and this
module's one-pager in chapter 07) drives the choice; nothing
about the formula changes.

## Compounding — why the rate is the number that matters

The rate compounds. A 5% WoW growth rate over a year is:

```
(1.05)^52 ≈ 12.6×
```

Twelve-and-a-half-x in a year. A 7% WoW growth rate over the same
year:

```
(1.07)^52 ≈ 32×
```

Thirty-two-x in a year. A 10% WoW growth rate:

```
(1.10)^52 ≈ 142×
```

One hundred forty two x. This is why Paul Graham's 5–7% band is not
a soft aspiration — it is the compounding zone that turns a
pre-seed company into a real business within a year. And why a 1%
WoW rate is Graham's "isn't really working yet" line — `(1.01)^52
≈ 1.68×`, i.e., 68% growth over a full year, which is fine for a
small business and inadequate for a company that has to justify
its cap-table by growing into it.

The same compounding maths applies to MoM at a slower cadence:

- 15% MoM over a year: `(1.15)^12 ≈ 5.4×`
- 20% MoM over a year: `(1.20)^12 ≈ 8.9×`

MoM rates are naturally larger per-period because months are longer
than weeks. The conversion isn't linear: 5% WoW is roughly
`(1.05)^4.33 − 1 ≈ 23%` MoM equivalent, not 20%. When you convert
between cadences, compound; do not multiply.

## The Paul Graham 5–7% yardstick

Paul Graham's `Startup = Growth` gives one calibration line every
founder in Foundations should be able to quote:

> A good growth rate during YC is 5-7% a week. If you can hit
> 10% a week you're doing exceptionally well. If you can only
> manage 1%, it's a sign you haven't yet figured out what you're
> doing.

The yardstick belongs to a specific context — YC-batch companies,
mostly SaaS or consumer, mostly measured on weekly revenue or
weekly active users, at the pre-seed / early-seed stage. Every part
of that context matters. The yardstick is *not* a claim that every
startup should grow at 5–7% WoW at every stage on every metric;
it is a calibration line for one common case that most other cases
can be reasoned about *against*.

Three concrete uses of the yardstick:

1. **Sanity-check your own current WoW.** If you're PRE-SEED or
   SEED, growing 6% WoW on a real North-Star, you are on the
   Graham line. Growing 2% WoW, you are not. Growing 25% WoW,
   your denominator is probably small enough to be noisy — the
   next few weeks will tell you whether the rate is real or
   whether one big deal moved the number.
2. **Sanity-check somebody else's growth claim.** A founder pitching
   "we're growing fast" without a rate is telling you nothing.
   A founder claiming "60% MoM" is claiming ~11% WoW equivalent —
   above the exceptional line. Ask for the underlying weekly
   series; the rate should have been stable for at least four
   weeks to count.
3. **Decide when to shift cadence.** As the company matures, the
   Graham 5–7% WoW line implicitly becomes an ~23–33% MoM line
   which almost no post-Series-A company sustains long-term.
   That is not a failure signal; it is the signal that the
   yardstick is stage-graduating and the company should move to
   MoM.

The rest of chapter 04 (default-alive / default-dead) uses the
same yardstick as the growth-side input to the survival composite.
This chapter is where you first hold your own number up against it.

## Which underlying quantity to grow

Growth as a rate requires an underlying quantity, and the choice of
underlying quantity is not trivial. For a startup, the almost-always-
right underlying quantity is **the one number that best captures
value delivered to customers** — i.e., the North-Star metric (chapter
06). Common defensible choices:

- **Revenue (MRR for subscription, GMV for marketplace, weekly
  transactional revenue for consumer).** The strictest measure;
  hard to hack; investors calibrate on it.
- **Paying customers.** Second-tightest; used when the revenue-per-
  customer is roughly stable and the count is the more legible
  signal.
- **Active users (weekly / monthly), for products that don't yet
  charge.** Used at pre-monetisation and consumer stages, with the
  caveat that "active" needs a strict definition (chapter 06).
- **Units of value delivered** (e.g., messages sent, contracts
  signed, deals closed, delivery legs served) — for products where
  the value the product delivers is more legibly counted than
  charged.

The choice of underlying quantity is a chapter 06 conversation.
This chapter's job is to say: **whatever quantity you chose, growth
is that quantity's rate of change, computed weekly at PRE-SEED and
monthly at post-PMF, expressed as a percentage, compared against
the yardstick and against your own prior weeks**.

## The specific ways rate calculations go wrong

Rate calculations are simple enough that they have exactly a few
common failure modes. Each of them makes a company's growth look
better than it is.

**1. Cherry-picking the base week.** Comparing this week against a
particularly weak week last month, instead of last week. If the
denominator is chosen, the growth rate is meaningless. The rule is:
this-week's rate is `(this_week / last_week) − 1`, always, with
"last week" being the immediately preceding week. If you want to
smooth noise, use a **trailing four-week rate** as an additional
number, not a substitute.

**2. Trailing 4-week averages presented as "our growth rate."** A
trailing 4-week average is a smoothed number and it is legitimate
as one of the numbers on the one-pager. It is not "our growth
rate" — it is "our trailing 4-week average growth rate." The
distinction matters because averages hide inflection: a company
that grew 10%, 10%, 10%, then 0% and 0% is trending badly, and the
trailing 4-week average smoothes the inflection into a comfortable
"6%".

**3. Growth on a total that quietly changed.** If the underlying
count definition shifted mid-quarter — "active user" got
redefined, revenue started including a new SKU, MRR started
including annual-prepaid — the rate before and after the change
are not comparable. Any change to the underlying quantity gets a
mod-004 decision-log entry with the exact date of the change, and
the rate series carries a visible break there.

**4. Growth compared week-over-week when the cycle isn't weekly.**
An enterprise B2B startup with 6-week average sales cycles will
have noisy WoW growth even at scale, because deals cluster. In
that case MoM is the honest signal *even at seed stage* — the WoW
number will look wildly volatile and cause reactive decisions. The
question to ask is: *what is the natural cycle time of the value
this product delivers?* — and use the next-longer cadence than
that.

**5. Reading growth without reading churn.** Net growth is
`(new − churned) / base`. A company with 20% new-user growth and
15% churn is really growing 5%. The one-pager reports the net
number, with new and churn as sublines. Missing this makes a
consumer product look great for a month or two and then flat for
the rest of the year.

**6. One massive week that "extends the trend."** One deal that
lands the same week — a large customer signing, a viral spike, a
press mention — can make WoW leap 40%. That is not a growth rate;
it is one event. Watch the next 2–3 weeks; if the elevated growth
compounds, it was real; if the rate crashes back, the single week
was an event, not a trend. Do not update the fundraise narrative
on the strength of one week.

## Where the rate goes

The growth rate lives on three artifacts:

- **The mod-004 metrics one-pager (weekly cadence)** — as one of
  the standing numbers, in the same three-values-per-line grammar
  (current, last week, target-for-this-week).
- **The founder-numbers one-pager in chapter 07** — as one of the
  six headline lines that gets the 90-second read.
- **The default-alive / default-dead composite in chapter 04** —
  as the growth-side input. The composite uses either the WoW or
  the MoM rate depending on stage; the choice is documented in the
  same place the rate is computed.

## Common failure modes

Five failure modes worth naming.

**1. Reporting total instead of rate.** The founder update that
reads "MRR is now $42,000" without saying `(this month up from
$39,000 last month, +7.7% MoM)` is failing to communicate the
one thing an investor cares about at seed.

**2. Reporting rate without the denominator.** "We grew 30% last
week" from 20 users to 26 is a real 30% but a very small signal.
"We grew 30% last week (26 vs 20 users)" lets a reader do the
calibration; "we grew 30%" alone leaves the reader either
over-impressed or annoyed.

**3. Chasing the yardstick against the wrong metric.** Growing
30% WoW in signups while paying customers stay flat and revenue
falls is not on the Graham line. The rate has to be on the metric
that best captures the value delivered — chapter 06's job — not on
the metric that grows fastest.

**4. Skipping weekly measurement because "the number's too small
to bother."** At small numbers, rate is exactly the way to make the
signal legible. If your MRR is $2,000 growing $200/week, that is
10% WoW — inside the exceptional band. Not measuring means you
don't know.

**5. Reporting an aspirational rate instead of a measured one.**
"We're growing 15% MoM" said as a plan is fine. Said as a report of
the current rate when the actual rate is 6% is a category error.
The one-pager reports what happened; the plan says what the founder
is aiming at; the two are separate rows.

## Summary

- Growth is a **rate**, not a total or a delta. The rate is the
  register that makes comparability possible.
- Two cadences: **WoW at PRE-SEED and early SEED**; **MoM at
  post-PMF and beyond**. The transition period runs both in parallel.
- Rates compound: 5% WoW is ~12.6× a year, 7% WoW is ~32×, 10% WoW
  is ~142×. Small-looking weekly numbers become enormous annual
  numbers.
- Paul Graham's yardstick — **5–7% WoW at seed** — is the
  calibration line. 10% is exceptional; 1% is "not yet."
- The underlying quantity should be the North-Star (chapter 06);
  the rate is computed on *that* quantity, not on whichever grows
  fastest.
- Common rate failure modes are patterned — cherry-picking base
  weeks, trailing averages presented as rates, silently changing
  definitions, reporting on the wrong cadence, ignoring churn,
  and reading one-off spikes as trends.
- The rate belongs on the founder-numbers one-pager alongside cash,
  burn, and runway; the composite in chapter 04 uses it.

## Homework

Exercise 03 (`Growth Rate — WoW and MoM Calculation`) walks the
computation for a specific real (or realistic) startup at both
cadences, compares against Graham's yardstick, and catches the
common failure modes on a real series. Exercise 04
(`Default Alive or Default Dead — Scenarios`) uses the rate as one
input to the composite.
