# The Stage Tag as Curriculum Instrument

## Motivation

Chapters 01 through 06 built the stage vocabulary and turned it into a
checklist a founder uses inside their own company. This last chapter closes
the loop by connecting that vocabulary to the way the entire
ai-startup-curriculum org **communicates stage information back to a
learner**.

Every module in every repo across the org — Foundations, the pillar repos
(product-gtm, finance-fundraising, operations-governance, exit), and the
role-pathway repos (founder-ceo, cto, cpo) — carries a `stage:` tag in the
front-matter of its `README.md`. That tag is the operational output of
everything in this module. It is how the curriculum says to a learner:
*you are pre-seed — do these, ignore those*.

This chapter teaches you the two operations you need to be fluent with the
tag: **reading it as a learner** (so you can filter the whole catalog to
your stage in under a minute) and **setting it as an author** (so that
when you eventually contribute a module or a project, the stage tag you
write is trustworthy).

The front-matter contract is defined once, in the root-level
[`STARTUP_STAGES.md`](../../STARTUP_STAGES.md). This chapter is the
reading key.

## The front-matter contract, in full

Every module `README.md` begins with YAML front-matter. The
stage-relevant fields:

```yaml
---
stage: SEED              # earliest stage at which this becomes actionable
stages: [SEED, SERIES-A] # optional: all stages where this applies
pillar: fundraising      # functional pillar (see FUNCTIONAL_CURRICULA.md)
requires:                # prerequisite module ids
  - mod-001-how-startups-work
---
```

Read each field precisely.

- **`stage:`** — the *earliest* stage at which the module becomes
  actionable. Not the stage that most benefits from it. Not the stage where
  founders most often read it. The **earliest** stage at which acting on
  the module's contents is not premature. A module whose contents cannot
  be productively acted on until SERIES-A carries `stage: SERIES-A` even
  if a curious PRE-SEED founder could read it earlier.
- **`stages:`** — the full list of stages where the module applies. A
  module about *founder-led sales* legitimately spans PRE-SEED through
  SERIES-A; `stages: [PRE-SEED, SEED, SERIES-A]` says that explicitly. A
  module about *incorporation basics* is `stages: [PRE-SEED]` — it
  becomes actionable at PRE-SEED and after that has been handled once, it
  goes into the reference file, not the active work list.
- **`pillar:`** — the functional pillar the module belongs to. Orthogonal
  to stage but referenced together when filtering.
- **`requires:`** — the module IDs that must be read first. Not a stage
  concept, but often correlated (a Series-A-tagged module usually
  requires earlier-tagged modules as prerequisites).

Markdown front-matter is the source of truth. The
`.aicg/curriculum-plan.json` manifest may mirror the tags but never
overrides them.

## The `stage:` vs `stages:` distinction

The single most common author mistake is treating `stage:` and `stages:` as
interchangeable. They are not.

