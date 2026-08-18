# Startup Foundations

<!-- aicg:site-banner -->
> 🎓 Part of the free, open-source **AI Career Curriculum** ecosystem — [Infrastructure](https://github.com/ai-infra-curriculum) · [ML Engineering](https://github.com/ml-engineering-curriculum) · [AI Engineering](https://github.com/ai-engineering-curriculum) · [Governance](https://github.com/ai-governance-curriculum) · [Startup](https://github.com/ai-startup-curriculum). Live cohorts &amp; team programs: **[ai-infra-curriculum.github.io](https://ai-infra-curriculum.github.io/)**.
<!-- /aicg:site-banner -->

> **How does a startup actually work as a system?** This is the root of the
> `ai-startup-curriculum` — an open-source startup operating school for technical
> founders. It defines the shared model every other curriculum in the org builds on.

Most founder education is a cloud of disconnected advice organized around authors,
accelerators, and anecdotes. This curriculum applies an engineering mentality
instead: *what does someone in this role need to understand, in what dependency
order, and what should they be able to do afterward?*

## The Three-Axis Model

Startup knowledge is organized on three axes, not one. Everything in this org is
tagged against all three.

### 1. Functional curricula — the bodies of knowledge (authored once)

The deep, reusable subjects. Each can be studied independently, and each lives in
one place so the same lesson (a cap table, a runway model) is never rewritten six
times. See **[FUNCTIONAL_CURRICULA.md](./FUNCTIONAL_CURRICULA.md)** for the full
dependency graph.

```
STARTUP FOUNDATIONS
   ├─► Customer Discovery ─► Product-Market Fit ─► GTM ─► Sales ─► Growth
   ├─► Corporate Structure ─► { Equity · Governance · Fundraising }
   └─► Startup Economics ─► { Financial Modeling · Runway · Unit Economics · Capital Allocation }
```

### 2. Role pathways — curated views over the functional curricula

A role is a *learning path*, not a separate body of knowledge. A CEO isn't one
subject; it's a role sitting on top of several systems. Each role repo declares
target coverage across the functional pillars:

| Pillar | CEO | CTO |
|---|----|----|
| Foundations | 100% | 100% |
| Strategy | 100% | — |
| Product | 60% | 70% |
| GTM / Sales / Marketing | 60% | 30% |
| Finance | 80% | 30% |
| Fundraising | 80% | — |
| People | 80% | 70% |
| Legal | 50% | — |
| Governance | 80% | 30% |
| Technical Leadership | 20% | 100% |

Role repos: **[founder-ceo](https://github.com/ai-startup-curriculum/founder-ceo-curriculum)**
· **[product & GTM](https://github.com/ai-startup-curriculum/startup-product-gtm-curriculum)**
· **[finance & fundraising](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum)**
· **[operations & governance](https://github.com/ai-startup-curriculum/startup-operations-governance-curriculum)**.

### 3. Startup stages — *when* things matter

`IDEA → PRE-SEED → SEED → SERIES-A → GROWTH → MATURE`. Every module is stage-tagged,
so the curriculum can tell you: *you're pre-seed — do these, ignore those.* A
seed-stage founder studying multinational transfer pricing isn't sophistication;
it's distraction. See **[STARTUP_STAGES.md](./STARTUP_STAGES.md)**.

## Learn by Building Real Artifacts

Exercises are founder artifacts, not MBA case-study fluff: cap tables with SAFEs
and option pools, 18-month runway models, investor funnels, board packets,
cost→pricing/margin conversions, customer-concentration crisis plans. Worked
exemplars live in each role repo under `exemplars/`.

## Where to Start

1. Read this file and the two taxonomy docs (stages + functional graph).
2. Pick your **stage** and your **role pathway**.
3. Work the functional modules your pathway calls for, in dependency order.

---

<!-- aicg:maintained-by -->
Maintained by [VeriSwarm.ai](https://veriswarm.ai)
