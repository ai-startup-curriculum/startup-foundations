# Where This Curriculum Sits

## Motivation

Every curriculum has a scope. The one that hides its scope tells you it covers
everything, which is the same as covering nothing well. Foundations is
explicit about its scope: it owns the *mental model* that every other
curriculum in the `ai-startup-curriculum` org depends on, and it defers depth
to the pillar curricula and role pathways.

This chapter makes the scope claim concrete. You should leave with a clear
answer to two questions:

- What is `startup-foundations` responsible for, and what is it deliberately
  not responsible for?
- Given a specific question I have as a founder, which repo do I look in?

## The level ladder

The org organizes curricula on a *level* — a rough number that says how
foundational a body of knowledge is relative to others. Lower level =
more foundational = studied earlier.

| Level | Repos | Role |
|---|---|---|
| **10** | `startup-foundations` | The shared root. Every pathway inherits this at 100%. |
| **20** | `startup-product-gtm-curriculum`, `startup-finance-fundraising-curriculum` | Functional pillars for the customer-facing and economics branches. |
| **25** | `startup-operations-governance-curriculum` | Functional pillar for the corporate-structure and people branches. |
| **30 / 35** | `founder-ceo-curriculum`, `cpo-curriculum` (30); `cto-curriculum` (35) | Role pathways — curated views over the pillar curricula. |
| **40** | `startup-exit-curriculum` | Functional pillar for the exit / endgame branch. |

Foundations at level 10 is intentionally the smallest of the curricula in
scope. Its job is to be the shared vocabulary, the shared taxonomy, and the
shared shape reference. It is not the deepest treatment of anything.

## What Foundations owns

Explicit ownership from `CURRICULUM.md`:

- **The system.** The definition of a startup (chapter 01), the two operating
  traditions it runs on (chapter 04), and the founder-as-search framing
  (chapter 05).
- **The graph.** The dependency map across the customer-facing branch, the
  corporate-structure branch, and the economics branch. Every artifact and
  question in a startup can be placed on a node; Foundations teaches the
  nodes and the edges, not the depth of any node. (Detailed in mod-002.)
- **The stages.** The stage ladder — IDEA → PRE-SEED → SEED → SERIES-A →
  GROWTH → MATURE — and what matters at each. (Detailed in mod-003.)
- **The founder's operating loop.** Decide, allocate, communicate, measure —
  as a repeatable weekly cadence sized for a 2–3 person startup. (Detailed
  in mod-004.)
- **The founder-numbers slice.** Runway, burn, growth, default alive /
  default dead, North-Star metric selection — enough numbers to instrument
  the search but not the full financial-modeling machinery. (Detailed in
  mod-005.)

That's the whole scope. Everything else is deferred.

## What Foundations defers up to a functional pillar

Foundations teaches the *position* of each pillar and its *shape*. Depth
lives in the pillar curricula themselves.

- **Customer discovery, PMF, GTM, sales, growth** → deferred to
  `startup-product-gtm-curriculum` (level 20). If you want an interview
  script, a positioning framework, a CAC model, a growth-loop treatment, or
  a channel-fit assessment, that repo owns it.
- **Financial modeling, unit economics, capital allocation, fundraising,
  equity mechanics** → deferred to `startup-finance-fundraising-curriculum`
  (level 20). Foundations teaches you what CAC, LTV, payback, and gross
  margin *are* (vocabulary tour in mod-005) so you can read the pillar
  curriculum without a glossary. It does not teach you how to build a
  three-statement model or negotiate a SAFE.
- **Hiring, comp, management, firing, org design, legal, governance,
  operations** → deferred to `startup-operations-governance-curriculum`
  (level 25). Foundations teaches the founder-agreement basics and the
  decision-log discipline in mod-004; everything else — including
  compensation-committee charters, employment law, and management-layer
  design — lives one level up.
- **M&A, secondaries, IPO, succession, shutdown** → deferred to
  `startup-exit-curriculum` (level 40). Foundations teaches you what an
  exit *is* as an outcome shape; the mechanics live in the exit repo.

