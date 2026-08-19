---
module: mod-004-founder-operating-basics
exercise: exercise-04
slug: one-objective-three-kr-drill
hours: 3
prereqs: [chapter-04-lightweight-okr]
---

# Exercise 04 — One Objective, Three KRs: The Drill

## Problem statement

Chapter 04 installed the lightweight OKR shape for a 2-3 person
startup — one objective, three key results, weekly check-in — and
named the four anti-patterns that make even this small shape
break: goals that are activities, KRs that are inputs, KRs that
can't be checked in-quarter, and a quarterly-only rhythm.

This exercise is where you write the OKR for a real (or
realistically-specified) startup and then run it through an
anti-pattern audit — the same one chapter 04 named — with a
before-and-after visible. You will also write the weekly
check-in shape you plan to use, so the OKR is not just a
document but a rhythm from the start.

## Requirements

### Part A — pick the startup and read the primary source (about 20 min)

Pick a PRE-SEED or SEED startup, same options as prior
exercises. Before writing, at minimum skim (ideally read) *one*
of the two primary OKR sources in `resources.md` — Grove's
`High Output Management` (the KR chapters) or Doerr's `Measure
What Matters` (the introduction and the two or three case
studies most relevant to your startup's shape).

Write **two sentences of context**: what the startup is doing
this quarter (roughly), and what stage of the search from
mod-001 chapter 05 (problem / solution / market / business model
/ team) the quarter is centred on. The stage of the search
usually determines the shape of the objective — an early-search
quarter has learning-heavy objectives; a later-search quarter
has metric-moving objectives.

### Part B — draft the objective (about 30 min)

Write **three candidate objectives** for the quarter. Each is one
sentence, qualitative, ambitious, memorable. Do not pick one
yet; write all three.

For each candidate, apply the **chapter 04 anti-pattern 1 check**:

- If we finished everything currently planned but reality didn't
  change, would the objective be accomplished?
- If yes, it is an activity. Rewrite it as the *change in the
  world* the activity is supposed to cause.

Now **pick one**. State briefly (one paragraph) why the chosen
objective is the right one for the quarter over the other two.
Common reasons: it is the one whose success would matter most
regardless of tactics; it is the one that the current stage
requires; it is the one that would still be endorsed in six
weeks when enthusiasm has faded.

### Part C — draft the three key results (about 60 min)

For the chosen objective, write **five candidate KRs**. Not
three; five. You will cut to three.

Each candidate KR is a number, with:
- **A starting value** (current state as best you know it).
- **An ending target** for the end of the quarter.
- **A direction** (up, down, cross a threshold).

Run each candidate through the **anti-pattern 2 check**:
- If we hit this KR but the objective didn't move, did we
  succeed?
- If yes, the KR is an input. Either rewrite it as an outcome,
  or (if it is a legitimate learning-heavy or
  instrumentation-heavy input per chapter 04) pair it with an
  outcome KR that the input is meant to unlock.

Run each candidate through the **anti-pattern 3 check**:
- By the last Friday of the quarter, will there be a specific
  number you can check to know whether you hit this?
- If not, move the KR upstream to the leading indicator this
  quarter's work is supposed to move.

Now **cut to three**. State briefly (one paragraph) why the
chosen three, together, cover the objective. Test the coverage
by asking: if all three hit at target, does the objective land?
If not, either the three don't cover the objective (change the
KRs) or the objective was too broad (change it back at Part B).

Legitimate cases for an input KR (from chapter 04) require
naming which case applies. If you use one, include the paired
outcome KR too and count them together as one of the three.

### Part D — the weekly check-in shape (about 30 min)

Write the **weekly KR check-in template** — the five-minute-max
addendum to the Friday shipped-and-learned that chapter 04
prescribes. Shape:

```markdown
### KR check-in (as of 2026-M-D)

| KR | Start | Current | Target end-of-quarter | Delta this week | Status |
|---|---|---|---|---|---|
| KR1 | ... | ... | ... | ... | on/off |
| KR2 | ... | ... | ... | ... | on/off |
| KR3 | ... | ... | ... | ... | on/off |

**Off-track KRs — cause and next-week action:**
- KR2: <one line cause>; <one line next-week action>.
```

Populate the table with your best estimate of *today's* values
(current) and your quarterly targets (target end-of-quarter).
Then simulate a "week 3 of the quarter" check-in: assume two of
the three KRs are roughly on-track and one is off. Fill in the
off-track row's cause and next-week action.

### Part E — the anti-pattern audit (about 30 min)

Chapter 04 named four anti-patterns. For each, write **one
sentence** on how the current draft of your O and KRs
specifically defends against it, plus **one sentence** on the
risk of drifting into the anti-pattern over the coming quarter
and one thing you plan to do to catch the drift.

The audit is not "did I make the mistake." The audit is "which
mistake would I most easily drift into, and what's my early
warning system?"

## Deliverable shape

A single Markdown file, `mod-004-exercise-04-okr-drill.md`,
structured:

```markdown
# One Objective, Three KRs — Drill for <Startup>

## Context
<two-sentence startup context + stage of search>

## Part B — objective drafting
### Candidate objectives (all three)
1. ...
2. ...
3. ...
### Anti-pattern 1 audit of each candidate
- Candidate 1: activity? ...
- Candidate 2: activity? ...
- Candidate 3: activity? ...
### Chosen objective and why
<paragraph>

