# Two Operating Traditions — Blank's Customer Development, Ries's Lean Startup

## Motivation

Paul Graham gives you the compass (growth) and the heuristics (things to do,
things to avoid). But heuristics are not a method — they tell you *what* to aim
at, not *how* to work day to day. This chapter installs the two operating
traditions that Foundations sits on top of and every downstream pillar assumes
you know.

Both traditions grew out of the same insight from the early 2000s: startup
failure is overwhelmingly a failure of *product-market misalignment*, not a
failure of engineering or execution, and the traditional management playbook
(business plan, sales forecast, waterfall execution) actively makes that
failure worse. Both traditions were built to replace the traditional playbook
with something that treats a startup as a learning system.

The two traditions are complementary. Blank named the discipline; Ries named
the loop. Together they are the working model this curriculum uses.

## Tradition 1 — Steve Blank's Customer Development

**Primary sources:**

- Steve Blank, *The Four Steps to the Epiphany* (2005, self-published; revised
  editions since).
- Steve Blank and Bob Dorf, *The Startup Owner's Manual* (2012) — the
  book-length, textbook-style expansion of the Four Steps.

**The core claim.** Traditional management is designed for companies that
*know* who their customer is and what to sell them. Startups don't know either.
So the traditional playbook — write a plan, execute it, adjust the numbers on
schedule — cannot work. Startups need a separate, parallel discipline whose
whole job is finding out who the customer is and what to sell them. Blank
calls this discipline **Customer Development**.

Customer Development runs *alongside* Product Development, not after it. While
engineers are building the product, founders are out learning who wants it,
what they'll pay, and how they'll buy it. The two tracks feed each other.

**The four steps.** Customer Development is structured as four sequential
stages:

1. **Customer Discovery** — get out of the building. Test whether the problem
   you think exists actually exists in the market you're targeting. Test
   whether your proposed solution actually addresses that problem. Talk to
   dozens of prospective customers before writing serious code. The output is a
   validated hypothesis about problem, customer, and rough solution shape.
2. **Customer Validation** — sell the product to early customers. Not for
   revenue's sake, but to prove that a repeatable sales process can be built
   around it. If you cannot get customer #1 through customer #10 by hand, you
   cannot get customer #1,000 through automation.
3. **Customer Creation** — now that a repeatable sale exists, invest in
   generating demand at scale. Marketing, positioning, category creation, paid
   acquisition. This is the first step that looks like a traditional company.
4. **Company Building** — transition from a startup organization (searching)
   to a functional company (executing). Departments, org design, management
   layers, systems. This is the graduation.

The four steps are stage-tagged in Foundations: **Discovery is IDEA / PRE-SEED,
Validation is SEED, Creation is SERIES-A, Company Building is GROWTH.** The
stage ladder in `STARTUP_STAGES.md` is aligned with them by design.

**The load-bearing idea.** Blank's biggest contribution is the discipline of
treating the customer as an experimental subject to be studied *before*
building. The most damaging move a founder can make is skipping Discovery —
building the product and then hoping someone shows up. Customer Development
says: no. First find them, then talk to them, then build for them.

**The output artifacts.** A Customer Development practice produces things you
can put on the graph in mod-002: customer interview notes, problem statements,
early ICP definitions, hypothesis-to-evidence tables. The Lean Canvas — an
adjacent tool from Ash Maurya — is a compressed way to capture a startup's
assumption set at any moment; mod-002 uses it as a working shape.

## Tradition 2 — Eric Ries's Lean Startup

**Primary source:**

- Eric Ries, *The Lean Startup* (Crown Business, 2011). Follow-up book *The
  Startup Way* (2017) extends the framework to large organizations.

**The core claim.** A startup is not a smaller version of a big company; it is
an institution designed to produce **validated learning** under uncertainty.
Progress is not measured in features shipped, meetings held, or dollars raised;
it is measured in learning. The whole methodology — the terminology, the loop,
the accounting — is designed to make that shift concrete.

