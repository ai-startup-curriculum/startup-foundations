---
module: mod-004-founder-operating-basics
exercise: exercise-03
slug: decision-log-first-ten-entries
hours: 3
prereqs: [chapter-03-the-decision-log]
---

# Exercise 03 — Decision Log: First Ten Entries

## Problem statement

Chapter 03 formalised the decision log — a running, dated,
append-only, three-column record of every founder-only call and
the reason it was made. This exercise is where the log gets
started for a real (or realistically-specified) startup, and where
you practise writing the *reason* column — the load-bearing and
most-often-botched part of the artifact.

The exercise has three parts: (a) ten log entries in the
three-column shape, (b) an audit of your own log against chapter
03's failure modes, and (c) one quarterly-re-read pass done
prospectively (imagining the same ten entries read three months
from now with outcomes visible).

## Requirements

### Part A — the ten entries (about 90 min)

Write **exactly ten decision-log entries** for a real or
realistically-specified startup at PRE-SEED / SEED. Same startup
selection rules as exercise 01: your own venture, one you advise,
or a well-constructed hypothetical.

At least **six of the ten** must be real founder calls made in the
last 60 days by someone you have direct access to (yourself, a
co-founder, a founder you're advising, a founder whose specific
recent decisions you know well enough to reconstruct honestly).
The remaining four can be plausibly-constructed decisions for the
same startup. The 60/40 rule is what keeps the exercise from
becoming a fiction-writing exercise.

Each entry must:

- Have a **specific date** (ISO format, `2026-M-D`). If the exact
  date is not recoverable, use the closest plausible date.
- Have a **one-sentence decision** in past tense, verb-first.
- Have a **one-to-three-sentence reason** describing why the call
  was made *given the information available at the time*.

Coverage rules (this is where your ten entries stretch across the
categories chapter 03 named):

- **At least two product / customer calls** (ship / don't ship /
  deprecate / partner with / discount / cancel).
- **At least two people calls** (hire / delay / contract / part
  ways / offer / decline).
- **At least one capital / spend call** (raise / decline / spend
  / defer).
- **At least one strategy call** (pivot / persevere / enter
  segment / exit segment / change North-Star).
- **At least one decision made by inaction** — an explicit
  entry naming the default that prevailed and why the founder
  chose to let it.
