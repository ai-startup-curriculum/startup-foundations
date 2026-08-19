# Startup Foundations Curriculum

**Role level:** 10 (foundational shared root — Startup family)
**Family:** Startup
**Status:** planned — modules and projects below are the planned scope authored from [`.aicg/curriculum-plan.json`](.aicg/curriculum-plan.json). Lessons and worked exemplars will be drafted by subsequent autonomous content cycles, oldest-gap first.

## Overview

The shared root every role pathway starts from (100% coverage for all roles). Foundations teaches the *system* and the *graph* — the mental model that makes every downstream pillar legible.

The five modules move a founder from a definition (*what is a startup, actually?*) through the dependency graph (*where does any business thing live and what does it depend on?*), the stage axis (*when does each thing matter?*), the operating loop (*how does a founder run a week?*), and the founder-numbers (*what do runway, burn, and growth mean together?*). Total planned commitment: **98 hours across 5 modules** + **85 hours across 3 projects** = **~183 hours**.

## Ownership rule

Following the project-wide ownership rule, this curriculum:

- **Owns** the *system* (what a startup is), the *graph* (the dependency map across customer-facing, corporate-structure, and economics branches), the *stages* (IDEA → PRE-SEED → SEED → SERIES-A → GROWTH → MATURE and what matters at each), the founder's core operating loop (decide → allocate → communicate → measure), and the founder-numbers slice (runway, burn, growth, default alive / default dead, North-Star metric selection).
- **Defers up** to [`startup-product-gtm-curriculum`](https://github.com/ai-startup-curriculum/startup-product-gtm-curriculum) (level 20) for customer-discovery, PMF, GTM, sales, and growth *depth*; to [`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum) (level 20) for financial-modelling, unit-economics, capital-allocation, fundraising, and equity *depth*; to [`startup-operations-governance-curriculum`](https://github.com/ai-startup-curriculum/startup-operations-governance-curriculum) (level 25) for people, legal, operations, and governance *depth*; to [`startup-exit-curriculum`](https://github.com/ai-startup-curriculum/startup-exit-curriculum) (level 40) for M&A, secondaries, IPO, succession, and shutdown *depth*.
- **Defers sideways** to the role-pathway repos ([`founder-ceo-curriculum`](https://github.com/ai-startup-curriculum/founder-ceo-curriculum), [`cto-curriculum`](https://github.com/ai-startup-curriculum/cto-curriculum), [`cpo-curriculum`](https://github.com/ai-startup-curriculum/cpo-curriculum)) that inherit this curriculum at 100% and add role-specific curated views — no fork, no duplication.

See [`JOB_REQUIREMENTS.md`](JOB_REQUIREMENTS.md) for the requirements-to-coverage map and the cited public references the catalog is grounded in. See [`FUNCTIONAL_CURRICULA.md`](FUNCTIONAL_CURRICULA.md) for the full pillar graph and [`STARTUP_STAGES.md`](STARTUP_STAGES.md) for the stage axis and front-matter contract.

## Module Plan

| Module | Stage | Pillar | Hours | Status |
|---|---|---|---|---|
| [`mod-001-how-startups-work`](lessons/mod-001-how-startups-work) | IDEA | foundations | 16 | planned |
| [`mod-002-the-dependency-graph`](lessons/mod-002-the-dependency-graph) | IDEA | foundations | 18 | planned |
| [`mod-003-stages-and-what-matters-when`](lessons/mod-003-stages-and-what-matters-when) | IDEA | foundations | 14 | planned |
| [`mod-004-founder-operating-basics`](lessons/mod-004-founder-operating-basics) | PRE-SEED | foundations | 22 | planned |
| [`mod-005-reading-the-numbers`](lessons/mod-005-reading-the-numbers) | PRE-SEED | economics | 28 | planned |

## Project Plan

| Project | Hours | Status |
|---|---|---|
| [`project-001-map-your-startup-on-the-graph`](projects/project-001-map-your-startup-on-the-graph) | 25 | planned |
| [`project-002-founder-numbers-and-cadence-packet`](projects/project-002-founder-numbers-and-cadence-packet) | 35 | planned |
| [`project-003-two-slide-startup-diagnostic`](projects/project-003-two-slide-startup-diagnostic) | 25 | planned |

Worked founder artifacts (filled cap tables, runway models, investor funnels, pitch narratives) for the projects and module exercises live under [`exemplars/`](exemplars/).

## Module summaries

### mod-001 — How Startups Work
Define a startup precisely — a temporary organisation searching for a repeatable, scalable business model under uncertainty — and distinguish it from a small business, a consulting project, a lifestyle business, and a research program. Read Paul Graham ('Startup = Growth', 'How to Start a Startup', 'The 18 Mistakes That Kill Startups'), Steve Blank (customer development), and Eric Ries (build-measure-learn) as the two operating traditions Foundations sits on top of. Read three canonical failure post-mortems (CB Insights + Founder Collective 'mortemas') and identify which layer of the graph the startup failed on.

### mod-002 — The Dependency Graph
Walk the customer-facing branch (Customer Discovery → PMF → GTM → Sales → Growth → Exit), the corporate-structure branch (Incorporation → Equity → Governance → Fundraising), and the economics branch (Startup Economics → Financial Modeling / Runway / Unit Economics / Capital Allocation). Place a real business artifact (a SAFE, a customer interview note, a runway model, a term sheet, an option-pool refresh, an ICP definition, a CAC / LTV table, a board pack) on the correct node and identify its dependencies. Use the Lean Canvas and Business Model Canvas as two working shapes for the assumption set under a startup.

### mod-003 — Stages and What Matters When
Read the stage ladder (IDEA → PRE-SEED → SEED → SERIES-A → GROWTH → MATURE), the founder's core question at each stage, and the typical focus. Diagnose stage-mismatched activity (a seed founder building a compensation-committee charter, a pre-seed founder studying multinational transfer pricing) and name the correct current focus instead. Read Paul Graham's 'Do Things That Don't Scale' as the canonical IDEA / PRE-SEED reconciliation and the Startup Genome premature-scaling framing as the empirical anchor. Given any candidate activity, decide whether it is stage-appropriate against a checklist.

### mod-004 — Founder Operating Basics
Run the founder's core operating loop — decide, allocate, communicate, measure — as a repeatable weekly cadence. Ship a founder-narrative in the Sequoia shape (company purpose → problem → solution → why now → market size → competition → product → business model → team → financials). Author a lightweight weekly cadence (Monday plan → Friday shipped-and-learned + metrics one-pager), a decision log, a lightweight OKR / commit-and-review shape sized for a 2-3 person startup, and a first investor-update template (highlights / lowlights / asks). Hand off hiring / comp / management depth to `startup-operations-governance-curriculum`, product / GTM operating loops to `startup-product-gtm-curriculum`, and capital-allocation depth to `startup-finance-fundraising-curriculum`.

### mod-005 — Reading the Numbers
Build a working runway model from a starting cash balance and a monthly burn (net cash out). Distinguish gross burn, net burn, and net burn after variable revenue. Read growth as a rate (week-over-week early-stage, month-over-month post-PMF) calibrated against the Paul Graham 5-7% WoW yardstick. Apply the 'Default Alive or Default Dead' composite. Name the four unit-economic terms (CAC, LTV, payback, gross margin) at the vocabulary level. Pick a North-Star metric for a chosen startup and defend the choice against three alternatives. Ship a founder-numbers one-pager readable in 90 seconds. Defer deep financial modelling, sensitivity analysis, capital-allocation frameworks, and full fundraising financial packages to `startup-finance-fundraising-curriculum`.

## Assessment

Each module ships **1 quiz** plus the exercises and labs listed in [`.aicg/curriculum-plan.json`](.aicg/curriculum-plan.json). Each project ships a portfolio-grade README under [`projects/`](projects/), a filled exemplar under [`exemplars/`](exemplars/) (runway model, cadence pack, two-slide diagnostic), and an explicit rubric covering graph-placement accuracy, stage-fit judgement, founder-narrative clarity, decision-log discipline, runway-model correctness, growth-rate calibration, default-alive / default-dead defensibility, and North-Star metric selection.

## Where to go after this curriculum

- **[`startup-product-gtm-curriculum`](https://github.com/ai-startup-curriculum/startup-product-gtm-curriculum)** (level 20) — customer discovery, PMF, GTM, sales, growth depth.
- **[`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum)** (level 20) — financial modelling, unit economics, capital allocation, fundraising, equity depth.
- **[`startup-operations-governance-curriculum`](https://github.com/ai-startup-curriculum/startup-operations-governance-curriculum)** (level 25) — people, legal, operations, governance depth.
- **[`startup-exit-curriculum`](https://github.com/ai-startup-curriculum/startup-exit-curriculum)** (level 40) — M&A, secondaries, IPO, succession, shutdown.
- Role pathways: **[`founder-ceo-curriculum`](https://github.com/ai-startup-curriculum/founder-ceo-curriculum)** (level 30) · **[`cto-curriculum`](https://github.com/ai-startup-curriculum/cto-curriculum)** (level 35) · **[`cpo-curriculum`](https://github.com/ai-startup-curriculum/cpo-curriculum)** (level 30) — inherit Foundations at 100% and add role-specific curated views.

<!-- needs-research: backfill industry-frequency evidence into JOB_REQUIREMENTS.md once the autonomous research loop runs with WebSearch / WebFetch exercised against the equivalent-title postings (Founder in Residence, Founding Engineer, Chief of Staff to Founder/CEO, EIR, Venture Studio Lead); demote any module or exercise whose underlying requirement does not show up across ≥3 in-window postings. -->

---

<!-- aicg:maintained-by -->
Maintained by [VeriSwarm.ai](https://veriswarm.ai)
