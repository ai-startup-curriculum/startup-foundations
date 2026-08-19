---
module: mod-002-the-dependency-graph
exercise: exercise-04
slug: place-a-real-artifact-on-the-graph
hours: 3
prereqs: [chapter-05-placing-artifacts-on-the-graph]
---

# Exercise 04 — Place a Real Artifact on the Graph

## Problem statement

Chapter 05 installed the five-step placement move: (1) what is the
artifact about, (2) which single node is its primary home, (3) which
upstream nodes did it need, (4) which downstream nodes will consume
it, (5) which pillar owns the depth. This exercise makes you run the
move against ten real artifacts — a mix from a supplied library, from
publicly available templates, and (ideally) from your own founder
work — until the placement move is automatic.

You will (a) place ten artifacts using the five-step move, (b) for
each, produce the *three-line placement metadata* block that chapter
05 recommends attaching to every consequential artifact, and (c)
identify at least two artifacts whose placement is ambiguous and
explain the ambiguity.

## Requirements

### Part A — placements

Place **ten artifacts**. Compose the ten from:

- **At least six** from the reference list below.
- **At least two** from publicly available templates you can link to
  (a YC SAFE, a Sequoia deck template, an NVCA term-sheet model, a
  Carta cap-table export, a specific founder-published board-pack
  template).
- **Up to two** from your own current work (if you have any) — do
  not include anything confidential.

Reference list (pick at least six):

1. A signed **YC SAFE** (post-money) at a $10M cap.
2. A **customer interview transcript** from a discovery call with a
   prospective early adopter.
3. A **runway model spreadsheet** showing 14 months of runway at
   current burn.
4. A **term sheet** for a $6M Series A led by an institutional
   investor.
5. An **option-pool refresh** proposal expanding the pool by 3% of
   post-money.
6. An **ICP definition** identifying "series-A-and-later SaaS
   companies with dedicated data teams" as the primary target.
7. A **CAC / LTV table by acquisition channel** covering paid
   search, content, outbound, and referral.
8. A **quarterly board pack** covering financials, product update,
   hiring plan, and risks.
9. A **founder-agreement document** covering IP assignment,
   vesting, and role definitions.
10. A **Lean Canvas** for a pre-seed developer-tools company.
11. A **positioning statement** in the "For [ICP], [product] is a
    [category] that [unique value]" shape.
12. A **hiring plan** for the next 6 months covering roles,
    compensation ranges, and start dates.
13. An **investor update** covering highlights, lowlights, and asks.
14. A **decision log entry** documenting the choice to pivot from
    SMB to mid-market.
15. A **first paid-acquisition experiment** budget of $10k on Google
    Ads targeting the primary ICP.

For each placement, produce the full five-field record:

```markdown
### Placement N — <artifact name>

- Source: <URL or "own work — not linked" or "reference list item">
- Description (one sentence): ...
- Primary node: ...
- Upstream dependencies: ...
- Downstream consumers: ...
- Owning repo: ...
- Placement metadata (3-line form): ...
```

The 3-line form is the shape chapter 05 recommends attaching to real
artifacts. It looks like this:

```
Node: <primary node>
Upstream: <comma-separated>; Downstream: <comma-separated>
Owning repo: <repo>
```

### Part B — ambiguous placements

Of the ten artifacts you placed, identify **at least two whose
placement was genuinely ambiguous** — not because the graph is
wrong, but because the artifact is doing more than one job. For each:

- Name the two (or more) nodes it could be placed on.
- Diagnose *why* it is doing multiple jobs.
- Recommend either (a) splitting the artifact, (b) placing on the
  primary node and noting the touched nodes, or (c) treating it as a
  cross-branch artifact like a canvas (chapter 06).

### Part C — one wrong placement you caught yourself making

Pick **one artifact** where your first-pass placement was different
from your final placement. Describe:

- The initial placement.
- What you noticed that made you change it.
- Which of the five placement steps caught the error.

This is a metacognition drill: the placement move only gets fast if
you can name your own misses. If none of your ten placements changed
during the exercise, either your placements are perfect (unlikely) or
you did not challenge them (more likely). Go back and challenge.

## Deliverable shape

A single Markdown file, `mod-002-exercise-04-artifact-placement.md`,
structured:

```markdown
# Placing Artifacts on the Graph — Ten Placements

## Part A — Placements
### Placement 1 — <artifact>
<full record>

### Placement 2 — <artifact>
...

(through Placement 10)

## Part B — Ambiguous placements
### Ambiguous placement 1
- Artifact: ...
- Candidate nodes: ...
- Why multiple jobs: ...
- Recommendation: ...

### Ambiguous placement 2
...

## Part C — One placement I caught myself changing
- Artifact: ...
- Initial placement: ...
- Final placement: ...
- What I noticed: ...
- Which step caught it: ...
```

## Starter guidance

- **The 3-line placement metadata is the deliverable that pays
  compound interest.** In real founder work, you attach it to the
  top of a document or in the commit message. This exercise is
  where you build the habit; keep it short and mechanical, not
  poetic.
- **Ambiguous placements are the most useful ones.** Chapter 05
  gives you three moves when placement is ambiguous — split the
  artifact, place on primary and note touched, or treat as
  cross-branch. Use all three across your Part B answers so you
  practise each move.
- **Prefer real artifacts over invented ones.** If you have your
  own SAFE, your own runway model, your own board pack, place
  those. Real artifacts have real ambiguities that invented ones
  smooth over.
- **Placement is fast when done well.** By artifact 5 or 6 you
  should be doing the whole five-step move in 2–3 minutes. If
  you are still spending 15 minutes per artifact by artifact 10,
  you are over-thinking — trust the graph and move on.

## Acceptance criteria

You have completed the exercise when:

- [ ] Part A has ten distinct artifacts placed with all six
      required fields per placement (source, description, primary
      node, upstream, downstream, owning repo) plus the 3-line
      placement metadata form.
- [ ] At least six of the ten come from the reference list; at
      least two come from publicly linkable templates; up to two
      are from your own work.
- [ ] Every placement identifies a *single primary node* and
      lists at least one upstream dependency and one downstream
      consumer.
- [ ] Every placement names a specific owning repo from the
      chapter 07 ownership table.
- [ ] Part B has at least two ambiguous placements with the
      required structure (candidate nodes, why multi-job,
      recommendation).
- [ ] Part C names one placement you actually changed during the
      exercise and diagnoses which of the five steps caught it.
- [ ] The file is committed as
      `mod-002-exercise-04-artifact-placement.md`.

## Common failure modes to avoid

- Placing artifacts on *branches* instead of *nodes*. "Corporate
  structure" is not a placement; `Equity` or `Governance` or
  `Fundraising` is.
- Listing every node as an upstream dependency. If everything is
  upstream, nothing is; the exercise is about the *specific*
  hand-off the artifact needed.
- Skipping the owning-repo field. That field is the entire point
  — it is the address the placement gives you to go deep when
  you need to.
- Using the exercise as an excuse to write essays. The five-step
  move is short and mechanical; the value comes from doing it
  ten times, not from decorating each placement with prose.

## What good looks like

A completed placement dossier a co-founder could scan in ten
minutes and instantly know, for each of your ten artifacts, where
it lives, what it needs, what it feeds, and where to go deeper.
The three-line metadata blocks should be short enough that you
could imagine attaching them, unchanged, to the real artifacts in
your working repo tomorrow.
