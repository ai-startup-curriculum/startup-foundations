# Lightweight OKRs at Two People — One Objective, Three KRs, Weekly Check-in

## Motivation

The weekly cadence artifacts from chapter 02 keep a founder's *week*
honest. On their own, they do not keep the quarter honest. Twelve
good weeks in a row can still add up to a quarter that went
sideways — if the weeks were each locally sensible but were not
adding up to the same larger commitment.

The tool for making a quarter's worth of weeks add up is a **goal**.
Concretely, at the scale this module cares about (a two-or-three
person startup at PRE-SEED or SEED), the tool this module recommends
is a **lightweight OKR** — one company objective, three key results,
weekly check-in — deliberately trimmed down from the full OKR
practice that Grove and Doerr documented for larger organisations.

This chapter installs the lightweight shape, explains why it works
at this scale, and — most importantly — names the four anti-patterns
that make OKRs at this scale go sideways. The anti-patterns are the
load-bearing part of the chapter; getting the shape wrong is far
easier than getting it right.

## The shape — one, three, weekly

Every quarter, the founder writes exactly one **Objective (O)** and
exactly three **Key Results (KRs)**. The whole thing fits on a
single sticky note. That is the entire scale of the practice at
this stage; if it gets bigger, chapter 07's ownership map says the
depth belongs in the operations pillar, not here.

**Objective.** One sentence, qualitative, ambitious, memorable. The
objective is what the quarter is *about*. It is the thing you would
say if a co-founder, a first employee, and a friendly investor each
asked "what are you focused on this quarter?" and you had to give
the same answer to all three.

Not "grow revenue." Not "improve product." Both of those are true
of every quarter forever; they say nothing about *this* quarter.
Better:

- "Prove we can close five accounting-firm customers without a
  founder in the room for the full sales cycle."
- "Make onboarding the day-one wow, not the week-one recovery."
- "Get to a repeatable second-week retention above 40%."

An objective is *directional*: pointed enough that you know where
"good" is, big enough that it is not obviously reached, focused
enough that you could describe the quarter as "the quarter we did
X" three months from now.

**Key results.** Exactly three, all quantitative, each independently
checkable, each tied to the objective in a way an outsider can see.

Not:
- "Talk to more customers." (No number.)
- "Ship the roadmap." (Not tied to the objective.)
- "Achieve product-market fit." (Not checkable inside a quarter.)

