# The Stage Axis — Why *When* Is the Third Axis

## Motivation

A founder holding the dependency graph from mod-002 knows *where* every business
thing lives — customer discovery here, fundraising there, governance over there.
That is a huge upgrade from a flat menu of topics. It is not yet enough.

The most common failure of over-schooled founders is not that they don't know
where a topic lives. It is that they work topics in the wrong *order in
calendar time*. They read about board committees before their first customer.
They study international transfer pricing before their first invoice. They
optimise a landing-page funnel while the product still doesn't work. They are
not being lazy or stupid; they are treating the graph as a to-do list and
picking the topic that feels most sophisticated to the reader on the syllabus.

The graph is not a to-do list. It is a map. To turn the map into a work list
you need a *clock* — something that says "of the nodes visible on your map,
these are load-bearing this week, and those are not." That clock is the **stage
axis**, and it is the third axis of the three-axis model in this repo's README.

This chapter installs the axis, tells you what it is measuring, and explains
how it composes with the graph and the pillars so the rest of the module has
something concrete to build on.

## The three-axis model, restated

The org's `README.md` frames startup knowledge on three axes, not one:

1. **Functional pillars** — the deep, reusable bodies of knowledge. Customer
   Discovery, Product-Market Fit, GTM, Sales, Growth, Incorporation, Equity,
   Governance, Fundraising, Financial Modeling, Runway, Unit Economics,
   Capital Allocation, Exit. Authored once, in the pillar repos.
2. **Role pathways** — curated views over the pillars for a given role
   (founder-CEO, CTO, CPO). A role is not its own body of knowledge; it is a
   *filter* over the pillars.
3. **Startup stages** — the ordering of *when* each pillar becomes actionable
   for a given company. `IDEA → PRE-SEED → SEED → SERIES-A → GROWTH →
   MATURE`.

mod-002 taught you axis 1 — the pillars and how they connect. This module is
axis 3 — the clock. Axis 2 (role) is layered on top of both and lives in the
role-pathway repos; it isn't the subject here.

The load-bearing property is that **every module and every project in the org
is tagged against all three axes**. When you read the front-matter of a module
and see `stage: PRE-SEED, pillar: economics`, you are reading two of the three
tags at once. The stage tag is not decoration. It is the operational output
of everything in this module.

## What the stage axis is measuring

The stage ladder is often mistaken for a **funding ladder** because the names
of the middle stages — pre-seed, seed, Series A — are also fundraising terms.
That collision is unfortunate. The stage axis is measuring something more
fundamental than what round of capital you last raised.

The stage ladder is a measure of **search progress**. It answers: how much of
the repeatable, scalable business model from the mod-001 definition has been
*found*?

- **IDEA** — nothing has been found yet. You have a hunch and a candidate
  problem.
- **PRE-SEED** — you're finding out whether *any* solution to your problem
  could work. You're building the first thing that a real user might use.
- **SEED** — you have early evidence a solution works and you're finding out
  whether it repeats: same value proposition, next customer, and the one
  after that.
- **SERIES-A** — the solution repeats and you're finding out whether the
  motion around it (pricing, sales, marketing, onboarding, retention) scales
  into a machine an investor would underwrite.
- **GROWTH** — the machine works. Now you're scaling it — headcount, spend,
  geography, product surface — without breaking the load-bearing parts.
- **MATURE** — the business is durable. You're not searching for the model
  anymore; you're stewarding, governing, and steering to an outcome. This is
  the stage where mod-001's definition says you have stopped being a startup.

Fundraising rounds correlate loosely with this ladder because investors also
try to underwrite by search progress. But you can be pre-seed *without ever
raising a pre-seed round*, seed *without ever taking a check called "seed,"*
and Series A *long after your priced round closed if the search stalled after
the money landed.* The ladder is about what you have and haven't found, not
about what wired in the last quarter.

The org-level `STARTUP_STAGES.md` gives the canonical one-liner for each
stage. Chapter 02 of this module unpacks each row into a signal, a founder's
core question, and a typical focus. Chapter 03 shows what it looks like to
run activities from the wrong row.

## Why a clock and not just a checklist

The stage ladder has three properties a flat checklist cannot encode.

**1. Prerequisite ordering across stages.** You cannot productively work SEED
questions before the PRE-SEED question is answered. You can *think* about them,
you can even write documents about them, but the answers won't stick because
they depend on evidence you don't have yet. A founder who tries to underwrite
unit economics before they have a repeatable sale is answering the wrong
question in a lot of detail; the answer will be replaced the moment real data
arrives. The ladder tells you which questions are answerable now and which are
premature.

**2. Composition with the graph.** Each stage lights up a specific *subgraph*
of mod-002. At IDEA, the customer-facing branch's first node (Customer
Discovery) is on and everything downstream is off. At PRE-SEED, Customer
Discovery is still on, plus you now touch Incorporation and enough of Runway
to know how long the money lasts. At SEED, most of the graph comes online —
early Fundraising, first PMF signals, GTM shape, Unit Economics vocabulary. At
SERIES-A and beyond, the graph is fully lit and the stage tells you which
nodes are the *current constraint* rather than which are on. The stage is the
zoom-and-highlight on top of the map.

