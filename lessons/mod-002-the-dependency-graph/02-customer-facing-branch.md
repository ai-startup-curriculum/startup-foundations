# The Customer-Facing Branch

## Motivation

Of the three branches on the graph, this is the one that decides whether the
company exists as a business at all. The corporate-structure branch is the
container the company is poured into; the economics branch is the
instrumentation for how long the container lasts and how efficient it is; but
the customer-facing branch is where the *value* is discovered, delivered, and
turned into revenue. A perfect cap table over an unwanted product is worth
nothing. Foundations puts the customer-facing branch first because it is the
one every other branch is ultimately serving.

This chapter walks the branch node by node — Customer Discovery → Product-Market
Fit → GTM Strategy → Sales → Growth → Exit — and, for each node, names three
things: what the node *produces*, what the next node *needs from it*, and
which pillar owns the depth.

## The branch, drawn as a pipeline

```
Customer Discovery ─► Product-Market Fit ─► GTM Strategy ─► Sales ─► Growth ─► Exit
```

Everything on this branch is deferred for depth to
[`startup-product-gtm-curriculum`](https://github.com/ai-startup-curriculum/startup-product-gtm-curriculum),
with Exit deferred to
[`startup-exit-curriculum`](https://github.com/ai-startup-curriculum/startup-exit-curriculum).
Foundations owns the fact that this ordering is *load-bearing* — you cannot
skip an upstream node without paying downstream — not the depth of any
individual node.

## Node 1 — Customer Discovery

**What it is.** The discipline of finding out — before you build — whether
there is a real customer with a real problem worth solving. It is the first
step of Steve Blank's Customer Development framework (introduced in mod-001
chapter 04). The primary artifacts are customer interviews, problem
validation notes, and a written statement of *who* has the problem and *how
badly*.

**What it produces.** A defensible answer to two questions: **who** the
customer segment is (concretely, not "SMBs" but "operations leads at 20–200
person SaaS companies who own the on-call rotation"), and **what job** they
are trying to get done that the current alternatives do not do well. That
answer is written down.

**What the next node needs from it.** Product-Market Fit cannot be evaluated
without a target segment and a problem definition — otherwise "fit" is
against no one in particular. If Customer Discovery is skipped, the PMF
signal you eventually get is either meaningless or lucky.

**Owner curriculum.**
[`startup-product-gtm-curriculum`](https://github.com/ai-startup-curriculum/startup-product-gtm-curriculum)
owns the depth — interview scripts, problem framing, jobs-to-be-done, the
whole Customer Development playbook from Blank's *Four Steps* and *Startup
Owner's Manual*.

## Node 2 — Product-Market Fit

**What it is.** The moment when the product satisfies the market well enough
that people who use it want more of it, tell their friends, and complain when
it breaks. The concept is Marc Andreessen's; the operating definition most
founders use came from him and has been sharpened by many since.

<!-- needs-research: verify the exact wording of Marc Andreessen's original PMF definition (from the June 2007 essay 'The Only Thing That Matters' on the pmarchive blog) and cite the specific line in resources.md. -->

**What it produces.** Evidence — quantitative and qualitative — that the
target segment retains, refers, and pays. Common instruments in practice
include cohort retention curves, referral rates, net-revenue-retention for
subscription products, the Sean Ellis "how would you feel if you could no
longer use this product" survey, and the direct observation that customers
pull the product out of the founder's hands rather than the reverse.

<!-- needs-research: confirm the origin of the 40%-would-be-very-disappointed threshold attributed to Sean Ellis and the primary source it appeared in before citing a specific threshold number in learner-facing content. -->

**What the next node needs from it.** GTM Strategy is the design of a
repeatable customer-acquisition engine. That design only makes sense once
there is *something worth acquiring customers into*. Building a GTM engine
before PMF is one of the most common premature-scaling failure modes (mod-001
chapter 06); the paid channel scales the losses, not the wins.

**Owner curriculum.**
[`startup-product-gtm-curriculum`](https://github.com/ai-startup-curriculum/startup-product-gtm-curriculum)
owns the depth — the metrics, the diagnostics, the pivot-vs-persevere calls,
and the transition-out-of-PMF-search work.

## Node 3 — GTM Strategy

**What it is.** The design of *how the company gets its product in front of
the customers who want it, repeatably*. GTM covers positioning, messaging,
pricing, packaging, channel strategy, and the funnel model (from first
touch to closed-won). At startup stage it is often a document plus a
whiteboard; at scale it is an entire org function.

**What it produces.** A written GTM plan — positioning statement, ICP
(ideal customer profile), pricing and packaging, chosen channels, funnel
stages with rough conversion assumptions — plus enough evidence that the
plan is not fiction. April Dunford's *Obviously Awesome* is the canonical
treatment of the positioning slice; the broader GTM discipline is a
pillar-curriculum concern.

<!-- needs-research: verify the publication year and publisher of April Dunford's Obviously Awesome and cite in resources.md. -->

**What the next node needs from it.** Sales needs a plan to execute against.
Without a defined ICP, the sales team (which at pre-seed / seed is the
founder) chases anyone who will take a meeting and burns cycles. Without
defined pricing, every deal is negotiated from zero. Without a chosen
channel, the sales motion has no shape.

**Owner curriculum.**
[`startup-product-gtm-curriculum`](https://github.com/ai-startup-curriculum/startup-product-gtm-curriculum)
owns the depth.

## Node 4 — Sales

**What it is.** The actual motion of taking a lead from first touch to a
signed contract or a first-paid subscription. At early stage this is
almost always **founder-led sales** — the founder is the only person with
enough context to have a real conversation with a serious prospect.
Foundations touches founder-led sales as part of mod-004's operating loop
but hands off depth here.

**What it produces.** Signed customers, closed-won revenue, and — as
important — a written record of what worked and what didn't in each
attempt. That record is what turns a founder's sales motion into
something a first sales hire can eventually run.

**What the next node needs from it.** Growth requires a *repeatable* sales
motion. If every deal is bespoke, there is no motion to scale — there is
consulting (which is mod-001 chapter 01's contrast with a startup). The
transition from founder-led sales to a repeatable motion is a distinct
piece of work owned by the GTM pillar.

**Owner curriculum.**
[`startup-product-gtm-curriculum`](https://github.com/ai-startup-curriculum/startup-product-gtm-curriculum)
owns the depth — founder-led sales, sales-team design, quotas, sales
enablement, discovery calls, proof-of-concept management.

## Node 5 — Growth

**What it is.** The stage at which the company has a working, repeatable
sales motion (or product-led motion), and the operating question shifts
from *find the model* to *scale the model without breaking it*. Growth
here covers acquisition, activation, retention, and expansion — the
whole loop that turns marketing dollars into customer LTV.

Sean Ellis introduced the term "growth hacker"; Andrew Chen, Reforge, and
Brian Balfour have shaped much of the modern growth-loop literature.
Foundations does not teach any of that in depth — it teaches that the
node exists and comes strictly after Sales-motion repeatability, not
before it.

<!-- needs-research: verify attribution of 'growth hacker' term to Sean Ellis (2010) and confirm the primary source citation before publishing. -->

**What it produces.** Growth-loop diagrams, cohort curves, channel-level
CAC / payback data, retention-driven expansion revenue, and a durable
increase in the *rate* of company growth over time.

**What the next node needs from it.** Exit / Endgame — whether via
acquisition, IPO, or continued private compounding — is priced on the
*rate and durability of growth* that the company can demonstrate over
multiple quarters or years. A one-quarter growth spike does not create
exit optionality; a durable growth curve does.

**Owner curriculum.**
[`startup-product-gtm-curriculum`](https://github.com/ai-startup-curriculum/startup-product-gtm-curriculum)
owns the depth — growth loops, retention modeling, activation, expansion,
channel diversification.

## Node 6 — Exit / Endgame

**What it is.** The end state of the company as an independent entity —
acquired, IPO'd, taken private again, continued as a durable independent
compounder, or wound down. Exit is drawn as the convergent endpoint of
the customer-facing branch and the corporate-structure branch (chapter
03) because it is literally the moment those two branches settle up.

**What it produces.** An outcome for founders, employees, and investors —
liquidity, distribution, or dissolution. It also produces the constraint
set for the *next* company each of those founders will build.

**What the next node needs from it.** There is no next node — Exit is
the endpoint. It does, however, feed back into the *next startup* the
founders build, which is why the org has a full pillar curriculum on
exits at all.

**Owner curriculum.**
[`startup-exit-curriculum`](https://github.com/ai-startup-curriculum/startup-exit-curriculum)
owns the depth — M&A, IPOs, secondaries, succession, shutdown.

## The hand-off table

The whole point of walking the branch is to internalise the hand-offs.
Read this table as an answer to "what does the next node *need* from the
one before it, and what breaks if that hand-off is skipped?"

| From | To | Hand-off | What breaks if skipped |
|---|---|---|---|
| Customer Discovery | PMF | Target segment + validated problem statement | PMF signal is measured against no one in particular; false positives dominate |
| PMF | GTM Strategy | Evidence of retention, referral, willingness to pay | GTM engine scales the losses; paid CAC burns without payback |
| GTM Strategy | Sales | ICP, positioning, pricing, chosen channel | Every deal is a snowflake; founder time is the entire sales team indefinitely |
| Sales | Growth | Repeatable, written sales motion | No motion to scale; growth spend produces one-off wins, not compounding revenue |
| Growth | Exit | Durable growth rate over multiple quarters/years | Exit is priced as a one-off, not as a compounding asset; optionality collapses |

## Two common misreads

**Misread 1 — the branch is not a stage sequence.** Customer Discovery is
the *upstream* node for PMF, not the *first stage* of a company. A Series-A
company still does Customer Discovery — it just does it against new
segments, new problems, or new adjacent products. The graph tells you the
prerequisite structure; the stage axis (mod-003) tells you what mix of
nodes is stage-appropriate.

**Misread 2 — "we skipped Customer Discovery and it worked out."** Survivor
bias is heavy here. The companies that skipped Customer Discovery and
succeeded are visible; the ones that skipped it and shipped an unwanted
product are dead and unreported. CB Insights (mod-001 chapter 06) has
"no market need" as the single most-cited startup failure reason across
editions of their top-reasons report — precisely a Customer Discovery
failure. Read that as the base rate.

## Coupling to the other branches

The customer-facing branch does not stand alone. Two edges into other
branches you will meet again in chapters 03 and 04:

- **Sales / Growth ► Runway (economics branch).** Sales revenue and Growth
  spend are the two largest inputs to `Runway`. A weak sales motion or a
  wasteful growth spend directly shortens the runway calculated in mod-005.
- **PMF ► Fundraising (corporate-structure branch).** The seed round and
  the Series-A round are gated primarily on PMF evidence. Without it, the
  raise is either impossible or done on such punishing terms that
  `Equity` and `Governance` downstream get warped.

Chapter 05 has the full cross-branch coupling diagram; for now just note
that these two edges exist.

## Summary

- The customer-facing branch runs Customer Discovery → PMF → GTM → Sales
  → Growth → Exit, in that dependency order.
- Each node produces a specific hand-off the next node cannot substitute
  around. Skipping upstream is the origin of the most common
  premature-scaling failure mode.
- Foundations teaches the *positions* and the *hand-offs*.
  [`startup-product-gtm-curriculum`](https://github.com/ai-startup-curriculum/startup-product-gtm-curriculum)
  owns the depth of every node except Exit, which lives in
  [`startup-exit-curriculum`](https://github.com/ai-startup-curriculum/startup-exit-curriculum).
- The branch is not a calendar and it is not a team; a founder loops back
  to Customer Discovery every time the product enters a new segment.

## Homework

Exercise 01 (`Graph Tour — Customer-Facing Branch`) walks the branch as
a series of specific hand-off drills. Do it after this chapter and
before moving on to chapter 03.
