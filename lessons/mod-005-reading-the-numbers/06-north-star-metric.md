# Picking a North-Star Metric

## Motivation

Chapter 03 established growth as a rate. The rate requires an
*underlying quantity*, and the choice of that quantity is not
mechanical. Two thoughtful founders looking at the same startup will
often disagree about which number is the one that best captures the
value the product delivers, and the disagreement almost always
changes the operating loop that follows from it. Different metrics
produce different weekly plans, different hiring priorities,
different fundraise narratives, and different default-alive /
default-dead verdicts.

This chapter installs the **North-Star metric** — one number, chosen
deliberately, understood by everyone, and defended against
alternatives. It is the metric the founder-numbers one-pager
(chapter 07) leads with on the growth side, the metric the mod-004
weekly cadence checks against, and the metric investors ask about
first.

The North-Star framing was popularised in the startup / growth
community by Sean Ellis and elaborated in Amplitude's writing on
product analytics (see `resources.md`). This chapter uses the same
core idea and adds the pieces Foundations cares about most: a
concrete selection process and an adversarial defence against three
plausible alternatives.

## What a North-Star metric is

A **North-Star metric** is *the single number that most directly
captures the value your product delivers to its customers*. Three
properties every good North-Star has:

1. **It captures value delivered, not activity performed.** "Messages
   sent per active user per week" captures value; "logins per user
   per week" does not. Logins are how a user gets to the value; the
   messages are the value itself.
2. **It is a leading indicator of long-run business success.**
   Movement in the North-Star should reliably precede movement in
   revenue, retention, and other financial outcomes. If your
   North-Star can go up while every downstream financial metric
   stays flat, it is a proxy of your imagination, not of your
   business.
3. **It is legible enough that everyone on the team can name it and
   move it.** A North-Star that requires a spreadsheet to explain is
   not a North-Star; it is a dashboard. The mod-004 metrics
   one-pager exists so the North-Star can sit on line 1 and stay
   there.

The typical shape of a North-Star is a *rate* or a *count of
value events per period*, not a static total. "Weekly active
customers who sent at least three messages" is a North-Star
candidate; "total registered users" is almost never a North-Star.

## The three axes of a good North-Star

A useful selection heuristic — adapted from the Amplitude and Sean
Ellis writing — is that a strong North-Star sits at the intersection
of three axes:

**1. Value to the customer.** The metric moves *because* the
customer received something they came for. If the number goes up
while customers get less value, the metric is broken (see the
vanity-metric section below).

**2. Value to the business.** The metric correlates with revenue
over time. It doesn't have to *be* revenue — early on, revenue is
often too small or too lumpy to be the best week-to-week signal —
but the direction has to reliably predict revenue.

**3. Legibility across the team.** Every person in the operating
loop (co-founders, first hires, later hires) can define the metric,
name today's value, and name at least one lever they can pull to
move it. If half the team gives half the definition, the metric is
not doing its job.

A candidate metric that scores well on all three is a North-Star
candidate. One that scores well on only two is a supporting metric;
one that scores well on only one is a vanity metric.

## The four common candidate shapes

Almost every workable North-Star metric fits one of four shapes.
Which shape is right for your startup depends on the business model.

**1. A value-event-per-time count.** *"Messages sent per week."*
*"Meetings scheduled per week."* *"Contracts signed per week."*
*"Deliveries completed per week."* Best for consumer, marketplace,
communication, and transactional products where the product delivers
a discrete value event.

**2. A revenue count or rate.** *"Weekly recurring revenue."*
*"Monthly recurring revenue."* *"Weekly GMV."* Best for subscription
and marketplace products past the point where revenue is stable
enough to be a week-to-week signal. Often the *right* choice but
often *premature* at pre-seed / early-seed where revenue is small
and lumpy.

**3. An engaged-customer count.** *"Weekly active customers who
completed at least one core action."* *"Monthly active accounts using
feature X at least three times."* Best for product-led SaaS and
consumer products where value is delivered continuously and paying
customers alone don't reflect the whole engagement picture.

**4. A unit-of-value-delivered.** *"Miles driven."* *"Rides
completed."* *"Loans funded."* *"Hours of work assigned."* Best for
marketplaces and infrastructure products where the count of value
delivered is the most direct measure — often correlated with revenue
via a take-rate.

Any of the four can be a defensible North-Star for the right
company. The wrong choice is not usually "the wrong shape"; it is
"the right shape defined too loosely to be honest."

## Vanity metrics — the trap the North-Star exists to defeat

