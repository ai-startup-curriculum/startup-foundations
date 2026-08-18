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

*Exit / Endgame* (M&A, secondaries, IPO, succession, shutdown) sits at the far
end of the graph — it draws on Growth, Governance, Finance, and Equity, and only
becomes actionable at the later stages.

## The pillars and where they live

| Pillar | What it covers | Owning repo |
|---|---|---|
| **Foundations** | How a startup works as a system; the graph itself | `startup-foundations` (this repo) |
| **Strategy** | Vision, positioning, capital/attention/people allocation | `founder-ceo-curriculum` |
| **Product** | Discovery, PMF, prioritization, product management | `cpo-curriculum` |
| **GTM / Sales / Marketing** | Positioning, demand gen, founder-led sales, growth | `startup-product-gtm-curriculum` |
| **Finance** | Financial modeling, runway, unit economics, capital allocation | `startup-finance-fundraising-curriculum` |
| **Fundraising** | Angels → pre-seed → seed → Series A; mechanics & strategy | `startup-finance-fundraising-curriculum` |
| **Equity** | SAFEs, cap tables, option pools, dilution | `startup-finance-fundraising-curriculum` |
| **People** | Hiring, comp & equity, management, culture, firing | `startup-operations-governance-curriculum` |
| **Legal** | Incorporation, contracts, IP, employment basics | `startup-operations-governance-curriculum` |
| **Operations** | Corporate ops, vendors, processes, metrics, systems | `startup-operations-governance-curriculum` |
| **Governance** | Boards, fiduciary duty, controls, risk, accountability | `startup-operations-governance-curriculum` |
| **Technical Leadership** | Turning technology into a scalable company capability | `cto-curriculum` |
| **Exit & Endgame** | M&A, secondaries, IPOs, succession, shutdowns | `startup-exit-curriculum` |

> **Reuse over duplication.** A module lives in exactly one owning repo. Role
> pathways *reference* it (with a target coverage %) rather than re-authoring it.
> As a pillar's material outgrows a bundle repo, it graduates into its own repo
> and the references update — never a copy-paste fork.

## Repos: functional curricula vs. role pathways

The org has two kinds of repo, both built on this graph:

- **Functional / topic curricula** (the bodies of knowledge above):
  `startup-foundations`, `startup-product-gtm-curriculum`,
  `startup-finance-fundraising-curriculum`,
  `startup-operations-governance-curriculum`, `startup-exit-curriculum`.
- **Role pathways** (curated views declaring target coverage, no duplicated
  content): `founder-ceo-curriculum`, `cto-curriculum`, `cpo-curriculum`.

## Role pathways over the pillars

Each role pathway's `CURRICULUM.md` declares target coverage across the pillars:

| Pillar | Founder/CEO | CTO | CPO |
|---|----|----|----|
| Foundations | 100% | 100% | 100% |
| Strategy | 100% | 40% | 60% |
| Product | 60% | 70% | 100% |
| GTM / Sales / Marketing | 60% | 30% | 80% |
| Finance | 80% | 30% | 30% |
| Fundraising / Equity | 80% | 20% | 20% |
| People | 80% | 70% | 50% |
| Legal | 50% | 20% | 20% |
| Governance | 80% | 30% | 20% |
| Technical Leadership | 20% | 100% | 40% |
| Exit & Endgame | 60% | 40% | 30% |

---

<!-- aicg:maintained-by -->
Maintained by [VeriSwarm.ai](https://veriswarm.ai)
