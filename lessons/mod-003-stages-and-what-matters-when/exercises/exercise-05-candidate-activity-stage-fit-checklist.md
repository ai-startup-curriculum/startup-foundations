---
module: mod-003-stages-and-what-matters-when
exercise: exercise-05
slug: candidate-activity-stage-fit-checklist
hours: 3
prereqs: [chapter-06-the-stage-fit-checklist]
---

# Exercise 05 — Candidate-Activity Stage-Fit Checklist

## Problem statement

Chapter 06 gave you the six-question stage-fit checklist and the
four-verdict output — proceed, defer, delegate, replace. This
exercise is where the checklist stops being a chapter and starts
being an operating tool.

You will apply the checklist to **five real (or realistic) candidate
activities** across **three different stages**, produce a verdict for
each with the defence line, and then produce a **retrospective read**
of one of the activities as if a week had passed and you were
evaluating whether the verdict held.

The output is an artifact you will reuse in mod-004 (`Founder
Operating Basics`) as the input format for the weekly plan and the
weekly review. Treat this exercise as the template, not the
one-off.

## Requirements

### Part A — pick five candidate activities

Pick **five distinct candidate activities** across **three different
stages**. Suggested spread:

- **2 activities at IDEA / PRE-SEED** — a mix of activities that
  should verdict as *proceed* and activities that should verdict as
  *defer* (working ahead) or *replace* (wrong branch).
- **2 activities at SEED / SERIES-A** — the transitional stages
  where mismatch shapes 1, 2, and 3 are all common.
- **1 activity at GROWTH / MATURE** — often the stage where
  founders are prone to shape-2 mismatches (not letting go of
  earlier work).

The activities can be:

- Activities from your own real or hypothetical startup.
- Activities you have seen described in a real, publicly documented
  startup's operating cadence (a founder update, a podcast
  transcript describing a founder's week, an S-1 section on
  strategy).
- Activities from the case studies in exercise 02 (mismatch
  teardowns) or exercise 04 (post-mortem read). Reusing exercises 02
  and 04 material is fine — it means you're building on the same
  base.

The activities must be **specific**. Not "improve GTM" or "hire
better." Specific: "retain a fractional CFO for 20 hours a month at
$8k/mo," "sign a two-year enterprise SaaS contract with
[specific-tool] for the entire team," "personally do a two-hour
onboarding call with every new user this month."

Cover **at least one instance of each of the four verdicts** —
proceed, defer, delegate, replace — across the five activities. If
your five activities all verdict as *proceed*, you have picked too
softly; find at least one candidate that fails the checklist so
you exercise the verdict-and-defence machinery.

### Part B — run the checklist for each activity

For each of the five activities, run the full six-question
checklist from chapter 06 in order. Produce the checklist output in
this structure:

```markdown
### Activity N: <one-line description>

**Stage of the founder:** [X]

**Q1 — Node:** [node on mod-002 graph]
**Q2 — Current stage:** [stage, with 1-line signal evidence]
**Q3 — In typical focus?** yes / no. [one line]
**Q4 — Premature-scaling dimension check:**
- Team: [yes/no with 1-line]
- Product: [yes/no with 1-line]
- Customer: [yes/no with 1-line]
- Business model: [yes/no with 1-line]
- Financials: [yes/no with 1-line]
**Q5 — Contributes to stage's core question?** yes / no / partial. [one line]
**Q6 — Right person?** yes / no. [one line]

**Verdict:** [proceed / defer / delegate / replace]

**Defence line:** <full defence-line format from chapter 06>

**Falsification signal:** <one line — what would tell you the
verdict was wrong>
```

The **falsification signal** is not in chapter 06's minimum verdict
form; add it here because it turns the verdict from a decision into
a *testable* decision. The signal is what you look for over the
next 1–4 weeks to see whether the verdict held.

### Part C — produce one override

For one of the five activities — ideally one where the checklist
verdicts as *defer* or *replace* — walk through the **override
protocol** from chapter 06:

- Which check is being overridden (Q1–Q6).
- Why the check does not apply to this specific case (one
  paragraph — the specific reason your case is a legitimate
  exception).
- What signal would tell you the override was wrong.
- When you will re-run the checklist to see if the exception has
  passed.

The override is not a rubber stamp. Force yourself to write the
override paragraph honestly. If you find you can't defend the
override in writing, the correct move is to accept the original
verdict — that is the point of the protocol.

### Part D — one retrospective read

Pick **one of the five activities** and produce a **retrospective**
read as if one week has passed. Imagine the week happened, the
activity was executed (or deferred, or delegated, or replaced per the
verdict), and you're now looking back to check whether the verdict
held.