Ries acknowledges Blank as a direct predecessor (Ries was Blank's student). What
Ries adds is a much sharper operational vocabulary and a general-purpose loop
that fits inside Blank's four steps.

**The Build-Measure-Learn loop.** The heart of Lean Startup is a single loop:

```
IDEAS ──build──► CODE ──measure──► DATA ──learn──► IDEAS ...
```

- **Build.** Turn the current hypothesis into the smallest thing you can put in
  front of customers. This is the **MVP** — the Minimum Viable Product — the
  *smallest* thing that lets you test the current hypothesis, not the *simplest
  version of the product you plan to build*. The distinction matters. An MVP
  is a test instrument, not a first release.
- **Measure.** Put the MVP in front of customers and instrument it. Collect
  data about the specific hypothesis you're testing. Ries emphasizes
  **innovation accounting** — measuring the metrics that reveal learning, not
  the vanity metrics that make you feel good.
- **Learn.** Compare what happened to what you predicted. Either your
  hypothesis was validated (invest more) or it was invalidated (change
  something). The "change something" case has a specific term: the **pivot** —
  a structured change to one hypothesis while keeping others constant.

The loop is meant to run as fast as possible. Time through the loop, not
features per week, is the throughput metric.

**Other core ideas.** The Lean Startup vocabulary is now standard. The terms
Foundations will use later, from Ries directly, include:

- **Validated learning** — evidence about customer behavior collected through
  experiments, not opinions collected through meetings.
- **MVP** — a Minimum Viable Product built as a test instrument.
- **Pivot vs. persevere** — the founder's structured decision after each loop
  iteration, based on what the data said.
- **Innovation accounting** — the metrics discipline that supports pivot vs.
  persevere decisions.
- **Vanity metrics** — numbers that make you feel productive without evidence
  the business is progressing.

**The load-bearing idea.** Ries's biggest contribution is *cadence*. Blank
tells you *what discipline* to run; Ries tells you *how fast the loop should
turn*. Together they let a founder honestly answer at any moment: what
hypothesis are we testing right now, what evidence would prove it, when will we
have the evidence?

## How the two traditions fit together

Blank and Ries are not competitors. They stack:

- Blank names the **stages** of the startup's outer arc — Discovery →
  Validation → Creation → Company Building.
- Ries names the **inner loop** you run *inside* each stage —
  Build-Measure-Learn, over and over, on whatever hypothesis is currently
  binding.

A concrete way to see it: during Customer Discovery (Blank), you run many
Build-Measure-Learn loops (Ries) on the problem hypothesis. During Customer
Validation, you run many loops on the sales hypothesis. And so on. The stages
are the search agenda; the loop is the operating tempo.

Where they nominally disagree, they usually agree on substance. Ries has been
more emphatic about the MVP as a real deployed artifact; Blank has emphasized
customer conversations before code. In practice, mature Customer Development
teams run MVPs and mature Lean Startup teams do customer discovery — the two
traditions have converged in practice.

## Where Foundations sits

Foundations is not itself a Customer Development or a Lean Startup textbook.
That depth lives in:

- `startup-product-gtm-curriculum` (level 20) — customer discovery, PMF,
  positioning, GTM, sales, growth.

What Foundations owns is the mental model that lets you make sense of those
depth courses when you get to them:

- The definition of a startup that both traditions assume.
- The stage ladder that both traditions map onto.
- The founder-numbers instrumentation (mod-005) that both traditions require
  to actually run.
- The dependency graph (mod-002) that lets you locate any artifact from either
  tradition on a shared map.

If you take away one thing from this chapter, it is this: **when you see a
technique in a later curriculum — an interview script, a landing-page smoke
test, a cohort retention chart, a pricing experiment — you should be able to
name which tradition it comes from (Discovery / Validation / Creation /
Company-Building for Blank; Build / Measure / Learn for Ries) and where on the
graph it lives.** That's the reason to read the primary sources.

## Summary

- Customer Development (Blank) is the discipline: get out of the building,
  study the customer as an experimental subject, run four sequential stages —
  Discovery → Validation → Creation → Company Building.
- Lean Startup (Ries) is the loop: Build → Measure → Learn, iterating on
  hypotheses with MVPs, backed by innovation accounting and decided with
  pivot-vs-persevere.
- The two stack: Blank's stages are the outer arc, Ries's loop is the tempo
  inside each stage.
- Foundations installs the mental model; depth lives in
  `startup-product-gtm-curriculum`.

## Homework

Read at least the introductions and first two chapters of both primary works
before doing exercise 03:

- Steve Blank, *The Four Steps to the Epiphany* — or the more accessible
  Blank & Dorf, *The Startup Owner's Manual*. Steve Blank's public writing at
  <https://steveblank.com> is also a strong starting point.
- Eric Ries, *The Lean Startup* (2011). The author's public site is
  <http://theleanstartup.com>.

Exercise 03 (`Customer Development vs Lean Startup Compare`) will ask you to
build a two-column comparison of the traditions on specific dimensions and
argue where each is stronger.
