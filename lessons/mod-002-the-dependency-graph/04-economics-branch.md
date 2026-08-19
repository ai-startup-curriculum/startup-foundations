# The Economics Branch

## Motivation

The customer-facing branch decides whether there is a business. The
corporate-structure branch decides whether the container is sound. The
economics branch is the *instrumentation* that tells the founder how long the
search can continue, whether each dollar is being converted into more than a
dollar of value, and how the finite capital in the bank should be allocated
across the finite options in front of the company.

Every founder eventually confronts one grim, load-bearing question: **will the
money run out before the search finishes?** The economics branch is the set
of nodes that answer that question. Foundations does not teach financial
modeling to depth — that lives in
[`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum).
It teaches the *positions* of the economic nodes and, crucially, *which of
the numbers matters at which stage*.

## The branch, drawn as a spread

Unlike the customer-facing branch (a pipeline) and the corporate-structure
branch (a fan-out with a convergent endpoint), the economics branch spreads
from a single root into four sibling nodes:

```
                     ┌──► Financial Modeling
                     │
Startup Economics ───┼──► Runway
                     │
                     ├──► Unit Economics
                     │
                     └──► Capital Allocation
```

`Startup Economics` is the umbrella body of knowledge — the vocabulary and
concepts every founder needs regardless of stage. The four sibling nodes are
the specific instruments a founder uses at specific stages. They are not
strictly sequential — Runway matters from day one, Unit Economics becomes
load-bearing later, Capital Allocation becomes primary at Growth — but they
are always available.

Depth for the whole branch lives in
[`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum).
Foundations owns a **founder-numbers slice** — runway, burn, growth,
default-alive/default-dead, and unit-economics vocabulary — which is authored
in mod-005. This chapter names the nodes, the hand-offs, and which numbers
matter at which stage.

## Node 1 — Startup Economics (the root)

**What it is.** The umbrella body of knowledge covering the specific economic
patterns of venture-backed startups: high fixed costs early, near-zero
marginal costs late, capital consumed as a substitute for time, growth
compounding non-linearly, and the *power-law* distribution of outcomes across
a portfolio.

**What it produces.** Vocabulary and framing. A founder who has done a
first pass on Startup Economics understands terms like *burn*, *runway*,
*gross margin*, *contribution margin*, *unit economics*, *cohort*, *LTV*,
*CAC*, *payback period*, and *capital efficiency* — not deeply, but well
enough to read a fundraising deck or an investor update without a glossary.

**What downstream needs from it.** All four sibling nodes assume this
vocabulary. You cannot build a runway model without knowing what burn is.
You cannot compare unit economics without knowing what a cohort is.

**Owner curriculum.**
[`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum)
owns the depth. Foundations mod-005 covers the *founder-numbers vocabulary
slice*.

## Node 2 — Financial Modeling

**What it is.** The construction of a *forward-looking model* of the
company's financials — usually a spreadsheet (or increasingly a spreadsheet
plus a modeling tool) that projects revenue, costs, headcount, and cash
month by month for the next 12–36 months. At startup stage this is
typically a founder-owned bottom-up model driven by unit assumptions
(customers × ARPU, or seats × price, or transactions × take-rate).

**What it produces.** A model file — the artifact — plus the *assumption
set* that drives it (customer growth assumptions, churn assumptions,
pricing assumptions, hiring plan, cost assumptions). The assumption set is
often more valuable than the numeric output, because it is what the model
is *actually claiming about the future*.

**What is load-bearing at which stage.**

| Stage | What the model must do |
|---|---|
| IDEA / PRE-SEED | Rough runway math from a starting cash balance and a burn estimate. Foundations mod-005 territory. |
| SEED | Bottom-up model driven by explicit customer + hiring assumptions; scenarios (base / stretch / worst); named milestones the seed round is being raised against. |
| SERIES-A | Full monthly model with revenue drivers, cohort assumptions, unit economics, hiring plan, gross margin, and sensitivity tables. The model becomes a diligence artifact. |
| GROWTH / MATURE | Three-statement model (P&L, balance sheet, cash flow) with departmental budgeting, board-pack outputs, and increasingly formal review cadence. |

The load-bearing shift from *runway math* (pre-seed) to *bottom-up model
with sensitivities* (Series A) is one of the largest single jumps in the
economics branch. Founders often try to skip stages here — either building
a three-statement model too early (over-engineered, brittle) or refusing to
build a real model long past the point where it is required for the round.

**Owner curriculum.**
[`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum)
owns depth — three-statement construction, scenario modeling, sensitivity
analysis, driver-based modeling, forecast-actual variance analysis.

## Node 3 — Runway

**What it is.** The number of months the company can survive at its current
burn rate before running out of cash, assuming no additional capital and no
change in monthly cash flow. It is the single most load-bearing number in
early-stage startup operations.