The reason "North-Star" is a named concept and not just "your main
metric" is that founders have a persistent bias toward metrics that
look good and mean little. The literature calls these **vanity
metrics** (Eric Ries's phrasing in `The Lean Startup`; see
`resources.md`).

Three common vanity-metric patterns:

**Cumulative totals.** *"Total downloads."* *"Total users ever
registered."* *"Cumulative signups since launch."* These numbers can
only go up (or stay flat), so they always look good, regardless of
whether the product is actually delivering value this week.

**Top-of-funnel counts without a value gate.** *"Sign-ups per week."*
*"Homepage visits per week."* *"App installs per week."* Real
numbers, useful for marketing conversations, but they don't measure
whether anyone got the value the product promised. The North-Star
requires a value gate — "signed up **and** completed core action" —
that filters out the visitors who never became customers of the
value proposition.

**Ratios whose denominators quietly grow.** *"Retention rate,"* if
the definition of "retained" quietly loosens as the cohort matures.
*"Growth rate,"* if the underlying quantity's definition drifts.
Ratios are useful; they need to be defined explicitly and locked.

Naming a candidate metric as a vanity metric is not an insult; it
is a diagnosis. Vanity metrics are often legitimately useful as
*supporting* metrics on the one-pager. They just can't be the
North-Star.

## The selection process

A working selection process for a PRE-SEED / SEED founder has
four steps.

**Step 1 — draft the candidate list.** Write down every metric the
company could plausibly use as a North-Star. Do not prune yet. A
typical draft list has 8–12 candidates: revenue, paying customers,
weekly active users, monthly active users, weekly value events,
retention rate, unit shipments, and so on. Include the ones you
suspect are vanity; the point of the next steps is to eliminate.

**Step 2 — score each candidate against the three axes.** For each
candidate, rate it high / medium / low on (a) value to the customer,
(b) value to the business, (c) legibility across the team. A
candidate that scores high on all three is a real candidate; one
that scores low on any is out.

**Step 3 — pick the top candidate and define it precisely.** The
definition matters more than the choice. If your North-Star is
"weekly active customers," the definition needs to name: *what
counts as a customer?* (a distinct account? a distinct human?), *what
counts as active?* (any event? a specific event?), *what counts as
the week?* (rolling 7 days? Monday-to-Sunday?). The specificity is
what lets everyone on the team compute the same number.

**Step 4 — defend the choice against the three closest
alternatives.** For each of the three most plausible runner-up
metrics, write one paragraph on *why the runner-up is not the
North-Star for this company at this stage*. The defence forces the
founder to reason explicitly about the trade-off rather than
picking on gut. Exercise 06 is where this defence gets written.

## A worked example

Take the same two-founder PRE-SEED SaaS from prior chapters.
Suppose the product is a lightweight scheduling tool for professional
services firms and the pilot customers are three accounting practices
using it internally.

**Draft candidate list.**

1. Total registered accounts.
2. Total registered users across all accounts.
3. Weekly active users.
4. Weekly active *accounts* (any user from the account was active).
5. Monthly recurring revenue (MRR).
6. Paying customer count.
7. Meetings scheduled per week per active account.
8. Meetings scheduled per week (aggregate).
9. Retention rate.
10. Homepage traffic.

**Scoring against the three axes.**

