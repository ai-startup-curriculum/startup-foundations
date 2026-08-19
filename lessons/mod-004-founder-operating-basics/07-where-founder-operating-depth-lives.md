# Where Founder-Operating Depth Lives

## Motivation

The previous six chapters described the founder's operating loop
and the seven artifacts that carry it. That treatment is
deliberately shallow in specific places — hiring, comp, management,
firing, product-team operating loops, GTM operating loops, capital
allocation, and investor-communication at scale. Each of those
areas has genuine depth that a founder eventually needs, and each
of them has an *owning pillar repo* where the depth lives.

This chapter is the deferral map. It draws the boundary around the
founder-operating slice this module owns and points every
adjacent depth to its home. mod-002 chapter 07 gave the
node-level ownership map for the whole graph; this chapter is the
same rule applied to the founder-operating slice specifically.

The ownership rule from mod-002 is worth restating: *Foundations
owns positions and edges; the pillar repos own depth.* Without the
rule, this module would silently expand into a full operating
manual for a company at any size — and by trying to teach
everything, would teach nothing well.

## The founder-operating slice — what this module actually owns

This module owns, and only owns, four things:

1. **The four-part operating loop** — decide, allocate,
   communicate, measure — as a repeatable weekly cadence (chapter
   01).
2. **The seven cheap artifacts that carry the loop** — Monday
   plan, Friday shipped-and-learned, metrics one-pager, decision
   log, OKR (one/three/weekly), Sequoia-shape narrative, first
   investor update (chapters 02–06).
3. **The four-audience re-frame of the narrative** — co-founder,
   first employee, first customer, first investor (chapter 05).
4. **The transition survival properties** — the loop and the
   artifacts are sized so they survive (a) going from one founder
   to two, (b) taking the first hire, and (c) starting to send an
   investor update, without redesign.

Everything else — and there is a lot of "everything else" — is
depth in an owning pillar. The rest of this chapter walks the
deferrals.

## Deferral 1 — hiring, comp, management, firing

**What this module says.** Chapter 01 names "hires" as one of the
three scarce founder resources that "allocate" moves. Chapter 03
lists people calls as a category of the decision log. Chapter 05's
team section says the narrative should name what's missing on the
team. That is the full extent of the treatment.

**What this module does NOT teach.**
- How to write a job description or a scorecard.
- How to structure an interview loop, calibrate interviewers, or
  make a hire/no-hire call as a team.
- How to price a role, structure the compensation package, size
  the equity grant, choose a vesting schedule, or handle a
  refresh grant.
- How to onboard a hire past the first day.
- How to run 1:1s, give feedback, set expectations, or evaluate
  performance.
- How to have the hard conversation, put someone on a PIP, fire
  someone, or manage the departure legally and humanely.

