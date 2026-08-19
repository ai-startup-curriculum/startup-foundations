---
module: mod-005-reading-the-numbers
exercise: exercise-01
slug: build-a-runway-model-from-zero
hours: 4
prereqs: [chapter-01-runway-from-zero, chapter-02-gross-net-after-revenue-burn]
---

# Exercise 01 — Build a Runway Model from Zero

## Problem statement

Chapter 01 walked the seven-column, month-by-month runway model
end to end. This exercise is where you build one from an empty
spreadsheet for a real (or realistic) startup you care about.

The exercise is deliberately mechanical. The point is not to
produce a clever model; the point is to produce a *working, defensible,
weekly-touched* model that lets you read your runway as a number of
months and a calendar date instead of a hedge. If the model you
finish this exercise with is the same one you keep updating for the
next year, the exercise succeeded.

## Requirements

### Part A — pick the startup and the source of truth (about 30 min)

Pick a startup. Two acceptable options:

- **A real startup you have some access to.** Your own current or
  prior venture, one you are advising, one whose founder is a close
  friend or a former co-worker willing to share numbers with you.
  Anonymise names and shift numbers by a small consistent factor
  if you need to.
- **A well-specified hypothetical.** A PRE-SEED or SEED company
  with a defensible product, a named ICP, a realistic starting
  cash balance, a realistic burn breakdown by category, and a
  plausible forward plan. If you construct one, spend real thought
  on the specifics — a hypothetical that is too vague makes the
  exercise fake.

**Deliverable A**: a one-paragraph startup context — what it does,
current stage (PRE-SEED or SEED per mod-003), how many people are
on the operating side, and the two-or-three current sources of
truth for the numbers (bank account name, payroll provider,
accounting spreadsheet, etc.).

If you don't know where the numbers *live* today, the exercise's
first output is discovering that. That discovery is itself the
value; do it before opening the spreadsheet.

### Part B — build the seven-column model (about 90 min)

Open a fresh spreadsheet. Build the model with the exact columns
from chapter 01:

```
Month | Starting cash | Cash in | Cash out (gross) | Net cash flow | Ending cash | Cumulative burn
```

Rules:

- **24 rows.** One per calendar month, starting with the current
  month. Every row is a *dated month* (e.g., 2026-01), not a
  relative label.
- **Starting cash on row 1** = the current bank-account balance
  today. Cite the source (which account, sum across if multiple,
  currency and exchange rate if not USD).
- **Cash in per row**: the total of all cash inflows expected that
  month. Break out the sources on a companion tab or below the
  main table.
- **Cash out per row**: the total of all cash outflows expected
  that month, with a per-category breakdown on the companion tab.
  Categories from chapter 01: (1) people — cash comp; (2) people
  — benefits / payroll tax / PEO; (3) hosting / tools / infra;
  (4) contractors / freelancers / professional services;
  (5) marketing / sales / ads; (6) rent / office / physical.
- **Net cash flow** = Cash in − Cash out.
- **Ending cash** = Starting cash + Net cash flow. This is the
  starting cash of the next row.
- **Cumulative burn** = sum of all months' `−Net cash flow` from
  the model start through this row.

Every value has a source. Sources acceptable:

- The bank balance (starting cash only).
- The last three months' average from bank statements (base
  monthly cash out and base monthly cash in).
- A signed offer / signed contract / signed SAFE (planned hires,
  planned cash in).
- A mod-004 decision-log entry (planned spend changes, planned
  hires not yet made).

Values with no source do not go in the base model. They can go in
a separate scenario column, clearly marked (see Part C).

### Part C — build the forward plan (about 30 min)

On the same sheet or an adjoining one, list every *planned change*
to the base burn line over the 24-month horizon. Chapter 01's
three components:

1. **Planned hires** — one row per hire, with role, expected
   start month, monthly fully-loaded cost, and source
   (signed offer / decision-log-approved plan / etc.).
2. **Planned non-hire spend changes** — hosting bumps, annual
   renewals, marketing pushes, one-time legal / tax events.
   Each one dated to a specific month.
3. **Planned cash in** — expected SAFE tranches with signed
   docs, grants with signed award letters, expected revenue
   step-changes from a signed customer.

