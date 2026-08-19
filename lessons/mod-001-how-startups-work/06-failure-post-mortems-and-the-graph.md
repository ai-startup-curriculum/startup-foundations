# Failure Post-Mortems and the Graph

## Motivation

Reading founder stories about *why we succeeded* is unreliable education —
survivors overweight their own decisions and underweight luck. Failure
post-mortems are the more honest source. Founders who wrote them either lost
the company or watched a company they invested in lose, and had strong
incentive to name the actual cause.

This chapter has one job: teach you to read failure post-mortems in a
particular way — not as cautionary tales, but as **data about which layer of
the dependency graph the startup failed on.** Once you can do that, patterns
emerge across many failures and you get a working prior for which failures are
common at which stages.

We use two sources of post-mortem data:

- **CB Insights — "Top Reasons Startups Fail."** A recurring compiled report
  based on public post-mortem essays written by founders of failed startups.
  The report ranks the most-cited causes of failure across many companies.
- **Founder Collective — the "mortemas" series.** A collection of failure
  post-mortem writeups (and analysis of others' writeups) published by seed-stage
  VC firm Founder Collective, with a particular focus on how premature
  scaling contributes to failure.

The exercise at the end of this module (`exercise-05`) makes you actually read
three failure post-mortems and classify them. This chapter installs the
classification.

## The graph layers a startup can fail on

Every startup failure is a failure at one or more nodes on the dependency
graph in `FUNCTIONAL_CURRICULA.md`. Foundations groups them into seven layers
for the purposes of post-mortem classification:

| Layer | What failure at this layer looks like |
|---|---|
| **Problem** | No one had the problem, or the problem wasn't painful enough to pay to solve. |
| **Solution** | The product didn't solve the problem, or solved it worse than the alternative. |
| **Market** | The problem is real but the addressable market is too small, too fragmented, or unreachable at reasonable CAC. |
| **Business model** | The product works and customers want it, but you can't make money — CAC exceeds LTV, margins are thin, payback is too long. |
| **GTM / distribution** | Product-market fit exists but you can't reliably reach the customers who want it — the sales motion, channel, or positioning is broken. |
| **Capital structure** | The corporate, equity, or governance shape prevents the company from raising the next round, keeping the team, or making a strategic decision. |
| **Team** | The wrong founders, a broken co-founder relationship, bad early hires, or a founder-fit-with-work problem breaks the company independent of the product. |

These are the same seven layers referenced in the module's learning
objectives. Every failure you read should be classifiable to at least one, and
often to two or three that interacted.

## What CB Insights says

The CB Insights Top Reasons Startups Fail report is compiled from many
public founder post-mortems and ranks the most-cited causes. Across the
editions of the report published to date, the top cluster of reasons has been
remarkably stable, and maps cleanly onto the graph layers above.

The recurring top reasons include:

- **No market need** — a **problem-layer** failure. Consistently the single
  most-cited reason across editions of the report.
- **Ran out of cash** — a **capital-structure and business-model composite**;
  usually a symptom of one of the other failures (product not compelling
  enough, growth too slow, burn too high) manifesting as capital exhaustion.
- **Not the right team** — a **team-layer** failure.
- **Got outcompeted** — usually a **market** or **GTM** failure; the market
  existed, but the company was not the one that captured it.
- **Pricing / cost issues** — a **business-model** failure.
- **User-unfriendly product** — a **solution-layer** failure.
- **Product without a business model** — a **business-model** failure that
  presents as a solution-layer success.
- **Poor marketing** — a **GTM** failure.
- **Ignore customers** — a cross-cutting failure, usually catalyzing a
  problem-layer or solution-layer breakdown.
- **Product mistimed** — a **market / why-now** failure.

<!-- needs-research: pull the current CB Insights report edition and confirm the exact ordering, wording of each reason, and the reported percentage for the top reason ("no market need"). Update the citation in resources.md to the specific edition. Do not publish the specific percentages until they are pulled from the primary report. -->

The key thing to notice: **"no market need" is consistently the top reason.**
That is a problem-layer failure — the startup built something that no one
actually needed enough. It is the same finding that produced Blank's Customer
Development (chapter 04) as a discipline and the same failure Graham warns
against in the "something people want" ingredient of `How to Start a Startup`
(chapter 03). The three sources converge, which is why they are all in this
module together.

## What Founder Collective's mortemas add

Founder Collective is a seed-stage venture firm that has published a series of
failure post-mortem writeups (their "mortemas" collection) focused on
patterns visible from the investor's side. The specific contribution of the
mortemas series, relative to CB Insights, is emphasis on **premature scaling**
as a distinct failure mode.

The premature-scaling pattern goes:

1. The startup raises significant capital before the search from chapter 05
   is complete — before the problem, solution, or market has been validated.
2. With capital in the bank, the founder feels compelled to scale — to hire,
   to spend on paid acquisition, to open regions, to build the second product.
3. Scaling activity moves the founder off the search. The unresolved
   questions from earlier searches stay unresolved because no one is doing
   the search work anymore.
4. Money runs out before the searches finish. The company dies with a
   half-built product, a scattered team, and a large cap-table overhang.

This is the same pattern Startup Genome named in their research on premature
scaling; it is the reason mod-003 (`Stages and What Matters When`) treats
stage-mismatched activity as a first-class failure mode.

The mortemas series also emphasizes a specific **capital-structure failure
mode**: raising too much at too high a valuation early, then being unable to
raise the next round because the numbers don't support the previous
valuation. This is a failure at the capital-structure layer, downstream of a
business-model failure, and it is one of the more preventable causes of
startup death.

<!-- needs-research: pull the Founder Collective "Mortemas" landing page (foundercollective.com) and cite the specific writeups referenced by learners in exercise 05. The specific mortemas featured on the Founder Collective site may change over time — verify the recommended reading list before shipping the exercise. -->

## The two moves after reading a post-mortem

For every failure post-mortem you read, do two things.

**Move 1 — surface classification.** Which layer(s) did the company fail on?
Force yourself to pick from the seven-layer list above. If a failure feels
like it doesn't fit any layer, either the layer list is wrong (unlikely for a
first-pass read) or your read of the failure is fuzzy. Sharpen it.

