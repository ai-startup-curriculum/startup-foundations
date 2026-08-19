# The Weekly Cadence — Monday Plan, Friday Shipped-and-Learned, Metrics One-Pager

## Motivation

Chapter 01 named the four-part operating loop and the seven artifacts
that carry it. This chapter formalises the three that fire *every*
week — the **Monday plan**, the **Friday shipped-and-learned**, and
the **metrics one-pager** — and shows how the three interlock into a
single weekly shape that survives the transitions this module cares
about most: (a) going from one founder to two, (b) taking the first
hire, and (c) starting to send an investor update.

The three cadence artifacts are the *chassis* of the loop. Everything
else — the decision log, the OKR check, the narrative rewrite, the
investor update — plugs into the same three-artifact chassis. If the
chassis is wrong, nothing else fits; if the chassis is right,
everything else is a small addition to something that already runs.

## The three-artifact chassis

The chassis has exactly three parts and they run in a fixed order
across the week:

```
Monday morning        Wednesday morning         Friday afternoon
─────────────────     ──────────────────        ─────────────────
Monday plan       ─►  Metrics one-pager    ─►   Friday shipped-and-learned
(30–60 min)           (10–15 min check-in)      (45–60 min)
                                                metrics one-pager updated
                                                decision log reviewed
                                                OKR key-results checked
```

Each artifact is one page or less. Each fits in the time budget above.
Each has the same simple properties: a fixed shape that does not
change from week to week, a bounded length so it never spirals into a
project, and an explicit relationship to the next artifact in the
chain.

## The Monday plan

**Purpose.** The Monday plan is the pre-commitment for the week. It
is the founder saying, on the record, *here is where I intend to
spend the week's attention, and here is what I expect to be true by
Friday*. It is small enough to be written in half an hour and firm
enough that when Wednesday tries to knock it sideways, the founder
can see the drift.

**Shape.** A working PRE-SEED Monday plan has four sections. Each
section has a length ceiling — the ceiling is the important part;
brevity is the artifact's job.

1. **This week's three-to-five things.** Not "this week's twenty
   things." Three-to-five. Each item is one sentence starting with a
   verb: *ship the Zapier integration; run five customer interviews
   with the accounting-firm segment; close the LOI with acme.co;
   review Ann's take-home for the founding-eng role*. Each item has a
   hours-of-founder-attention budget next to it (a rough estimate is
   fine — this is the arbitrage detector, not a Gantt chart).
2. **What is on the metrics one-pager this week.** One line per
   number — the current value, the target for the week, the direction
   you expect it to move. This is where you commit *in advance* to
   what you'll be looking at on Wednesday and Friday. If a number is
   not on the one-pager, you are not measuring it this week; that is
   a decision.
3. **Decisions expected this week.** One line per anticipated call,
   with the owner (usually you). Not every call has to appear here —
   surprise calls happen — but any call you already know is coming
   should be pre-declared. This section pre-populates the decision
   log (chapter 03).
4. **What could take the week off-course.** Two or three sentences
   naming the specific things that could realistically knock the plan
   off — a customer emergency you can already smell coming, a
   candidate you're waiting on, a vendor issue you've been ignoring.
   Not paranoia; just the specific risks visible at Monday morning.

**Where it comes from.** The Monday plan is written from three
inputs, in this order:
- Last week's **Friday shipped-and-learned** — what carried over that
  wasn't finished.
- The **decision log** — any call made in the last week whose
  follow-through belongs in this week.
- The current **OKR key-results** — the quarter's commitment that
  the week should be advancing.

**Length ceiling.** One page. If it takes more than a page, either
the three-to-five list has grown to seven-to-ten (fix by cutting) or
the "what could take the week off-course" section has grown into an
essay (fix by narrowing to two or three concrete named risks).

**The failure mode it defends against.** Chapter 01 named this:
attention arbitrage. Without a Monday plan, the day's shape gets set
by whoever emailed last. With a Monday plan, the day still gets
pulled around by inbound, but now the pull is visible against
something. When the founder ends up spending Tuesday afternoon on
something that wasn't on Monday's list, that is not automatically
bad — the world moves. What is bad is when the founder cannot see
the drift because there was nothing to drift *from*.

## The metrics one-pager

**Purpose.** The metrics one-pager is the week's numbers on one page,
readable in ninety seconds, updated Monday (read), Wednesday
(check), and Friday (close). It is the artifact that makes "measure"
in the operating loop real. It is not a dashboard. Dashboards are
for browsing; the one-pager is for deciding.

**Shape.** A working PRE-SEED metrics one-pager fits on one screen or
one page and has three sections:

1. **The founder-numbers.** Cash, monthly burn (both gross and net —
   see mod-005), runway in months, default alive / default dead call.
   These do not change week to week in shape; only in value.
