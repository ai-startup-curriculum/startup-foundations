# The Decision Log — Dated Calls, Reasoned, Kept

## Motivation

The operating loop's first verb is **decide**. Chapter 01 named the
failure mode the "decide" step defends against as *decision-by-drift*
— the pattern where the founder never actually makes a call and the
situation resolves itself six weeks later in the direction of least
resistance. This chapter formalises the artifact that fixes the fix:
a **decision log**.

The decision log is the least glamorous artifact in the module. It
is a running, dated list of the calls the founder has made and the
reason each call was made. It has no template beyond three columns.
It has no tool requirement beyond a plain-text file. It is boring on
purpose — the discipline is the value, not the format.

It is also, in the founders' own retrospective view, the single most
useful cheap artifact of the operating loop. Almost every failure
mode the module defends against — revisionism, private context,
amnesia, drift — is either prevented outright by the log or made
visible early enough to correct.

## What a decision log actually is

A decision log is a table (a Markdown table, a spreadsheet row per
call, a notes file with dated entries — the tool does not matter)
with three columns:

| Date | Decision | Reason |
|---|---|---|

That is it. Every entry is one row. Every entry has a date. Every
entry has a one-sentence description of the call. Every entry has a
one-sentence description of *why the call was made given the
information available at the time*.

The log is **append-only**. You do not edit past entries when the
world changes. If a call was wrong in hindsight, you write a new
entry that supersedes it and cite the original by date. The
append-only property is where most of the log's value comes from —
it is the property that makes the log a defensible record of what
you actually thought, rather than a rolling summary of what you
currently think.

A working entry looks like this:

> **2026-03-04** — Decided to pause outbound sales for four weeks and
> reallocate two-founder-days per week to closing the top-three
> current-pipeline accounts. Reason: three of the last five customer
> interviews said the current onboarding is the blocker to signing;
> new outbound produces no signal we can act on until onboarding is
> fixed.

Not:

> ~~2026-03-04 — Paused outbound sales.~~

The bad version records the call and loses the reason. Six months
later, when someone asks "why did we stop outbound?", the founder is
either remembering (unreliable) or defending (motivated). The good
version answers on its own.

## Why append-only matters

The append-only property is the property most first-time
decision-log-keepers get wrong, and it is the property most of the
log's value depends on. Two failure modes it prevents:

**"We always thought that" revisionism.** The most human thing a
founder does is remember the past through the lens of the present.
Once a call turns out well, the founder tends to remember the
reasoning as more prescient than it was. Once a call turns out
badly, the founder tends to remember the reasoning as more
skeptical than it was. Either way, the actual reasoning at the time
gets lost. An append-only log is the check — you cannot edit the
entry to make yourself look better, so you don't.

**Silent belief drift.** Over a quarter, a founder's beliefs about
their market, their customer, and their product move a lot. Some of
that movement is *learning* (evidence changed the belief); some is
*drift* (the founder's mood or the last conversation changed the
belief without evidence). The log makes drift visible: if the entry
on 2026-01-15 says one thing about the ICP and the entry on
2026-03-04 says the opposite, either something happened between
those dates that should have its own log entry, or the founder is
drifting and needs to notice.

The append-only property is *the* thing that distinguishes a
decision log from an ordinary notes file. Every notes file starts
with good intentions and becomes a rolling summary of the founder's
current view; the log stays honest because you cannot go back and
retrofit.

## What belongs in the log

Every founder-only call belongs in the log. In practice, at
PRE-SEED, that is somewhere between five and fifteen entries a week.
The categories are worth naming:

**Product calls.** Ship / don't-ship the half-working feature.
Deprecate / keep the feature that six customers use. Rewrite / patch
the module the team keeps hitting bugs in. Buy / build the
integration.

**Customer / GTM calls.** Pursue / decline the enterprise pilot that
would consume a founder-quarter. Discount / hold the line on
pricing for the anchor logo. Pick / drop the channel that isn't
producing. Fire / keep the customer that is 30% of revenue and 90%
of the support load.