Better, for the second objective above ("make onboarding the day-one
wow"):
- KR1: median time-to-first-value drops from 22 minutes to under 5.
- KR2: percentage of new signups that reach the "first invoice
  sent" step within 24 hours rises from 18% to 50%.
- KR3: day-7 retention of new cohorts rises from 24% to 40%.

Each KR is a **number**, with a **starting value**, an **ending
target**, and a **direction**. If you cannot write a KR with those
three pieces, the KR is not yet a KR — go back and sharpen.

**Weekly check-in.** Every Friday, as part of the shipped-and-learned,
each KR gets a two-column update: current value and delta from last
week. If a KR is on-track, one line: "on track." If a KR is off-track,
two lines: "off track — cause; next-week action." The whole
check-in is the last five minutes of the Friday shipped-and-learned;
it does not need a separate meeting.

## Why one, why three, why weekly

Every one of the three parameters (one objective, three KRs, weekly
check-in) is a deliberate departure from the full OKR practice as
Grove and Doerr describe it. Each deviation is calibrated to the
scale this module addresses.

**Why exactly one objective?** In a larger company, teams have their
own objectives that ladder up to a company objective. A two-person
company has no laddering — the company objective *is* the founder's
objective, is the co-founder's objective, is the team's objective.
More than one company objective at this scale means the founder is
either (a) not focused, in which case the extra objectives are
distractions, or (b) actually a much bigger company than two
people, in which case chapter 07 says the OKR practice depth belongs
in the operations pillar.

**Why exactly three KRs?** Three is the smallest number of key
results that resists the "one metric" failure mode (where the KR
becomes the target and the objective is lost) and the largest that
fits in a founder's short-term memory. Two KRs is fragile — if one
turns out to be measuring the wrong thing, half the quarter's
instrumentation is gone. Four KRs starts optimising for coverage and
loses focus. The empirical rule in Grove's and Doerr's writing is
three-to-five for teams; at two-person scale, three is the ceiling,
not the mid-point.

**Why weekly, not quarterly?** The standard OKR practice runs on a
quarterly-set / quarterly-review cadence. That works at company
scale because the between-quarter drift is small relative to the
company's mass. At two-person / two-quarter scale, drift is fast —
five to six weeks of misalignment can cost the quarter. Weekly
check-in catches drift at the point it is small enough to correct
cheaply. It also folds naturally into the Friday
shipped-and-learned that is already firing.

## The four anti-patterns

These are the four failure modes the lightweight shape is
specifically designed to defend against. Each is common enough to be
worth naming. Each has a symptom, a cause, and a fix.

### Anti-pattern 1 — the goal that is really an activity

**Symptom.** The objective sounds like a to-do list. "Ship v2."
"Run the offsite." "Fix the deploy pipeline." All fine as work; none
are objectives. If the objective is achieved by completing a task
rather than by moving a state of the world, it is an activity.

**Why it happens.** Because activities are easier to write than
objectives. Activities have a done-state; objectives have a
direction. Writing objectives forces the founder to name what
*success looks like* rather than what *work looks like*.

**Fix.** For each candidate objective, ask: *if we finish everything
we have planned but reality doesn't change, was the objective
accomplished?* If yes, it is an activity. Rewrite the objective as
the *change in the world* the activity is supposed to cause. "Ship
v2" becomes "reduce customer time-to-value to under five minutes";
the ship of v2 is the mechanism, not the goal.

### Anti-pattern 2 — the KR that is an input

**Symptom.** The key result measures what the team *did* rather
than what *happened*. "Ran 30 customer interviews." "Shipped 12
features." "Sent 500 outbound emails." These are inputs; they tell
you the team worked, not whether the objective moved.

**Why it happens.** Because inputs are easy to control and outcomes
are not. A team that misses a KR because they didn't do the work
feels responsible; a team that misses a KR because reality was
harder than expected feels helpless. The temptation to write
controllable KRs is real.

**Fix.** For each candidate KR, ask: *if we hit this KR but the
objective doesn't move, did we succeed?* If yes, the KR is an
input. Rewrite it as the outcome you were hoping the input would
cause: "run 30 customer interviews" becomes "learn enough that we
can name the top-three onboarding-drop reasons and cite them from
five different customers." The interviews are *how*; the naming is
*whether it worked*.

Two exceptions where input KRs are legitimate at this stage:

- **Learning-heavy objectives** where the point of the quarter is
  to accumulate evidence, not to move a metric ("interview 30
  target-segment prospects" is a fine KR when the objective is
  "figure out which segment to commit to"). Even here, add a
  paired outcome KR ("by end of quarter, name the chosen segment
  with three specific reasons") so the input has a check.
- **Instrumentation-heavy objectives** where the metric doesn't yet
  exist and the quarter's work is to build the measurement itself.
  Again, pair the input ("instrument day-7 retention") with the
  outcome that instrumentation makes possible ("by end of quarter,
  the metric is on the one-pager and we've seen a full 7-day
  window of data").

### Anti-pattern 3 — the KR you cannot check inside the quarter

**Symptom.** The KR describes an outcome that takes six-to-twelve
months to fall out. "Achieve product-market fit." "Become the
category leader." "Reach $1M ARR." All fine as *company* aspirations;
none checkable inside a single quarter's window.

**Why it happens.** Because founders confuse the *goal* with the
*proximate KR that measures whether the goal is getting closer this
quarter*. Product-market fit is the goal; the proximate KR this
quarter is something like "second-week retention above 40% on 100+
new cohort accounts."

**Fix.** For each candidate KR, ask: *by the last Friday of the
quarter, will I have a number I can put next to this and know
whether we hit it?* If the honest answer is "we won't know until
next quarter," the KR is too far downstream. Move it upstream — pick
the leading indicator that *this quarter's work* is supposed to
move.

### Anti-pattern 4 — the quarterly-only rhythm

**Symptom.** OKRs are set at the start of the quarter, filed, and
re-read only at the end of the quarter. The middle 11 weeks are
run against the Monday plan and the shipped-and-learned but the KRs
themselves are invisible.

**Why it happens.** Because the standard OKR practice as taught
runs on a quarterly rhythm and founders inherit the cadence without
asking whether the cadence fits the scale. At two-person scale, a
quarter-long feedback loop is too slow — the loop only tells the
founder they were off after they are eleven weeks off.

**Fix.** Add the KR check to the Friday shipped-and-learned. Every
week, every KR gets one line: current value, delta, on-track or
not. If the same KR is off-track two Fridays in a row, that is a
signal for the following Monday's plan — either the plan needs to
change or the KR needs to. If the same KR is off-track four Fridays
in a row, that is a signal to *revise the KR* explicitly (log the
revision in the decision log per chapter 03) rather than let it
silently miss.

## Setting the OKR — the 90-minute exercise

Setting a good lightweight OKR takes about 90 minutes, once a
quarter. The exercise:

1. **Look back (20 min).** Re-read the last quarter's decision log
   and the last month's Friday shipped-and-learneds. What was the
   quarter *actually* about? What moved? What didn't? What did the
   metrics one-pager say by the end?
2. **Draft the objective (20 min).** Write three candidate
   objectives. Pick the one you would still endorse in six weeks
   when the enthusiasm has worn off. Run it through anti-pattern 1:
   is it a state of the world, not an activity?
3. **Draft the KRs (30 min).** For the chosen objective, write five
   candidate KRs. Cut to three. Run each through anti-patterns 2
   and 3: is it an outcome, not an input? Is it checkable inside
   the quarter?
4. **Sanity check with a co-founder or advisor (20 min).** Read the
   O and three KRs to someone who is close enough to the work to
   push back and honest enough to do so. The single most common
   thing a good sanity check catches is that the objective is
   secretly a project plan and the KRs are its milestones — that
   is anti-pattern 1 in a disguise, and the outside reader will
   often see it faster than the founder.

Once set, the OKR gets pinned somewhere the founder sees every
week — the top of the Monday plan is a good place — and gets
checked every Friday.

## What happens when the OKR turns out to be wrong

An OKR set on week 1 of a quarter is often partly wrong by week 4.
That is not a failure of goal-setting; it is what learning inside a
quarter looks like. The question is what to do about it.

**Three responses, in order of preference:**

1. **Keep the OKR, adjust the plan.** Most-off-track KRs are off
   because the plan for the week didn't advance them. This is the
   right response 60–70% of the time — the objective and KRs are
   still what the quarter is about; the tactics need to catch up.
2. **Revise a single KR.** Sometimes a KR turns out to be the wrong
   proximate measure. Rewrite it (log the revision in the decision
   log per chapter 03) and continue. Do this when the objective is
   still right but the measurement chosen was wrong.
3. **Change the objective.** Rarely — once or twice a year at
   most. When something material about the market or the product
   changes, the whole quarter's frame is wrong and continuing
   would be sunk cost. When you do change the objective, log the
   change explicitly; the log is what defends against "we always
   thought that" (chapter 03).

The order matters. Founders who default to response 3 lose focus.
Founders who default to response 1 without ever considering
response 2 or 3 keep grinding on wrong measurements. The Friday
check is what surfaces which response is called for; the decision
log is what records the choice.

## Where the OKR interlocks with the rest of the loop

- **Monday plan.** The Monday plan's "this week's three-to-five
  things" section should visibly include work that advances at
  least one KR. If a week goes by with no plan item pointing at a
  KR, either the KR is silently forgotten or the KR is the wrong
  one. Both are worth noticing.
- **Metrics one-pager.** The KR numbers live on the one-pager's
  watch-list section (chapter 02). The one-pager is where the KRs
  become weekly-visible without being weekly-nagged.
- **Friday shipped-and-learned.** The KR check is the last section
  of the shipped-and-learned. Same file, same weekly ritual.
- **Decision log.** Any revision to a KR or to the objective is a
  founder-only call and belongs in the log (chapter 03). Any
  major action taken because a KR is off-track (a pivot in tactics,
  a resource reallocation) belongs in the log.
- **First investor update.** The monthly investor update's
  highlights and lowlights (chapter 06) are often exactly the
  places where the KRs moved or didn't. The update is where the
  quarter's OKR meets its external audience.

## Where OKR depth lives

This module's OKR treatment is deliberately narrow: the shape and
the anti-patterns that show up at two-person scale. The full OKR
practice — cascading OKRs across a multi-team organisation, the
tooling, the calibration exercises, the org-design implications —
is operating-pillar depth and lives in
[`startup-operations-governance-curriculum`](https://github.com/ai-startup-curriculum/startup-operations-governance-curriculum).

The primary sources (Grove, Doerr) are in `resources.md`. Reading
them is worth an evening even at PRE-SEED; the anti-patterns from
this chapter map cleanly onto the failures Grove and Doerr each
document from their own companies.

## Summary

- The lightweight OKR is one objective, three key results, weekly
  check-in. That is the entire shape.
- Each parameter (one, three, weekly) is a deliberate departure
  from the full practice, calibrated to a two-or-three-person
  startup.
- Four anti-patterns are what break the practice at this scale:
  goals that are activities, KRs that are inputs, KRs that can't
  be checked in-quarter, and a quarterly-only rhythm.
- The KR check folds into the Friday shipped-and-learned; it does
  not need its own meeting.
- When an OKR turns out to be wrong, prefer adjusting the plan,
  then revising a KR, then (rarely) changing the objective. Log
  the revision explicitly.
- Full OKR practice depth lives in
  `startup-operations-governance-curriculum`; this module owns the
  founder-scale slice.

## Homework

Exercise 04 (`One Objective, Three KRs — the Drill`) is where the
shape gets exercised against a real startup, including the
anti-pattern audit. Exercise 01 (`Founder Week Simulation`) uses
the OKR in the Friday shipped-and-learned check.