**Where depth lives.**
[`startup-operations-governance-curriculum`](https://github.com/ai-startup-curriculum/startup-operations-governance-curriculum)
(level 25). The operations-governance repo owns the people pillar,
which includes hiring practice, comp architecture, management
practice, and firing practice. When you get to the point in your
operating loop where "hire the first engineer" is a live call, the
depth for how to run that hire is one repo over. Come back to this
module for the *loop that surfaces the call*; go to the pillar for
*how to execute the call*.

**Adjacent depth.** Equity mechanics for hires (cap-table impact
of a hire's option grant, the option-pool refresh math, 409A
valuations) live in the finance-fundraising pillar
([`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum))
because they are cap-table decisions. The operations pillar and
the finance pillar coordinate on hires but each owns half.

## Deferral 2 — product / GTM operating loops

**What this module says.** Chapter 01 names customer- and
product-facing calls as categories of the decision log. Chapter
05's customer re-frame of the narrative is the customer-facing
communication artifact. The metrics one-pager includes a
North-Star metric and its supporting numbers, which are almost
always product / GTM instrumentation. That is the full extent.

**What this module does NOT teach.**
- How to run a customer discovery interview, a jobs-to-be-done
  session, or a positioning workshop.
- How to define an ICP, a persona, a segmentation, or a
  messaging framework.
- How to run a product-management operating loop — the sprint
  cadence, the roadmap review, the release checklist, the PMM
  handoff.
- How to run a sales operating loop — the pipeline review, the
  forecast cadence, the deal desk, the ramp plan for a new AE.
- How to run a growth operating loop — the experiment intake,
  the analysis cadence, the channel review, the retention
  program.

**Where depth lives.**
[`startup-product-gtm-curriculum`](https://github.com/ai-startup-curriculum/startup-product-gtm-curriculum)
(level 20). The product/GTM repo owns the customer-facing branch
end to end — customer discovery, PMF, GTM strategy, sales, and
growth — each with its own operating loop at the appropriate
scale. The founder's operating loop in this module *feeds into*
each of those loops (a founder-only decision from chapter 03
might change a roadmap; a Monday plan item from chapter 02 might
be "run this week's customer discovery"), but the loops
themselves are pillar depth.

**When to reach for the pillar.** The signal that the
product/GTM pillar depth is now load-bearing is when the
founder has hired the first product-role or GTM-role and the
question becomes "how does that role run their weekly
operating loop?" — which is exactly the moment the pillar
starts being read.

## Deferral 3 — capital allocation and investor-update-at-scale

**What this module says.** Chapter 01 names capital as one of the
three scarce founder resources that "allocate" moves. Chapter 03
lists capital calls (raise / don't raise, take / decline strategic,
approve / decline discretionary spend) as a decision-log category.
Chapter 06 covers the *first* monthly investor update at the
pre-seed / seed scale — one page, three sections. That is the full
extent.

**What this module does NOT teach.**
- How to build a capital-allocation framework — the deliberate
  process by which a company decides how much goes to product vs.
  GTM vs. R&D vs. corp-dev on what timeline against what expected
  return.
- How to construct a bottom-up financial model, a three-statement
  model, or a sensitivity analysis behind an allocation decision.
- How to structure a fundraise — the round type, the instrument
  (SAFE vs. priced), the pricing, the process, the term sheet, the
  legal negotiations.
- How to write an investor update at Series-A and later — the KPI
  packs, the board-update-as-distinct-artifact, the segmented
  updates for different audience tiers, the accompanying
  financial statements.
- How the board pack is structured, how board meetings are run,
  and how the update-to-board rhythm differs from the
  update-to-investors rhythm.

**Where depth lives, split.**

- **Capital allocation frameworks, financial modelling,
  fundraising, later-stage investor updates** —
  [`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum)
  (level 20). The finance-fundraising pillar owns the numbers-side
  of capital decisions end to end.
- **Board packs, board governance, and the corporate-governance
  rhythm** —
  [`startup-operations-governance-curriculum`](https://github.com/ai-startup-curriculum/startup-operations-governance-curriculum)
  (level 25). The operations-governance pillar owns the
  governance-side.

**When to reach for the pillars.** The finance-fundraising pillar
becomes load-bearing when the founder starts running a real
fundraise (typically at SEED transitioning to SERIES-A). The
operations-governance pillar becomes load-bearing when there is a
real board (typically post-Series-A priced round). Chapter 06's
first investor update is deliberately positioned *before* either
of those inflections so the discipline is in place when they hit.

## Deferral 4 — OKR practice at organisational scale

**What this module says.** Chapter 04 formalises the *lightweight*
OKR shape at two-to-three people — one company objective, three
KRs, weekly check-in — and names the four anti-patterns that make
even this small shape go sideways.

**What this module does NOT teach.**
- How OKRs cascade across teams, functions, and pods when the
  company grows past ~10 people.
- Calibration exercises across teams — the meetings and rituals
  by which one team's KRs are checked against another team's KRs.
- The tooling that scales OKR practice (dedicated OKR software,
  integration with performance-review cycles).
- How the OKR rhythm interacts with the annual-planning rhythm,
  the budget rhythm, and the compensation rhythm at company
  scale.

**Where depth lives.**
[`startup-operations-governance-curriculum`](https://github.com/ai-startup-curriculum/startup-operations-governance-curriculum).
Full OKR practice is a people-and-management topic that scales
with headcount; the operations-governance pillar owns it. The
primary sources (Grove, Doerr — see `resources.md`) are the same
either way; this module reads them for the two-person shape, the
pillar reads them for the multi-team shape.

## Deferral 5 — the mechanics of the pitch deck itself

**What this module says.** Chapter 05 covers the *ten-part
Sequoia shape* of the underlying founder-narrative, and the
four-audience re-frame. That is the underlying story from which a
deck is derived.

**What this module does NOT teach.**
- How to design specific slides — the layout, the typography, the
  chart choices, the appendix structure.
- How to sequence the deck differently for a first meeting vs. a
  partners meeting vs. a follow-up ask.
- How to prepare for the specific investor's specific model, the
  specific fund's stage focus, the specific partner's known
  patterns.
- How to answer specific investor-diligence questions (customer
  references, cohort analysis, competitive positioning,
  regulatory posture).
- How to run the fundraise process itself — the outreach
  cadence, the meeting sequencing, the term-sheet negotiation.

**Where depth lives.**
[`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum).
The fundraising pillar owns the deck's *specific realisation*
against the *specific investor process*. This module owns the
narrative's underlying ten-part shape; the pillar owns everything
about how that shape becomes a deck that closes a round.

## The ownership map in one table

| Topic | Owning repo | This module's role |
|---|---|---|
| **Weekly operating loop and its 7 artifacts** | Foundations mod-004 (this module) | Full ownership |
| **Founder-narrative shape and audience re-frames** | Foundations mod-004 | Full ownership |
| **First investor-update template (one-pager)** | Foundations mod-004 | Full ownership |
| **Lightweight OKR at 2-3 people** | Foundations mod-004 | Full ownership |
| **Decision log discipline** | Foundations mod-004 | Full ownership |
| Hiring / comp / management / firing depth | [`startup-operations-governance-curriculum`](https://github.com/ai-startup-curriculum/startup-operations-governance-curriculum) | Founder calls only |
| Product / customer-discovery / PMF / GTM / sales / growth loops | [`startup-product-gtm-curriculum`](https://github.com/ai-startup-curriculum/startup-product-gtm-curriculum) | Feeds into via founder-only calls and narrative |
| Capital allocation frameworks and financial modelling | [`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum) | Founder-numbers slice only (mod-005) |
| Fundraising process and later-stage investor updates | [`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum) | Only the *first* one-pager update |
| Full OKR practice at company scale | [`startup-operations-governance-curriculum`](https://github.com/ai-startup-curriculum/startup-operations-governance-curriculum) | Only the 2-3 person lightweight shape |
| Board governance, board packs, board meeting rhythm | [`startup-operations-governance-curriculum`](https://github.com/ai-startup-curriculum/startup-operations-governance-curriculum) | None — pre-board only |
| Pitch-deck specific realisation / fundraising process | [`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum) | Only the underlying ten-part narrative shape |

## The deferral formula in this module

mod-002 chapter 07 defined the deferral formula Foundations uses
throughout:

> `<Node>` — position on the graph, brief description of what the
> node is, and hand-off. **Depth lives in `<owning repo>`.**
> Foundations does not go further; do not go read the deep
> material until it is stage-appropriate for your work.

This module uses the formula against every topic listed above. When
a chapter mentions a hire, a fundraise, a capital allocation, or a
board pack, it names the topic, connects it to the founder's
operating loop (which is what Foundations owns), and points at the
owning pillar. No chapter tries to be the pillar; every chapter
points at the pillar it needs.

## Why the boundary matters

Three reasons for keeping the boundary sharp.

**1. This module has to be finish-able at PRE-SEED / SEED.** A
pre-seed founder needs the operating loop *now*; they cannot wait
for a comp-architecture module to be read first. The boundary is
what makes the module 22 hours instead of 220.

**2. The pillar work is stage-gated too.** A pre-seed founder does
not need to read the operations-governance pillar's full hiring
depth; they will hire one person, using the pillar's introductory
material, when it becomes stage-appropriate. Sending them to the
whole pillar too early violates mod-003's premature-scaling
warning.

**3. Every pillar keeps a single source of truth.** When YC updates
the SAFE, the update lands in the finance-fundraising pillar. When
labor law changes, the update lands in the operations-governance
pillar. When PMF frameworks evolve, the update lands in the
product-GTM pillar. This module's job is to point to the pillars,
not to duplicate their content — so it never falls out of date on
depth topics that change faster than Foundations does.

## Summary

- This module owns the *founder's operating loop* and the *seven
  artifacts* that carry it. Nothing more.
- Hiring / comp / management / firing depth lives in
  [`startup-operations-governance-curriculum`](https://github.com/ai-startup-curriculum/startup-operations-governance-curriculum).
- Product / GTM / sales / growth operating loops live in
  [`startup-product-gtm-curriculum`](https://github.com/ai-startup-curriculum/startup-product-gtm-curriculum).
- Capital allocation, fundraising, and later-stage investor-update
  depth live in
  [`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum).
- Full OKR practice at organisational scale, and board governance,
  live in
  [`startup-operations-governance-curriculum`](https://github.com/ai-startup-curriculum/startup-operations-governance-curriculum).
- The founder-narrative's ten-part shape and audience re-frames are
  owned here; the deck's specific realisation for a specific
  fundraise is finance-fundraising pillar depth.
- The boundary is what keeps this module tractable and keeps the
  pillars authoritative.

## Homework

This chapter has no dedicated exercise. Its content is exercised
implicitly in every other exercise in the module — when a hire, a
fundraise, a customer-discovery play, or a board decision surfaces,
the writer is expected to name the depth as pillar-owned and stop
there. The exercise reviewers (and the module quiz, when written)
check that the boundary is respected.
