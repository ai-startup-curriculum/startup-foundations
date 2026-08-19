---
module: mod-002-the-dependency-graph
exercise: exercise-06
slug: owning-repo-lookup-drill
hours: 2
prereqs: [chapter-07-ownership-rule-in-action]
---

# Exercise 06 — Owning-Repo Lookup Drill

## Problem statement

Chapter 07 gave you the ownership table — every node on the graph mapped
to its owning pillar curriculum — and argued that Foundations' whole job
depends on you being able to name the owning repo in under ten seconds
for any node. This exercise makes you time yourself, honestly, against
a mixed list of founder questions and artifacts until you hit the
speed target.

You will (a) run a **timed lookup pass** against 30 mixed items, (b)
score the pass against the ownership table, (c) diagnose your misses,
and (d) run a second timed pass after diagnosis to prove the fix.

## Requirements

### Part A — the item list

Below is a mixed list of 30 founder-facing items. Some are node names,
some are artifacts, some are founder questions. Your job for each item
is to name **the single primary owning repo** for that item and, if
Foundations owns a *founder-slice*, note that too.

The five candidate owning repos:

- `startup-foundations` (this repo)
- `startup-product-gtm-curriculum`
- `startup-finance-fundraising-curriculum`
- `startup-operations-governance-curriculum`
- `startup-exit-curriculum`

The 30 items:

1. A signed YC SAFE.
2. A customer interview script for a discovery call.
3. A 3-statement financial model.
4. A term sheet from a Series A lead.
5. An option-pool refresh proposal.
6. An ICP definition.
7. A CAC / LTV table by channel.
8. A quarterly board pack.
9. A founder-agreement covering IP assignment and vesting.
10. A Lean Canvas for a pre-seed startup.
11. A positioning statement in the classic "For [ICP] …" shape.
12. A 6-month hiring plan with compensation ranges.
13. A monthly investor update.
14. A runway calculation from cash and burn.
15. A cohort retention curve for a SaaS product.
16. A protective-provisions negotiation in a Series A term sheet.
17. A go / no-go decision on an M&A offer at $250M.
18. A choice between Delaware C-corp and Wyoming LLC at
    incorporation.
19. A framework for allocating $10M across product, GTM, and G&A.
20. A pivot decision from SMB to mid-market.
21. A first paid-acquisition experiment plan.
22. A founder-numbers one-pager (runway, burn, growth,
    default-alive-or-dead).
23. A pre-IPO S-1 prospectus draft.
24. A "which node does this artifact live on?" question.
25. A weekly Monday plan / Friday shipped-and-learned cadence.
26. A channel-fit assessment across 5 candidate channels.
27. A 409A valuation for common-stock repricing.
28. A board-consent matrix for a 5-person board.
29. A wind-down / shutdown plan for a failed startup.
30. A choice between running with the Lean Canvas or the BMC as the
    working canvas for the assumption set.

### Part B — timed pass 1

Set a timer. Target: **under 5 minutes for all 30 items**. (10 seconds
per item, on average.) For each item, write:

- Primary owning repo (single answer).
- Foundations slice? (yes / no; if yes, which module.)

Do not consult the ownership table during the timed pass. Do not
skip items — if you don't know, write your best guess and move on.

Record the total elapsed time at the end of the pass.

### Part C — score the pass

After the timed pass, open chapter 07 and score each answer:

- Correct primary repo: +1
- Wrong primary repo: 0
- Missed Foundations-slice flag when it applies (items 14, 22, 25):
  −0.5 from the +1 you got for the primary repo answer.

Target: **28 / 30 or better.** If you scored below 28, do not
proceed to Part D until you have re-read the ownership table.

### Part D — diagnose the misses

For each item you got wrong (or partly wrong), write **one sentence**
naming *why* the miss happened. Common causes:

- Confused two adjacent branches (Equity vs Governance, for
  example).
- Missed the Foundations founder-slice for a runway / operating-loop
  item.
- Confused an artifact with the node it primarily consumes vs the
  node that owns its depth.
- Did not know the item exists at all — in which case the fix is to
  read chapter 07 more carefully, not to memorise more.

If you missed zero items, skip Part D and celebrate.

### Part E — timed pass 2

After Part D, wait at least 30 minutes (do something else). Then run
a *second* timed pass on the same 30 items. Same rules. Record the
new time and the new score.

Target for pass 2: **all 30 correct in under 4 minutes.**

## Deliverable shape

A single Markdown file, `mod-002-exercise-06-owning-repo-drill.md`,
structured:

```markdown
# Owning-Repo Lookup Drill

## Part A — Item list
(reproduce the 30-item list or reference it)

## Part B — Timed pass 1
- Total time: MM:SS

| # | Item | Primary repo | Foundations slice? |
|---|---|---|---|
| 1 | ... | ... | ... |
...

## Part C — Score
- Score: N / 30

## Part D — Diagnoses
- Miss 1 (item #): ...
- Miss 2 (item #): ...
...

## Part E — Timed pass 2
- Total time: MM:SS
- Score: N / 30

## Retrospective (3 sentences)
- What was hard: ...
- What was easy: ...
- What I'll re-drill: ...
```

## Starter guidance

- **The speed target is real.** Foundations is only useful if
  ownership lookups are automatic. A five-minute lookup against
  the ownership table is *fine* the first time; a five-minute
  lookup on the tenth ask is a signal you have not internalised
  the map.
- **The Foundations founder-slice flag is the trickiest.**
  Runway (item 14), the founder-numbers one-pager (item 22), and
  the weekly cadence (item 25) all have Foundations *slice*
  ownership and pillar *depth* ownership. Score both to force
  the distinction into your working memory.
- **Do not skip Part D.** Diagnosing your misses is where
  memorisation turns into understanding. If you got 30 / 30 on
  the first pass, well done; but you don't get to skip the
  metacognition step just because you were right.
- **Pass 2 should be noticeably faster than pass 1.** If it is
  not, the fix in Part D was probably too shallow — you
  memorised the specific miss without generalising to the
  pattern.

## Acceptance criteria

You have completed the exercise when:

- [ ] Part B: timed pass 1 completed with elapsed time recorded
      and every one of the 30 items answered.
- [ ] Part C: scored honestly against the chapter-07 ownership
      table, with the score written down (even if it's ugly).
- [ ] Part D: every missed item has a one-sentence diagnosis
      (or the file explicitly notes "no misses").
- [ ] Part E: second timed pass completed at least 30 minutes
      after Part D, with elapsed time and score recorded, and
      the score is 30 / 30 in under 4 minutes.
- [ ] Retrospective: 3 sentences on hard / easy / re-drill.
- [ ] The file is committed as
      `mod-002-exercise-06-owning-repo-drill.md`.

## Common failure modes to avoid

- Consulting the ownership table during the timed pass.
  Discipline yourself; the exercise is meaningless without the
  time pressure.
- Getting only 20 / 30 and shrugging. The whole ownership rule
  depends on this being close to automatic; a 20 / 30 means you
  will misroute learners (and yourself) to the wrong repo for
  a third of your founder questions.
- Skipping Part E because pass 1 went well. The 30-minute-gap
  second pass is the retention check; without it, you don't
  know if the fix stuck.
- Turning the retrospective into a self-critique essay. Three
  sentences. What was hard, what was easy, what to re-drill.

## What good looks like

A completed drill that a co-founder or first hire could read as
your credibility on the ownership map. A 30 / 30 in under 4
minutes on pass 2 tells them (and you) that the map is loaded
into working memory and Foundations is doing its job for you.
This is the mechanical drill; the payoff is that every founder
question after Foundations gets routed correctly on the first
try.