- 1 (total registered accounts): cumulative — vanity.
- 2 (total registered users): cumulative — vanity.
- 3 (WAU): OK on value-to-customer, low on business (people can be
  active without producing value for the customer's *organisation*),
  medium on legibility.
- 4 (weekly active accounts): OK on all three but hides usage
  intensity.
- 5 (MRR): high on business, low on value-to-customer (revenue can
  go up while customer value goes down for a period), low at this
  stage on legibility (small numbers, lumpy month-to-month).
- 6 (paying customer count): high on business, medium on
  value-to-customer, high on legibility — a strong contender.
- 7 (meetings scheduled per week per active account): high on all
  three — captures value delivered, correlates with retention and
  therefore revenue, easy to explain.
- 8 (meetings scheduled per week, aggregate): high on all three but
  hides per-account intensity — you can't tell if it's growing
  because more accounts are using it or because the same accounts
  are using it more.
- 9 (retention rate): important but too slow-moving at PRE-SEED to
  be a weekly signal.
- 10 (homepage traffic): vanity.

**Top candidate.** *Meetings scheduled per week per active account*
(#7).

**Precise definition.** *"The count of meetings created in the
product between Monday 00:00 and Sunday 23:59 (customer local
timezone), divided by the count of accounts that had at least one
user log in during the same window."*

**Defence against three alternatives.**

- Against #6 (paying customer count): at PRE-SEED, paying customer
  count is a very small number that moves lumpily; it is the right
  North-Star at SEED and beyond, and at PRE-SEED the intensity
  metric is a better weekly signal.
- Against #7's aggregate variant #8: aggregate meetings per week can
  climb because of one hyper-active pilot customer; per-active-
  account normalises out the account-size effect and stays honest
  as account count grows.
- Against #4 (weekly active accounts): active-account count is a
  gate, not a value metric — an account can be "active" (log in) and
  produce zero value. Meetings-per-account measures the value.

That is the shape of a defensible North-Star choice: a specific
metric with a precise definition and a written defence against the
most plausible alternatives.

## The North-Star as it evolves with stage

The North-Star chosen at PRE-SEED will almost never be the
North-Star five years later. That is not a problem; it is expected.
Common evolution patterns:

- **PRE-SEED / early-SEED**: a value-event-per-active-account rate,
  because the customer count is too small to be the primary signal.
- **Mid-SEED to SERIES-A**: often a paying-customer count or
  MRR-equivalent, once the customer count is stable enough to move
  week to week meaningfully.
- **GROWTH and beyond**: often a segmented revenue or engaged-
  customer number by cohort, because average metrics stop being
  informative when the business has multiple segments with very
  different economics.

The North-Star is versioned. Changing it is a mod-004 decision-log
entry with a reason. The founder-numbers one-pager (chapter 07)
carries only the current version; the decision log carries the
history.

## The North-Star relative to the four unit-economic terms

Chapter 05 named CAC, LTV, payback, and gross margin as vocabulary.
The North-Star is different from all four:

- The North-Star is chosen and updated *weekly*. The four
  unit-economic terms are computed *quarterly-or-slower* and
  become stable only past mid-SEED.
- The North-Star should be legible to everyone on the team. The
  four unit-economic terms are legitimately technical and often
  need a finance-savvy person to interpret.
- The North-Star drives the mod-004 weekly cadence. The four
  unit-economic terms drive fundraise decisions and pillar-level
  strategy.

They are complementary — the North-Star tells the founder *how the
week is going*; the unit-economics tell the founder *whether the
business model works at scale* — and they sit in different sections
of the founder-numbers one-pager (chapter 07).

## Common failure modes

Five failure modes worth naming.

**1. Picking the metric that grows fastest.** The fastest-growing
number is often the least meaningful (cumulative signups, home-page
traffic). The North-Star is picked for *what it means*, not for how
easy it is to make go up.

**2. Picking a metric before defining it.** *"Our North-Star is
active users"* without a written definition means every person on
the team is computing a different number every week. The definition
is the artifact.

**3. Never running the alternatives defence.** Picking a North-Star
without adversarially checking it against 3–5 runner-ups is picking
on gut. The runner-ups often expose a definitional flaw in the
choice that leads to a definition improvement, or to a different
top candidate.

**4. Refusing to update the North-Star as the stage shifts.** The
right North-Star at PRE-SEED with 12 pilot customers is almost
never the right North-Star at SEED with 200 paying customers.
Holding the old metric because "we already chose one" is scope
comfort, not discipline.

**5. Optimising for the North-Star at the expense of everything
else.** The North-Star is a compass, not a destination. A team that
gets its North-Star up while cash burn triples, retention halves,
and the four unit-economic terms all degrade has not won; it has
turned the metric into a goal (Goodhart's Law). The one-pager
carries the North-Star alongside cash, burn, runway, and the
default-alive / default-dead verdict; watching all six together is
what keeps the North-Star honest.

## Summary

- A **North-Star metric** is one number, defined precisely, that
  best captures the value your product delivers.
- It sits at the intersection of value-to-customer,
  value-to-business, and team legibility.
- Four common shapes: value-event-per-time, revenue rate, engaged-
  customer count, or unit-of-value-delivered.
- The selection process: draft candidates, score against three
  axes, pick and precisely define, defend against three closest
  alternatives.
- Vanity metrics (cumulative totals, top-of-funnel without a value
  gate, ratios with drifting denominators) are the failure mode the
  North-Star exists to defeat.
- The North-Star evolves with stage; changing it is a decision-log
  entry.
- On the founder-numbers one-pager, the North-Star sits alongside
  cash, burn, runway, and the default-alive / default-dead verdict;
  it is a compass, not a goal.

## Homework

Exercise 06 (`North-Star Metric Selection and Defence`) runs the
full selection process against a chosen real or hypothetical
startup, produces a written defence against three alternatives, and
adds the chosen North-Star to the mod-004 metrics one-pager.
Exercise 07 (`Founder-Numbers One-Pager Authoring`) then folds the
North-Star into the six-line composite one-pager the module ships.