**Move 2 — root-cause classification.** The layer where the *symptom* appears
is rarely the layer where the *root cause* lives. A company that runs out of
cash (capital-structure symptom) usually did so because growth wasn't fast
enough to justify the burn (business-model root), which usually was true
because the market wasn't as big as they thought (market root), which usually
was true because the problem was narrower than they believed (problem
root). The chain of because-becauses is what makes a post-mortem useful.

The seven-layer taxonomy is not just for classifying — it is for tracing.

## Reading tips

- **Read the primary post-mortem, not a summary.** Founders' summaries of
  their own failures are usually more honest and more specific than
  third-party writeups. When CB Insights or Founder Collective links to a
  primary post-mortem essay by the failed founder, click through.
- **Watch for the retrospective narrative bias.** Failed founders sometimes
  attribute their failure to a single tidy cause — "the market wasn't ready"
  — when the honest read is a compound failure. If a post-mortem sounds too
  clean, sharpen it against the seven layers.
- **Don't over-generalize from one story.** A single company failed for a
  cluster of specific reasons. The lesson is *this class of failure is
  possible and looks like this*, not *therefore no one should do X.*
- **Bring the failure back to your own startup.** After each post-mortem,
  spend two minutes asking: *am I doing this right now, and if so, which
  layer would I be failing on?* That is the loop the exercise codifies.

## Summary

- Failure post-mortems are the honest source; success stories are noisy.
- Every failure can be classified to at least one of seven graph layers:
  problem, solution, market, business model, GTM, capital structure, team.
- CB Insights consistently ranks "no market need" (problem-layer) as the
  single most-cited failure — the same finding Blank, Ries, and Graham each
  independently made.
- Founder Collective's mortemas emphasize premature scaling and
  over-capitalization as distinct, preventable failure modes.
- After reading each post-mortem, do two moves: surface classification and
  root-cause tracing.

## Homework

Exercise 05 (`Three Failure Post-Mortems Teardown`) walks you through this on
three real cases. Chapter 06 is the reading list and the frame; exercise 05
is the practice.
