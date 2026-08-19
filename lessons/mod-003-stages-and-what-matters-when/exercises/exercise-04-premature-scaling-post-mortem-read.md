---
module: mod-003-stages-and-what-matters-when
exercise: exercise-04
slug: premature-scaling-post-mortem-read
hours: 2
prereqs: [chapter-05-startup-genome-premature-scaling]
---

# Exercise 04 — Premature-Scaling Post-Mortem Read

## Problem statement

Chapter 05 introduced the Startup Genome premature-scaling framing — a
company fails when one or more of its dimensions (team, product,
customer, business model, financials) scales ahead of the others. This
exercise puts the framing to work on a real, publicly documented
company failure.

You will (a) read the Startup Genome report (or the currently-canonical
version of it) at enough depth to extract the consistency dimensions and
the operating framing, (b) pick one real, publicly documented startup
failure post-mortem, and (c) diagnose the failure across the
premature-scaling dimensions and defend the diagnosis against one
alternative explanation.

## Requirements

### Part A — read the primary source

Read the Startup Genome report (or the currently-canonical follow-up).

<!-- needs-research: identify the specific current-canonical URL for the Startup Genome material (the original 2011 release, the follow-up "A Deep Dive into Why Most High-Growth Startups Fail," or any later re-issue that Startup Genome or a successor organisation still hosts). List the specific edition and URL the exercise expects the learner to read. -->

Produce a short reading note (200–400 words) with:

- **The core claim** in your own words.
- **The list of consistency dimensions** the report names (verify
  against the specific edition; the dimension list has varied
  across editions).
- **The headline empirical claim** (the percentage of high-growth
  startups the report identifies as scaling prematurely along at
  least one dimension). Quote the number exactly and cite the
  edition.
- **The mechanism of failure** the report describes — how does
  premature scaling in one dimension cause the company to fail?

### Part B — pick a startup failure post-mortem

Pick **one real, publicly documented startup that failed** and for
which a substantive post-mortem exists. Acceptable sources for the
post-mortem:

- A founder's own written post-mortem (blog post, essay, LinkedIn
  post). The gold-standard source when it exists.
- A published journalistic post-mortem (a magazine feature, a
  long-form business article) that draws on interviews with
  founders and investors.
- CB Insights startup failure post-mortem entries (referenced in
  mod-001 chapter 06 and resources).
- Founder Collective "mortemas" series.
- A shutdown announcement plus a subsequent press retrospective
  that together provide enough detail on what the company was
  doing in its final 12–18 months.

**Do not** pick:

- A private company you know personally through insider access.
- A company whose failure has not been documented in enough
  detail to name the specific activities that were happening in
  its final year.
- A very obscure failure with only single-source coverage. You
  need enough independent evidence to defend the diagnosis.

The post-mortem doesn't have to be huge — a well-written founder
essay of 2000–3000 words is often more than enough. It has to
provide enough detail on what the company was doing across the
consistency dimensions at the time it failed.

### Part C — the diagnosis

Produce a diagnosis with the following structure.

**1. Placement on the stage ladder at the time of failure.** Using
chapter 02's signal column, where was the company on the ladder in
its final 12 months? Cite the specific signals from the post-mortem
that support the placement.

**2. Dimension-by-dimension scaling assessment.** For each of the
Startup Genome consistency dimensions (team, product, customer,
business model, financials), name:

- What stage the dimension was operating at (using the same
  chapter 02 signal-column vocabulary).
- The specific evidence from the post-mortem that supports the
  placement.

The output is a small table with 5 rows.

**3. Which dimension(s) scaled prematurely?** Name the one or two
dimensions that were operating at a *later* stage than the others.
This is where the diagnosis lives — a company that scaled
consistently across all dimensions and still failed is not a
premature-scaling case, and you should either pick a different
company or note that the report's framework doesn't fit.

**4. The mechanism of failure.** In one paragraph, walk the causal
chain: the premature-scaling dimension consumed [what resource],
which prevented [what stage-appropriate work], which meant [what
underlying question stayed unanswered], which is what killed the
company. Anchor each link to specific evidence from the
post-mortem.

### Part D — one alternative explanation

Post-mortems typically offer more than one plausible cause of
failure. Name **one alternative explanation** for the failure of
your chosen company — an explanation that does not involve
premature scaling. Common alternatives:

- The problem wasn't real (chapter 03 shape-1 mismatch at the
  earliest stage; the founder never validated the problem search).
- The market wasn't there (the market search — mod-001 chapter 05
  search 3 — failed).
- The founding team broke down (team search — mod-001 chapter 05
  search 5).
- The macro environment turned (a recession, a rate hike, a
  specific competitor move) and the company couldn't survive it.
- A regulatory / legal event killed the company independently of
  its operating fitness.

Then defend your **premature-scaling diagnosis** against the
alternative. Show why the premature-scaling story is either
*primary* (the alternative was a symptom, not a root) or
*complementary* (both were operative, but premature scaling
determined the timing).

