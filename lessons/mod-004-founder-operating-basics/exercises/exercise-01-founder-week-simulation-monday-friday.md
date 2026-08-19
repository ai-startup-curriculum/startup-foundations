---
module: mod-004-founder-operating-basics
exercise: exercise-01
slug: founder-week-simulation-monday-friday
hours: 3
prereqs: [chapter-01-the-operating-loop, chapter-02-the-weekly-cadence, chapter-03-the-decision-log]
---

# Exercise 01 — Founder Week Simulation: Monday to Friday

## Problem statement

Chapters 01–03 installed the four-part operating loop and its
weekly cadence artifacts. This exercise is where those chapters
first get exercised as one system, end-to-end, across a single
simulated week.

You will simulate one week for a specific PRE-SEED / SEED startup
— a real one or a well-specified hypothetical — and produce the
four operating-loop artifacts that fall out of a real founder
week: a **Monday plan**, a **Wednesday metrics check note**, a
**Friday shipped-and-learned**, and the **decision-log entries**
made during the week. The simulation is deliberate: you are not
running a real week, you are *staging* one to prove you can build
the interlocked artifacts and see the failure modes the chapters
described.

## Requirements

### Part A — the setup (about 30 min)

Pick a startup for the simulation. Two options:

- **Real startup you have some access to.** Your own current or
  prior venture, one you're advising, one whose founder is a close
  friend or a former co-worker. Anonymise names/numbers if
  needed; the exercise doesn't require identifiable detail, just
  realistic detail.
- **Hypothetical startup you construct.** A PRE-SEED or SEED
  company at a realistic stage, with a defensible product, a
  named ICP, a named North-Star metric, a plausible runway
  (three-to-eighteen months), and one to three people on the
  operating side. If you construct one, spend real thought on the
  specifics — a hypothetical that is too vague makes the whole
  simulation fake.

Write a **one-paragraph setup**: what the startup does, current
stage (PRE-SEED or SEED per mod-003), how many people are on the
operating side, roughly how much runway, and the current chosen
North-Star metric.

Then write, in three or four sentences, **what happened in the
week before this one** — what shipped, what didn't, what
customer signal came in, what's carried over. This is the
substrate the simulated week's Monday plan will build against.

### Part B — the Monday plan (about 30 min)

Write the Monday plan for the simulated week, in the shape
specified in chapter 02. Four sections:

1. **This week's three-to-five things.** Each item: one sentence,
   verb-first, with a rough founder-attention hours budget.
2. **What is on the metrics one-pager this week.** One line per
   number — current value, target for the week, expected
   direction.
3. **Decisions expected this week.** One line per anticipated
   founder-only call.
4. **What could take the week off-course.** Two-to-three concrete
   named risks (not paranoia).

Length ceiling: one page.

Constraint: at least one plan item must visibly advance a KR.
(You are not required to have authored the full OKR — exercise
04 covers that — but you should be able to name the current
quarterly objective in one line to check that at least one plan
item is doing work for it.)

### Part C — one mid-week disruption (about 15 min)

The point of the exercise is not to run a friction-free week.
Real weeks have inbound. Write **two-to-three sentences describing
one realistic mid-week event** that happens on Tuesday or
Wednesday and that a real founder would have to respond to. Some
options:

- A customer reports the flagship feature is broken for their
  whole account.
- A candidate you extended an offer to counter-offers with 30%
  more comp.
- A prospective investor reaches out unexpectedly and asks for a
  meeting Thursday.
- A key metric moves in the wrong direction by more than you
  expected.
- A co-founder or first employee raises a concern that changes
  what should happen this week.

Then write, in two-to-three sentences, **how the founder responds**
in a way that is consistent with the operating loop from chapter
01. You may (and often should) update the Monday plan in response
— that is normal. If you do, note the update as a *plan revision*
with a timestamp; do not silently overwrite the Monday version.

### Part D — the decision log (about 30 min)

Write **five-to-eight decision-log entries** made during the
simulated week, in the three-column shape from chapter 03: date,
decision (one sentence, past-tense, verb-first), reason (one-to-three
sentences).

Cover a spread of categories: at least one product / customer
call, at least one people / hiring call, at least one capital /
spend call, at least one strategy / prioritisation call.

At least one of the entries should be the response to the
mid-week disruption from Part C.

At least one of the entries should be a decision that was made
*by inaction* — the founder chose not to make an explicit call
and the default prevailed. Log it explicitly per chapter 03's
rule.

### Part E — the Friday shipped-and-learned (about 30 min)

Write the Friday shipped-and-learned in the shape from chapter
02. Three sections:

1. **Shipped.** One line per thing that shipped this week
   (delivered, deployed, signed, closed). Half-shipped things do
   not go here.
2. **Learned.** Two-to-five sentences on what the week told you
   that you didn't know on Monday. Each Learned should be
   anchored to a specific number that moved, a specific
   customer signal, or a specific decision from the log.
3. **What next week has to carry.** Two lists: unfinished plan
   items rolling over, and new items generated by this week's
   events.

Length ceiling: one page.

Constraint: at least one Learned entry should reference a
decision-log entry from Part D (by date) and reflect on whether
the reason held up as the week unfolded.

### Part F — the debrief (about 15 min)