2. **The North-Star metric and its supporting numbers.** The one
   number that captures the value the product delivers, plus two or
   three inputs to it. The North-Star selection is a mod-005 topic;
   this chapter assumes you have picked one.
3. **This week's watch-list.** Two or three numbers that are not
   standing metrics but that this quarter's OKR key-results require
   you to move. Watch-list items rotate as the KRs rotate. Anything
   that's *always* on the list belongs in section 1 or 2, not
   section 3.

Every number has three values next to it: **current, last week,
target-for-this-week**. That is the entire dashboard grammar. No
sparklines yet. Sparklines are the SEED / SERIES-A version of the
same artifact; at PRE-SEED, three numbers per line are enough to
see whether the week is going in the right direction.

**Where it comes from.** The one-pager is populated from:
- The runway model (mod-005) for the founder-numbers row.
- Whatever product / GTM instrumentation is running for the
  North-Star row. If nothing is instrumented, the one-pager is
  telling you the truth: you're not yet measuring the North-Star.
- The OKR (chapter 04) for the watch-list row.

**Length ceiling.** One page. Twelve rows is a soft ceiling; if it
grows past that, one of the sections is doing the wrong job (usually
watch-list is including everything and section 1 is doing nothing).

**The failure mode it defends against.** Chapter 01 named this:
vibes-based reasoning. The founder who runs without a one-pager
still has a sense of "the week went well," but the sense is not
falsifiable. The one-pager is the small, boring artifact that makes
weekly feelings check against weekly numbers, and it catches the
compounding kind of bad feeling — the "growth is fine" feeling that
turns out on inspection to have been flat for six weeks — early
enough to do something about it.

## The Friday shipped-and-learned

**Purpose.** The Friday shipped-and-learned is the retrospective end
of the week. It closes the loop: the Monday plan committed to X;
what actually shipped, what actually got learned, and — most
importantly — what the *delta* between plan and reality means for
next week's plan.

**Shape.** A working PRE-SEED Friday shipped-and-learned has three
sections:

1. **Shipped.** One line per thing that shipped this week. Shipped
   means the thing left your desk — code deployed, integration live,
   contract signed, hire made, interview transcribed, customer
   emailed with the answer. Half-shipped things do not go here; they
   go in section 3 as roll-overs.
2. **Learned.** Two to five sentences on what the week *told* you
   that you did not know on Monday. This is not a diary; it is the
   answer to "if I had to run this week again, what would I do
   differently?" and "what did we discover about the customer, the
   product, the market, or ourselves?" Every honest answer to that
   pair is a candidate decision-log entry (chapter 03).
3. **What next week has to carry.** Two lists: (a) unfinished items
   from this week's plan that roll over, and (b) things that
   happened this week (from decisions, from customer signal, from
   metrics moves) that create new work for next week. Section 3
   pre-populates next Monday's plan.

Sometimes there is a section 4: **the ask** — one line, only used if
there is a specific external ask (of a co-founder, an investor, a
mentor) that came out of this week. Most weeks section 4 is empty.

**Where it goes.** Two audiences:
- **The founder themselves**, next Monday morning, as the primary
  input to the next plan. This is the audience that matters most —
  the shipped-and-learned is the artifact that gives Monday's plan
  its context.
- **The co-founder or first employee**, as the weekly async update.
  When there is only one founder and no employees, this audience is
  the future founder — the person who will read six months of
  shipped-and-learneds when trying to reconstruct what happened
  during the quarter that turned. That reconstruction is worth an
  hour a week now.

**Length ceiling.** One page. If Shipped is longer than five items
or Learned is longer than five sentences, either it is a two-week
recap (write it every week) or the founder is padding to feel
productive (the length ceiling is the honesty check).

**The failure mode it defends against.** Chapter 01 named this:
amnesia. Without a Friday shipped-and-learned, months compress in
memory into a fuzzy sense of "we worked hard on things." With one,
the record is checkable: what did we ship, what did we learn, what
did we defer. This is the record a founder returns to when a
customer, a board member, an investor, or their own future self
asks "why did we do it that way?"

## The interlocks — why the three artifacts are one system

The three artifacts share a single system property: **each is the
primary input to the next**. Break the interlock and the shape
collapses into three separate documents that nobody keeps up.

- **Monday plan → metrics one-pager.** Monday's plan names the
  numbers this week's watch-list should include. If a plan item
  doesn't have a corresponding number, either the item is un-measurable
  (be honest about it in the plan) or the one-pager is missing the
  right number (fix the one-pager). The plan sets the measurement
  agenda.
- **Metrics one-pager → Friday shipped-and-learned.** The Wednesday
  check on the one-pager surfaces the numbers that moved and the
  ones that didn't. Friday's Learned section is where the founder
  says what the movements mean. Without the one-pager, "Learned" is
  a vibes essay; with it, "Learned" is anchored to specific numbers
  that moved specific amounts.
