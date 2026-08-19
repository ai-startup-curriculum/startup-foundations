---
module: mod-005-reading-the-numbers
exercise: exercise-02
slug: gross-vs-net-burn-drill
hours: 2
prereqs: [chapter-02-gross-net-after-revenue-burn]
requires: [exercise-01-build-a-runway-model-from-zero]
---

# Exercise 02 — Gross vs Net Burn Drill

## Problem statement

Chapter 02 named the three burns — gross, net, and net-after-
variable-revenue — and named the specific self-deceptions each
enables. This exercise is a short mechanical drill: pick a specific
month for the startup from exercise 01, compute all three burns
against real cash-in and cash-out data, name which of the three is
the honest planning number for that month, and defend the answer
in one paragraph.

The drill is deliberately short (2 hours) because the value is in
the *habit* of computing all three, not in the analytical depth.
Once the three-burn discipline is a reflex, it applies every month
for the rest of your founder career.

## Requirements

### Part A — pick a month (about 10 min)

Pick a single specific month from the startup you modelled in
exercise 01. Two acceptable choices:

- **The most recently closed month** — the highest-signal choice
  because the numbers are real and known.
- **A month with a known one-off** — a month where you know there
  was a lumpy revenue event (a grant, a big pilot pre-payment, a
  tax rebate, a founder cash injection, an annual invoice paid up
  front) — because the drill's whole point is to catch the
  divergence.

**Deliverable A**: one sentence naming the month, one sentence on
why you picked it.

### Part B — list the cash-in lines (about 20 min)

Break the month's total cash in into individual line items. For
each item, name:

- **Amount.**
- **Source** (the customer, the grant, the tax authority, the
  founder loan, whatever).
- **Category**: **recurring** or **one-off**.

The recurring vs. one-off rule matters. Use the definition your
runway model uses (from exercise 01 / chapter 02); if the model
doesn't have one yet, adopt this default:

> An inflow is **recurring** if it will happen again next month,
> in approximately the same amount, without any *new* action by
> the founder. An inflow is **one-off** otherwise.

Under that rule, subscription revenue from an existing customer is
recurring, a grant is one-off, a one-time pilot invoice is one-off,
an R&D tax rebate is one-off, a founder cash injection is one-off
(and, per chapter 02, is a financing event that shouldn't count as
revenue at all — flag it).

**Deliverable B**: a table of cash-in items with the three columns
above. Sum the recurring items separately from the total.

### Part C — list the cash-out lines (about 20 min)

