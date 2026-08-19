# The Ownership Rule in Action

## Motivation

mod-001 chapter 07 introduced the ownership rule at the *repo* level: this
curriculum owns the mental model; the pillar curricula own the depth. This
chapter drills the rule down to the *node* level. For any node on the graph,
you should be able to answer instantly: **which pillar curriculum owns the
depth of this node, and why?**

The ownership rule is what makes the whole three-axis model work. Without
it, every curriculum eventually re-teaches every other curriculum badly, and
learners hunt across duplicate content for the "real" version. With it, each
piece of knowledge lives in exactly one place — the *correct* place — and
every other curriculum in the org points to it. Foundations is the piece
that has to enforce the ownership rule most rigorously, because it sits at
level 10 and defers everything else.

This chapter is the reference table you will use for the rest of Foundations
and the rest of the org. Learn it well enough that when a founder question
lands, you can name the owning repo in under ten seconds.

## The ownership table — node by node

The table below covers every node on the graph as drawn in
[`FUNCTIONAL_CURRICULA.md`](../../FUNCTIONAL_CURRICULA.md).

| Node | Branch | Owning repo | Rationale |
|---|---|---|---|
| **Customer Discovery** | Customer-facing | [`startup-product-gtm-curriculum`](https://github.com/ai-startup-curriculum/startup-product-gtm-curriculum) | Whole customer-facing branch is product/GTM territory. |
| **Product-Market Fit** | Customer-facing | [`startup-product-gtm-curriculum`](https://github.com/ai-startup-curriculum/startup-product-gtm-curriculum) | PMF is the primary product/GTM diagnostic. |
| **GTM Strategy** | Customer-facing | [`startup-product-gtm-curriculum`](https://github.com/ai-startup-curriculum/startup-product-gtm-curriculum) | Namesake pillar. |
| **Sales** | Customer-facing | [`startup-product-gtm-curriculum`](https://github.com/ai-startup-curriculum/startup-product-gtm-curriculum) | Sales — including founder-led sales — is part of the GTM depth. |
| **Growth** | Customer-facing | [`startup-product-gtm-curriculum`](https://github.com/ai-startup-curriculum/startup-product-gtm-curriculum) | Growth loops, retention, expansion — GTM pillar depth. |
| **Incorporation** | Corporate-structure | [`startup-operations-governance-curriculum`](https://github.com/ai-startup-curriculum/startup-operations-governance-curriculum) | Legal + operations pillar. |
| **Equity** | Corporate-structure | [`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum) | Cap-table mechanics live with the finance/fundraising pillar. |
| **Governance** | Corporate-structure | [`startup-operations-governance-curriculum`](https://github.com/ai-startup-curriculum/startup-operations-governance-curriculum) | Board design, fiduciary duty, controls — operations/governance pillar. |
| **Fundraising** | Corporate-structure | [`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum) | Namesake pillar. |
| **Startup Economics** (root) | Economics | [`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum) | Vocabulary and framing owned with the finance pillar. |
| **Financial Modeling** | Economics | [`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum) | Bottom-up and three-statement modeling is finance pillar depth. |
| **Runway** | Economics | [`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum) | Depth here; **founder-slice** authored in Foundations mod-005. |
| **Unit Economics** | Economics | [`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum) | CAC / LTV / payback / gross margin — finance pillar depth. |
| **Capital Allocation** | Economics | [`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum) | Allocation frameworks and portfolio decisions — finance pillar depth. |
| **Exit / Endgame** | Convergent endpoint | [`startup-exit-curriculum`](https://github.com/ai-startup-curriculum/startup-exit-curriculum) | M&A, IPO, secondaries, succession, shutdown. |

Two ownership notes worth calling out explicitly.

**Runway (and burn, growth-rate, default alive / default dead).** These live
in the finance pillar for *depth* but Foundations owns a **founder-numbers
slice** authored in mod-005. The slice is deliberately narrow: enough to
instrument the search in the first two rounds without importing the whole
finance pillar. The rule for slice-vs-depth is: if the number is required to
run a founder's week at pre-seed / seed, Foundations owns it; everything
past that is finance-pillar depth.

**Incorporation vs Equity.** Both live on the corporate-structure branch but
own to *different* pillars — Incorporation to operations/governance, Equity
to finance/fundraising. This is deliberate: incorporation is a legal /
operational choice; equity is a financial instrument. The two pillars
coordinate on the branch but do not overlap on any node.

## The founder's lookup — from question to repo

The most useful form of the ownership table is not the node view but the
*question view*. When a founder asks a question, they want the answer, not
a taxonomy. The table below covers the most common founder questions in
Foundations' scope and points to the answer's home.

| Founder question | Where to look |
|---|---|
| "What is this artifact and where does it live on the map?" | Foundations mod-002 (this module) |
| "How do I actually run a customer interview?" | [`startup-product-gtm-curriculum`](https://github.com/ai-startup-curriculum/startup-product-gtm-curriculum) |
| "Do I have PMF? What would evidence look like?" | [`startup-product-gtm-curriculum`](https://github.com/ai-startup-curriculum/startup-product-gtm-curriculum) |
| "How do I write a positioning statement / define an ICP?" | [`startup-product-gtm-curriculum`](https://github.com/ai-startup-curriculum/startup-product-gtm-curriculum) |
| "How do I structure a founder-led sales motion?" | [`startup-product-gtm-curriculum`](https://github.com/ai-startup-curriculum/startup-product-gtm-curriculum) |
| "How do I build a growth loop / choose a channel?" | [`startup-product-gtm-curriculum`](https://github.com/ai-startup-curriculum/startup-product-gtm-curriculum) |
| "Should I incorporate as a C-corp or an LLC?" | [`startup-operations-governance-curriculum`](https://github.com/ai-startup-curriculum/startup-operations-governance-curriculum) |
| "How do I structure a co-founder agreement / vesting schedule?" | [`startup-operations-governance-curriculum`](https://github.com/ai-startup-curriculum/startup-operations-governance-curriculum) |
| "How should the board work / what's a board pack?" | [`startup-operations-governance-curriculum`](https://github.com/ai-startup-curriculum/startup-operations-governance-curriculum) |
| "What is a SAFE and how does it convert?" | [`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum) |
| "How do I read a term sheet / negotiate valuation?" | [`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum) |
| "How do I size an option pool / refresh it at a round?" | [`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum) |
| "How do I build a bottom-up financial model?" | [`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum) |
| "What is my runway right now, and how do I calculate it?" | Foundations mod-005 (founder-slice) then [`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum) for depth |
| "How do I model CAC / LTV / payback for my business?" | [`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum) |
| "How do I allocate capital across product vs GTM vs hires?" | [`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum) |
| "How do I run an M&A / IPO / secondary process?" | [`startup-exit-curriculum`](https://github.com/ai-startup-curriculum/startup-exit-curriculum) |
| "How does a CEO / CTO / CPO curriculum sequence these?" | The relevant role pathway: [`founder-ceo-curriculum`](https://github.com/ai-startup-curriculum/founder-ceo-curriculum), [`cto-curriculum`](https://github.com/ai-startup-curriculum/cto-curriculum), [`cpo-curriculum`](https://github.com/ai-startup-curriculum/cpo-curriculum) |

## Why the rule matters — three failure modes it prevents

The ownership rule is not administrative tidiness. It prevents three
concrete failure modes that any large curriculum accumulates over time.

**1. Duplication decay.** Without ownership, the same topic gets taught in
three different repos slightly differently. Learners either read all three
and get confused, or they pick one and miss updates the other two get.
The ownership rule says: exactly one authoritative treatment, referenced
from everywhere it is needed.

**2. Depth-vs-position confusion.** Without ownership, curricula either
skip depth entirely ("we'll cover cap tables in a later module that
never gets written") or drown in depth in the wrong place ("here are 40
pages on SAFE mechanics in the middle of a customer-discovery
lecture"). The ownership rule pushes depth to its right home and lets
Foundations be genuinely concise.

**3. Update lag.** When SAFEs change (as YC's did in 2018 from pre-money
to post-money), the update has to happen in exactly one place. Under
ownership, that place is the finance pillar. Everything else points to
it and inherits the update for free.

## The deferral formula

Every time Foundations mentions a node whose depth is elsewhere, it uses
a consistent formula that the exercises will make you practise:

> "`<Node>` — position on the graph, brief description of what the node
> is, and hand-off. **Depth lives in `<owning repo>`.** Foundations does
> not go further; do not go read the deep material until it is
> stage-appropriate for your work."

The formula does three jobs at once — names the node, gives just enough
context, and *tells you where to stop*. That last part is the discipline
Foundations is training. Depth is available, one repo away, at a click;
Foundations' job is to make sure you don't visit the depth before your
work needs it.

## Foundations' three exceptions to the ownership rule

Foundations does teach a small amount of depth in a few narrow slices,
because those slices are what make Foundations *practical* rather than
purely descriptive:

1. **Runway / burn / growth-rate / default-alive-or-default-dead
   (mod-005).** Enough founder-numbers depth to instrument the search in
   the first two rounds.
2. **Founder operating loop and weekly cadence (mod-004).** Enough
   process depth to run a real week, including the decision log, the
   Monday plan / Friday shipped-and-learned rhythm, the first
   investor-update template, and the light OKR shape.
3. **The graph itself (this module).** The map is *the* Foundations
   artifact; everyone else references it.

Everything outside those three slices is deferred. When in doubt about
whether Foundations should teach something to depth, apply the rule:
*does the founder need this to survive the first two rounds?* If yes,
Foundations' slice covers it. If no, defer.

## Summary

- The ownership table maps every node on the graph to exactly one owning
  pillar repo. Learn it well enough to name the repo in under ten
  seconds for any node.
- Runway (and the founder-numbers vocabulary) is the one node with a
  Foundations *slice* and a finance-pillar *depth*; the split is
  deliberate and follows the survive-first-two-rounds rule.
- The founder-question lookup table is the practical form of the
  ownership rule — question in, repo out.
- The ownership rule prevents duplication decay, depth-vs-position
  confusion, and update lag.
- The deferral formula (`<node>: position + brief + "depth in <repo>"`)
  is used everywhere in Foundations; the exercises will make you
  practise it against real nodes.

## Homework

Exercise 06 (`Owning-Repo Lookup Drill`) is a timed lookup drill against
a mixed list of founder questions and artifacts. If you cannot beat the
target time, re-read the ownership table until you can.
