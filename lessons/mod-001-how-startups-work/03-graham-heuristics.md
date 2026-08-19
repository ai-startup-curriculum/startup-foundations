# Paul Graham — Heuristics: `How to Start a Startup` and `The 18 Mistakes That Kill Startups`

## Motivation

`Startup = Growth` gives you the compass. Two earlier Graham essays give you the
heuristics — what actually to do and what actually kills you. Read together, they
are the most compressed founder-education document available in public.

- `How to Start a Startup` (March 2005) — the affirmative shape: what you need in
  order to have a chance.
- `The 18 Mistakes That Kill Startups` (October 2006) — the negative shape: the
  failure modes to avoid.

The two essays don't just complement each other; they explicitly define each
other. The mistakes are all failures to satisfy the requirements. Both are
required reading for this module.

## Essay 1 — `How to Start a Startup`

Graham compresses the requirements for a startup to have a chance into a small
number of ingredients. The essay works through them and their consequences.

The three ingredients he foregrounds are:

- **Good people.** Founders and early team who are technical, ambitious, and
  determined enough to survive the search. Graham argues, and Foundations
  agrees, that team selection is the most important early decision — because it
  gates every later decision. A wrong co-founder is much harder to unwind than a
  wrong product.
- **Something customers actually want.** The single most common form of startup
  failure is building a product no one needs. The essay elevates this above
  cleverness, technology, or presentation. It is a claim about which failure
  mode is empirically most common, and it is the same claim CB Insights makes
  in the failure post-mortem data in chapter 06.
- **Spending as little money as possible.** Every dollar spent shortens the
  runway you have to keep searching. Graham's argument is that low burn is not
  frugality theatre; it is what buys you the time to iterate. Every founder
  who has raised money and then watched runway shrink faster than the search
  progressed has re-discovered this the hard way.

The essay makes several other load-bearing points that recur throughout
Foundations:

- Startups are hard in a specific way — the difficulty is not physical or
  intellectual, it is psychological. Uncertainty compounds and the search takes
  longer than founders expect.
- The founder's job is to solve whatever the biggest problem is *this week*,
  not to specialize. This is the origin of what mod-004 calls the founder's
  operating loop.
- Timing matters. Some ideas that fail at one moment work five years later.
  This is why the Sequoia narrative shape in mod-004 asks explicitly for a
  "why now" section.

The essay is short. Read it.

## Essay 2 — `The 18 Mistakes That Kill Startups`

The companion essay lists eighteen specific failure modes Graham had observed in
the first years of Y Combinator. It is deliberately a list, not a framework —
each mistake is a discrete thing you can check yourself against.

Rather than reproduce the list here (read the primary source), we group the 18
into five clusters. The clusters map cleanly onto the graph layers in mod-002,
which is not a coincidence: each mistake is a failure at a specific point on
the dependency graph.

### Cluster A — team-layer mistakes

Failures that are really about *who is doing the work*. These include picking
the wrong co-founder, being a solo founder, launching from a bad location for
your industry, and not committing full-time.

The mistakes in this cluster tend to be the earliest and the hardest to
recover from because the team is upstream of every other decision. Foundations
returns to this in mod-002 (team as a graph node) and the founder-agreement
work in mod-004.

### Cluster B — problem/solution-layer mistakes

Failures about *what you're building and for whom*. Picking a market that's
hard to reach, targeting users who don't have money to spend, building
something you don't want yourself, having no clear picture of the user.

These map onto the customer-facing branch of the graph (Customer Discovery →
PMF). The countermeasure is Blank's Customer Development discipline from
chapter 04 — you find these mistakes by talking to customers early and often.

### Cluster C — process-layer mistakes

Failures about *how the work is done*. Building too slowly, launching too
late, launching too early, being too obsessed with the idea vs. the execution,
being a perfectionist.

These are the most tractable mistakes because they are inside the founder's
control on any given week. Ries's Build-Measure-Learn from chapter 04 is
largely a discipline for avoiding this cluster.

### Cluster D — commercial-layer mistakes

Failures about *making money*. Not charging, charging too little, being
afraid to sell, being unwilling to do sales that don't scale early on.

These map onto GTM and Sales in mod-002. Foundations does not teach GTM depth
(that's `startup-product-gtm-curriculum`) but it does insist that a founder
know when they are avoiding sales for the wrong reasons.

### Cluster E — capital-layer mistakes

Failures about *money in and money out*. Raising too little, raising too
much, spending too fast, hoping fundraising will fix a broken business.

These map onto the corporate-structure and economics branches. Foundations
covers the founder-numbers instrumentation in mod-005; capital-structure depth
lives in `startup-finance-fundraising-curriculum`.

<!-- needs-research: cross-check the 18 mistakes against Graham's original list to confirm each is present in the essay and to attach the exact wording per mistake before the module ships to learners. The five-cluster grouping is our synthesis; the mistakes themselves must be quoted from the essay. -->

## Why this list matters

The 18 mistakes are not an inspirational reading. They are diagnostic. When
something is going wrong in your startup and you can't name what, the list is a
menu of hypotheses to test yourself against: *am I doing one of these?*

The two counter-uses to watch for:

- **Do not treat the list as an anti-pattern checklist to run once and file
  away.** Startups regress. A founder who was charging appropriately in month
  six can be underpricing in month twelve because a new competitor scared them.
  The list is a re-diagnostic, not a one-shot exam.
- **Do not treat the list as complete.** It is Graham's observations from a
  specific vintage of Y Combinator companies. Failure modes not on the list
  exist. It is a starting point, not a taxonomy.

## The relationship between the essays

`How to Start a Startup` says: get good people, build something people want,
spend little. `The 18 Mistakes` says: here are the eighteen ways you'll fail to
do those three things. The mistakes essay is the negation of the how-to essay
made specific.

Read them in that order, once for surface understanding, then again with the
graph layers from mod-002 in mind. The second reading is what makes the failure
post-mortems in chapter 06 legible.

## Summary

- `How to Start a Startup` compresses the startup problem to three ingredients:
  good people, something people want, spend little.
- `The 18 Mistakes` enumerates the failure modes that violate those three
  requirements.
- The mistakes cluster into five graph-layer groups: team, problem/solution,
  process, commercial, capital. Chapter 06 uses these clusters to read real
  post-mortems.
- The list is a re-diagnostic, not a one-shot. Return to it every quarter.

## Homework

Read both primary essays:

- Paul Graham, `How to Start a Startup`, March 2005 — <https://paulgraham.com/start.html>
- Paul Graham, `The 18 Mistakes That Kill Startups`, October 2006 — <https://paulgraham.com/startupmistakes.html>

Exercise 05 (`Three Failure Post-Mortems Teardown`) will ask you to map real
failure cases onto both the 18-mistake list and the graph layers from mod-002.
