# Placing an Artifact on the Graph

## Motivation

Chapters 02, 03, and 04 walked the three branches. This chapter turns the map
into a tool. The recurring founder question — *what do I actually do with a
thing in front of me?* — becomes a placement problem: **which node owns this
artifact, which nodes does it depend on, and which repo owns the depth?**

The founders who get the most out of Foundations use this move dozens of
times a week. A SAFE hits your inbox — place it. An investor asks for
your ICP — place it. Your co-founder proposes an option-pool refresh —
place it. Placement is fast, reproducible, and it either surfaces the
right next move or surfaces the missing upstream work that must be done
first.

This chapter installs the placement move as a five-step procedure and
walks it against eight concrete artifacts drawn from real founder work.

## The five-step placement move

For any artifact — a document, a decision, a spreadsheet, a legal
instrument, an operational choice — apply five questions in order.

1. **What does the artifact claim to be about?** Read the artifact
   itself; do not go from the name alone. A "board pack" can be a
   governance artifact, a fundraising artifact, or a founder-numbers
   artifact depending on what is actually inside it.
2. **Which single node is the artifact's primary home?** Pick one — the
   node that would *own* the artifact if the graph were the whole map.
   Ambiguity here is a hint the artifact is doing two jobs and should
   probably be split.
3. **Which upstream nodes did this artifact depend on to be produced?**
   List them explicitly. If any of the listed upstream nodes have not
   been done, the artifact is being written on missing foundations and
   is likely to be wrong or misleading.
4. **Which downstream nodes will consume this artifact?** List them. The
   artifact's value is measured in what it enables downstream; if
   nothing downstream needs it, the artifact is probably premature.
5. **Which pillar curriculum owns the depth for the primary node?** Name
   the specific repo. That is the address the reader goes to when they
   need to actually work the artifact for real.

Two rules of thumb:

- **One primary node, many touched nodes.** Artifacts almost always
  belong to a single node primarily and *touch* several others. Placement
  is about naming the primary; the touched nodes fall out.
- **Force yourself to name the missing upstream.** Half the value of
  the exercise is discovering that an artifact is being drafted with a
  missing prerequisite. Don't paper over that with "well, we can figure
  it out later" — that's exactly the misplacement Foundations is
  training against.

## Worked placements — eight founder artifacts

The eight artifacts below cover the placements you are most likely to
have to make in a real founder week. Read each one; the pattern is the
point.

### Placement 1 — A signed SAFE (Simple Agreement for Future Equity)

- **Primary node:** `Fundraising` (corporate-structure branch).
- **Upstream dependencies:** `Incorporation` (must have an entity to
  sign as); `Equity` (the SAFE is a *promise* of future equity — the
  cap table must be able to receive it).
- **Downstream consumers:** `Runway` (economics branch — the SAFE
  proceeds become cash and extend runway); `Equity` (at conversion,
  the SAFE becomes preferred stock on the cap table).
- **Owning repo:** [`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum).

### Placement 2 — A customer interview note

- **Primary node:** `Customer Discovery` (customer-facing branch).
- **Upstream dependencies:** the segment definition itself — even a
  bad one — is upstream of the interview being scoped correctly.
- **Downstream consumers:** `Product-Market Fit` (the aggregate of many
  interviews is one of the primary PMF signals); potentially `GTM
  Strategy` (interview language often lands directly in positioning).
- **Owning repo:** [`startup-product-gtm-curriculum`](https://github.com/ai-startup-curriculum/startup-product-gtm-curriculum).

### Placement 3 — A runway model spreadsheet

- **Primary node:** `Runway` (economics branch).
- **Upstream dependencies:** `Startup Economics` vocabulary; the
  *current* Financial Modeling artifact (or the founder-numbers-tier
  model from mod-005) that produces the burn number; `Fundraising`
  (as source of the cash-on-hand starting balance).
- **Downstream consumers:** every stage-appropriate operating decision
  — hiring plan (which is a `Capital Allocation` artifact), fundraise
  timing (`Fundraising`), pivot/cut decisions (all branches).
- **Owning repo:** [`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum);
  Foundations mod-005 owns the founder-slice version.

### Placement 4 — A term sheet from a lead investor

- **Primary node:** `Fundraising` (corporate-structure branch).
- **Upstream dependencies:** `Incorporation` (structure and jurisdiction
  must match the term-sheet terms); `Equity` (existing cap table drives
  the dilution math and the option-pool ask); `Governance` (the term
  sheet will add board seats and protective provisions to whatever
  already exists); on the customer-facing side, the *reason the
  investor is willing to lead* — usually `Product-Market Fit`
  evidence and directional unit economics.
- **Downstream consumers:** the whole corporate-structure branch — the
  round modifies Equity, adds to Governance, and lands cash in
  `Runway`.
- **Owning repo:** [`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum)
  for the terms; [`startup-operations-governance-curriculum`](https://github.com/ai-startup-curriculum/startup-operations-governance-curriculum)
  for the governance-affecting terms.

### Placement 5 — An option-pool refresh (adding shares to the pool)

- **Primary node:** `Equity` (corporate-structure branch).
- **Upstream dependencies:** `Incorporation` (structure must permit it);
  `Governance` (the refresh usually requires board — and sometimes
  investor — approval under the consent matrix); `Fundraising` (the
  refresh is most often triggered by a priced round requiring a target
  post-money pool size).
- **Downstream consumers:** the hiring plan (`Capital Allocation`); the
  next round's dilution math (`Fundraising`); the preference stack at
  `Exit`.
- **Owning repo:** [`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum).

