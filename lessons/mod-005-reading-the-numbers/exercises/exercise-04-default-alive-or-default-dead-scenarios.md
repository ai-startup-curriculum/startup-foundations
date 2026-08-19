---
module: mod-005-reading-the-numbers
exercise: exercise-04
slug: default-alive-or-default-dead-scenarios
hours: 4
prereqs: [chapter-04-default-alive-or-default-dead]
requires: [exercise-01-build-a-runway-model-from-zero, exercise-02-gross-vs-net-burn-drill, exercise-03-growth-rate-wow-and-mom-calculation]
---

# Exercise 04 — Default Alive or Default Dead: Scenarios

## Problem statement

Chapter 04 formalised the Paul Graham default-alive / default-dead
composite: at your current growth rate, does projected revenue
cross projected expense before projected cash goes to zero? This
exercise is where you actually run the composite — for a real base
case and two variations — for the startup from exercises 01–03.

The exercise is the most consequential in the module. The verdict
is a live signal, not a one-time reading, but the *first* time you
run it end-to-end is the moment the module's whole argument becomes
real for your specific startup. If you never sit down and compute
the two lines, chapter 04 was theory. This exercise makes it
practice.

## Requirements

### Part A — assemble the four inputs (about 30 min)

Pull the four inputs from prior exercises:

1. **Current cash** — from the runway model in exercise 01.
2. **Current net burn** — from exercise 02. Choose between net
   burn and net-burn-after-variable-revenue per chapter 04's
   guidance (if the two diverge, use the higher / more honest
   number). Record the choice and the reason.
