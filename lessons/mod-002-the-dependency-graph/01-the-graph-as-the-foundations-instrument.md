# The Graph as the Foundations Instrument

## Motivation

A founder gets asked about a hundred different things in a week — a customer
interview, a SAFE, an ICP definition, a runway model, a term sheet, a board
pack, an option-pool refresh, a CAC / LTV table, a pricing decision, a hiring
plan, a growth-loop diagram. Each is a real thing that owes something to the
things around it. None of them stand alone.

The instinct most founder education encourages is to treat these as a flat list
of topics — a menu of MBA seminars — and to read them in the order they show
up on a syllabus. That works fine until you hit a hard call. At that moment
you need to know two things at once: *what does this artifact depend on that I
haven't done yet?* and *what will break downstream if I ship it wrong?* A flat
list cannot answer those questions. A graph can.

Foundations gives you a graph. Its whole job is to be the mental model that
tells you where any startup question lives, what it depends on, and where the
depth lives when you eventually need it. This module installs that graph and
teaches you to place things on it.

## The graph in one picture

The graph has one root (Foundations itself), three main branches, and one
convergent endpoint (Exit / Endgame). This is the same picture published in
[`FUNCTIONAL_CURRICULA.md`](../../FUNCTIONAL_CURRICULA.md); the module treats
that file as the authoritative reference and this chapter as the reading key.

```
STARTUP FOUNDATIONS  (this repo — the shared root)
        │
        ├──► Customer Discovery
        │         │
        │         ▼
        │    Product-Market Fit
        │         │
        │         ▼
        │    GTM Strategy ──► Sales ──► Growth ──► Exit / Endgame
        │
        ├──► Corporate Structure
        │         ├──► Equity
        │         ├──► Governance ──► Exit / Endgame
        │         └──► Fundraising
        │
        └──► Startup Economics
                  ├──► Financial Modeling
                  ├──► Runway
                  ├──► Unit Economics
                  └──► Capital Allocation
```

Three branches. One root. One endpoint. The rest of this module walks the
branches (chapters 02, 03, 04), teaches you to place any artifact on a node
(chapter 05), gives you two canvases for the assumption set (chapter 06), and
names which pillar curriculum owns which node (chapter 07).

## What is a node, what is an edge

Loose usage of the word "graph" often means "diagram." Here the word carries
its precise sense.

- A **node** is a body of knowledge and practice — a coherent thing that owns
  a set of artifacts, a set of methods, and a set of decisions. `Customer
  Discovery`, `Fundraising`, `Runway`, and `Governance` are each nodes.
- An **edge** is a *dependency* — an arrow that says "the downstream node
  cannot be sensibly worked without something the upstream node produces."
  The arrow from `Customer Discovery` to `Product-Market Fit` says: you cannot
  claim PMF against a customer you never talked to.
- A **branch** is a run of nodes connected by edges that form a coherent path.
  The customer-facing branch is one such run; the corporate-structure branch
  is another.

The graph is a **directed acyclic graph** in shape — dependencies flow in one
direction and (with one intentional exception discussed below) do not loop
back. The one intentional exception is Exit: it is drawn as a convergent
endpoint reached from both the Growth end of the customer-facing branch and
the Governance end of the corporate-structure branch, because an exit is
literally the moment those branches settle up.

## Why a graph and not a list

The graph shape encodes three things a list can't.

**1. Prerequisite order.** The nodes are drawn so that you cannot skip
upstream without paying for it downstream. If you build a `Sales` motion
without doing the `Customer Discovery` and `PMF` work upstream, you are
selling to no one in particular; if you fundraise (`Fundraising`) without a
clean `Equity` structure and a functioning `Governance` shape, you are
raising into a broken container. This is the same argument mod-001 chapter 06
made about failure post-mortems: startups die by failing at the *upstream*
layer while the *symptom* shows up further down. The graph makes the
prerequisite legible before the failure happens.

**2. Cross-branch coupling.** The three branches look independent when drawn
side by side. They are not. `Runway` (economics branch) is directly gated by
`Fundraising` (corporate-structure branch) and by the sales output of the
customer-facing branch. `Governance` (corporate-structure branch) constrains
what you can do at `Capital Allocation` (economics branch) and at `Exit`
(customer-facing branch endpoint). The graph is drawn with three visual
branches because that is how founders think about them; the actual dependency
structure is a weave, and later chapters show which edges cross which.