Write a **one-paragraph debrief** on the simulation itself. Not
what the simulated founder learned about the week — what *you*
learned about the operating loop from having to run it end to
end. Some questions to answer at least one of:

- Which of the four loop parts (decide / allocate / communicate
  / measure) felt heaviest? Which felt lightest? Why?
- Which failure mode from chapter 01 did you see yourself
  drifting toward during the simulation, and how did the
  artifacts catch it?
- What is one thing about the shape of the artifacts you would
  change if you were sizing them for the *specific* startup you
  chose?

## Deliverable shape

A single Markdown file, `mod-004-exercise-01-founder-week-simulation.md`,
structured:

```markdown
# Founder Week Simulation — Monday to Friday

## Setup
<one paragraph startup context; three-to-four sentence "week before" context>

## Monday plan (2026-M-D)
### This week's three-to-five things
- ...
### On the metrics one-pager this week
- ...
### Decisions expected this week
- ...
### What could take the week off-course
- ...

## Mid-week disruption (2026-M-D)
<two-to-three sentence event; two-to-three sentence response>
### Plan revision (if any)
- ...

## Decision log entries this week
| Date | Decision | Reason |
|---|---|---|
| ... | ... | ... |

## Friday shipped-and-learned (2026-M-D)
### Shipped
- ...
### Learned
- ...
### What next week has to carry
- Roll-overs: ...
- New: ...

## Debrief
<one paragraph on what you learned about the loop itself>
```

Total length: 1200–1800 words across the whole file. The artifact
shapes themselves are one-page each; the debrief and setup add
context.

## Starter guidance

- **Choose one startup for the whole simulation.** Do not switch
  midway. The interlocks between Monday plan → metrics → Friday
  shipped-and-learned only work if all three are about the same
  reality.
- **Fill numbers with realistic specificity.** "Retention is
  going up" is not a metric line. "D7 retention: 24% current,
  28% target this week, up." is. If you don't have real numbers,
  make plausible ones up — the exercise is about the *shape*,
  not the accuracy of the numbers.
- **Write in a real founder's voice, not a template voice.** The
  artifacts a real founder writes are terse, specific, and
  slightly informal. If your Monday plan reads like a
  consulting deliverable, cut adjectives until it reads like a
  note to yourself.
- **Make the disruption disruptive.** The mid-week event should
  actually change something in the week. If the response is "no
  change to plan," you picked too small a disruption; pick a
  bigger one.
- **Read chapter 03 before writing the decision log.** The
  three-column shape looks trivial and is not; the reason
  column is where the exercise is either passed or failed.

## Acceptance criteria

You have completed the exercise when:

- [ ] A setup paragraph and prior-week context establish the
      simulated startup, its stage, its people count, its runway,
      and its North-Star metric.
- [ ] A Monday plan in the four-section shape is present,
      one-page-max, with hours budgets on the three-to-five
      things and at least one item advancing a stated KR.
- [ ] A mid-week disruption and the founder's response are
      documented; any plan revision is dated and separate from
      the original Monday plan.
- [ ] Five-to-eight decision-log entries are present in the
      three-column shape, spread across at least four categories
      (product/customer, people, capital, strategy), including
      at least one decision-by-inaction and at least one
      response to the disruption.
- [ ] A Friday shipped-and-learned in the three-section shape
      is present, one-page-max, with at least one Learned that
      references a decision-log entry by date.
- [ ] A one-paragraph debrief reflects on the loop itself, not
      just the simulated week's content.
- [ ] The file is committed to your notes as
      `mod-004-exercise-01-founder-week-simulation.md`.

## Common failure modes to avoid

- **Perfect week theatre.** A simulation with no disruption, no
  off-track KR, no reason-in-doubt log entry, and no plan
  revision is telling you that you skipped the honest part. Real
  weeks have friction; simulated weeks that don't are practicing
  the wrong muscle.
- **Wall-of-text artifacts.** Any of the four artifacts over one
  page is failing the primary discipline (chapter 02 explicitly:
  the length ceiling is the artifact's shape). Trim until each
  is one page or less.
- **Log entries that record activity, not decisions.** "Talked
  to five customers." Not a decision. "Committed to closing the
  acme.co pilot before opening new-segment outbound." That's a
  decision.
- **Learned entries that read like a diary.** Chapter 02: Learned
  is what the week told you you didn't know on Monday, not how
  you felt about the week.
- **Every plan item tied to the same KR.** If all three-to-five
  plan items point at one KR, either the OKR has one KR (violates
  chapter 04) or the plan is too narrow to run the actual
  company for a week.

## What good looks like

A simulation whose four artifacts a *reader* — a friend, a
mentor, another Foundations learner — could pick up, read in ten
minutes, and immediately understand (a) what the simulated
startup is trying to do this quarter, (b) what specifically got
worked this week, (c) what decisions were made and why, (d) what
the founder learned, and (e) what next week has to pick up.

If a reader has to ask any of those five questions after reading
your four artifacts, an interlock from chapter 02 is broken.
Fix the interlock, not the reader's question.

The simulation is not the real thing; the *lab* (authored in a
separate cycle) will run a real week with real artifacts. This
exercise is where you prove the shapes work together before
you spend a real week's founder-attention on them.