**People calls.** Hire / delay the role. Contract / employ. Extend
/ pass on the offer. Have / don't have the hard conversation with
the co-founder or the underperforming early hire. Depth on people
calls lives in
[`startup-operations-governance-curriculum`](https://github.com/ai-startup-curriculum/startup-operations-governance-curriculum);
the log is where the call itself is recorded.

**Capital calls.** Raise / don't raise now. Take / decline the
strategic check. Approve / decline the discretionary spend line.
Deferral of major capital calls to
[`startup-finance-fundraising-curriculum`](https://github.com/ai-startup-curriculum/startup-finance-fundraising-curriculum)
for depth, but the *call* still lands in the log.

**Strategy calls.** Persevere / pivot. Enter / leave the segment.
Reprioritise the OKR. Change the North-Star metric. These are the
lowest-frequency and highest-impact entries in the log.

What does *not* belong: (a) tactical execution calls that are not
founder-only ("pick this font size" — unless you're a solo founder
and it is your call); (b) opinions the founder holds but has not
acted on (that is a note file, not a log); (c) calls where the
"decision" was made by inaction. If a call was made by inaction,
log it explicitly: "we did not decide X, and the default of Y
prevailed. Why we let it default: ...".

## The three-column entry, in detail

The three columns are date, decision, reason. Each has a specific
discipline.

**Date.** The date the call was made (not the date the situation
became visible, not the date the outcome was seen). Use ISO format
(`2026-03-04`) so entries sort. If the call was made across a few
days of thinking, use the date the call became operative — the day
you stopped deliberating and started acting.

**Decision.** One sentence, past tense, starting with a verb.
"Paused outbound sales for four weeks and reallocated two
founder-days per week to closing three current-pipeline accounts."
Not "decided to think about outbound." Not "considered pausing
outbound." A decision is the point where you moved from
deliberation to commitment; the log records commitments.

**Reason.** One-to-three sentences on *why the call was made, given
the information available at the time*. Two disciplines here:

- **Given the information available at the time.** Do not
  retroactively insert data you didn't have. If the reason was
  "three customer interviews," write "three customer interviews,"
  even if you now know it was actually a bad sample; the point of
  the log is to record what you were reasoning from, not what was
  eventually true.
- **Reason first, source second.** The reason is the load-bearing
  content. If specific sources or numbers back the reason, list
  them after the reason ("three of five interviews from the
  accounting-firm segment"). Do not turn the reason into a citation
  dump — a reason no one can read past isn't a reason.

Optionally, some founders add a fourth column: **check date** — the
date they promised themselves they would come back and see whether
the call was right. Chapter 04's OKR check-in is where a batch of
"check dates" naturally get reviewed.

## How the log interlocks with the loop

The decision log is fed by, and feeds, the three weekly cadence
artifacts from chapter 02.

- **The Monday plan pre-populates the log.** The plan's "decisions
  expected this week" section names calls the founder anticipates
  making. When the call is made, the entry goes into the log with
  the actual date; if the call didn't get made, the plan is
  updated for the following week.
- **The Friday shipped-and-learned reviews the log.** The
  Learned section is where calls made this week that didn't make
  it into the log get caught. On Friday, scan the week for any
  founder-only call not yet logged; add it now while the reason
  is still fresh.
- **The metrics one-pager cross-references the log.** When a
  number moved (up or down) more than the founder expected, look
  at the log for the calls in the two weeks before the movement.
  This is the cheap version of causal analysis — not a
  proof-of-causation, but a first hypothesis.

The interlock keeps the log alive. A log kept in isolation dies
within a month; a log kept as one part of the loop stays honest
because the loop keeps returning to it.

## The log at the quarterly checkpoint

Once a quarter — practically, on the last Friday of the quarter —
the founder should re-read the log end-to-end. This is the single
highest-return process ritual in the operating loop, and it takes
under an hour.

Three passes:

1. **Skim for pattern.** Read every entry. Note the categories that
   dominate (product, customer, people, capital, strategy). If one
   category is 70% of entries, that is the category the quarter
   was actually about — often different from the category the
   founder *thinks* the quarter was about.
2. **Check the calls that turned out.** For each call whose outcome
   is now visible, mark whether the outcome was as expected, better
   than expected, or worse than expected. Do not edit the entry;
   add a follow-up entry dated today. Two-thirds of a working
   founder's calls come out as expected; the interesting one-third
   is where the learning is.
3. **Look for the calls not made.** Scan the quarter for major
   decisions that *should* be in the log and are not. Every missing
   call is either (a) a call that was actually made by inaction (log
   it now, explicitly) or (b) a decision the founder is still
   putting off (add it to the current Monday plan).

The quarterly review is where the log stops being a bookkeeping
artifact and becomes a founder-development artifact. Reading a
quarter of your own reasoning back to yourself — with the outcomes
visible and the temptation to revise removed — is how founders
learn to make better calls.

## Two nuances

**Nuance 1 — the log is private-then-shared.** At solo-founder scale,
the log is a private file. Once there's a co-founder, the log becomes
shared with the co-founder (append-only still) but not necessarily
public to the team; some entries touch personnel and legal decisions
that don't belong in shared team spaces. When the company gets a
board, some log entries feed the board update (chapter 06 and
onward), but the log itself remains a founder / co-founder artifact
in most companies. The rule is: **be shared enough that revisionism
is checked, private enough that hard calls can still be honestly
recorded.**

**Nuance 2 — the log is not the same as an ADR.** Engineering
readers will notice the resemblance to an Architecture Decision
Record. The two are cousins, not the same:

- An **ADR** documents an engineering decision with context,
  options considered, and consequences, and it lives in the
  codebase alongside the code the decision governs.
- A **founder decision log** documents *all* founder-only calls
  (not just engineering), with a much shorter shape (one sentence
  per column), and it lives in the founder's operating notes.

If your team already runs ADRs for engineering decisions, keep
those; the founder decision log covers the calls ADRs don't
(customer, capital, people, strategy) and any engineering call
that had to be made at founder scope rather than team scope.

## The log versus the memo

Some founders substitute a **weekly memo** (a long-form written
essay-per-week) for the decision log. The two are complementary,
not substitutes.

- The memo is where the founder *thinks*. It captures the shape of
  a hard problem, the alternatives considered, the reasoning walked
  through.
- The log is where the founder *commits*. It captures the actual
  call made, dated, with the reason in a form that survives being
  read six months later.

Founders who write only memos tend to defer commitments — the memo
becomes the place where deliberation lives forever. Founders who
keep only a log tend to under-explore — the log records commitments
without the reasoning depth. The pattern that works at PRE-SEED and
SEED is: **memos for hard calls, log entries for all calls,
including the ones the memo argued for**.

## Common failure modes

**1. Retrofitting the log at week's end.** A log written every
Friday from memory of the week is a summary, not a log. The
Wednesday entries have already been softened, the Tuesday entries
compressed, the Monday entries partially forgotten. The log needs
entries within a day of the call; the Friday shipped-and-learned
is the *check* on the log, not the log's origin.

**2. Editing past entries when new information arrives.** Adding a
strikethrough or a comment is fine; overwriting the reasoning is
not. If you feel the need to edit an old entry, that is the signal
that a new entry is called for — write the update as a new dated
row, with a reference back to the old one.

**3. Writing reasons that are not reasons.** "Because it was the
right thing to do." "Because everyone agreed." "Because I felt
strongly about it." These are not reasons; they are what a reason
sounds like when the founder has skipped the step of naming *why*
they felt what they felt. Push the reason one level deeper: what
piece of evidence, what customer signal, what number, what
constraint drove the call?

**4. Logging every decision, including trivial ones.** The log is
for founder-only calls. If a call could have been made by anyone on
the team (including the founder acting as team member), it doesn't
belong. Logging trivial calls dilutes the log's signal and the
founder eventually stops keeping it.

**5. Not reviewing the log quarterly.** A log nobody re-reads is a
notepad. The quarterly re-read is where the log's second half of
value shows up — it is where "how am I actually making decisions?"
becomes visible.

## Summary

- The decision log is a running, dated, append-only record of every
  founder-only call and the reason it was made.
- Three columns — date, decision, reason. That is the entire
  format.
- Append-only is load-bearing: it prevents revisionism and makes
  belief drift visible.
- The log interlocks with the weekly cadence — the Monday plan
  pre-populates it, the Friday shipped-and-learned catches missing
  entries, the metrics one-pager cross-references it when numbers
  move.
- The quarterly re-read is the highest-return ritual in the loop —
  under an hour, and where the log becomes a founder-development
  artifact rather than a bookkeeping one.

## Homework

Exercise 03 (`Decision Log — First Ten Entries`) is where the log
gets started — ten entries, all in the three-column shape, at least
half of them from a real recent stretch of founder work. Exercise 01
(`Founder Week Simulation`) includes decision-log entries as part
of the end-to-end week.
