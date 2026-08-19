---
module: mod-003-stages-and-what-matters-when
exercise: exercise-01
slug: stage-signal-drill-am-i-here
hours: 1
prereqs: [chapter-01-the-stage-axis, chapter-02-walking-the-stage-ladder]
---

# Exercise 01 — Stage Signal Drill: Am I Here?

## Problem statement

Chapter 02 walked the six-row stage ladder and gave, for each stage, the
signal you're in it, the founder's core question, and the typical focus.
This exercise is where you prove you can *locate a specific startup on
the ladder* using only the signal column — no vibes, no self-report from
the founder, no press-release language.

You will (a) place three real (or realistic) startups on the ladder
using only observable signals, (b) defend each placement against one
adjacent rung — the stage above and the stage below — and (c) name what
would have to change for each startup to have earned the placement one
rung above.

## Requirements

### Part A — the placement drill (3 startups)

Pick **three startups**. At least two of the three must be **real,
publicly documented startups** (a company you can point at a
founder essay, a blog post, a press release, an S-1, a podcast
transcript, or a well-covered news article about). The third may be
realistic — a hypothetical company you construct yourself — as long
as its signal set is internally consistent.

Cover **at least three different stages** across the three startups.
Do not pick three companies you believe are all at SEED; the drill
is about discriminating between stages, so cover a spread.

For each startup, produce:

- **The signal evidence.** A short list — 3 to 6 items — of *observable*
  signals about the company today. Each item should be something an
  outsider could verify (funding round announced, revenue disclosed,
  headcount reported, product features shipped, customer count
  reported, board seat filled). No "the founders feel like they're
  Series A" items — those are self-reports and are inadmissible for
  this drill.
- **The stage claim.** One line: "This company is at [stage]."
- **The mapping.** For each signal item, name the row on chapter 02's
  signal column that the item matches. If a signal doesn't match any
  row, flag it — you may have mis-placed the company or the signal
  isn't stage-diagnostic.

### Part B — adjacent-rung defence

For each of the three startups, defend the placement against **both
adjacent rungs**:

- **The stage above.** Why is this startup *not* one rung more
  advanced than you claimed? Name the specific signal from the
  higher-stage row of chapter 02 that is *missing*.
- **The stage below.** Why is this startup *not* one rung less
  advanced than you claimed? Name the specific signal from the
  lower-stage row of chapter 02 that *is present* and rules the
  lower stage out.

If you cannot defend one of the two, that is itself the finding —
the startup is on the boundary between two stages, and the mismatch
diagnosis in chapter 03 usually gets sharper if you assume the
earlier of the two.

### Part C — what would earn the next rung?

For each of the three startups, name **the specific signal from the
next rung up** that the startup would have to add to earn the
placement at that stage. Then name **the specific work** the
current-stage focus (from chapter 02) would have to complete for
that signal to appear.

This is a forward-looking exercise. The goal is to see whether the
current-stage focus you'd recommend to that founder actually
produces the transition signal. If it doesn't, either the focus is
wrong or the transition signal you named is not the right one.

## Deliverable shape

A single Markdown file, `mod-003-exercise-01-stage-signal-drill.md`,
structured:

```markdown
# Stage Signal Drill — Am I Here?

## Startup 1: <name>

**Sources:** <URLs or citations>

### Part A — signal evidence and placement
- Signal 1: <observable>. → row match: [stage]
- Signal 2: ...
- ...
- **Placement:** This company is at [stage].

### Part B — adjacent-rung defence
- **Not one stage above ([X]):** missing signal — <specific>.
- **Not one stage below ([Y]):** present signal — <specific>.

### Part C — what would earn the next rung?
- Next-rung signal to add: <specific>.
- Current-stage work that would produce it: <specific>.

---

## Startup 2: <name>
<same structure>

## Startup 3: <name>
<same structure>

## Cross-cutting note
<one paragraph on what the three placements together taught you about
using the signal column vs. self-report>
```

Total length: 800–1200 words across the three startups.

## Starter guidance

- **Signals are observable, not inferred.** "Revenue growing" is not
  observable unless someone published a number. "Company raised $12M
  Series A led by [firm]" is observable. Discipline the signal list
  to what an outsider could verify.
- **Prefer companies with post-mortems, founder essays, or S-1
  filings.** They are honest sources. Avoid company-blog "here's how
  we succeeded" pieces — they are marketing and they systematically
  lag the actual signal by 12–18 months.
- **Do not use inside information from a private company you know
  personally.** The exercise is about publicly-defensible placement.
  If you use a private company you have inside knowledge of, you
  cannot defend the placement to a reader who doesn't share your
  access, and the drill loses its point.
- **Do not conflate the funding round with the stage.** A company
  that raised a "seed round" of $12M with an institutional lead and
  a board seat is often really at SERIES-A on the signal column.
  Signal columns beat round names.
- **When in doubt, pick the earlier rung.** Every downstream chapter
  in this module (especially chapter 05 on premature scaling) treats
  the earlier rung as the safer default. Getting placed one stage
  too *late* is a much smaller error than one stage too *early*.

## Acceptance criteria

You have completed the exercise when:

- [ ] Three startups placed, with at least two of the three being
      real and publicly documented, and with a spread across at
      least three different stages.
- [ ] Each startup has a signal-evidence list of 3–6 observable
      items, each mapped to the chapter 02 signal-column row.
- [ ] Each placement is defended against the adjacent-rung above
      (missing higher-stage signal) and adjacent-rung below
      (present current-stage signal).
- [ ] Each startup has a "next-rung signal + current-stage work"
      section that connects the current focus to the transition.
- [ ] Sources are cited for the two real startups (URL or
      book / episode / filing reference per source).
- [ ] The file is committed to your notes as
      `mod-003-exercise-01-stage-signal-drill.md`.

## Common failure modes to avoid

- Using "vibes" signals. "They feel like a Series-A company" is not
  a signal. "They have 200 employees and an institutional-lead
  Series B" is a signal. Sort the difference.
- Picking three startups that all sit at the same stage. The drill
  is about discrimination between stages; three placements at the
  same stage lose 70% of the exercise's value.
- Defending a placement against only the adjacent rung *above*.
  The "why not the stage below?" check is what catches the
  premature-badge failure mode from chapter 01.
- Writing the "next-rung work" section in generic terms ("we should
  scale sales"). Chapter 02's typical-focus column has specific
  activities; use the specific ones.

## What good looks like

A three-startup placement that a reader could use as a working
example of *how to place their own company on the ladder*. Someone
who reads your file should be able to look at their own company,
apply the same signal-first discipline, and produce their own
placement with the same shape of defence and the same shape of
forward-looking transition. If a reader can't do that, the exercise
was performed but not learned.

The signal discipline you build here is what chapter 06's
stage-fit checklist depends on. Chapter 06's Question 2 is
"what is my current stage?" — and this exercise is where you build
the muscle to answer it honestly.