### Placement 6 — An ICP definition (Ideal Customer Profile)

- **Primary node:** `GTM Strategy` (customer-facing branch).
- **Upstream dependencies:** `Customer Discovery` (segment definition
  and problem validation); `Product-Market Fit` (evidence that the
  segment retains and pays).
- **Downstream consumers:** `Sales` (targeting, discovery calls,
  qualification); pricing decisions; `Growth` (channel selection is
  ICP-dependent).
- **Owning repo:** [`startup-product-gtm-curriculum`](https://github.com/ai-startup-curriculum/startup-product-gtm-curriculum).

### Placement 7 — A CAC / LTV table by channel

- **Primary node:** `Unit Economics` (economics branch).
- **Upstream dependencies:** `Sales` and `Growth` (they generate the
  raw cohort and channel data); `Startup Economics` vocabulary; `GTM
  Strategy` (channel definitions and ICP).
- **Downstream consumers:** `Capital Allocation` (channel spend
  decisions are directly driven by this table); `Financial Modeling`
  (the model's revenue drivers use per-cohort assumptions); the
  Series-A pitch narrative.
- **Owning repo:** [`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum).

### Placement 8 — A board pack for the quarterly board meeting

- **Primary node:** `Governance` (corporate-structure branch).
- **Upstream dependencies:** basically everything — `Financial Modeling`
  and `Runway` and `Unit Economics` from the economics branch;
  `Sales`, `Growth`, `PMF` evidence from the customer-facing branch;
  `Equity` and `Fundraising` updates from the corporate-structure
  branch. A board pack is one of the few artifacts that legitimately
  touches almost every node.
- **Downstream consumers:** the board's decisions — approvals, hires,
  strategic direction — which then flow back into `Capital
  Allocation`, `Fundraising`, and the operating loop of mod-004.
- **Owning repo:** [`startup-operations-governance-curriculum`](https://github.com/ai-startup-curriculum/startup-operations-governance-curriculum).

## The cross-branch coupling diagram

Chapters 02, 03, and 04 each named coupling edges into the other branches.
Here they are in one place — the wiring behind the three-branch drawing.

```
Sales / Growth ────────────────► Runway            (revenue affects burn)
Fundraising ──────────────────► Runway            (round is a cash step)
PMF ──────────────────────────► Fundraising       (round is priced on PMF evidence)
Governance ───────────────────► Capital Allocation (board consent gates big allocations)
GTM Strategy ─────────────────► Unit Economics    (channels define per-unit economics)
Growth ───────────────────────► Exit              (durable growth prices the outcome)
Governance ───────────────────► Exit              (board approves the exit process)
Equity ───────────────────────► Exit              (preference stack resolves at exit)
```

Every artifact you place will touch at least one of these edges. When you
place an artifact and one of these edges is not honored — for example, an
option-pool refresh proposed without Governance approval, or a Runway
model with no reference to the Fundraising cash step — the missing edge
is where the artifact is broken.

## The "check the placement before you ship" rule

The move Foundations recommends is small and cheap: before any
consequential founder artifact leaves your desk, do the five-step
placement and write the primary node + upstream + downstream + owning
repo in the top of the document (or in the commit message, or in the
email accompanying it). Three lines of placement metadata is enough.

The reason this rule pays for itself: the majority of expensive founder
mistakes are misplacements — an artifact built on a missing upstream, or
built for a downstream consumer that doesn't need it yet, or shipped
without engaging the owning-repo depth when it should have been. Writing
the placement forces the check to happen at the cheapest possible time —
before the artifact is shipped.

## What if you can't place it?

If you cannot place an artifact on the graph in under two minutes, one
of three things is happening:

1. **The artifact is trying to do two jobs.** Split it. A "GTM /
   Fundraising" combined document is almost always a positioning
   document *and* a fundraising narrative that should be two files.
2. **The artifact is genuinely premature.** It has no downstream
   consumer at your current stage. Consider deferring it. mod-003 has
   the stage-fit machinery to make this call sharper.
3. **The graph doesn't have the right node.** This is rare but real.
   Novel businesses (deep-tech, marketplaces with unusual take-rate
   structures, hybrid open-source-plus-commercial models) sometimes
   exercise a corner of the graph the standard nodes don't quite
   capture. In this case, work out which existing node is closest and
   name the mismatch — that is itself a Customer Discovery finding.

## Summary

- Placement is a five-step move: what is the artifact about, what is
  its primary node, what upstream did it need, what downstream will
  consume it, which pillar owns the depth.
- Eight canonical placements — SAFE, interview note, runway model, term
  sheet, option-pool refresh, ICP, CAC / LTV table, board pack — cover
  most of a founder's week.
- The cross-branch coupling diagram is the wiring behind the three-branch
  drawing; missing edges in a placement are where the artifact is
  broken.
- Ship placement metadata (three lines) with every consequential
  artifact. It's the cheapest quality check available.
- Un-placeable artifacts almost always mean: doing two jobs, premature,
  or exercising a genuinely novel node.

## Homework

Exercise 04 (`Place a Real Artifact on the Graph`) makes you run the
placement move against real artifacts from your own work. This is the
first exercise in the module that generalises beyond the specific
branches; do it after chapters 02–05 are all loaded.