- `stage:` is a **decision** — the earliest stage at which the module is
  worth spending time on. This is what a learner filters by ("I'm SEED,
  show me all modules with `stage:` <= SEED").
- `stages:` is a **description** — the full set of stages where the
  module remains relevant. This is what a learner uses to decide whether
  a module they already read at an earlier stage is worth re-reading now
  ("I read the founder-led sales module at PRE-SEED; is it still relevant
  at SEED?" → check `stages`).

A module missing `stages:` implicitly claims `stages: [<stage>]` — that
is, "only at the earliest actionable stage." Most modules are wider than
that. Set `stages:` explicitly whenever the module applies past its
earliest actionable stage.

## Reading the tag as a learner

The learner-facing use of the tag is simple. Two operations:

**1. Filter the whole catalog to your stage.** Open the org index, filter
every module by `stage: <= your-current-stage`. What remains is the
*actionable* set. Everything else is on the map but not on today's list.
For most learners this cuts the catalog down by 60–80%.

**2. Filter the actionable set to what you have not already handled.**
Modules that carry only `stage:` (no `stages:` continuation) are one-shot
— read once, done, on to the next. Modules with `stages:` are recurring
references you re-visit as the company progresses.

Both operations are meant to be programmatic. The
`.aicg/curriculum-plan.json` manifests are machine-readable specifically
so a learner (or a tool) can compute these filters without hand-work.

### A worked reading

Imagine you're PRE-SEED and you're opening
`startup-finance-fundraising-curriculum` for the first time. Two
possible browsing paths:

**Wrong path.** Read the module list top to bottom. Encounter
`mod-020-Series-B-Bridge-Rounds`. Read it because it looks interesting.
Waste three hours. Realise it isn't actionable for years. Reassure
yourself that "background knowledge is valuable."

**Right path.** Filter by `stage: PRE-SEED`. The module list drops from
30 modules to a handful — first check under fundraising, first runway
model, first cap table. That is your reading order for the next
quarter. The Series-B module has `stage: SERIES-A` (or later); it does
not appear in the PRE-SEED view. It becomes visible only when your
own stage tag advances.

That is the entire user-facing operation. Chapter 06's checklist is
what you use *inside your company*; the stage tag is what you use
*against the catalog*.

## Setting the tag as an author

Authors are the ones who make the learner-side operation work or fail.
The three rules:

### Rule 1 — Tag to the earliest *actionable* stage, not the earliest *readable* stage.

A learner could, in principle, read anything at any stage. That does
not mean everything applies at every stage. The tag is a claim about
*actionability*, not about intellectual accessibility.

Concretely: an author writing a module on multi-jurisdictional
transfer pricing should tag it `stage: GROWTH` (or the earliest stage
at which a startup actually has cross-border revenue material enough
to matter). The fact that a PRE-SEED founder *could* read it and would
*understand* it is beside the point. The tag is about when it becomes
worth their time.

Chapter 03's shape-1 mismatch (working ahead) is the failure mode this
rule prevents in the catalog. If authors tag modules to the earliest
*readable* stage, the catalog becomes a menu that encourages exactly
the mismatch the module is teaching learners to avoid.

### Rule 2 — Do not tag defensively.

A tempting author move: tag conservatively to `stage: IDEA` on the
grounds that "someone at IDEA might want to know about this." That
defensive tagging destroys the filter's value. If everything is
tagged IDEA, IDEA-stage learners see the whole catalog and are back
to the flat-menu problem.

Tag honestly. If the module's contents are premature for IDEA
learners, tag it later. Trust the learner to reach it when they get
there.

### Rule 3 — Set `stages:` explicitly when the module is a recurring reference.

A module about *runway modeling* is not one-shot. It is a
reference you consult continually from PRE-SEED through SERIES-A.
Its front-matter should be:

```yaml
stage: PRE-SEED
stages: [PRE-SEED, SEED, SERIES-A]
```

A module about *first-time incorporation choices* is one-shot. Its
front-matter should be:

```yaml
stage: PRE-SEED
# stages omitted → implicit stages: [PRE-SEED]
```

The distinction is what tells a SEED-stage learner whether to
re-visit the module (yes, if `stages:` includes SEED) or move on
(no, if it doesn't).

## How mod-003's own tag is set

Look at this module's own `README.md` front-matter:

```yaml
---
stage: IDEA
stages: [IDEA]
pillar: foundations
hours: 14
requires: [mod-001-how-startups-work, mod-002-the-dependency-graph]
---
```

Why `stage: IDEA` and `stages: [IDEA]`?

- **`stage: IDEA`** — the stage vocabulary in this module becomes
  actionable at the very earliest stage. A learner who has not yet
  incorporated should be running the stage-fit checklist against
  their own IDEA-stage candidate activities from week one. Later is
  worse.
- **`stages: [IDEA]`** — but why not include the later stages,
  since a founder benefits from the checklist through GROWTH? The
  answer is that the *vocabulary* is one-shot: once a founder has
  learned it, they carry it. The *application* recurs weekly but
  that application is scoped to mod-004 (the operating cadence),
  not to re-reading mod-003. Tagging `stages: [IDEA, ..., GROWTH]`
  would tell later-stage learners they should re-read the module,
  which is not what we want them to do.

That is the reasoning behind every tag in this repo, applied
transparently so you can copy the pattern when you author your own.

## The tag interacts with role pathways, not just stages

The stage tag is one of the three axes. The role tag (implicit in
which role-pathway repo you're reading) is another. The `pillar:`
field is the third.

A learner filtering by role (e.g., "I'm reading the CTO pathway") is
looking at a curated subset of pillar modules where each carries its
own stage tag. Filtering by both role *and* stage — "CTO at
PRE-SEED" — gives the smallest, most actionable view of the org.
That is the intended user experience.

The three axes compose:

- **Pillar** filters the catalog by *body of knowledge*.
- **Role** filters the catalog by *whose job this belongs to*.
- **Stage** filters the catalog by *when this becomes actionable*.

All three filters applied at once gives a small, specific work list
for a specific person in a specific role at a specific stage. That
is the design goal. Chapter 07 has established that mod-003's
contribution to that design is the stage axis.

## What happens when the tag is wrong

Two failure modes to watch for as a contributor:

**Failure mode 1 — the module drifts past its tagged stage.** A module
originally written to be actionable at SEED gets updated over time
with content that is really SERIES-A. The tag stays at SEED. Learners
filtering at SEED get material that is premature for them. The fix is
to re-tag when material changes, or to *split* the module into a
SEED-first section and a SERIES-A extension.

**Failure mode 2 — the module tag is right but the internal chapters
are stage-mixed.** A single module tagged SEED can legitimately have
chapters that lean earlier (PRE-SEED holdover material) or later
(preview of SERIES-A). The convention across the org is that the
module tag reflects the *load-bearing majority* of the module. If
half the chapters are actually PRE-SEED and half are actually
SERIES-A, the correct move is again to split the module.

## Summary

- Every module carries a `stage:` tag (earliest actionable stage) and,
  optionally, a `stages:` tag (all stages where the module applies).
- Learners use the tag to filter the catalog to their actionable set —
  usually cutting the visible catalog by 60–80%.
- Authors tag to the earliest *actionable* stage, not the earliest
  *readable* stage, and do not tag defensively.
- The stage tag composes with `pillar:` and with the role-pathway
  filter (implicit in which repo you're reading) to produce a
  small, specific view of the org for a specific learner.
- mod-003 itself is tagged `stage: IDEA / stages: [IDEA]` because the
  stage vocabulary is one-shot and best learned early.

## Homework

No exercise for this chapter directly — it is the operational
extension of the whole module. Two follow-ups to do inside a week
after you finish:

1. Open one pillar repo (e.g.,
   `startup-product-gtm-curriculum`) and manually filter its module
   list to your current stage using the front-matter `stage:` tag.
   Note how much shorter the actionable list is than the full list.
2. When you next author or update a module in your own work,
   apply the three tagging rules from this chapter. If you find
   you can't decide on the tag, that itself is a signal that the
   module's scope is stage-mixed and should be split.

This is where the vocabulary from mod-003 stops being about your
own weekly plan and starts being about how the whole org talks to
its learners.