**3. Deferral discipline.** Foundations' whole design is that depth lives in
pillar repos and Foundations only teaches positions and edges. The stage tag
is what lets the deferral be *safe*: it is not "you'll never need this," it
is "you'll need this at this stage, and here is where to find it." A learner
who reads Foundations at IDEA sees the whole graph but is only asked to
*execute* the IDEA-appropriate slice; the rest is registered on the map for
the moment when it becomes their problem.

## How the stage axis composes with the graph

Concretely, put the graph and the stage axis on the same page and you get a
matrix — nodes on one axis, stages on the other — with three kinds of cells:

- **Active** — this node is a load-bearing focus for a founder at this stage.
  The founder should be working it directly this week.
- **On but delegated** — this node is functioning inside the company but is
  handled by someone other than the founder. The founder still tracks it as
  an input to their decisions but is not the operator of it.
- **Off / premature** — this node's work will happen later. Working it now is
  a waste of the founder's most scarce resource — attention.

The typical IDEA-stage cross-section:

- Active: Customer Discovery.
- On but delegated: (nothing — nothing else exists yet at IDEA).
- Premature: everything else — PMF metrics, GTM strategy, Sales pipeline,
  Growth loops, Equity structure, Governance, Fundraising, Financial Modeling,
  Unit Economics, Capital Allocation, Exit.

The typical PRE-SEED cross-section:

- Active: Customer Discovery (still), MVP scoping (part of the Solution search
  from mod-001 chapter 05), Incorporation, first Runway math, first Founder
  Agreements.
- On but delegated: (still nothing — founders do everything).
- Premature: Series-A-level unit economics, board governance, capital
  allocation frameworks, exit planning.

The typical SEED cross-section fans wider — early Fundraising, first PMF
metrics, GTM prototype, first hires (Team search from mod-001 chapter 05),
runway model that a fund can read. And so on up the ladder. Chapter 02 makes
each cross-section explicit.

The important observation is that **the "premature" column is not empty at any
stage before MATURE.** There is always more of the graph *not* to work than to
work. Founder attention is a fixed budget; the stage tells you where the
budget goes.

## Where the stage axis lives in the org

The stage axis is a first-class concept across the org, not something invented
in this module. Three places to look for it:

- **`STARTUP_STAGES.md`** (this repo, at the root). The canonical one-page
  reference for the six stages, with the signal / core question / typical
  focus table. This module's chapter 02 walks the same rows in more depth.
- **The front-matter of every module `README.md`** in every repo in the org.
  Every module carries `stage:` (the earliest stage at which it becomes
  actionable) and optionally `stages:` (all stages where it applies). Chapter
  07 of this module explains how to read and set those fields.
- **`.aicg/curriculum-plan.json`** and the equivalent manifests in the pillar
  and role repos. The stage tag is mirrored into the machine-readable
  manifests so the whole catalog can be filtered by stage programmatically.

When you finish this module and open `startup-product-gtm-curriculum` or
`startup-finance-fundraising-curriculum` for the first time, the *first*
filter you'll apply is your own stage. Chapter 07 makes that operation
concrete.

## Two ways the axis gets misread

Two failure modes to name before chapter 02 walks the ladder.

**Failure mode 1 — treating the stage as a badge.** "We're a Series-A
company" is often used as a status claim, not a description of search
progress. Founders who lead with the badge tend to import Series-A behaviours
(compensation committees, board committees, formal capital-allocation
processes) into companies that have not yet closed the earlier searches. The
result is a company that *acts* Series-A while its underlying business is
still SEED or worse. The stage is a diagnosis of the business, not a title on
the founder.

**Failure mode 2 — treating the stage as fixed.** Stages can regress. A
Series-A company that loses PMF has a Series-A cap table and a SEED-stage
underlying business; the founder's job is to recognise the regression and
work the SEED-stage question, not to keep executing Series-A activities on
top of a broken foundation. The stage ladder is where you *are*, not where
you were.

## How the rest of this module builds on this chapter

- **Chapter 02** walks the six stages in depth — for each, the signal, the
  founder's core question, and the typical focus.
- **Chapter 03** shows what stage-mismatched activity looks like in the wild
  and gives you the taxonomy for diagnosing it.
- **Chapter 04** reads Paul Graham's `Do Things That Don't Scale` as the
  canonical reconciliation of the IDEA / PRE-SEED stage with the fact that
  the mod-001 definition demands scalability *eventually*.
- **Chapter 05** reads the Startup Genome premature-scaling report as the
  empirical anchor: what happens to companies that skip stages.
- **Chapter 06** turns everything into a **checklist** you can point at any
  candidate activity to decide stage-appropriateness.
- **Chapter 07** ties it back to the org — how the `stage:` tag on every
  module in every repo makes the whole curriculum filterable by where you
  are.

## Summary

- The stage axis is the third axis of the three-axis model — the *clock* on
  top of the graph's *map*.
- It measures search progress (how much of the repeatable, scalable business
  model has been found), not fundraising history.
- The ladder is `IDEA → PRE-SEED → SEED → SERIES-A → GROWTH → MATURE`; each
  step has a distinct signal, question, and focus (chapter 02).
- The stage tells you which nodes on the mod-002 graph are active, delegated,
  or premature at any given moment.
- Every module in every repo in the org carries a `stage:` tag. Chapter 07
  makes reading and setting those tags operational.

## Homework

No exercise for this chapter directly — it is the frame for the whole module.
The stage signal drill (exercise 01) grounds chapter 02; the mismatch teardown
(exercise 02) grounds chapter 03; the checklist exercise (05) grounds chapter
06.
