# CAC, LTV, Payback, Gross Margin — the Vocabulary Tour

## Motivation

The four terms named in the title show up in almost every
conversation about a startup that is past the earliest days of
customer discovery. Any investor pitch of a real business, any
board conversation past Series-A, any GTM operating review, and
any strategic capital-allocation call refers to one or more of
them. A founder who cannot define them fluently reads those
conversations at a disadvantage — not because the math is hard, but
because the vocabulary hides an assumption structure that only
becomes visible once the terms are named cleanly.

This chapter's scope is deliberately narrow. It teaches the four
terms at the **vocabulary level** — the definition, the formula, the
common denominator disagreements, and the specific way each term is
mis-used — and then it stops. Depth on unit economics — cohort
analysis, gross-margin engineering, LTV-CAC segmentation, payback
optimization, and the model architecture that ties them together —
lives in
[`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum).
The goal of this chapter is that a Foundations graduate can walk
into that pillar's unit-economics module without a glossary.

## The four terms

### CAC — Customer Acquisition Cost

**Definition.** The average total cost to acquire one new customer,
measured over a defined period.

**Formula (basic form).**

```
CAC = total_sales_and_marketing_spend_in_period / new_customers_in_period
```

**The definitional decisions.** CAC is not one number; it is a small
family of numbers depending on what "sales and marketing spend"
covers. Three common definitions:

- **Fully-loaded CAC.** All sales, marketing, and business-development
  cost, including salaries, benefits, ads, tools, and any events or
  content produced. This is the most conservative version and the
  one investors calibrate on at scale.
- **Paid CAC.** Only the paid-media spend (ads, affiliate commissions,
  paid channels) divided by customers attributed to paid channels.
  Useful for channel-level decisions; misleading as a company-level
  headline.
- **Blended CAC.** Something between — often all direct acquisition
  spend but not the fully-loaded team cost. Common at seed / early
  Series-A, dangerous at scale because the underlying definition
  drifts.

The definition your company uses matters more than the number the
formula returns. If two people at the same company give two
different CACs, they are almost always using two different
definitions. Chapter 08 defers the definitional depth to the finance
pillar; this chapter's job is to know the disagreement is real and
to state which definition you are using every time you quote a CAC.

**The specific mis-use.** *"Our CAC is $200."* Quoted without
specifying the period, the channel mix, or the definition variant,
is a number that means nothing. The three follow-up questions —
*which definition, over what period, in which channels* — should be
answered on the same line as the number.

### LTV — Lifetime Value

**Definition.** The total gross-margin dollars a company expects to
earn from an average customer over the customer's full lifetime with
the product.

**Formula (basic subscription form).**

```
LTV = (average_revenue_per_customer_per_month × gross_margin_percent) / monthly_churn_rate
```

For a transactional (non-subscription) business the formula shape is
different, but the underlying idea is the same: sum, over the
expected life of a customer, the revenue you will earn from them,
adjusted for gross margin.

**The definitional decisions.** LTV shifts significantly depending
on:

- **Which margin.** Gross margin (revenue minus cost-of-goods-sold)
  is the standard; some founders quote *contribution margin* (also
  netting variable operating costs) and call it LTV. Same word,
  different number.
- **Which churn.** Monthly, quarterly, annual, or cohort-based
  churn all give different LTVs. Churn calculated on a small early
  cohort may be wildly optimistic or pessimistic relative to the
  real long-run rate.
- **Whether time-value-of-money is included.** A discounted LTV
  (using a discount rate for future cash) is more honest for
  long-lived subscriptions and is standard at scale; undiscounted
  LTV is common at seed and is fine for the vocabulary level of
  this chapter.

**The specific mis-use.** *"Our LTV is $18,000."* Quoted from six
months of customer data on a subscription with a two-year expected
life is extrapolating well beyond the observation window. LTV
computed on cohorts with less than a year of history should carry a
visible caveat. The number becomes real once you have real churn
data over a real period.

### Payback — Payback Period

**Definition.** The number of months (or years) it takes for the
gross margin from a customer to repay the CAC that acquired them.

**Formula (basic form).**

```
payback_months = CAC / (average_revenue_per_customer_per_month × gross_margin_percent)
```

**Why payback matters even more than LTV/CAC ratio at early
stage.** A high LTV/CAC ratio can look great and mask a payback
period of three years — meaning the company needs three years of
runway funded before any customer becomes cash-positive. For a
capital-constrained startup, payback is often the more important of
the two numbers because it is the *cash-flow* view of unit economics.

Rough conventional bands (from the SaaS-metrics literature; see
`resources.md`):

- **Under 12 months payback** — comfortably fundable at seed.
- **12–24 months payback** — normal for many B2B SaaS models.
- **Over 24 months payback** — needs a very large LTV or a
  strategic reason to justify.

These bands are conventions, not laws; the exact numbers vary by
segment and business model. The important property is that payback
is quoted in *months*, alongside CAC and LTV, so the cash-flow
consequences are legible.

**The specific mis-use.** Reporting LTV/CAC ratio without also
reporting payback. A company with LTV/CAC of 5× and payback of 36
months has different cash-flow behaviour from a company with LTV/CAC
of 3× and payback of 8 months, and it matters.

### Gross margin

**Definition.** Revenue minus the cost of delivering that revenue
(the direct cost of goods sold), expressed as a percentage of
revenue.

**Formula.**

```
gross_margin = (revenue − cost_of_goods_sold) / revenue
```

**What counts as COGS.** The variable and semi-variable direct
costs of delivering the product: hosting for the specific customer,
third-party API calls the product depends on, payment processing
fees, direct customer-support cost, sometimes a portion of
implementation-services cost, and — for hardware or physical
products — the manufactured cost of the units sold.

What does NOT count as COGS: general R&D salaries, most sales
and marketing spend, executive salaries, general office overhead.
(There are edge cases and industry conventions; the finance-pillar
module owns them.)

**Why gross margin is the term that couples the other three.**
Both LTV and payback have gross margin *in the formula*. A change
in gross margin — a hosting-cost improvement, a payment-processor
change, a support-cost reduction — moves LTV *and* payback in the
same direction, without changing CAC or revenue at all. That
coupling is why gross margin is the term most worth improving at
the earliest stages: one gross-margin move improves every
unit-economics number the business runs on.

**Rough conventional bands (again from the SaaS-metrics literature;
see `resources.md`; industry-specific):**

- **SaaS, pure-software**: often 70–85% gross margin at scale.
- **Marketplace / transactional**: often 20–50% take-rate margin
  on the intermediated volume, with the definition of "revenue"
  varying.
- **Hardware or physical goods**: often 20–50% gross margin.
- **Services-heavy or infrastructure-heavy AI product**:
  meaningfully lower than pure-software SaaS in the current
  environment; the finance-pillar module owns the depth on this
  emerging pattern.
  <!-- needs-research: verify a defensible current-band range for AI-heavy products' gross margins with primary sources (e.g., recent public S-1 filings, well-regarded VC benchmarks such as Bessemer / Meritech state-of-cloud reports); the pillar module owns the depth, but a rough anchor here would help the vocabulary tour without pretending to specificity. -->

**The specific mis-use.** *"Gross margin is high for SaaS."* Said
about a product whose actual variable costs include a large
third-party LLM API bill or a large hosting bill per customer is
often wrong. Gross-margin conventions travel with the historical
software model; they need to be checked against your actual
per-customer variable cost, especially for infrastructure-heavy or
model-inference-heavy products.

## The composite metric — LTV / CAC ratio

The four terms are often summarised together in one composite: the
LTV/CAC ratio.

```
ltv_cac_ratio = LTV / CAC
```

Convention (again from the SaaS-metrics literature) suggests:

- **Under 1×** — losing money on every customer; not fundable at
  scale.
- **1–3×** — thin; growth funded from capital, not from unit
  economics.
- **3× and above** — healthy at scale.
- **Above 5×** — either genuinely great or under-invested in growth
  (leaving expansion on the table).

The ratio is a useful summary and is not a substitute for the four
underlying numbers. Two companies can both quote 4× LTV/CAC and
one can have a 6-month payback and the other a 36-month payback —
same ratio, very different businesses.

## When these four terms become load-bearing

The four terms are named in this chapter at the *vocabulary level*
because — for a PRE-SEED / early-SEED startup — they are almost
always premature to optimize against. The founder does not yet have
enough customers, over a long enough period, to compute any of them
reliably. Trying to optimize them at that stage is stage-mismatched
activity per mod-003.

The four terms become **load-bearing** — worth building a real
model against, worth optimising against, worth quoting to
investors — at roughly these transitions:

| Term | Becomes load-bearing at | Why |
|---|---|---|
| Gross margin | Late SEED | The cost profile of the product is stable enough to compute |
| CAC | SEED-to-SERIES-A | The company has enough consistent acquisition to average over |
| Payback | Same time as CAC | Payback depends on CAC and gross margin |
| LTV | SERIES-A onward | LTV needs churn data over a long enough window |

Before those transitions, the terms are still worth *understanding*
— which is what this chapter is for — but not worth *optimising
against* as headline metrics. mod-003 chapter 03 has the general
form of this argument (stage-mismatched activity); the specific case
for unit economics is a common enough form of that argument that it
gets its own section here.

## The specific pillar hand-off

This is the shortest hand-off chapter in the module. Everything past
the vocabulary — the cohort methodology, the CAC-by-channel
attribution, the LTV-by-segment decomposition, the payback
sensitivity analysis, the gross-margin ladder, and the composite
model that ties it together — lives in the
[`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum)
unit-economics module.