## Part C — KR drafting
### Candidate KRs (all five)
| # | KR | Start | Target | Direction | Input or outcome? |
|---|---|---|---|---|---|
| 1 | ... | ... | ... | ... | ... |
| ... |

### Anti-patterns 2 and 3 audit of each candidate
- Candidate 1: outcome or input? checkable in-quarter? ...
- ...

### Chosen three KRs and why
<paragraph on coverage of the objective>

## Part D — weekly check-in template
### KR check-in (as of week 3 simulated)
| KR | Start | Current | Target | Delta | Status |
| ... |
### Off-track KR — cause and next-week action
- ...

## Part E — anti-pattern audit
- Anti-pattern 1 (activity-goal): defence ...; drift risk ...; early warning ...
- Anti-pattern 2 (input KR): ...
- Anti-pattern 3 (uncheckable-in-quarter KR): ...
- Anti-pattern 4 (quarterly-only rhythm): ...

## Reflection
<one paragraph on what the drill surfaced about goal-setting for
this specific startup at this specific stage>
```

Total length: 1200–1800 words.

## Starter guidance

- **Start with the objective, not the KRs.** Founders who start
  with KRs and back into the objective almost always produce an
  activity-shaped objective. Chapter 04's ordering — objective
  first, KRs second — is the ordering that produces coherent OKRs.
- **Draft more than you need, then cut.** Five KR candidates cut
  to three beats three KR candidates that all made the list on
  the first draft. The cut is where the anti-pattern-2 and -3
  checks actually bite.
- **Numbers over adjectives.** "Improve" and "grow" and "reduce"
  are not KRs; they are hopes. A KR has a starting value, an
  ending target, and a direction. If any of those three is
  missing, the KR is not yet a KR.
- **Sanity-check with a real person.** Chapter 04's 90-minute
  exercise ends with 20 minutes of sanity-checking with a
  co-founder or advisor. Do it. The most common thing a good
  reader catches is that the objective is secretly a project
  plan and the KRs are its milestones — much easier for an
  outside reader to see than for the author.
- **A pre-seed founder's OKR is not the same shape as a
  Series-A founder's OKR.** At PRE-SEED, learning-heavy objectives
  ("figure out which segment") with paired input+outcome KRs are
  legitimate. At SEED, metric-moving objectives with pure outcome
  KRs are more common. Stage the OKR to the search stage.

## Acceptance criteria

You have completed the exercise when:

- [ ] Three candidate objectives are written, each audited
      against anti-pattern 1, with a chosen one and a paragraph
      of rationale.
- [ ] Five candidate KRs are written with start, target, and
      direction for each; each is audited against anti-patterns
      2 and 3; the chosen three are stated with a coverage
      paragraph.
- [ ] The weekly check-in template is populated with realistic
      values including a simulated week-3 off-track KR with
      cause and next-week action.
- [ ] Each of the four anti-patterns has a two-sentence entry in
      the audit (defence + drift risk / early warning).
- [ ] A one-paragraph reflection surfaces something the drill
      taught about the specific startup's goal-setting at its
      specific stage.
- [ ] The file is committed to your notes as
      `mod-004-exercise-04-okr-drill.md`.

## Common failure modes to avoid

- **Rewriting existing KRs to match the exercise, without the
  audit.** The point is the audit. If you skipped anti-pattern
  2 and 3 checks on each KR candidate, you did the drill by
  copying, not by thinking.
- **Objective that reads like an OKR-textbook example.** "Delight
  our customers." "Become the leader in our space." Textbook
  language is a red flag — it usually means the objective is
  generic. A good objective is specific enough that swapping
  companies would make it wrong.
- **KRs that all fire at the same moment.** If your three KRs
  all peak in the last two weeks of the quarter, the weekly
  check-in has nothing to check for eleven weeks. Prefer KRs
  with continuous movement — a metric that drifts every week
  is checkable every week.
- **A weekly check-in that recomputes every value.** The
  check-in is a five-minute addendum. If populating the current
  column takes an hour, either the KRs are measuring
  hard-to-get numbers (fix the KR, not the check-in) or the
  metrics one-pager (chapter 02) is not yet doing its job.
- **Anti-pattern audit that says "no risk" everywhere.** Every
  founder is at risk of at least one of the four anti-patterns;
  the audit is honest about which one. "No risk" answers are a
  sign the audit wasn't taken seriously.

## What good looks like

An OKR — O plus three KRs — that a reader can look at and
understand (a) what the quarter is about, (b) how you will know
if it worked, and (c) what the weekly rhythm on this specific
OKR is going to look like. The audit is where a reader can also
understand (d) which failure mode you are personally at risk of
drifting toward and what your early-warning is.

If a co-founder or advisor could pick up your artifact and, on
the last Friday of the quarter, run the KR check-in on the same
numbers with the same criteria — that is the sign the KR-shape
discipline landed. If the check-in requires the author to
translate every KR ("what I really meant by 'improve retention'
was..."), the KRs still have work to do.

The OKR you write here feeds directly into exercise 01 (`Founder
Week Simulation`) — the plan item advancing a KR is checked
against this OKR — and into exercise 05 (`Monday Plan / Friday
Shipped`) — the KR check-in is the last section of the Friday
shipped-and-learned. The three exercises share one OKR; do not
re-invent one for each.