The two definitions worth naming:

- **Gross burn** — total monthly cash out (all costs).
- **Net burn** — total monthly cash out minus monthly cash in (net cash
  consumed). At early stage, when revenue is small, gross and net burn are
  similar; as revenue grows they diverge.

Runway is `cash on hand / net burn`. Foundations mod-005 walks this
calculation in detail with a worked example.

**What it produces.** A number, in months, and an implicit deadline. That
deadline drives every major stage-appropriate decision — when to raise, how
aggressively to hire, whether to cut, whether to pivot, whether to close.

**What is load-bearing at which stage.**

| Stage | What runway drives |
|---|---|
| IDEA | Not yet — no entity, no burn. |
| PRE-SEED | The founder's timeline for hitting the first evidence needed to raise the seed round. |
| SEED | The countdown to when the seed round's milestones must be visible enough to raise Series A. Standard framing: raise 18–24 months of runway per round; start the next raise 6 months before the money runs out. |
| SERIES-A | Same shape as seed but with larger cash balances, larger monthly burn, and formalized runway tracking as part of the board pack. |
| GROWTH | Runway is still tracked but is one of many capital-efficiency numbers; capital allocation across pillars now dominates. |
| MATURE | Runway is not the primary lens; the P&L, cash-flow durability, and reinvestment decisions are. |

<!-- needs-research: verify the current market-typical target-runway-per-round guidance (commonly cited as 18–24 months) across a set of primary sources (YC, Sequoia, a16z, First Round) before publishing specific month numbers in learner-facing materials. -->

**Paul Graham's "Default Alive or Default Dead"** is the composite that
combines Runway with the growth rate — it asks: at your current burn *and*
your current growth rate, will you become profitable before the money runs
out? If yes, you are default alive; if not, you are default dead and must
either raise or cut. Foundations mod-005 walks this in detail.

<!-- needs-research: link to Paul Graham 'Default Alive or Default Dead?' primary essay (October 2015) in the resources file for this module. -->

**Owner curriculum.** Same as the branch — depth in
[`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum);
founder-slice in Foundations mod-005.

## Node 4 — Unit Economics

**What it is.** The economics of a single unit of the business — usually a
single customer, but sometimes a single transaction, seat, or cohort.
Unit economics answer the question *if we serve one more customer, do we
make money on that customer over their lifetime, and how quickly?*

The four terms every founder must know at least at vocabulary level (mod-005
covers this):

- **CAC — Customer Acquisition Cost.** The average fully-loaded cost of
  acquiring one customer. Includes sales cost, marketing spend, and often
  the fully-loaded cost of a founder's time.
- **LTV — Lifetime Value.** The expected total gross margin from one
  customer over their expected lifetime with the company.
- **Payback period.** The number of months of gross margin from the
  customer to recover the CAC. Shorter is better; the industry heuristic
  in SaaS is that a payback under 12 months is healthy and over 24 months
  is a warning.
- **Gross margin.** Revenue minus the direct cost of delivering the
  product, expressed as a percent of revenue. SaaS gross margins are
  typically high (often 70%+); marketplace, hardware, and services
  businesses are lower and structured differently.

<!-- needs-research: verify SaaS payback-period and gross-margin heuristics against current primary sources (Bessemer, OpenView, KeyBanc SaaS survey) before quoting specific ranges in learner content. -->

**What it produces.** A per-unit view of profitability that scales as the
company scales — if the unit works, the business works; if it doesn't, no
amount of growth fixes it (it makes it worse faster).

**What is load-bearing at which stage.**

| Stage | Unit-economics work |
|---|---|
| IDEA / PRE-SEED | Vocabulary only. There is no cohort to measure yet. |
| SEED | Directional CAC and payback estimates from founder-led sales. Enough to know if the model *could* work. |
| SERIES-A | Real cohort data. LTV / CAC ratio, payback period, and gross margin become primary diligence numbers. The Series-A story is a unit-economics story. |
| GROWTH | Unit economics become the *steering wheel* — channel-level CAC, cohort-level retention, segment-level payback. Capital allocation across channels is driven by these numbers. |
| MATURE | Unit economics graduate to segment-level P&Ls and portfolio management. |

**Owner curriculum.**
[`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum)
owns the depth — CAC construction, LTV modeling with cohort retention,
channel unit economics, marketplace take-rate analysis, contribution-margin
modeling.

## Node 5 — Capital Allocation

**What it is.** The set of decisions about *how the finite capital in the
bank should be spent across the finite options in front of the company*.
Capital allocation covers headcount planning, spend on paid acquisition,
product investment, geographic expansion, M&A, and — at the mature end —
buybacks and dividends.

