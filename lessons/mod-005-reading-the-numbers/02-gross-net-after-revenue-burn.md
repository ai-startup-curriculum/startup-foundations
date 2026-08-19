# Gross Burn, Net Burn, Net-After-Revenue Burn

## Motivation

Chapter 01 treated "burn" as one line — total cash out per month —
because that is all the runway formula needs. In practice, founders
have three different numbers all called "burn" and each of them
supports a slightly different decision. Founders who conflate the
three end up defending a plan against the flattering version and
running out of cash against the honest one.

This chapter names the three burns explicitly, shows how each is
computed from the runway model in chapter 01, and — most importantly —
names the specific way founders lie to themselves about which number
they are watching. The lies are patterned. Naming the pattern is what
the chapter is for.

## The three burns

The three burns come from a single monthly cash-flow row:

```
    cash in (all sources)
  − cash out (all uses)
  = net cash flow
```

Each of the three burns collapses a different pair of terms.

### Gross burn — cash out, full stop

**Definition.** All cash that left the bank this month. Every payroll
run, every vendor payment, every subscription, every reimbursement.

Symbolically:

```
gross_burn = cash_out
```

**What it answers.** *"How much did we spend?"* — the operating
question a founder asks when deciding whether a specific spend was
justified against a specific outcome.

**What it does NOT answer.** How much runway that month cost. Any
revenue the company took in offsets some of the spend, and gross
burn ignores that offset.

**When gross burn is the right number.** Cost-discipline conversations
(*"we cut $8k a month by consolidating four SaaS tools into two"*),
vendor negotiations, and any spending-decision that has to be
justified independent of the company's revenue picture.

### Net burn — cash out minus cash in

**Definition.** Gross burn less the total cash that came in during
the same month. This is the number the runway formula uses in chapter
01.

Symbolically:

```
net_burn = cash_out − cash_in       (positive when losing money)
```

Or equivalently, from the chapter 01 formula:

```
net_burn = −net_cash_flow
```

**What it answers.** *"How much runway did we spend this month?"* —
the survival question. When founders talk about "our burn is
$30k/month," the honest version of that sentence almost always
means net burn.

**When net burn is the right number.** Every runway conversation.
Every default-alive / default-dead call (chapter 04). Every investor
update where the ask is "we have N months of runway." The runway
formula in chapter 01 depends on net burn, not gross burn.

### Net burn after variable revenue — the honesty check

**Definition.** Net burn recomputed with only the **variable,
recurring, non-one-off** revenue counted on the cash-in side.
One-time grants, refunds, milestone payments, tax rebates, R&D
credits, and other lumpy inflows are excluded.

Symbolically:

```
recurring_cash_in = cash_in − one_off_items
net_burn_after_variable_revenue = cash_out − recurring_cash_in
```

**What it answers.** *"What is my runway if the one-off doesn't
repeat next month?"* — the reality-check question. Almost every
month has some kind of one-off. Founders who compute net burn against
the full cash-in line and don't strip the one-offs end up making
a plan that assumes the one-offs are recurring.

**When net-burn-after-variable-revenue is the right number.** Any
projection more than one month forward. Any conversation with an
investor about "the trajectory." Any decision to hire a new person
against a revenue line that hasn't repeated three times yet.

## The three burns in one table

For the two-founder PRE-SEED SaaS example from chapter 01 in the
month 2026-04 (the month the first engineer starts):

| Line item | Amount |
|---|---|
| Cash in — recurring pilots | $8,500 |
| Cash in — one-time R&D tax rebate | $12,000 |
| **Total cash in** | **$20,500** |
| Cash out — total | $37,500 |

| Burn variant | Formula | Value |
|---|---|---|
| Gross burn | $37,500 | **$37,500** |
| Net burn | $37,500 − $20,500 | **$17,000** |
| Net burn after variable revenue | $37,500 − $8,500 | **$29,000** |

Three numbers, one month, one company. All three are correct answers
to different questions. The founder who quotes "$17,000 a month" in
an investor update this month and next month builds up ten months of
runway on the R&D rebate that only happens once. The founder who
quotes "$29,000 a month" gives the honest projection.

The pattern generalises: **for any month with a one-off cash in, the
distance between net burn and net-burn-after-variable-revenue is
the size of the founder self-deception.** If the two numbers are
close, the one-offs are small and the picture is stable. If the two
numbers diverge, the one-offs are load-bearing and the founder
should be looking at the *higher* burn number for planning.

## The lies founders tell themselves

Each of the three burns has a specific self-deception it enables. The
patterns are common enough to be worth naming out loud.

### The lie enabled by gross burn — "spending isn't burn if we can afford it"

Some founders quote gross burn during cost-conscious conversations
because the sub-lines are legible ("we spend $8k on hosting"), and
never quote net burn because it is the smaller, scarier number after
the current-month pilot revenue is netted out. Then the pilot ends and
"our burn is still $8k on hosting" is unchanged while runway falls
off a cliff.

**The check.** Every founder-numbers conversation names the *net*
burn as the headline number and drops gross-burn to the second line.
Gross burn is a legitimate secondary metric; it is a broken headline
metric.

### The lie enabled by net burn — "our net burn is fine because we booked a big invoice this month"

The most common self-deception. A one-off — a grant, a big pilot
invoice paid up front, a founder-put-in of personal money, a refund
of a duplicate charge — depresses net burn for one month, and the
founder reads the runway extension as sustainable. Six months later
the runway is materially shorter than "net burn" said it would be,
because the one-off didn't repeat.

**The check.** Compute net-burn-after-variable-revenue every month
alongside net burn. When the two diverge, the divergence is the
one-off contribution, and the projection should be run against the
higher number.