This step is what keeps the diagnosis from being a mono-causal
Just-So story. The Startup Genome framework is one lens; the
alternative check keeps you honest about the lens's limits.

## Deliverable shape

A single Markdown file, `mod-003-exercise-04-premature-scaling-post-mortem.md`,
structured:

```markdown
# Premature-Scaling Post-Mortem — <company>

## Part A — Startup Genome reading note
<200-400 words: core claim, dimensions list, headline number,
mechanism of failure. Cite the specific edition read.>

## Part B — post-mortem source
- Company: <name>
- Sources: <URLs / citations>

## Part C — diagnosis

### Placement at failure
Stage: [X]. Signal evidence: <2-3 items>.

### Dimension-by-dimension assessment
| Dimension | Stage | Evidence |
|---|---|---|
| Team | ... | ... |
| Product | ... | ... |
| Customer | ... | ... |
| Business model | ... | ... |
| Financials | ... | ... |

### Premature-scaling dimension(s)
<1-2 dimensions named, with specific evidence>

### Mechanism of failure
<one paragraph — the causal chain>

## Part D — alternative explanation
### The alternative
<one paragraph — the strongest alternative explanation>

### Defence of the premature-scaling diagnosis
<one paragraph — why premature scaling is primary or complementary>
```

Total length: 1000–1500 words.

## Starter guidance

- **Founder-written post-mortems are the highest-value source.**
  They tend to name the specific activities that consumed founder
  attention in the final year, which is what the diagnosis needs.
- **Post-mortems from investors are second-best.** Investors have
  the incentive alignment to talk about premature scaling
  (they've seen it many times) but sometimes over-diagnose it
  because it fits their model.
- **The dimension table should not have all five dimensions at
  the same stage.** If it does, either the company is a
  counter-example to the Startup Genome framing (rare but real
  — write that up honestly) or you're missing evidence on one or
  more dimensions.
- **The mechanism-of-failure paragraph is the exercise's
  keystone.** A weak causal chain ("they hired too many people →
  they ran out of money") loses to a specific one ("the
  60-person sales team was hired against a $12M ARR forecast
  that assumed 60% net retention; actual retention was 30%, so
  the pipeline they were built to convert never materialised;
  burn hit $2.5M/mo against a $30M raise; the money lasted 12
  months instead of the planned 24"). Push for specificity.
- **Do not use a company you personally worked at unless the
  failure is fully public.** The exercise depends on the
  post-mortem being defensible from public evidence; if you can't
  cite it, you can't use it.
- **Watch for confirmation bias.** You are looking for
  premature-scaling patterns; you will find them even where they
  aren't the primary story. The Part D alternative-explanation
  step is designed to protect against this — take it seriously.

## Acceptance criteria

You have completed the exercise when:

- [ ] The Startup Genome reading note is 200–400 words and cites
      the specific edition read.
- [ ] A real, publicly documented startup failure post-mortem is
      chosen and sourced (2+ sources ideal, 1 minimum for founder
      post-mortems).
- [ ] The stage-at-failure placement uses signal-column evidence
      from chapter 02.
- [ ] The dimension-by-dimension table has all 5 rows filled with
      evidence-backed stage placements.
- [ ] The premature-scaling dimension(s) are named with specific
      evidence.
- [ ] The mechanism-of-failure paragraph is a specific causal
      chain, not a generic story.
- [ ] Part D presents one alternative explanation and defends the
      premature-scaling diagnosis against it.
- [ ] The file is committed to your notes as
      `mod-003-exercise-04-premature-scaling-post-mortem.md`.

## Common failure modes to avoid

- Diagnosing every failure as premature scaling. The report's
  framework is powerful but not universal; some failures are
  problem-search failures, some are team failures, some are
  macro. If your chosen company doesn't cleanly fit the
  premature-scaling story, pick another company or note the
  mismatch honestly.
- Treating "they hired too many people" as sufficient. The
  dimension the report cares about is team, and "hired too
  many people" is the surface symptom. The diagnosis needs to
  show the team dimension was at a *later stage* than the
  other dimensions and cite the specific evidence.
- Skipping the alternative-explanation step because "premature
  scaling is obviously the answer." The purpose of the step is
  to force you to check.
- Reading only chapter 05 and skipping the primary source. The
  Startup Genome report is short enough that reading it
  directly is a small investment for a big payoff.

## What good looks like

A post-mortem diagnosis that reads as *evidence-backed structural
analysis*, not opinion. A reader should finish the file and be
able to name (a) what the Startup Genome framework says, (b)
what the specific company's dimensional profile looked like at
failure, (c) what the causal chain of failure was, and (d) why
premature scaling is the better explanation than the natural
alternative.

The diagnostic discipline you build here is what chapter 06's
checklist embeds as Q4 (premature-scaling check). This exercise
is where the pattern-recognition gets built; the checklist is
where it gets used weekly.