**What it produces.** Written allocation plans (budgets, hiring plans,
channel spend caps, expansion decisions) and the underlying reasoning that
would let a board and an executive team make the same decision the same way
under similar circumstances.

**What is load-bearing at which stage.**

| Stage | Capital-allocation work |
|---|---|
| IDEA / PRE-SEED | Trivial — there is almost nothing to allocate. |
| SEED | The seed round's allocation decision — how much on the founding team, how much on the first hires, how much on the product, how much reserved. |
| SERIES-A | Formal budget across product / engineering / GTM / G&A; hiring plan tied to model; runway locked to allocation choices. |
| GROWTH | Primary. Multi-departmental budgeting, portfolio decisions across product lines, channel allocation, M&A, geographic expansion. This is the stage at which capital allocation dominates founder attention. |
| MATURE | Capital allocation is the CEO's core job — Warren Buffett's framing that "capital allocation is the CEO's most important task" applies most directly here. |

<!-- needs-research: locate the exact Warren Buffett shareholder-letter passage where he makes the 'capital allocation is the CEO's most important task' argument, and cite by year and letter. -->

**Owner curriculum.**
[`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum)
owns the depth — allocation frameworks, hurdle rates, ROI evaluation,
build-vs-buy-vs-partner, M&A analysis, portfolio approach.

## Which numbers are load-bearing at which stage — one-page compass

If you internalise one table from this chapter, make it this one.

| Stage | Load-bearing numbers | What is *not* load-bearing yet |
|---|---|---|
| **IDEA** | None yet — you are pre-money. Focus on the search. | Runway, unit economics, allocation |
| **PRE-SEED** | Starting cash, monthly burn, runway (in months), the milestone that must be visible before the seed raise. | Full P&L, cohort-based LTV, channel CAC |
| **SEED** | Runway, monthly burn (gross and net), growth rate, directional CAC / payback, default alive / default dead, the seed-round milestones the raise is priced against. | Three-statement model, sensitivity tables, capital allocation across many channels |
| **SERIES-A** | Cohort-based LTV, channel CAC, payback period, gross margin, growth rate, net burn, cash-out date, board-pack numbers. The Series-A story is a unit-economics story. | Buybacks, dividends, complex M&A analysis |
| **GROWTH** | Channel-level unit economics, capital efficiency across departments, hiring plan, sales-efficiency metrics (Magic Number, Rule of 40), retention cohorts. Capital allocation is now primary. | — |
| **MATURE** | Three-statement financials, cash-flow durability, capital-allocation portfolio choices. | — |

<!-- needs-research: verify definitions and current usage of 'Magic Number' (attributed to Scale Venture Partners) and 'Rule of 40' as SaaS operating benchmarks; cite the primary sources before quoting the specific formulas in learner-facing content. -->

The compass makes two things obvious in one glance. **First**, a lot of the
famous startup finance vocabulary — three-statement models, Rule of 40,
capital-allocation portfolios — is not load-bearing at all until the
company has reached a stage where the underlying dynamics justify the
lens. Applying it too early is one of the most common stage-mismatched
activities mod-003 catalogs. **Second**, the *early-stage* numbers are
tiny in count — cash, burn, runway, growth rate, a directional CAC — and
those handful of numbers do almost all the operational work of the first
two rounds. Foundations mod-005 owns that early slice.

## Coupling to the other branches

Two edges you have already met, seen from the economics side:

- **Runway ◄ Fundraising (corporate-structure branch).** Every round is a
  step-change in runway. This is the primary reason runway is tracked so
  aggressively at seed and Series A — the timing of the next raise is a
  function of when the current runway runs out.
- **Runway ◄ Sales / Growth (customer-facing branch).** As revenue grows,
  gross and net burn diverge, and runway lengthens without any additional
  capital. This is the mechanism by which a working customer-facing branch
  *earns* the company more runway even between rounds.

## Summary

- The economics branch spreads from `Startup Economics` (the vocabulary
  root) into four siblings: Financial Modeling, Runway, Unit Economics,
  and Capital Allocation.
- Runway is load-bearing from PRE-SEED onward; Unit Economics becomes
  load-bearing at SEED and dominates from SERIES-A; Capital Allocation
  becomes primary at GROWTH.
- The load-bearing-numbers compass in this chapter is the single most
  reusable piece — memorise which numbers matter at which stage so you
  don't burn cycles on numbers that don't matter yet.
- Foundations owns a *founder-numbers slice* (runway, burn, growth,
  default alive / default dead, unit-economics vocabulary), authored in
  mod-005; depth lives in
  [`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum).

## Homework

Exercise 03 (`Graph Tour — Economics Branch`) walks the branch as a series
of "which numbers matter here, and why not the others?" drills. Do it
after this chapter and before moving on to chapter 05.