### The lie enabled by net-burn-after-variable-revenue — "we're bootstrapped now, look at our low net-after-revenue burn"

The rarer but more dangerous version. Some founders discount
recurring revenue too *aggressively* — they exclude any revenue they
suspect could churn, any revenue with a term shorter than a year,
any revenue from a customer they aren't sure about — and end up with
a net-burn-after-variable-revenue number that looks so low they
declare themselves "essentially profitable" while their bank
balance still falls every month. The number becomes a narrative
convenience.

**The check.** The three burns are three columns of a single row;
they get computed the same way every month with the same
one-off-inclusion rules; the rules are documented at the top of the
sheet; the rules do not change between months to make the current
month's number look better.

## Which burn goes on which artifact

The three burns each have a different audience.

| Artifact | Which burn goes here | Why |
|---|---|---|
| The runway model (chapter 01) | **Net burn** | The formula requires cash-in minus cash-out |
| The founder-numbers one-pager (chapter 07) | **Net burn** (headline) plus **net-after-variable-revenue** (second line) | The one-pager exists to make the delta visible |
| The mod-004 investor update | **Net burn** (headline) and any month-over-month change explained | Investors calibrate on net burn; the explanation is the trust move |
| Vendor / cost negotiations | **Gross burn** and the specific line items | Nobody negotiates hosting against your revenue picture |
| Fundraise deck / financial model | Depth beyond this module — see chapter 08 and the finance pillar | Full three-statement financial modelling is pillar work |

The one-pager (chapter 07) is where the three burns first coexist on
one artifact. Chapter 07 formalises the row shape: net burn as the
headline, gross burn as a subline, net-after-variable-revenue as a
subline, and — implicitly — the ratio between them as the
self-deception detector.

## The special case — negative net burn

If cash in exceeds cash out in a month, net burn is *negative* —
i.e., the company made money that month. Two common cases:

1. **A one-off inflated the month.** A big pilot paid up-front for
   a year, a grant landed, the tax rebate came through. Net burn
   goes negative for that one month; net-burn-after-variable-revenue
   is still positive. This is not profitability; it is a lumpy
   month. Do not update the "we are profitable now" narrative on
   the strength of one month.
2. **The recurring revenue crossed the burn line.** Both net burn
   *and* net-burn-after-variable-revenue are negative for two or
   more consecutive months. This is the real thing —
   default-alive / default-dead (chapter 04) is a much easier call
   from here, and mod-005's job downstream is to make sure the
   founder does not accidentally hire back into a positive burn.

The distinction between the two cases is exactly the
gross / net / net-after-variable-revenue split. Founders who don't
run all three will confuse the two cases.

## Update discipline

The three burns are computed together, monthly, on the same day, as
part of the monthly reconciliation from chapter 01. The
computation is fully mechanical:

1. Sum every cash-out line for the month → gross burn.
2. Sum every cash-in line for the month → cash in.
3. Subtract → net burn.
4. Sum only the recurring cash-in lines for the month, per the
   rules at the top of the sheet → recurring cash in.
5. Subtract from gross burn → net burn after variable revenue.

The result is three numbers per month for the last 6–12 months, laid
out as a small time series next to the runway model. That time
series is what turns the three burns from static numbers into a
picture of how the business's cash is behaving.

## Common failure modes

Five failure modes worth naming.

**1. Only ever quoting one of the three.** The founder who always
quotes net burn (or worse, gross) is not seeing the divergence when
it opens up. All three are needed to see the whole shape.

**2. Redefining "recurring" month by month.** If the recurring-vs-
one-off rules change from month to month to make the number look
better, the number stops meaning anything. Document the rules at
the top of the sheet and change them only in an explicit,
decision-logged move.

**3. Treating founder-contributed personal money as revenue.** A
founder loan or a personal capital top-up is a *financing* event,
not revenue. It belongs on a separate row of the cash-in column,
tagged as financing, and does NOT count toward net burn improvement
in any of the three variants.

**4. Confusing burn with P&L expense.** Burn is *cash out*, not
accrued expense. A $12,000 annual bill paid in month 1 is $12,000
of burn in month 1, not $1,000/month of burn amortised. The runway
model is a cash model; accrual accounting is the finance pillar's
job.

**5. Not showing all three on the one-pager.** The one-pager
(chapter 07) exists to make the delta between net burn and
net-burn-after-variable-revenue visible on the artifact everyone
reads. Hiding two of the three defeats the purpose.

## Summary

- **Gross burn** = cash out. Answers *"how much did we spend?"*
- **Net burn** = cash out − cash in. Answers *"how much runway did
  the month cost?"* — the number the runway model uses.
- **Net burn after variable revenue** = cash out − *recurring*
  cash in. Answers *"what is the projection if the one-off doesn't
  repeat?"* — the honest planning number.
- Each of the three burns enables a specific founder self-deception;
  running all three catches the deception on the artifact instead of
  six months later against the bank balance.
- The three burns coexist on the founder-numbers one-pager
  (chapter 07) with net burn as the headline and the other two as
  sublines.
- The rules for what counts as recurring are documented at the top
  of the sheet and change only through a logged decision.

## Homework

Exercise 02 (`Gross vs Net Burn Drill`) walks the three burns for a
specific month against a specific company and forces the founder to
name which of the three is the honest planning number and why.
Exercise 04 (`Default Alive or Default Dead — Scenarios`) uses
net-burn-after-variable-revenue as the input on the burn side; if
this chapter's discipline is in place, exercise 04's composite call
becomes much sharper.
