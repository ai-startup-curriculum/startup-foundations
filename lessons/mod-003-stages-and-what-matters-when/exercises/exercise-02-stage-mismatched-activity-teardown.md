---
module: mod-003-stages-and-what-matters-when
exercise: exercise-02
slug: stage-mismatched-activity-teardown
hours: 2
prereqs: [chapter-02-walking-the-stage-ladder, chapter-03-stage-mismatched-activity]
---

# Exercise 02 — Stage-Mismatched Activity Teardown

## Problem statement

Chapter 03 named the three shapes of stage-mismatched activity — **working
ahead**, **not letting go**, and **working the wrong branch** — and gave
the four-step diagnosis: locate the activity on the mod-002 graph, locate
the founder on the stage ladder, ask if the node is in that stage's
typical focus, classify the mismatch and name the correct current focus.

This exercise is where you run the diagnosis on real, publicly documented
cases and produce a teardown that another founder could learn from.

You will find **three real, publicly documented examples** — one for each
of the three mismatch shapes — and, for each, produce a full four-step
teardown plus the recommended replacement activity.

## Requirements

### Part A — pick three real cases

Find **three real, publicly documented cases** of stage-mismatched
activity. Each case must be from a **different mismatch shape**:

- **One case of shape 1 — working ahead.** A founder doing later-stage
  work at an earlier stage.
- **One case of shape 2 — not letting go.** A founder still doing
  earlier-stage work long past when it should have been delegated.
- **One case of shape 3 — working the wrong branch.** A founder
  spending majority attention on a branch of the graph that isn't
  where the current stage's binding constraint lives.

For each case, the source material has to be enough that an outside
reader could verify the diagnosis. Acceptable sources:

- Founder essays where the founder describes what they were doing
  and, ideally, why in retrospect it was the wrong focus. (Post-mortem
  essays are gold for shape 1 and shape 3.)
- Failure-of-a-good-idea case studies — CB Insights, Founder
  Collective mortemas, published startup-obituary essays.
- Long-form founder interviews (podcasts, magazine profiles) where
  the founder describes their weekly focus at a specific stage.
- S-1 filings and 10-Ks that describe changes in organisational
  structure or founder role over time.
- Published board minutes, quarterly investor letters (rare but
  exist), or shareholder letters where the founder describes their
  focus.

Not acceptable sources:

- A private startup you know personally through insider access.
- A company blog post where the founder describes their focus at
  the time of writing. (Not because the founder is lying, but
  because the framing lags the actual outcome and you can't yet see
  whether the focus turned out to be mismatched.)
- Any case where you have to speculate about what the founder was
  actually doing week to week. If you can't cite the specific
  activity, you can't do the teardown.

### Part B — the four-step teardown

For each of the three cases, produce a **four-step teardown** in the
shape chapter 03 specifies:

1. **Locate the activity on the mod-002 graph.** Which node does the
   activity live on? Be specific.
2. **Locate the founder on the stage ladder.** Use signal-column
   evidence (chapter 02), not the funding round name. Cite the
   observable evidence.
3. **Ask: is the node in the stage's typical focus?** Refer to
   chapter 02's typical-focus column. Yes / no with a one-line
   reason.
4. **Classify the mismatch and name the correct current focus.**
   Which of the three shapes? What *specific* stage-appropriate
   activity should have taken the slot?

### Part C — the counterfactual

For each case, write a **one-paragraph counterfactual**: what would
plausibly have happened if the founder had done the correct current
focus instead? Not a fantasy; a specific, defensible chain of what
would have changed. Anchor the counterfactual to what other
comparable startups at the same stage actually did.

The counterfactual is the discipline that keeps the teardown honest.
It is easy to say "this founder should have done X"; it is harder
to say "and here's what would plausibly have happened if they had,
based on this comparable case."

### Part D — cross-cutting note

