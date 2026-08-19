# The Corporate-Structure Branch

## Motivation

The customer-facing branch decides whether the company has a business worth
having. The corporate-structure branch decides whether the *container* holding
that business is one investors, employees, and acquirers can operate inside of.

Founders under-invest in this branch because it feels administrative — legal
paperwork, cap-table lines, board mechanics, term sheets — none of which
directly builds product. The consequence, seen across many failed and
almost-failed startups, is that a working business is trapped inside a broken
container: cap tables that can't take the next round, governance structures
that can't approve a strategic decision, incorporation choices that block a
lead investor from participating at all. The container failures are usually
fixable early and expensive-to-impossible to fix late.

This chapter walks the corporate-structure branch — Incorporation → Equity /
Governance / Fundraising → Exit — and names, for each node, what it produces,
what it gates downstream, and why the equity structure and the governance
structure in particular gate every future round.

## The branch, drawn as a fan-out

Unlike the customer-facing branch, the corporate-structure branch fans out
from a single starting node into three parallel workstreams that eventually
converge again at Exit:

```
                  ┌──► Equity ─────────────┐
                  │                        │
Incorporation ────┼──► Governance ─────────┼──► Exit
                  │                        │
                  └──► Fundraising ────────┘
```

`Incorporation` gates all three downstream nodes — you cannot issue equity,
form a board, or take outside capital before you exist as a legal entity.
`Equity` and `Governance` gate `Fundraising` at every round in a way most
founders discover the first time they try to raise. `Exit` is the convergent
endpoint from all three.

Depth for this whole branch is split across two pillar curricula:
[`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum)
owns Equity and Fundraising;
[`startup-operations-governance-curriculum`](https://github.com/ai-startup-curriculum/startup-operations-governance-curriculum)
owns Incorporation and Governance.

## Node 1 — Incorporation

**What it is.** The choice of legal entity, jurisdiction, and founder-agreement
structure the company is formed into. In the U.S. venture context this is
typically a **Delaware C-corporation** because the legal precedent, tax
treatment, and investor familiarity make every downstream step easier — but
LLCs, S-corps, PBCs, and non-U.S. structures are all real choices with real
trade-offs.

<!-- needs-research: verify that Delaware C-corp remains the market-default recommendation of the top three startup-focused law firms (Cooley, Gunderson, Wilson Sonsini) and cite each firm's public guidance page. -->

**What it produces.** A registered legal entity with a name, a state of
incorporation, founding stock issued to the founders under a stock-purchase
agreement, an EIN, a bank account the entity (not the founders personally)
owns, and a founder-agreement structure covering IP assignment, vesting,
and role definition.

**What downstream needs from it.** Every other node on this branch needs the
entity to exist. Equity cannot be issued into a non-entity; Governance requires
a board that must be a board *of* something; Fundraising requires the round
to close *into* an entity investors can wire money to.

**Why the choice matters gate-wise.** The most common expensive mistake at
this node is choosing a structure that later has to be converted — for example,
starting as an LLC and later converting to a C-corp because a lead investor
requires it. Conversions cost real money, real time, and real legal fees, and
they usually happen at the worst possible moment (mid-fundraise, mid-hire).

**Owner curriculum.**
[`startup-operations-governance-curriculum`](https://github.com/ai-startup-curriculum/startup-operations-governance-curriculum)
owns the depth — entity comparison, jurisdiction choice, founder agreements,
IP assignment, initial 83(b) elections, and the "get your legal house in
order before you raise" playbook.

## Node 2 — Equity

**What it is.** The structure of ownership of the company — the cap table.
Equity covers founder stock, common stock, preferred stock (issued in priced
rounds), option pools (for employees), convertible instruments (SAFEs, notes),
warrants, and the mechanics of dilution when new shares are issued.

**What it produces.** A cap table document (increasingly maintained in
software — Carta, Pulley, LTSE Equity, Shareworks) recording who owns what
and under what terms, plus the underlying agreements that legally back each
line (stock-purchase agreements, option grants, SAFE documents, priced-round
purchase agreements).

<!-- needs-research: verify the current list of the most-used cap-table software providers among venture-backed U.S. startups; cite the Carta State of Private Markets or an equivalent primary source, and update the vendor list here based on current data. -->

**What downstream needs from it.** Every future round of Fundraising modifies
the cap table. A cap table that is clean, current, and legally sound makes
the next round mechanical. A cap table that is confused (missing agreements,
disputed founder splits, unassigned IP, over-issued options) makes the next
round expensive — sometimes impossible.

**Why the equity structure gates every future round.** Investors will not
close a round on top of a broken cap table. During diligence they inspect
every line — every SAFE with unusual terms, every option grant that missed
board approval, every founder-share vesting schedule, every promise of stock
made informally. Every irregularity is a red flag; a critical mass of them
kills the round. This is why "clean cap table hygiene from day one" is one
of the most-repeated pieces of advice in early-stage founder writing — the
cost of fixing it later is orders of magnitude greater than the cost of
doing it right now.

The **option pool** is a specific case worth naming. Priced rounds typically
require the option pool to be sized to some target percent of post-money
before the investment closes, which means the *dilution* from the pool
refresh falls on the *pre-round* cap table (founders and existing investors)
rather than the new investor. Founders who don't know this in advance
discover it during term-sheet negotiation, when the dilution is largest.

<!-- needs-research: pull a citation for a current market-typical post-money option-pool size at Series A (frequently discussed but the exact percentage varies by market cycle); avoid quoting a specific percentage in learner-facing content until sourced. -->

**Owner curriculum.**
[`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum)
owns the depth — SAFEs (YC's post-money and pre-money variants, and the
whole family of convertible notes), cap-table mechanics, dilution math,
option-pool sizing, 409A valuations, founder vesting.