3. **Current growth rate** — from exercise 03. Use the trailing
   four-week WoW converted to monthly-equivalent, or the
   trailing-three-months MoM if you are post-PMF. If your
   underlying quantity is not revenue, you need one more input:
   a *defensible translation* from the North-Star to revenue
   (e.g., "revenue growth tracks paying-customer growth 1:1 at
   this stage because ARPA is stable").
4. **Current forward plan** — from exercise 01's forward-plan
   table.

**Deliverable A**: a four-row table listing each input, its value,
its source, and (for net burn and growth rate) the specific
definitional decision that produced the value.

### Part B — build the base-case projection (about 60 min)

Extend your exercise 01 runway model with two new columns
alongside `Cash out (gross)`:

- **Projected revenue** — starting from current revenue, growing
  at the current monthly growth rate. `revenue[m] = revenue[m-1] ×
  (1 + monthly_growth_rate)`.
- **Projected expense** — starting from current gross monthly
  cash out and stepped up per the forward plan (hires, non-hire
  spend changes) in the months they land.

Recompute `Ending cash` in the model as:

```
Ending cash[m] = Ending cash[m-1] + Projected revenue[m] − Projected expense[m]
```

Note that this replaces the base-case cash-in and cash-out lines
in the projection — the composite runs the projection off *growth
of revenue*, not off the flat cash-in assumption from exercise 01.

Read the two crossings:

- **`m_c` — profitability crossover** — the smallest `m` for
  which `Projected revenue[m] ≥ Projected expense[m]`.
- **`m_z` — zero-cash** — the smallest `m` for which
  `Ending cash[m] < 0`.

**Verdict**:

- **DEFAULT ALIVE** if `m_c ≤ m_z`.
- **DEFAULT DEAD** if `m_c > m_z`, or if `m_c` never occurs in
  the 24-month horizon.

**Deliverable B**: the base-case projection with the two
crossings identified and the verdict written in one sentence,
per chapter 04's language.

### Part C — scenario 1: growth cut (about 45 min)

Copy the base case into a new column set. Change one input:
**cut the growth rate in half**. Everything else — cash, burn,
forward plan — stays the same.

Re-run the projection. Re-read `m_c` and `m_z`. Record the new
verdict.

Then answer, in two-to-three sentences:

- **Did the verdict flip?** From alive to dead, or dead to
  worse-dead, or (if the base was dead) unchanged.
- **What does the growth-cut scenario correspond to in the real
  world?** Naming a specific plausible cause is what makes the
  scenario useful: *"one of the three pilot customers churns,"*
  *"the new-signup channel we've been using degrades,"* *"the
  competitor lands the segment we've been converting from."*

### Part D — scenario 2: burn cut (about 45 min)

Copy the base case again. This time change a different input:
**cut monthly gross burn by 25%**. Practically, this means one
of these moves (pick the one most realistic for your startup):

- Defer the next planned hire by six months.
- Defer *all* planned hires until after `m_c` in the base case.
- Reduce a specific non-hire spend line (marketing budget, a
  contractor, a tools consolidation) — name which.
- A founder-paycut plus a specific spend reduction (name both).

Re-run the projection. Re-read `m_c` and `m_z`. Record the new
verdict.

Then answer:

- **Did the verdict flip?** From dead to alive, from marginal to
  robust, from alive-with-Green-runway to alive-with-Yellow.
- **What is the operating cost of the burn-cut?** A deferred
  hire is not free — the North-Star may grow more slowly without
  the extra capacity. Name the trade-off in one sentence.

### Part E — the composite reading (about 30 min)

Write, in a short prose paragraph (four to six sentences), the
composite reading for the startup as of today. Cover:

- The **base-case verdict** in one sentence.
- The **key sensitivity** — which of the four inputs, when moved
  in a realistic direction, most changes the verdict. (Exercises
  02, 03, and this exercise are your evidence.)
- The **specific lever most within your control** to hold or
  flip the verdict from where it is today, and the mod-004
  decision-log entry you would need to log to pull it.

This paragraph is the exercise's core output. It is what you would
say to a co-founder at the beginning of the Monday plan the week
after you finish this exercise.

### Part F — the update discipline plan (about 20 min)

Write, in three bullets, the specific cadence at which you will
re-run the composite going forward:

- **Weekly** — which mod-004 metrics-one-pager touch triggers the
  re-check.
- **Monthly** — which mod-004 investor-update authoring triggers
  the full re-projection.
- **Per decision-log entry** — which specific categories of
  decision (hire, defer, spend, cash in) will trigger an
  immediate re-run.

This is what turns the composite from a one-time exercise into a
live artifact.

## Deliverable shape

Two artifacts:

**1. The extended runway model** with the projected revenue and
projected expense columns, the base-case projection, and both
scenario columns.

**2. A Markdown write-up**, `mod-005-exercise-04-default-alive.md`,
structured:

```markdown
# Default Alive or Default Dead — [Startup Name]

## Inputs
| Input | Value | Source | Definitional note |
|---|---|---|---|
| Current cash | ... | exercise 01 | — |
| Current net burn | ... | exercise 02 | <net vs net-after-variable-revenue> |
| Current growth rate | ... | exercise 03 | <cadence and underlying quantity> |
| Current forward plan | (see below) | exercise 01 | — |

Forward plan summary:
- <hire 1, month, cost>
- <hire 2, month, cost>
- <non-hire change, month, effect>

## Base-case projection
- Profitability crossover (m_c): month N (calendar YYYY-MM)
- Zero-cash (m_z): month N (calendar YYYY-MM) or "never in horizon"
- Verdict: DEFAULT ALIVE / DEFAULT DEAD
- One-sentence reason: <chapter 04 language>

## Scenario 1 — growth rate cut in half
- New growth rate: X%
- New m_c: ...
- New m_z: ...
- New verdict: ...
- What this scenario corresponds to in the real world: <two-to-three sentences>

## Scenario 2 — 25% burn cut
- Specific burn-cut move: <one line>
- New m_c: ...
- New m_z: ...
- New verdict: ...
- Operating cost of the burn-cut: <one sentence>

## Composite reading
<four-to-six sentence paragraph per Part E>

## Update discipline
- Weekly: ...
- Monthly: ...
- Per decision-log entry: ...
```

Total write-up length: 700–1100 words.

## Starter guidance

- **Run the base case honestly before the scenarios.** If you
  find yourself wanting to nudge the base-case growth rate up
  because the verdict looks bad, resist. The base case is your
  best current-measurement estimate; the *scenarios* are where
  you explore what could change it.
- **Do the WoW→MoM conversion carefully.** Chapter 03: `(1 + WoW)^4.33 − 1`.
  A common error is multiplying by 4.33 or by 4, which gives a
  materially different number for larger WoW rates.
- **Do not conflate "default dead" with "failing."** Chapter 04
  and Graham's essay are explicit: many good startups are
  default-dead for portions of their life. The value is in
  knowing you are.
- **Do not run more than the two scenarios.** More scenarios are
  finance-pillar work (chapter 08's deferral). The two scenarios
  here — one on growth, one on burn — are the minimum viable
  sensitivity check.

## Acceptance criteria

You have completed the exercise when:

- [ ] All four inputs are documented in a table with sources and
      definitional notes.
- [ ] The base-case projection is run in the extended runway
      model, with `m_c` and `m_z` explicitly identified.
- [ ] The base-case verdict (DEFAULT ALIVE or DEFAULT DEAD) is
      written in chapter-04 language.
- [ ] Scenario 1 (growth cut in half) is run, verdict recorded,
      and real-world correspondence named.
- [ ] Scenario 2 (25% burn cut) is run, verdict recorded, and
      operating trade-off named.
- [ ] A four-to-six-sentence composite-reading paragraph is
      written.
- [ ] The update-discipline plan is written in three bullets.
- [ ] The write-up is committed as
      `mod-005-exercise-04-default-alive.md`.

## Common failure modes to avoid

- **Aspirational growth rate.** The base case uses the *measured*
  rate from exercise 03, not the rate you think you can hit.
  Aspiration goes in a *third* scenario (which this exercise
  does not require but you may add).
- **Base case computed on net burn when the two burns diverge.**
  Chapter 02 and chapter 04 both apply: use the honest number.
- **Verdict without a written reason.** *"DEFAULT ALIVE"* alone
  is not a verdict; it is a label. The reason is what makes it
  defensible next week when the numbers move.
- **Running the composite once and never again.** Part F exists
  because the composite is a live signal, not a one-shot.
- **Skipping the two scenarios because the base case looks
  fine.** The scenarios are where the sensitivity becomes
  visible, which is where the actionable insight lives.

## What good looks like

A finished exercise where the founder can, from the composite-
reading paragraph, name in one sentence today whether the
startup is default alive or default dead, name the input that
would flip the verdict fastest, and name the specific move they
would make against a decision-log entry to defend or change the
verdict. If a co-founder read the paragraph tomorrow morning,
they should be able to agree or disagree with the verdict on the
evidence — not the founder's feeling.