The Foundations promise is that a graduate of this module can walk
into that pillar's module and:

- Read every term without stopping to look it up.
- Recognise which definitional variant is being used.
- Ask the right follow-up question (*"which CAC — fully-loaded, paid,
  or blended?"*, *"which margin in the LTV formula — gross or
  contribution?"*, *"discounted or undiscounted LTV?"*, *"payback in
  months?"*).
- Recognise the stage at which the term becomes load-bearing so
  they don't spend PRE-SEED / early-SEED time optimising a number
  that isn't real yet.

That is the whole scope of this chapter. Everything beyond it is
pillar depth.

## Where the four terms show up on this module's artifacts

The four terms are *named* but not *tracked* on the founder-numbers
one-pager at PRE-SEED / SEED. That is deliberate — the one-pager
carries the numbers the founder acts on every week; the four
unit-economics terms are not stable enough to act on weekly at those
stages. What the one-pager *does* carry is a placeholder line
acknowledging the deferral:

> **Unit economics:** Deferred to
> [`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum)
> unit-economics module (stage: SERIES-A). Current stage: PRE-SEED /
> SEED.

Chapter 07 formalises the one-pager. The placeholder line moves off
the one-pager and into a real tracked row somewhere between late
SEED and SERIES-A, at which point the founder is either in the
pillar module or working with someone (a CFO, a first finance hire,
a fractional operator) who is.

## Common failure modes

Four failure modes worth naming.

**1. Quoting a unit-economics number as if it were stable when the
underlying cohort is small.** LTV computed on three customers, CAC
computed on last month's ads, payback computed on last quarter alone
— all are numbers, none are useful. Any unit-economics quote should
carry the sample size and the observation window.

**2. Optimising unit economics before there are enough customers to
have unit economics.** The PRE-SEED founder building a customer-
acquisition-cost dashboard when they have twelve customers total is
practising the wrong skill for the stage. Chapter 03 of mod-003
applies.

**3. Ignoring gross margin because "the software is basically free
to serve."** The 2020s AI-heavy product world has undone that
assumption. Variable per-customer inference costs, third-party API
costs, and specialised infrastructure costs mean many "software"
products now have gross margins closer to marketplace or hardware
than to classical SaaS. Check the number; don't inherit the
convention.

**4. Treating LTV/CAC ratio as the whole picture.** Two identical
ratios can hide very different payback periods and very different
cash-flow behaviours. If only one number gets quoted, quote payback
(cash-flow view), not the ratio.

## Summary

- **CAC** — cost to acquire a customer. Definitional variants matter
  (fully-loaded / paid / blended); quote the variant explicitly.
- **LTV** — expected gross-margin dollars per customer over their
  lifetime. Depends on the margin definition, the churn measurement,
  and (at scale) on discounting.
- **Payback** — months for cumulative gross margin from a customer
  to repay their CAC. Often more actionable than LTV/CAC ratio at
  early stage.
- **Gross margin** — revenue minus cost of delivering the revenue.
  Couples LTV and payback; improving it improves both.
- All four are stage-gated in usefulness: they become load-bearing
  between late SEED and SERIES-A. Optimising them earlier is
  stage-mismatched.
- Depth (cohort methodology, attribution, segmentation, model
  architecture) is owned by
  [`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum);
  this module owns only the vocabulary.
- The founder-numbers one-pager (chapter 07) carries a deferral
  line at PRE-SEED / SEED, not real tracked numbers.

## Homework

Exercise 05 (`CAC, LTV, Payback, Gross Margin — Vocabulary Tour`)
walks the four terms against a chosen real or hypothetical company,
forces you to name the definitional variant for each, and cross-references
each to the pillar module that owns the depth. The exercise is a
vocabulary check, not a modelling exercise — you should be able to
finish it without spending time on cohort analysis.