Each planned change lands in the specific month of its
`Cash in` or `Cash out` row in the base model. If you want to
model a change whose source is not yet signed (e.g., "the round
we're pitching"), put it in a *separate scenario column* labelled
so, not the base case.

### Part D — read the runway (about 30 min)

Compute and record three numbers from the model:

1. **Constant-burn approximation.** `current_cash / average_net_burn`.
2. **Full model projection — count of months.** The row number at
   which `Ending cash` first becomes negative, minus the current
   row. If it never goes negative in 24 months, note that.
3. **Full model projection — calendar month.** The dated month
   that corresponds to (2). Present both formats.

Compare the two projections. If the constant-burn approximation
and the full model diverge by more than 3 months, name — in one
sentence — the specific step-change in the forward plan responsible
for the gap.

Finally, assign the **zone** per chapter 01 (Green / Yellow / Red)
based on the full model projection, and write one sentence naming
the boundary you used.

### Part E — the honesty check (about 30 min)

Before you're done, run the five-point honesty check derived from
chapter 01's failure modes. For each check, write one sentence
naming the outcome:

1. **Constant-burn only?** Are you relying on the approximation as
   your headline, or is the full projection the answer?
2. **Dated months?** Every row a real calendar month, not a
   relative label?
3. **Unsigned money in the base case?** Is any planned cash in the
   base case not backed by a signed instrument? If yes, move it
   to a scenario column.
4. **Semi-annual and annual costs?** Are annual legal renewals,
   insurance premiums, annual SaaS bills, tax filings, and
   accountant invoices in the specific months they land in?
5. **Weekly touch discipline?** Do you have a plan to update this
   model at least once a week (chapter 01's cadence)?

Any check that fails gets fixed before Part F.

### Part F — the summary line (about 15 min)

Write one sentence, in the form you would say it to a co-founder
or a candidate investor at the top of a conversation:

> *"We have $X on hand, we're burning $Y a month, our runway is
> approximately N months (through calendar month M), zone: Z."*

That single sentence is the model's job. If you can say it, from
memory, on Friday afternoon, without opening the spreadsheet, the
model is doing its job. If you can't, either the sentence needs
more work or the model is too complex to summarise.

## Deliverable shape

Two artifacts:

**1. The spreadsheet.** A single file with:
   - The base model (24 rows, seven columns).
   - The forward plan (hires, non-hire changes, cash in), with
     sources.
   - Optional: one or two clearly-marked scenario columns.
   - A sources tab noting where each input came from.

**2. A short Markdown write-up**, `mod-005-exercise-01-runway-model.md`,
structured:

```markdown
# Runway Model — [Startup Name]

## Setup
<one paragraph startup context; sources of truth for the numbers>

## Model summary
- Starting cash: $X (as of YYYY-MM-DD, source: ...)
- Average base monthly cash in: $Y (source: ...)
- Average base monthly cash out: $Z (source: ...)
- Base monthly net burn: $B

## Forward plan (base case)
- <hire 1, month, cost, source>
- <hire 2, month, cost, source>
- <non-hire change 1, month, effect, source>
- <cash-in event 1, month, amount, source>

## Runway readings
- Constant-burn approximation: N months
- Full model projection: N months, ending YYYY-MM
- Zone: GREEN / YELLOW / RED
- Divergence between approximations: <one sentence, if any>

## Honesty check
1. Constant-burn only? <one sentence>
2. Dated months? <one sentence>
3. Unsigned money in the base case? <one sentence>
4. Semi-annual / annual costs? <one sentence>
5. Weekly touch discipline? <one sentence>

## The summary line
<one sentence in the form of the Part F template>

## What surprised me
<two to four sentences on what building the model taught you that
you didn't know before>
```

Total write-up length: 500–1000 words.

## Starter guidance

- **Use whatever spreadsheet you already use.** Google Sheets,
  Excel, Numbers, Airtable, plain CSV. The exercise is about the
  shape and the discipline; the tool doesn't matter.
- **Fill inputs from real sources or realistic estimates — not
  aspirations.** If the base burn is $30k/month today and you
  hope to get it to $18k, put $30k in the base case and $18k in a
  scenario column.
- **If you don't know a number, name that.** *"Cash on hand:
  unknown — need to reconcile with bank statement"* is a
  perfectly acceptable input for the first draft. It tells you
  what to do next (get the bank statement) and it appears on the
  model so you don't forget.
- **Don't over-engineer.** Twenty-four rows, seven columns, one
  companion tab. If your model has ten tabs and pivot tables and
  a dashboard, you have built a fundraise model, not a runway
  model. Trim.

## Acceptance criteria

You have completed the exercise when:

- [ ] A one-paragraph startup context is written, naming the
      startup's stage and the two-or-three sources of truth for
      its numbers.
- [ ] A 24-row, seven-column runway model exists in a spreadsheet
      with every row a *dated month*.
- [ ] Every input (starting cash, base cash in, base cash out,
      each forward-plan item) has a documented source.
- [ ] The forward plan carries every hire, spend change, and
      cash-in event over the 24-month horizon, each dated to its
      specific month.
- [ ] Any planned cash in without a signed instrument is in a
      *separate scenario column*, not the base case.
- [ ] Both the constant-burn approximation and the full model
      projection are computed; any divergence is explained in one
      sentence.
- [ ] Runway is expressed as both a count of months *and* a
      calendar month, plus a zone (Green / Yellow / Red).
- [ ] The five-point honesty check is answered (one sentence per
      point).
- [ ] The one-sentence summary line is written in the Part F
      template form.
- [ ] The write-up file is committed as
      `mod-005-exercise-01-runway-model.md`.

## Common failure modes to avoid

- **Reporting only the constant-burn approximation.** The
  approximation is a check; the full projection is the answer.
- **Rows labelled "Month 1, Month 2, ..."** — dated months
  survive time; abstract labels don't.
- **Counting a signed-but-unfunded round in starting cash.**
  Starting cash is what would wire out today. Announcements go in
  scenario columns.
- **Modelling the salaries and forgetting the payroll tax and
  benefits.** For US-based operations these are typically 15–25%
  on top of cash comp; missing them under-states burn
  meaningfully.
- **A 24-tab spreadsheet.** One base sheet, one forward-plan
  sheet, one sources sheet. Anything more is scope creep.

## What good looks like

A model that, six months from now, is still being updated every
Friday because it is small enough to update and useful enough to
consult. A summary line the founder can say out loud without
looking at the spreadsheet. A forward plan that catches every
step-change the founder has already committed to. A honest zone
(Green / Yellow / Red) that reflects reality rather than a
target.

The specific test: if a co-founder or a candidate investor asked
you *"how much runway do you have?"* right after you finished
this exercise, could you answer with one number and one date,
without hedging? If yes, the exercise did its job.