- **Friday shipped-and-learned → next Monday's plan.** The
  shipped-and-learned's roll-overs and new-work items pre-populate
  the next plan. Without the shipped-and-learned, Monday's plan
  starts from a blank page and re-invents context that already
  existed.

The interlocks are why the three-artifact chassis is not the same as
"three separate documents you should write." Any one of them alone
does about a third of the work. Together they compound.

## Surviving the first hire

The first hire — a co-founder joining, a founding engineer, a first
salesperson, a chief of staff — is the transition that most
one-founder cadences break at. The three-artifact chassis is
designed to survive it with two small extensions and no
re-invention:

1. **The Monday plan gets a section per operator.** Section 1 (the
   three-to-five things) is grouped by *who owns each item*. When
   there are two of you, that is two mini-lists inside the same
   page. Section 2 (the metrics) and section 3 (the decisions
   expected) remain shared.
2. **The Friday shipped-and-learned gets one round of round-robin.**
   Each operator writes their own Shipped and their own Learned.
   Section 3 (what next week carries) is shared and gets
   reconciled together in a 15-minute review before the artifact
   ships.

Nothing else changes. The metrics one-pager is unchanged; the
decision log is unchanged; the OKR is unchanged. The chassis was
sized for two-to-three from the beginning, so the transition costs
minutes, not weeks.

## Surviving the first investor update

Chapter 06 is the full treatment of the first investor update; the
relevant point here is that **the update is authored from the four
weeks of shipped-and-learned and metrics one-pagers**, not from
scratch. Investor updates that get written monthly from a blank
page are the ones founders learn to dread. Updates authored by
summarising the four weeks of cadence artifacts already on hand
take under an hour.

Concretely: at the end of the last week of the month, the founder
adds a "monthly rollup" pass to the Friday shipped-and-learned —
scan the last four weeks' Shipped for the two-to-three items worth
telling investors about, the last four weeks' Learned for the
one-or-two lowlights that belong in the update, and the current
metrics one-pager for the numbers the update will lead with. That
rollup is the raw material for the investor update. Chapter 06
formalises the finishing shape.

## Common failure modes

Five failure modes are common enough to name up front.

**1. The plan becomes a wish-list.** A Monday plan with fifteen
items is not a plan; it is a wish-list. Cut ruthlessly to three-to-five.
If everything feels essential, the founder is missing the decision
about what *isn't* essential this week, and that missing decision is
the actual problem.

**2. The metrics one-pager has forty rows.** A one-pager that fills
three screens is a dashboard, not a one-pager. Dashboards are for
browsing; this artifact is for deciding. The discipline of
one-page-and-no-more is the entire value.

**3. The shipped-and-learned becomes a diary.** Learned is not
"here's how I felt this week." Learned is what the week told you
that you didn't know on Monday, and specifically what a co-founder
or a future you should carry forward. If the Learned section reads
like a journal entry, cut it and re-write it as three-to-five bullet
findings.

**4. The three artifacts drift into different tools.** The plan
lives in Notion, the metrics live in a Google Sheet, the
shipped-and-learned lives in Slack. Fine; whatever the tool. But
each artifact needs to be one file (or one page) that a future
reader can retrieve. If the shipped-and-learned is scattered across
Slack messages nobody can find, it is not doing the job.

**5. The cadence gets skipped "just this week."** Every founder
skips a week eventually. That is not the failure mode. The failure
mode is skipping *two consecutive weeks*, because the shipped-and-learned
carrying the roll-overs is now two weeks stale and next Monday's
plan starts from a blank page. The recovery is easy: run one plan
against last week, run one shipped-and-learned this Friday, and
you're back on the loop. Do not try to reconstruct the missing
weeks; they are gone.

## Summary

- The three cadence artifacts — Monday plan, metrics one-pager,
  Friday shipped-and-learned — are one system, not three
  documents. The interlocks are the point.
- Each artifact is one page, has a fixed shape, and defends against
  a specific failure mode from chapter 01 (attention arbitrage,
  vibes reasoning, amnesia).
- The Monday plan is the pre-commitment; the metrics one-pager is
  the measurement; the Friday shipped-and-learned is the
  retrospective. Each is the primary input to the next.
- The chassis is sized to survive the first hire (add a section per
  operator) and to feed the monthly investor update (a
  four-weeks-of-cadence-artifacts rollup) without redesign.
- The whole shape costs about two hours a week and returns a
  founder who can name, on Friday, what they did, why, and what
  moved.

## Homework

Exercise 05 (`Monday Plan / Friday Shipped Cadence`) is where the
three artifact shapes get exercised on a real week. Exercise 01
(`Founder Week Simulation — Monday to Friday`) runs a whole week
through the loop including these three artifacts and the decision
log. The lab (authored separately) runs one real week end-to-end.