Break the month's total cash out into the six chapter-01 categories.
For each category, sum the amount for the month and note anything
non-standard (e.g., "included the annual legal renewal — $6,000
one-time on top of the normal $500/month retainer").

**Deliverable C**: a six-row table of cash-out amounts by category
plus a total.

### Part D — compute the three burns (about 15 min)

Using the definitions from chapter 02:

- **Gross burn** = total cash out.
- **Net burn** = total cash out − total cash in.
- **Net burn after variable revenue** = total cash out −
  recurring cash in.

**Deliverable D**: the three numbers, each with the formula written
out one line above, so a reader can retrace the computation.

### Part E — name the divergence (about 15 min)

Compute the two informative deltas:

- `gross_burn − net_burn` = total cash in for the month (the
  amount your revenue is currently offsetting your burn by).
- `net_burn_after_variable_revenue − net_burn` = size of the
  one-off contribution this month (chapter 02's "size of the
  founder self-deception" if the founder is only watching net
  burn).

Then answer, in one paragraph:

- **Which of the three burns is the honest planning number for
  this month, and why?**
- If the two burns (net vs. net-after-variable-revenue) diverge
  by more than about 10% of net burn, name the specific one-off
  responsible and describe what the projection looks like if you
  planned against the flattering number.

### Part F — the pattern check (about 20 min)

Repeat Parts B–D (only the totals, not the itemised tables) for
the **two months prior** to your chosen month. This gives you a
three-month series of the three burns:

|  | Month N−2 | Month N−1 | Month N (chosen) |
|---|---|---|---|
| Gross burn | | | |
| Net burn | | | |
| Net burn after variable revenue | | | |

Look at the series. Answer, in two-to-four sentences:

- **Which of the three moves the most?** Volatility tells you
  something — often that the one-offs are inconsistent.
- **Are net burn and net-burn-after-variable-revenue converging
  or diverging?** Convergence means the revenue base is
  stabilising; divergence means one-offs are load-bearing.
- **What would you tell an investor about "our burn" if you had
  to quote one number for the month?** Which one, why, and with
  what caveat.

### Part G — update the model (about 20 min)

Return to the runway model from exercise 01. Add three explicit
columns (or rows on the companion tab) tracking gross burn, net
burn, and net-burn-after-variable-revenue for each month. Populate
the last three months (with the values from Parts B–F). Note in
the model's sources tab which of the three variants the runway
projection uses.

If the projection currently uses net burn but net-burn-after-
variable-revenue is materially higher, decide (and record the
decision) whether to switch. Chapter 02 suggests using the higher
number for the honest projection; the choice is yours to make and
log.

## Deliverable shape

A single Markdown file, `mod-005-exercise-02-gross-vs-net-burn.md`,
structured:

```markdown
# Gross vs Net Burn Drill — [Startup Name], [Month]

## Setup
- Month: YYYY-MM
- Why chosen: <one sentence>

## Cash-in items
| Amount | Source | Recurring / One-off |
|---|---|---|
| ... | ... | ... |

Recurring cash in total: $X
One-off cash in total: $Y
Total cash in: $Z

## Cash-out items
| Category | Amount | Notes |
|---|---|---|
| People — cash comp | ... | ... |
| ... | ... | ... |

Total cash out: $W

## The three burns
- Gross burn = $W
- Net burn = $W − $Z = $A
- Net burn after variable revenue = $W − $X = $B

## Divergences
- Total cash in offsetting burn: $Z
- One-off contribution to net burn: $B − $A = $C

## Which is the honest planning number, and why
<one paragraph>

## The three-month pattern
| | Month N−2 | Month N−1 | Month N |
|---|---|---|---|
| Gross burn | | | |
| Net burn | | | |
| Net burn after variable revenue | | | |

<two-to-four sentence discussion>

## Model update
- Which burn variant the runway projection now uses: <one sentence>
- If changed, why: <one sentence>
```

Total length: 500–800 words plus the tables.

## Starter guidance

- **Do not smooth or average until you have the raw month.** The
  point of the drill is to see one month's numbers honestly first;
  averaging is a chapter 03 discipline, not this one.
- **A founder cash injection is a financing event, not revenue.**
  Chapter 02 is explicit. Flag it in the cash-in table with a
  category label, and *do not* include it in either recurring
  cash in or the offset to gross burn.
- **When in doubt, put the item in "one-off."** The whole point of
  the recurring bucket is that you can safely project it forward
  next month. If you cannot state, with a straight face, that
  next month's same-source-same-amount inflow is expected, it is
  one-off.

## Acceptance criteria

You have completed the exercise when:

- [ ] A specific month is chosen and the reason recorded.
- [ ] Every cash-in line for the month is itemised with source
      and recurring / one-off classification.
- [ ] Every cash-out line for the month is bucketed into the six
      chapter-01 categories.
- [ ] All three burns are computed with formulas visible.
- [ ] The two deltas (total cash in as offset; one-off contribution)
      are computed.
- [ ] The one-paragraph honest-planning-number answer is written.
- [ ] The three-month pattern table is populated and the
      two-to-four-sentence discussion is written.
- [ ] The runway model from exercise 01 now tracks all three
      burn variants and the projection's chosen variant is
      recorded.
- [ ] The write-up is committed as
      `mod-005-exercise-02-gross-vs-net-burn.md`.

## Common failure modes to avoid

- **Skipping the itemisation and jumping to the numbers.** The
  itemisation is where the recurring vs. one-off decisions live.
  Skipping it hides the drift.
- **Redefining "recurring" to make net burn look better.** The
  rule is set once (in exercise 01's model or in this exercise's
  Part B) and does not change month to month.
- **Only running the drill once and never again.** The muscle is
  monthly. The runway model's monthly reconciliation (chapter 01)
  is where the drill runs from that point on.

## What good looks like

A finished exercise where the founder can point at their runway
projection and say *"we're projecting against
net-burn-after-variable-revenue rather than net burn because our
last three months included two meaningful one-offs, and the
honest projection is a year shorter than the flattering one would
have said."* The specific numbers matter less than the fact that
the founder now sees the divergence on the artifact instead of six
months later against the bank balance.
