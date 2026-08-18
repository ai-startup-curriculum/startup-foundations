# Startup Stages

The **stage axis** of the three-axis model. Every module in the org carries a
`stage:` (or `stages:`) tag in its front-matter drawn from this canonical list.
Stages answer the question education usually skips: *when does this matter?*

```
IDEA ─► PRE-SEED ─► SEED ─► SERIES-A ─► GROWTH ─► MATURE
```

| Stage | Signal you're here | The founder's core question | Typical focus |
|---|---|---|---|
| **IDEA** | No company yet; a hunch and a problem | Is this problem real and worth solving? | Customer discovery, problem/solution framing, first principles |
| **PRE-SEED** | Incorporated or about to be; building v0 | Can I get evidence a solution could work? | Lean modeling, MVP scoping, founder agreements, first capital |
| **SEED** | Early users/revenue; raising a first priced round | Can I find repeatable value and fund the search for PMF? | Runway, founder-led sales, seed fundraising, cap table, first hires |
| **SERIES-A** | PMF signals; metrics a fund will underwrite | Can I turn a working thing into a scalable machine? | Unit economics, GTM engine, org design, board governance |
| **GROWTH** | Repeatable growth; scaling headcount & spend | Can I scale without breaking the company? | Capital allocation, management layers, systems & controls |
| **MATURE** | Durable business; optionality on outcomes | How do I sustain, govern, and steer to an outcome? | Governance, risk, succession, M&A / secondaries / IPO |

## How to use the stage tag

- **As a learner:** filter to your stage first. The curriculum should hand you a
  short, ordered list — not the whole tree.
- **As an author (human or the autonomous pipeline):** tag each module with the
  earliest stage at which it becomes *actionable*, and list later stages where it
  deepens. Do not tag a module to a stage where acting on it is premature.

### Front-matter contract

Each module `README.md` begins with YAML front-matter:

```yaml
---
stage: SEED              # earliest stage this becomes actionable
stages: [SEED, SERIES-A] # optional: all stages where it applies
pillar: fundraising      # functional pillar (see FUNCTIONAL_CURRICULA.md)
requires:                # prerequisite module ids (dependency graph)
  - mod-002-lean-business-modeling
---
```

Markdown front-matter is the source of truth for tags; the curriculum-plan
manifests may mirror them but never override them.

---

<!-- aicg:maintained-by -->
Maintained by [VeriSwarm.ai](https://veriswarm.ai)