## Node 3 — Governance

**What it is.** The structure of decision-making authority in the company —
who can approve what, in what forum, with what quorum, with what documented
record. Governance covers the **board of directors** (composition, seats,
observer rights), the **board-consent matrix** (which decisions require
board approval versus founder / officer authority), and the **protective
provisions** in shareholder agreements (which decisions require investor
consent regardless of the board).

**What it produces.** Board composition documented in the corporate records;
board minutes and consents for material decisions; a shareholder agreement
containing the protective-provision matrix; and a running discipline of
"which decision routes to which forum" that scales from a two-founder
company to a many-stakeholder board.

**What downstream needs from it.** Fundraising rounds — especially priced
rounds from Series A onward — carve out **new board seats** and **new
protective provisions** for the incoming investor. Every subsequent round
inherits, modifies, and adds to the governance structure. A governance
structure that is already tangled (undocumented decisions, missing
consents, unclear board authority) is one an incoming investor demands be
cleaned up as a closing condition — again, at the worst possible moment.

**Why the governance structure gates every future round.** Two mechanisms:

1. **Diligence.** Institutional investors demand the corporate records —
   minutes, consents, actions taken. Missing or contradictory records slow
   diligence to a crawl and, in the pathological case, kill the round.
2. **Structural fit.** Investors often require specific governance shapes
   as a condition of investing — e.g., a specific board size, a specific
   set of protective provisions, a specific composition (X investor seats,
   Y independent seats, Z founder seats). Structures that cannot cleanly
   accommodate the demand require restructuring, which itself requires
   consent from existing stakeholders, which can fail.

**Governance also gates Exit.** An M&A transaction or an IPO requires a
board that can approve it under the applicable standard of care (fiduciary
duty to shareholders under the Revlon and related doctrines in Delaware),
with proper process, documentation, and — often — an independent-committee
review. A governance structure that has been treated as an afterthought
for six years cannot suddenly produce a defensible Revlon-standard sale
process. This is why the graph draws the Exit endpoint from Governance
explicitly.

<!-- needs-research: pull a citation for a plain-English primer on the Revlon duty and its applicability to startup M&A transactions (Wilson Sonsini and Cooley both publish accessible summaries); add the URL in resources.md. -->