Produce:

- **What actually happened.** One paragraph — a plausible narration
  of what the week looked like if the verdict was followed.
- **Did the falsification signal fire?** One line — yes / no / it's
  too early to tell.
- **Would you re-verdict differently now?** One paragraph — if
  yes, what changed; if no, what re-confirmed the verdict.

The retrospective is a rehearsal for the mod-004 Friday review that
this artifact will feed into. It teaches you to *close the loop* on
checklist verdicts rather than treating them as write-and-forget
decisions.

## Deliverable shape

A single Markdown file, `mod-003-exercise-05-stage-fit-checklist.md`,
structured:

```markdown
# Candidate-Activity Stage-Fit Checklist — Five Cases

## Part A — activity list

| # | Activity | Stage | Expected verdict |
|---|---|---|---|
| 1 | ... | IDEA | proceed |
| 2 | ... | PRE-SEED | defer |
| ... | ... | ... | ... |

## Part B — checklist runs

### Activity 1: <one-line description>
<full checklist structure from above>

### Activity 2: ...
...

## Part C — the override

**Activity being overridden:** [N]
**Check being overridden:** [Q1-Q6]
**Reason the check does not apply:** <one paragraph>
**Falsification signal:** <one line>
**Re-check date:** <specific date or trigger>

## Part D — the retrospective

**Activity:** [N]
**What actually happened:** <one paragraph>
**Did the falsification signal fire?** <one line>
**Would you re-verdict?** <one paragraph>
```

Total length: 1500–2500 words across the five checklist runs plus
the override and retrospective.

## Starter guidance

- **Specific activities, not categories.** "Do customer discovery"
  is a category. "Schedule 20 30-minute cold calls with prospects
  in [specific segment] over the next 10 days" is an activity. The
  checklist works on activities, not categories.
- **Force at least one non-*proceed* verdict.** If you softball
  the exercise so everything verdicts as proceed, you don't
  exercise the defend-and-defer machinery. The checklist earns
  its keep on the hard cases.
- **The falsification signal has to be observable.** "The
  activity was successful" is not observable. "Three of the 20
  calls resulted in a follow-up meeting" is observable. Signals
  are the same discipline as the stage-signal drill from exercise
  01.
- **The override paragraph is where honesty is tested.** It is
  easy to override a checklist verdict when you don't have to
  write down why. Forcing the write-up filters out the overrides
  you can't actually defend.
- **The retrospective doesn't require a real week to have
  passed.** Simulate it. The goal is to build the *loop-closing
  habit*, not to schedule a follow-up in your calendar.

## Acceptance criteria

You have completed the exercise when:

- [ ] Five specific candidate activities are chosen across at
      least three different stages.
- [ ] Each activity has a full six-question checklist run with
      Q1 through Q6 answered explicitly.
- [ ] The five activities collectively produce all four verdict
      types (proceed, defer, delegate, replace) — at least one
      of each.
- [ ] Each verdict has a defence line in the chapter-06 format
      and a falsification signal.
- [ ] One override is produced with the four-part structure
      (check overridden, reason, falsification, re-check date).
- [ ] One retrospective is produced with the three-part structure
      (what happened, did signal fire, would you re-verdict).
- [ ] The file is committed to your notes as
      `mod-003-exercise-05-stage-fit-checklist.md`.

## Common failure modes to avoid

- Vague activities. Every activity should be specific enough
  that a reader could tell if it happened or not.
- All-proceed verdicts. The checklist earns its keep on the
  hard cases; force at least one non-proceed verdict per two
  activities.
- Un-observable falsification signals. If the signal is not
  something you could actually measure in the next 1-4 weeks,
  it isn't a signal.
- Rubber-stamping the override. If you find you can't write
  the override paragraph honestly, accept the original
  verdict.
- Skipping the retrospective because the week hasn't happened.
  Simulate it. The retrospective habit is the loop-closing
  mechanism that keeps mod-004's cadence honest.

## What good looks like

A five-activity checklist run that a co-founder or a solo founder
could adopt directly as the input format for their weekly plan.
The verdicts should be specific, the defence lines should be
defensible, and the retrospective should model what closing the
loop feels like.

You will carry this artifact forward into mod-004 (`Founder
Operating Basics`) where the checklist becomes part of the
Monday-plan / Friday-review cadence. The stage vocabulary from
this whole module gets its operational payoff in that cadence.

If you are a working founder rather than a learner, this exercise
is the moment to convert the module into a live operating tool.
Take the checklist run you produced here and apply it to next
week's actual plan. The exercise then stops being an exercise and
starts being how you run your week.