- **At least one entry whose reason cites specific evidence** —
  a specific number, a specific customer signal, a specific
  named source. (This is the discipline of "reason first, source
  second" from chapter 03.)

### Part B — the self-audit (about 45 min)

Chapter 03 named five failure modes for decision-log writing:

1. Retrofitting the log at week's end (memory losses).
2. Editing past entries when new information arrives.
3. Writing reasons that are not reasons.
4. Logging trivial decisions.
5. Not reviewing the log quarterly.

For each of your ten entries, apply the following audit:

- **Is the reason a reason?** Check chapter 03's specific
  anti-example list: "because it was the right thing," "because
  everyone agreed," "because I felt strongly about it," "because
  it seemed like a good time" — if your reason is one level
  above naming the actual evidence, rewrite it.
- **Would a stranger reading this in six months understand the
  reasoning?** Not "would they *agree*" — would they *understand*.
  A reason that requires context only the founder has is not
  finished.
- **Is the decision founder-only?** A call anyone on the team
  could have made doesn't belong; delete it and add a
  founder-only call in its place.
- **Is the date the date the call was made?** Not the date the
  situation became visible, not the date you wrote the entry.

Produce a short **audit table** listing each entry number and,
for entries where you had to revise, one line on what was wrong
and what you changed. Do not silently rewrite entries; document
the revision.

### Part C — the prospective quarterly re-read (about 30 min)

Imagine reading your ten entries three months from now, with the
outcomes visible. For **five of the ten** (pick the ones with the
most consequential outcomes), write a **follow-up entry** dated
+3 months, in the three-column shape, that:

- References the original entry by date.
- Notes whether the outcome was as expected, better than
  expected, or worse than expected.
- Names one thing the founder learned from the follow-through
  that they didn't know when the original call was made.

This is the shape chapter 03 named for the quarterly re-read.
The exercise version is imagined; the real version, done
against the real log three months from now, is how the log stops
being bookkeeping and becomes founder-development.

Then write a **one-paragraph reflection** on what the prospective
quarterly re-read showed you about the shape of your ten entries.
Some questions to answer:

- Was there a category that dominated the ten? If so, is that the
  right category for the quarter, or is it a symptom of
  attention arbitrage (chapter 01)?
- Were the reasons robust enough that three-months-from-now you
  could reconstruct the call, or did some reasons rely on
  in-the-moment context that has already faded?
- Are there decisions in your imagined next-three-months that
  should already have been made in this batch of ten?

## Deliverable shape

A single Markdown file, `mod-004-exercise-03-decision-log.md`,
structured:

```markdown
# Decision Log — First Ten Entries

## Context
<one paragraph: startup name (anon if needed), stage, people count,
who is the founder in question, over what window the ten entries
were drawn>

## Part A — the log
| # | Date | Decision | Reason | Category |
|---|---|---|---|---|
| 1 | 2026-... | ... | ... | product |
| 2 | 2026-... | ... | ... | people |
| ...

## Part B — audit
| # | Failure mode found | Revision made |
|---|---|---|
| 3 | Reason was "because I felt strongly" | Rewrote as: three
of the last five interviews said X, which contradicted our thesis |
| ...

## Part C — prospective quarterly re-read
| Original # | Follow-up date | Outcome vs. expected | What was learned |
|---|---|---|---|
| 2 | +3 months | worse than expected | Underestimated the
integration effort by 3x; should have scoped it with an
engineer in the room |
| ...

## Reflection
<one paragraph on what the ten entries and the imagined re-read
surfaced about the founder's actual decision-making shape>
```

Total length: 1200–1800 words (most of the length in the log
entries and the reason column).

## Starter guidance

- **Reason column is the exercise.** Anyone can write a list of
  decisions. The specific skill this exercise trains is writing
  reasons that survive a stranger reading them in six months.
  Spend disproportionate time on the reason column.
- **Concrete beats abstract.** "Three of the last five interviews
  in the accounting-firm segment said onboarding was the
  blocker" beats "customer feedback suggested onboarding
  problems." Names, numbers, specifics.
- **Include one call you now regret.** The audit is more useful
  when the log has at least one honestly-difficult entry. If
  every one of your ten calls looks brilliant in hindsight, you
  are either running an unusually successful company or (much
  more likely) filtering out the ones that turned out badly. The
  log records the reasoning at the time; the follow-up records
  the outcome. Both are valuable.
- **The "decision by inaction" entry is not filler.** Chapter 03
  was explicit: decisions made by inaction are decisions. Naming
  one honestly is often the hardest single entry to write and
  the one that most reveals the founder's actual attention
  pattern.
- **Do not backdate entries as if you kept the log all along.**
  You are starting the log now. Some entries are reconstructions
  of past decisions; note the reconstruction (e.g., add a
  parenthetical "reconstructed from memory on <date>"). This is
  the exercise's honesty check.

## Acceptance criteria

You have completed the exercise when:

- [ ] Ten entries in the three-column shape are present, with at
      least six drawn from real recent founder calls.
- [ ] Coverage rules are met: at least two product/customer, at
      least two people, at least one capital/spend, at least one
      strategy, at least one decision-by-inaction, at least one
      reason citing specific evidence.
- [ ] The audit table lists any revisions with the failure-mode
      diagnosis; entries were not silently rewritten.
- [ ] The prospective quarterly re-read includes follow-up entries
      for at least five of the ten, in the three-column shape,
      dated +3 months.
- [ ] A one-paragraph reflection surfaces at least one insight
      about the founder's decision-making pattern from the ten
      entries.
- [ ] Reasons pass the "would a stranger in six months
      understand?" check — no "because it was the right thing"
      or equivalent.
- [ ] The file is committed to your notes as
      `mod-004-exercise-03-decision-log.md`.

## Common failure modes to avoid

- **Reasons that describe the decision.** "Decided to hire an
  engineer because we needed to hire an engineer." The reason
  should describe the *evidence or constraint* that led to the
  call, not restate the call.
- **All ten entries in one category.** A log with ten
  product/customer calls and no people, capital, or strategy
  calls means either the coverage rule was skipped or the
  founder is missing entire categories of calls that they are
  making by inaction. Either way, the audit should catch it.
- **Follow-up entries that edit the original.** The follow-ups
  are *new dated rows*, not amendments. Chapter 03: append-only.
- **Consulting-voice reasons.** "Aligning our resource allocation
  with our strategic priorities." That is not a reason; it is
  the sentence you write when you don't have one. Push through
  the abstraction and name the actual evidence.
- **Skipping the reflection.** The reflection paragraph is where
  most of the exercise's value lands. A ten-line log without a
  reflection is bookkeeping; with a reflection, it becomes the
  first step of the founder-development discipline chapter 03
  named.

## What good looks like

Ten entries that a reader — a co-founder, a mentor, another
Foundations learner — could pick up, read in five minutes, and
understand (a) what the founder has been deciding recently, (b)
what evidence or constraint drove each call, and (c) what
categories of decision-making are strong or weak.

The prospective quarterly re-read is what turns the exercise from
"I wrote ten entries" into "I can see the shape of my own
decision-making." Founders who complete this exercise honestly
often report that the reflection paragraph was the single most
useful hour they spent in the module — because reading their own
reasoning back to themselves, in the exercise's stripped-down
form, is the first time many founders see a pattern in how they
make calls that they hadn't noticed while making them.

The log you start here is the same log you keep for the rest of
your founder career. Every downstream Foundations exercise (01,
04, 05, 06) references the log; every future quarterly ritual
returns to it.