**Owner curriculum.**
[`startup-operations-governance-curriculum`](https://github.com/ai-startup-curriculum/startup-operations-governance-curriculum)
owns the depth — board formation, board-pack authoring, consent matrices,
fiduciary duty, D&O insurance, protective-provision negotiation.

## Node 4 — Fundraising

**What it is.** The process of raising outside capital — angels, pre-seed,
seed, Series A, and beyond. Fundraising covers the *instruments* (SAFEs,
notes, priced rounds), the *process* (list-building, pitching, term-sheet
negotiation, diligence, closing), and the *strategy* (how much to raise,
at what valuation, from whom, with what strings).

**What it produces.** Capital on the balance sheet — which becomes Runway
(chapter 04) — plus a new set of stakeholders on the cap table (Equity)
and typically new terms in the governance structure (Governance). The
round also produces the founder's next N months of accountability: the
milestones the round was raised against.

**What downstream needs from it.** Nothing else on the corporate-structure
branch strictly needs Fundraising; a bootstrapped company can complete the
whole branch without it. But the *economics branch* — specifically
`Runway` and `Capital Allocation` — depends on Fundraising directly, and
`Exit` depends on Fundraising indirectly through the preference stack
that gets built as rounds accumulate.

**Why the round gate matters.** Every round is a gate at which the whole
corporate-structure branch is inspected. Equity has to be clean. Governance
has to be clean. Incorporation has to be the right shape for the incoming
investor. Any node upstream that has been neglected surfaces here, in
diligence, in the term sheet, and in the closing conditions.

The Y Combinator SAFE — introduced in 2013 and revised to a post-money
form in 2018 — is the market-standard early convertible instrument used by
most pre-seed rounds. Priced Series A rounds use the NVCA (National Venture
Capital Association) model documents as the industry-standard starting
point. Foundations names both because they are the vocabulary you will hear
from investors; depth on how they actually work lives in the pillar
curriculum.

<!-- needs-research: verify the current version of the Y Combinator SAFE document and cite the primary source at ycombinator.com/documents. Verify current NVCA model-documents landing page and cite. -->

**Owner curriculum.**
[`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum)
owns the depth — round mechanics, valuation, investor targeting, pitch
narratives (the ones mod-004 introduces in the Sequoia shape), term-sheet
reading, diligence checklists, closing.

## The gating story, retold in one paragraph

The reason "the equity structure and the governance structure gate every
future round" is not a legal formality — it is a diligence reality. Every
priced round is a full inspection of the cap table and the corporate
records. Anything not clean surfaces there, requires fixing under time
pressure, and can kill the round. This is why founder writing on
corporate structure sounds so much more paranoid than it looks like it
should — because the people writing it have watched the round die from
under a preventable problem, and they are trying to save the next founder
from the same fate.

## The specific back-edge from Exit

The main graph shows Exit as an endpoint from Governance (and from Growth
on the customer-facing branch). There is also a *back-edge* from Exit to
Equity that shows up at closing: the **liquidation-preference stack** —
which preferred shareholders get paid what before common shareholders see
anything — is defined at each round in Equity terms but *resolves* at
Exit. A cap table that looked fine at each round can produce a nasty
common-shareholder outcome at Exit if the preference stack was allowed to
grow uncritically. This is another reason cap-table hygiene at Equity
matters even before Exit is imaginable.

<!-- needs-research: cite a plain-English primer on liquidation preferences (1x non-participating vs 1x participating vs multiple-x) and preference-stack behavior at exit. -->

## Coupling to the other branches

Two edges into other branches you will meet again in chapter 05:

- **Fundraising ► Runway (economics branch).** Every round is a
  step-change in cash and therefore a step-change in Runway. mod-005
  makes this the core of the runway model.
- **Governance ► Capital Allocation (economics branch).** Large capital
  decisions (acquisitions, big hires, geographic expansion) usually
  require board approval under the consent matrix. Governance shapes
  are literal constraints on what capital-allocation choices are
  available.

## Summary

- The branch fans out from Incorporation into three parallel workstreams
  — Equity, Governance, Fundraising — which converge at Exit.
- Incorporation gates all three downstream nodes; skipping it or
  choosing wrong forces later conversions at the worst possible time.
- Equity and Governance gate every future round through diligence. Clean
  cap-table hygiene and disciplined corporate records are the two
  cheapest, highest-leverage investments a founder can make early.
- Fundraising is a repeated event that inspects the whole corporate
  branch each time it occurs. The health of the round is the health of
  the container.
- Depth lives in two pillar curricula:
  [`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum)
  (Equity, Fundraising) and
  [`startup-operations-governance-curriculum`](https://github.com/ai-startup-curriculum/startup-operations-governance-curriculum)
  (Incorporation, Governance).

## Homework

Exercise 02 (`Graph Tour — Corporate-Structure Branch`) walks the branch
as a series of "what breaks if this upstream node is neglected?" drills.
Do it after this chapter and before moving on to chapter 04.