After the three teardowns, write a **short cross-cutting note** (one
paragraph) that names something you saw *across the three cases*
that you wouldn't have seen looking at any one of them alone. For
example: the founder in all three cases had recently taken an
investment from a specific type of investor; or the mismatch
started right after a specific external event (a new hire, a
market shift, a media event); or the mismatch was defended by the
same rationalisation ("we'll need this eventually," "I'm the only
one who can do this").

## Deliverable shape

A single Markdown file, `mod-003-exercise-02-mismatch-teardown.md`,
structured:

```markdown
# Stage-Mismatched Activity Teardown

## Case 1 — Shape 1 (working ahead): <company / founder>

**Sources:** <URLs / citations>

### Part B — four-step teardown
1. Activity node: <node>
2. Founder stage: [stage]. Signal evidence: <2-3 items>.
3. In typical focus? No. Reason: <one line>.
4. Shape: 1 (working ahead). Correct current focus: <specific
   stage-appropriate activity>.

### Part C — counterfactual
<one paragraph>

---

## Case 2 — Shape 2 (not letting go): <company / founder>
<same structure>

## Case 3 — Shape 3 (wrong branch): <company / founder>
<same structure>

## Part D — cross-cutting note
<one paragraph>
```

Total length: 1000–1500 words across the three teardowns.

## Starter guidance

- **Post-mortem essays are the highest-value source.** Founders
  writing after the fact have the incentive alignment to name the
  mismatched activity honestly. Landing pages and current-tense
  blog posts do not.
- **Do not diagnose from the outcome.** Do not reason "the company
  failed, therefore they must have been doing mismatched work." The
  mismatch has to be visible in the *activity itself* — the founder
  spending weeks on X — not in the eventual outcome. Some
  mismatched activities coexist with success; some correctly-stage
  activities coexist with failure. The teardown is about the
  activity's stage fit, not the company's outcome.
- **Chapter 04's un-scalable hand-work is not a shape-2 mismatch
  at IDEA / PRE-SEED.** Do not diagnose an IDEA-stage founder
  personally onboarding early users as "not letting go." That is
  the correct current focus at that stage. Shape 2 is specifically
  about *continuing an earlier-stage activity past the stage
  transition* — e.g., a SERIES-A founder still personally onboarding
  every user.
- **Chapter 05's premature-scaling framing overlaps heavily with
  shape 1.** If a case reads as "the team hired ahead of the
  business," you're really looking at premature scaling on the
  team dimension. That is a legitimate shape-1 case; note the
  overlap in your teardown.
- **Do not use the same company for two cases.** Spread across
  three distinct companies. Different companies tend to fall into
  different mismatch shapes, and spreading catches that.

## Acceptance criteria

You have completed the exercise when:

- [ ] Three real, publicly documented cases — one per mismatch
      shape — are named and sourced.
- [ ] Sources are cited (URL / book / episode / filing reference)
      for each case.
- [ ] Each case has a full four-step teardown with the specific
      node, the stage placement (with signal evidence), the
      typical-focus check, and the shape classification with the
      correct current focus.
- [ ] Each case has a one-paragraph counterfactual grounded in a
      comparable startup's actual behaviour.
- [ ] A cross-cutting note names a pattern visible across the
      three cases that would not have been visible in any one
      alone.
- [ ] The file is committed to your notes as
      `mod-003-exercise-02-mismatch-teardown.md`.

## Common failure modes to avoid

- Diagnosing from the outcome ("they failed → the activity was
  wrong"). The mismatch is about the activity's stage fit, not
  about the eventual outcome.
- Naming the correct current focus in generic terms ("focus more
  on customers"). Chapter 02 has specific stage-appropriate
  activities; use the specific ones.
- Using the same company for multiple cases. Spread across three
  companies, ideally across three different industries or business
  models, to catch the shape-level pattern rather than the
  company-level idiosyncrasy.
- Skipping the counterfactual because it feels speculative. The
  counterfactual is the discipline that keeps the teardown from
  becoming Monday-morning quarterbacking. If you can't name a
  plausible alternative, your diagnosis is probably wrong.

## What good looks like

A three-case teardown that another founder could read as a working
example of *how the mismatch shapes show up in real companies*. A
reader should finish the file and be able to look at their own
week's activities and identify shape-1, shape-2, or shape-3
mismatches in their own work. If they can't, the teardown was
performed but not internalised.

The four-step diagnosis you practise here is what chapter 06's
checklist embeds as Q3 (typical focus) and the classification step.
This exercise is where the muscle gets built; the checklist is where
the muscle gets used every week.
