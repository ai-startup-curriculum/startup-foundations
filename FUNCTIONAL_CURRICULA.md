# Functional Curricula & Dependency Graph

The **functional axis** of the three-axis model: the deep bodies of knowledge,
authored once and referenced by every role pathway. This file is the canonical
map — the pillars, how they depend on each other, and which repo owns each.

## The dependency graph

You don't learn startups as a flat list of facts; you learn the architecture that
connects them. Study in dependency order:

```
STARTUP FOUNDATIONS  (this repo — the shared root)
        │
        ├──► Customer Discovery
        │         │
        │         ▼
        │    Product-Market Fit
        │         │
        │         ▼
        │    GTM Strategy ──► Sales ──► Growth
        │
        ├──► Corporate Structure
        │         ├──► Equity
        │         ├──► Governance
        │         └──► Fundraising
        │
        └──► Startup Economics
                  ├──► Financial Modeling
                  ├──► Runway
                  ├──► Unit Economics
                  └──► Capital Allocation
```

## The pillars and where they live

| Pillar | What it covers | Owning repo |
|---|---|---|
| **Foundations** | How a startup works as a system; the graph itself | `startup-foundations` (this repo) |
| **Strategy** | Vision, positioning, capital/attention/people allocation | `founder-ceo-curriculum` |
| **Product** | Discovery, PMF, prioritization, product management | `startup-product-gtm-curriculum` |
| **GTM / Sales / Marketing** | Positioning, demand gen, founder-led sales, growth | `startup-product-gtm-curriculum` |
| **Finance** | Financial modeling, runway, unit economics, capital allocation | `startup-finance-fundraising-curriculum` |
| **Fundraising** | Angels → pre-seed → seed → Series A; mechanics & strategy | `startup-finance-fundraising-curriculum` |
| **Equity** | SAFEs, cap tables, option pools, dilution | `startup-finance-fundraising-curriculum` |
| **People** | Hiring, comp & equity, management, culture, firing | `startup-operations-governance-curriculum` |
| **Legal** | Incorporation, contracts, IP, employment basics | `startup-operations-governance-curriculum` |
| **Operations** | Corporate ops, vendors, processes, metrics, systems | `startup-operations-governance-curriculum` |
| **Governance** | Boards, fiduciary duty, controls, risk, accountability | `startup-operations-governance-curriculum` |
| **Technical Leadership** | Turning technology into a scalable company capability | `founder-ceo-curriculum` (CTO pathway) |

> **Reuse over duplication.** A module lives in exactly one owning repo. Role
> pathways *reference* it (with a target coverage %) rather than re-authoring it.
> As a pillar's material outgrows a bundle repo, it graduates into its own repo
> and the references update — never a copy-paste fork.

## Role pathways over the pillars

Each role repo's `CURRICULUM.md` declares target coverage. Starter pathways:

| Pillar | Founder/CEO | CTO* | Product & GTM | Finance & Fundraising | Ops & Governance |
|---|----|----|----|----|----|
| Foundations | 100% | 100% | 100% | 100% | 100% |
| Strategy | 100% | 40% | 60% | 40% | 40% |
| Product | 60% | 70% | 100% | 20% | 20% |
| GTM / Sales / Marketing | 60% | 30% | 100% | 20% | 30% |
| Finance | 80% | 30% | 30% | 100% | 50% |
| Fundraising / Equity | 80% | 20% | 20% | 100% | 40% |
| People | 80% | 70% | 40% | 30% | 80% |
| Legal | 50% | 20% | 20% | 40% | 100% |
| Governance | 80% | 30% | 20% | 40% | 100% |
| Technical Leadership | 20% | 100% | 30% | 10% | 20% |

\* The CTO pathway is authored inside `founder-ceo-curriculum` until it outgrows
it and graduates to its own `cto-curriculum` repo.

---

<!-- aicg:maintained-by -->
Maintained by [VeriSwarm.ai](https://veriswarm.ai)
