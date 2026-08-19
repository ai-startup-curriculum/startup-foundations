# Job Requirements — Startup Foundations

**Role level:** 10 (foundational shared root — Startup family)
**Track:** `startup-foundations`
**Research window:** 2026-05-21 → 2026-08-19 (last 90 days)
**Today:** 2026-08-19
**Live postings sampled this cycle:** 0 — see *Status* below

This file documents the requirements catalog used to seed the Startup Foundations curriculum. Raw normalised data lives in [`.aicg/job-requirements.json`](.aicg/job-requirements.json); the planned curriculum lives in [`.aicg/curriculum-plan.json`](.aicg/curriculum-plan.json).

## Status — bootstrap session, live postings deferred

Startup Foundations is the **shared root** of the ai-startup-curriculum org, not a hireable job title on its own. Every downstream functional pillar (`startup-product-gtm-curriculum`, `startup-finance-fundraising-curriculum`, `startup-operations-governance-curriculum`, `startup-exit-curriculum`) and every role pathway (`founder-ceo-curriculum`, `cto-curriculum`, `cpo-curriculum`) inherits this curriculum at 100%. The closest hireable equivalents in the market — where a live posting-frequency signal exists — are **Founder in Residence** (YC / Antler / EF / South Park Commons / venture-studio programs), **Founding Engineer / Founding Team** postings at pre-seed companies, **Chief of Staff to Founder/CEO** at pre-Series-A companies, **EIR / Entrepreneur in Residence** at accelerators and funds, and **Startup Studio Venture Lead** / accelerator program-manager postings. Those will backfill the `postings[]` array in [`.aicg/job-requirements.json`](.aicg/job-requirements.json) on the first live research cycle.

In this bootstrap cycle the required WebSearch / WebFetch tools were not granted, so the 25-in-window posting sample could not be pulled. The `postings` array is empty by design and every `requirement_themes[].frequency` is recorded as `"needs-research"` until the live cycle backfills it. This document instead grounds the requirements catalog in **authoritative public references** that publish what an early-stage founder is expected to know at the *foundations* level:

- **Practitioner canon (essays and books)** — [Y Combinator Startup School](https://www.startupschool.org/), the [Y Combinator Library](https://www.ycombinator.com/library), the [Paul Graham essays](https://paulgraham.com/articles.html) (in particular ['Startup = Growth'](https://paulgraham.com/growth.html), ['Default Alive or Default Dead'](https://paulgraham.com/aord.html), ['Do Things That Don't Scale'](https://paulgraham.com/ds.html), ['The 18 Mistakes That Kill Startups'](https://paulgraham.com/startupmistakes.html)), [Steve Blank — *The Four Steps to the Epiphany*](https://web.stanford.edu/group/e145/cgi-bin/spring/upload/handouts/Four_Steps.pdf), [*The Startup Owner's Manual* companion overview](https://steveblank.com/2020/03/03/the-startup-owners-manual-1-a-step-by-step-guide-for-building-a-successful-company/), [Eric Ries — *The Lean Startup* principles](http://theleanstartup.com/principles), [Ash Maurya — Running Lean & Lean Canvas](https://leanstack.com/lean-canvas), [Alexander Osterwalder — Business Model Canvas](https://www.strategyzer.com/library/the-business-model-canvas), and [First Round Review](https://review.firstround.com/).
- **Investor / VC canon** — [Sequoia Capital — Writing a Business Plan](https://articles.sequoiacap.com/writing-a-business-plan), the [Y Combinator SAFE documents and user guide](https://www.ycombinator.com/documents), the [NVCA Model Legal Documents](https://nvca.org/model-legal-documents/), and [Brad Feld & Jason Mendelson — *Venture Deals* companion articles](https://www.feld.com/archives/category/venture-capital/venture-deals-book).
- **Founder-numbers reference** — [Corporate Finance Institute — Startup Finance](https://corporatefinanceinstitute.com/resources/knowledge/finance/startup/), [David Skok — SaaS Metrics 2.0](https://www.forentrepreneurs.com/saas-metrics-2/), and [Sean Ellis / Amplitude — The North Star Metric](https://amplitude.com/blog/product-north-star-metric).
- **Empirical failure evidence** — [CB Insights — Top Reasons Startups Fail](https://www.cbinsights.com/research/startup-failure-reasons-top/), the [Founder Collective mortemas](https://foundercollective.com/mortemas/), and the [Startup Genome Report](https://startupgenome.com/reports) on premature scaling.
- **Neutral government reference** — the [US Small Business Administration — Starting a Business](https://www.sba.gov/business-guide/plan-your-business/write-your-business-plan) guide.

Every requirement below cites at least one such reference, and every requirement is shaped so posting-frequency evidence can be added underneath it without restructure.

## Methodology

1. Sourced the canonical founder-facing task domains at the *foundations* level from the public references catalogued in [`.aicg/job-requirements.json`](.aicg/job-requirements.json) `authoritative_references` — the practitioner canon (Paul Graham, Steve Blank, Eric Ries, Ash Maurya, First Round Review), the investor / VC canon (Sequoia, YC SAFE, NVCA, *Venture Deals*), and the founder-numbers references (Corporate Finance Institute, David Skok, North-Star Metric).
2. Anchored each task domain against the three-axis model already declared in [`README.md`](README.md), the pillar / owning-repo table in [`FUNCTIONAL_CURRICULA.md`](FUNCTIONAL_CURRICULA.md), and the stage ladder in [`STARTUP_STAGES.md`](STARTUP_STAGES.md) — so every module in the catalog has (a) a pillar, (b) a stage tag, and (c) an owning repo that is either this one (for a Foundations-level slice) or a functional pillar / role-pathway repo (for depth).
3. Applied the **ownership rule** — Foundations owns the *system*, the *graph*, the *stages*, the founder's core operating loop, and the founder-numbers slice (runway, burn, growth, default-alive / default-dead, North-Star). Everything deeper defers *up*:
   - *Up* to [`startup-product-gtm-curriculum`](https://github.com/ai-startup-curriculum/startup-product-gtm-curriculum) (level 20) for customer-discovery, PMF, GTM, sales, and growth depth.
   - *Up* to [`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum) (level 20) for financial-modelling, unit-economics, capital-allocation, fundraising (angel → pre-seed → seed → Series A), and equity (SAFEs, cap tables, option pools, dilution) depth.
   - *Up* to [`startup-operations-governance-curriculum`](https://github.com/ai-startup-curriculum/startup-operations-governance-curriculum) (level 25) for people (hiring, comp, management, culture, firing), legal (incorporation, contracts, IP, employment), operations (corporate ops, vendors, processes, metrics, systems), and governance (boards, fiduciary duty, controls, risk) depth.
   - *Up* to [`startup-exit-curriculum`](https://github.com/ai-startup-curriculum/startup-exit-curriculum) (level 40) for M&A, secondaries, IPOs, succession, and shutdown depth.
   - *Sideways* to the role-pathway repos ([`founder-ceo-curriculum`](https://github.com/ai-startup-curriculum/founder-ceo-curriculum), [`cto-curriculum`](https://github.com/ai-startup-curriculum/cto-curriculum), [`cpo-curriculum`](https://github.com/ai-startup-curriculum/cpo-curriculum)) that inherit Foundations at 100% and add role-specific curated views.
4. Flagged every theme's frequency as `needs-research` so the first live research cycle can populate the number without restructuring the catalog.

## Requirement themes → curriculum ownership

The table below lists each requirement theme, its posting frequency this cycle (all `needs-research` — see *Status* above), its planned owner per the level hierarchy, and the curriculum coverage path.

| # | Theme | Freq | Owner track | Coverage |
|---|---|---|---|---|
| 1 | Explain a startup as a system — a temporary organisation searching for a repeatable and scalable business model under uncertainty; distinguish it from a small business, a project, a lifestyle business, and a research program | <!-- needs-research --> | `startup-foundations` (this) | [`mod-001-how-startups-work`](lessons/mod-001-how-startups-work) |
| 2 | Place any 'business thing' on the dependency graph — Customer Discovery → PMF → GTM → Sales → Growth; Corporate Structure → Equity / Governance / Fundraising; Economics → Financial Modeling / Runway / Unit Economics / Capital Allocation — and know what depends on what | <!-- needs-research --> | `startup-foundations` | [`mod-002-the-dependency-graph`](lessons/mod-002-the-dependency-graph) |
| 3 | Map activities to startup stages (IDEA → PRE-SEED → SEED → SERIES-A → GROWTH → MATURE) and know what to ignore at your stage; diagnose stage-mismatched activity as a failure mode | <!-- needs-research --> | `startup-foundations` | [`mod-003-stages-and-what-matters-when`](lessons/mod-003-stages-and-what-matters-when) |
| 4 | Run the founder's core operating loop — decide → allocate → communicate → measure; ship a weekly cadence, a decision log, a lightweight OKR / commit-and-review shape, a first investor-update template, and a Sequoia-shape founder-narrative | <!-- needs-research --> | `startup-foundations` | [`mod-004-founder-operating-basics`](lessons/mod-004-founder-operating-basics) |
| 5 | Read the three founder numbers — runway, burn, growth — and their derived views (gross vs. net burn, WoW / MoM growth, default alive / default dead, North-Star metric, CAC / LTV / payback / gross-margin vocabulary) well enough to make weekly capital + attention allocation calls | <!-- needs-research --> | `startup-foundations` | [`mod-005-reading-the-numbers`](lessons/mod-005-reading-the-numbers) |
| 6 | Customer discovery, PMF, GTM, sales, and growth *depth* — Foundations names the pillar and its position on the graph; depth lives in `startup-product-gtm-curriculum` (level 20) | <!-- needs-research --> | `startup-product-gtm-curriculum` | Linked out (mod-002 places the pillar on the graph) |
| 7 | Financial modelling, unit economics, capital allocation, fundraising, and equity (SAFEs / cap tables / option pools / dilution) *depth* — Foundations covers the founder-numbers slice; depth lives in `startup-finance-fundraising-curriculum` (level 20) | <!-- needs-research --> | `startup-finance-fundraising-curriculum` | Linked out (mod-002 and mod-005 name the pillar and the vocabulary) |
| 8 | People (hiring, comp, management, culture, firing), legal (incorporation, contracts, IP, employment), operations, and governance (boards, fiduciary duty, controls, risk) *depth* — Foundations introduces the founder-operating loop; depth lives in `startup-operations-governance-curriculum` (level 25) | <!-- needs-research --> | `startup-operations-governance-curriculum` | Linked out (mod-004 hands off) |
| 9 | Exit and endgame (M&A, secondaries, IPO, succession, shutdown) *depth* — Foundations only names Exit as an endpoint on the graph; actionable only at MATURE; depth lives in `startup-exit-curriculum` (level 40) | <!-- needs-research --> | `startup-exit-curriculum` | Linked out (mod-002 names the endpoint) |
| 10 | Role-pathway inheritance — every role pathway (`founder-ceo-curriculum`, `cto-curriculum`, `cpo-curriculum`) targets 100% Foundations coverage and *references* this curriculum rather than re-authoring it | <!-- needs-research --> | `startup-foundations` (this — enforces the rule) | Threaded through every module; documented in [`CURRICULUM.md`](CURRICULUM.md) |

## Emerging themes — below curriculum threshold this cycle

None captured this cycle. The scaffold pass does not sample live postings and therefore does not produce below-threshold signal. The first live research cycle will populate `emerging_themes_below_threshold` in [`.aicg/job-requirements.json`](.aicg/job-requirements.json) once postings backfill.

## Posting evidence

0 in-window postings sampled 2026-05-21 → 2026-08-19 (scaffold cycle — WebSearch / WebFetch not granted). See [`.aicg/job-requirements.json`](.aicg/job-requirements.json) `research_status.needs_research_note` for the exact sampling contract the next cycle should honour, and this document's *Status* section for the equivalent-title bucket the next cycle should draw from.

<!-- needs-research: backfill 25+ live in-window postings on the first cycle where WebSearch / WebFetch is exercised — fan out across YC / Techstars / Antler / EF / South Park Commons founder-in-residence & founding-team programs, venture-studio job boards (Atomic, Human Ventures, AlleyCorp), accelerator program-manager postings, and 'Chief of Staff, CEO/Founder' postings at pre-Series-A companies. Filter out senior operator postings that assume PMF and hire for scale-up execution — those defer up to startup-operations-governance-curriculum / founder-ceo-curriculum. -->

## Ownership map — quick reference for the next cycle

When backfilling postings, use this ownership decision to keep Foundations from drifting into pillar or role-pathway territory:

- **Startup Foundations** (this repo, level 10) — owns the *system*, the *graph*, the *stages*, the founder's core operating loop, and the founder-numbers slice (runway, burn, growth read, default alive / default dead call, North-Star metric selection). *Every downstream pillar and role pathway inherits Foundations at 100% — never a copy-paste fork.*
- **Startup Product & GTM** (`startup-product-gtm-curriculum`, level 20) — customer-discovery, PMF, GTM strategy, sales, growth.
- **Startup Finance & Fundraising** (`startup-finance-fundraising-curriculum`, level 20) — financial modelling, unit economics, capital allocation, fundraising, equity.
- **Startup Operations & Governance** (`startup-operations-governance-curriculum`, level 25) — people, legal, operations, governance.
- **Startup Exit & Endgame** (`startup-exit-curriculum`, level 40) — M&A, secondaries, IPO, succession, shutdown; MATURE-stage only.
- **Founder / CEO** (`founder-ceo-curriculum`, level 30) — role pathway targeting Foundations 100%, Strategy 100%, plus curated slices of every other pillar.
- **CTO** (`cto-curriculum`, level 35) — role pathway targeting Foundations 100%, Technical Leadership 100%, plus curated slices.
- **CPO** (`cpo-curriculum`, level 30) — role pathway targeting Foundations 100%, Product 100%, plus curated slices.

## Salary evidence

Not gathered this cycle — Foundations is a curriculum root, not a hireable job title. On the first live cycle, the salary summary should aggregate published US ranges **per equivalent-title bucket** (Founder in Residence; Founding Engineer / Founding Team; Chief of Staff to Founder/CEO; EIR; Venture Studio Lead / accelerator program manager) rather than as a single headline aggregate, and should not quote any range until the strict per-bucket sample clears n≥8 with salary present. See [`.aicg/job-requirements.json`](.aicg/job-requirements.json) `salary_summary` for the machine-readable placeholder.