## What Foundations defers sideways to a role pathway

The role pathway repos (`founder-ceo-curriculum`, `cto-curriculum`,
`cpo-curriculum`) inherit Foundations at 100% coverage. They then add
role-specific curated views over the pillar curricula.

- A CEO learner: after Foundations, follow `founder-ceo-curriculum` to see
  which pillar modules a CEO needs and in what order.
- A CTO learner: after Foundations, follow `cto-curriculum` — same modules
  are pulled from the same pillar curricula, but the ordering and emphasis
  is different because the CTO's day looks different.
- A CPO learner: after Foundations, follow `cpo-curriculum`.

The role pathway repos do **not** re-teach Foundations. They point back at
this repo and depend on it. This is the org's *no-fork, no-duplication* rule:
the same lesson (cap table, runway model, decision log) is authored once, in
the correct repo, and referenced from wherever else it is needed.

## Given a question, where do I look?

A working founder does not have time to hunt across seven repos for an answer.
Here is a lookup table for the most common questions.

| Question | Where to look |
|---|---|
| "What is a startup, actually, and am I building one?" | `startup-foundations`, mod-001 |
| "Where does this artifact live on the map?" | `startup-foundations`, mod-002 |
| "Is this activity stage-appropriate for me right now?" | `startup-foundations`, mod-003 |
| "How should a founder structure their week?" | `startup-foundations`, mod-004 |
| "What do runway, burn, and growth mean together?" | `startup-foundations`, mod-005 |
| "How do I actually run a customer interview?" | `startup-product-gtm-curriculum` |
| "How do I build a three-statement financial model?" | `startup-finance-fundraising-curriculum` |
| "How do I structure a SAFE / priced round / option pool?" | `startup-finance-fundraising-curriculum` |
| "How do I write an offer letter / hire my first PM / structure comp?" | `startup-operations-governance-curriculum` |
| "How do I run a board / set up governance / manage cap-table hygiene?" | `startup-operations-governance-curriculum` |
| "How do I run an M&A process / IPO / secondary?" | `startup-exit-curriculum` |
| "What does a CEO / CTO / CPO curriculum look like as a whole?" | The relevant role pathway repo |

If the question involves the *mental model* — what something is, where it
lives, when it matters, how the founder connects it to the rest — the answer
is Foundations. If the question involves *how to actually do it in depth*,
the answer is the pillar curriculum. That's the whole ownership rule.

## The engineering rationale

Why is the curriculum sliced this way instead of one big "founder MBA"?
Because the same reason we don't write one giant Python module. Each pillar
is a coherent body of knowledge with its own vocabulary, its own experts, its
own maintenance rhythm, and its own natural depth. Bundling them together
would produce a curriculum that:

- Is impossible to maintain because every update has to be threaded through
  a monolith.
- Cannot be re-used at different depths for different roles without
  duplication.
- Cannot be filtered to a stage or a role without hand-selecting from a
  giant table of contents.
- Cannot be authored incrementally because everything depends on
  everything.

Slicing the curriculum along the pillar / role / stage axes lets each piece
be authored once, at the right depth, in the right repo, and stage-tagged so
that a specific learner at a specific stage gets a specific, short, ordered
reading list. That is the engineering mentality applied to curriculum
design, and Foundations is the piece that makes the slicing legible.

## Summary

- Foundations is level 10 — the shared root every pathway inherits at 100%.
- It owns the *mental model*: the system, the graph, the stages, the
  founder's operating loop, the founder-numbers slice.
- It defers *up* to the pillar curricula (product-gtm,
  finance-fundraising, operations-governance, exit) for depth.
- It defers *sideways* to the role pathways (founder-ceo, cto, cpo) for
  role-specific curation.
- The lookup table above answers "where do I look for X?" for the common
  cases.

## Homework

No specific exercise for this chapter — the whole module ends with the lab
`lab-01-one-page-your-startup-as-a-system` which integrates the definition
(mod-001, chapter 01), the search model (chapter 05), and the ownership map
(this chapter). Move on to the exercises.