**3. A canonical place for every artifact.** Anything a founder holds in her
hand — a term sheet, a customer interview note, a runway model, an ICP
definition — lives on exactly one node as its owner, and touches the nodes it
depends on. The graph gives you a canonical *address* for artifacts. That
address is what lets Foundations defer depth to a pillar curriculum without
losing the artifact — you know exactly where to send someone to go deep.

## What Foundations owns and what the pillars own

Foundations owns *the graph itself* — the nodes, the edges, the branches, and
the ownership rule. It does not own the depth of any node. That depth lives
in a pillar curriculum:

| Branch | Pillar curriculum that owns the depth |
|---|---|
| Customer-facing (Customer Discovery → PMF → GTM → Sales → Growth) | [`startup-product-gtm-curriculum`](https://github.com/ai-startup-curriculum/startup-product-gtm-curriculum) |
| Corporate-structure (Incorporation → Equity → Governance → Fundraising) | [`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum) for Equity / Fundraising; [`startup-operations-governance-curriculum`](https://github.com/ai-startup-curriculum/startup-operations-governance-curriculum) for Incorporation / Governance |
| Economics (Financial Modeling → Runway → Unit Economics → Capital Allocation) | [`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum) |
| Exit / Endgame (convergent endpoint) | [`startup-exit-curriculum`](https://github.com/ai-startup-curriculum/startup-exit-curriculum) |

Chapter 07 makes this ownership rule concrete and drillable. For now, the
takeaway is: Foundations teaches the *map*; the depth is one repo away, and
you can always find the right one by walking the graph to the node in
question and reading its owner.

## Two ways the graph gets misread

Two failure modes to name before you start walking the branches.

**Failure mode 1 — reading the graph as chronology.** The branches are drawn
in dependency order, not calendar order. `Customer Discovery` is upstream of
`PMF`, which is upstream of `GTM Strategy` — but in real founder time you
often do a little of each simultaneously in the earliest weeks, and you loop
back to Customer Discovery when the PMF signal weakens. The graph tells you
*which node's output the next node needs*, not *when you do each one in the
calendar week*. That's what the stage axis (mod-003) is for.

**Failure mode 2 — treating branches as independent teams.** The branches
correspond loosely to the traditional departmental cuts of a larger company
(product / finance / people-and-legal). At startup stage there are no
departments — there is one founder or a handful of them, and the branches
are three views on the *same* company. Any decision at any node has ripple
effects across all three branches. The graph is drawn as three branches so
you can talk about it; the company itself is the whole graph at once.

## How to use the graph over the whole curriculum

The graph is used three ways across Foundations.

- **In mod-002 (this module):** as an *object of study* — you walk it, you
  place artifacts on it, and you memorise which pillar owns which node.
- **In mod-003 (stage axis):** as the *scope* — the stage axis tells you
  which nodes on the graph you should be actively working *right now*, and
  which are premature or already delegated. A pre-seed founder does not work
  the `Governance` node; a Series-A founder does not stop working `PMF`.
- **In mod-004 (operating basics) and mod-005 (founder numbers):** as the
  *lookup index* — when a decision or a metric comes up, you address it to a
  node and know which upstream inputs to check before you decide.

The graph also outlives Foundations. Every downstream pillar curriculum
assumes you have this map already loaded. When
`startup-finance-fundraising-curriculum` says "this module lives at the
Fundraising node," it is speaking a language mod-002 taught you. If you skip
this module, every pillar curriculum reads like a flat menu of topics, which
is exactly the failure mode Foundations exists to prevent.

## Summary

- The map is a directed acyclic graph with three branches (customer-facing,
  corporate-structure, economics) sharing one root (Foundations) and one
  endpoint (Exit).
- Nodes are bodies of knowledge; edges are dependencies. Missing an upstream
  node causes downstream failure — the graph is the pre-mortem for that.
- The three branches look independent but are coupled across their nodes;
  chapters 02–04 walk each branch and chapter 05 makes the coupling explicit.
- Foundations owns the graph; each node's depth lives in a specific pillar
  curriculum. Chapter 07 drills the ownership.
- The graph is not a calendar and it is not an org chart. It is a
  prerequisite map.

## Homework

No exercise for this chapter directly — it is the frame for the whole module.
The three branch-tour exercises (01, 02, 03) walk the branches; do them as
you finish chapters 02, 03, and 04 respectively.
