---
module: mod-004-founder-operating-basics
exercise: exercise-06
slug: first-investor-update-template
hours: 3
prereqs: [chapter-06-the-first-investor-update]
---

# Exercise 06 — First Investor-Update Template

## Problem statement

Chapter 06 formalised the one-page, three-section
(**highlights, lowlights, asks**) monthly-cadence investor update
and argued for writing it from month zero, before there are outside
investors reading it. This exercise ships the template a founder
can reuse every month, and then uses it once to write a real (or
realistically-specified) first update for the same startup used
across mod-004's other exercises.

The exercise has three parts: (a) a reusable template file that
carries the one-page shape and the discipline notes into every
future month, (b) one first update authored against the template,
and (c) a short teardown that catches the two failure modes
first-update-writers most reliably fall into (highlights-only
drift, and vague asks).

## Requirements

### Part A — read the primary source and pin the URL (about 15 min)

Read the Y Combinator founder-update primer linked in
`resources.md`. If the current YC library URL differs from the one
in `resources.md`, note the discrepancy in your exercise write-up
so future authoring passes can pin the correct link.

Then read one additional primary reference from `resources.md` —
either the SaaStr investor-update template or the Mark Suster
"Right Way to Do Investor Reporting" post. The point is to see the
same shape argued by an investor-side voice and a founder-side
voice; the discipline is more portable when both voices land the
same way.

**Deliverable A**: one paragraph (three-to-five sentences) in your
own words on what the two primary sources agree on and where they
diverge. This becomes the top of your template file.

### Part B — the reusable template (about 45 min)

Write a Markdown file, `investor-update-template.md`, that carries
the monthly cadence's shape as a blank you fill in each month.
Structure:

```markdown
# [Company Name] — Investor Update — [Month Year]

**To:** [distribution list]
**From:** [founder name(s)]
**Sent:** [ISO date]

## Highlights
- [one line — specific event or number]
- [one line]
- [one line]
- [optional 4th, 5th]

## Lowlights
- [one-to-two lines: what happened + what you are doing about it]
- [one-to-two lines]
- [optional 3rd, 4th]

## Asks
- [one line — action + criterion + timing]
- [one line]
- [optional 3rd, 4th]

---
Numbers snapshot (from the founder-numbers one-pager):
- Cash: [current]
- Net burn: [current]
- Runway: [months + end date + zone]
- North-Star: [name] — [current] (vs. [prior], target [target])
```

Below the template body, add a short **discipline notes** section
that reproduces (in your own words, one line each) the specific
disciplines from chapter 06 you want future-you to see at the top
of every update-writing session:

- One page hard ceiling.
- Highlights: one line, specific event or number.
- Lowlights: what happened + what you are doing about it.
- Asks: action + criterion + timing.
- Never skip a month. Never batch.
- Don't include screenshots, charts, or concept explanations.
- Write lowlights first.

The template file is the artifact you will keep and reuse; treat
it as the canonical spec for your own updates from this month
onward.

### Part C — the first real (or realistic) update (about 90 min)

Fill in the template for the current or most-recent month, for
the same startup used across mod-004's other exercises. Same
selection rules as the prior exercises (your own venture, one
you advise closely, or a well-specified hypothetical).

Discipline rules for the fill-in:

- **Write lowlights first.** Chapter 06 argued for this order
  because it is the section that most tempts omission and most
  needs the first draft to land honestly. Write section 2 first,
  then section 1, then section 3.
- **Three-to-five highlights, two-to-four lowlights, two-to-four
  asks.** Fewer if honest; do not pad to hit a maximum. More is
  a violation of the one-page ceiling.
- **Each highlight names one specific event or number.** Not
  "great month for sales" — "signed Acme as our first six-figure
  customer" or "meetings-per-active-account climbed from 2.9 to
  3.4 over four weeks."
- **Each lowlight names what happened and one line on what you
  are doing about it.** Not "sales was hard" — "sales cycle
  length stretched from 42 to 68 days for the healthcare
  segment; we're testing a scaled-down pilot to shorten the eval
  before we commit more founder-time."
- **Each ask names a specific action a reader could take.** Not
  "any thoughts welcome" — "intros to VP-Eng at insurance-tech
  seed / Series-A companies who might advise on the SOC 2
  process."
- **The numbers snapshot at the bottom is drawn from the
  founder-numbers one-pager** (mod-005 chapter 07, or a
  placeholder if mod-005 has not yet been completed). Do not
  re-derive numbers in the update; quote the one-pager.

Save the filled update as
`investor-update-[YYYY-MM].md` in the same folder as the template.

### Part D — the two-failure-mode teardown (about 30 min)

Chapter 06 named five common failure modes. Two of them are
almost universal on first updates: **highlights-only drift** and
**vague asks**. Do a short teardown of your own first update
against those two:

1. **Highlights-only drift check.** Count the lines in your
   highlights section vs. your lowlights section. If highlights
   outnumber lowlights by more than 2:1, either the month really
   was frictionless (rare) or you are drifting. Look at your
   Friday shipped-and-learneds from the past four weeks; each
   "Learned" section (per mod-004 chapter 02) is a candidate
   lowlight. Anything missing? Add it.

2. **Vague-asks check.** Re-read your asks section. For each
   ask, ask: *if I were a reader with this asked of me, would
   I know what specific action would help?* If any ask is a
   wave rather than a request, rewrite in the *action +
   criterion + timing* form.

Then write a short reflection (three-to-five sentences) on
which of the two failure modes was harder for you to catch, and
what the effort suggests about the discipline you will need to
maintain the update on a monthly cadence.

### Part E — the audience list (about 15 min)

Write down the specific list of people you would send the update
to *this month*, applying chapter 06's zero-audience-stage
guidance. If you are at zero outside investors, the list is
still non-empty; it includes some subset of:

- Co-founder(s).
- First employee, once hired.
- Two-to-three mentors or advisors.
- Your own operating notes folder (the last name on the list).

Name each reader by role (not name) and one sentence on why they
are on the list. This audience list belongs at the top of the
template's monthly copy, next to `**To:**`.

## Deliverable shape

A **folder** — `mod-004-exercise-06-investor-update/` — containing
three files:

- `investor-update-template.md` — the reusable template + the
  discipline notes.
- `investor-update-[YYYY-MM].md` — the filled first update for
  the current or most-recent month.
- `reflection.md` — the two-failure-mode teardown from Part D
  and the audience list from Part E.

Total length: 800–1400 words across the three files. The
individual update stays under one page (roughly 250–400 words in
the body, not counting the numbers snapshot).

## Starter guidance

- **Write lowlights first.** Chapter 06 was explicit and the
  discipline is worth building on the first update. Founders who
  write highlights first usually run out of one-pager real estate
  before they get honest about the month.
- **Do not draft in the update — draft in the shipped-and-learned
  folder.** The update is a *summary* of the four Friday
  shipped-and-learneds and the current metrics one-pager (chapter
  02). If you find yourself composing new material for the
  update, the raw material for that material should already exist
  in the weekly artifacts.
- **Keep the update boring on purpose.** No emojis. No headers
  inside sections. No inline images. The shape's utility is in
  its predictability — a reader who has seen three of your
  updates knows exactly where to look for the ask that matters
  to them.
- **Ship the update even if the month was thin.** Chapter 06's
  "never skip" rule applies to this exercise. If the "real" month
  had nothing dramatic, ship a short update with three brief
  highlights, two honest lowlights, and two asks. A short update
  is fine; a skipped one is not.
- **The audience list is the exercise, not filler.** Zero-audience-
  stage founders often want to skip Part E on the grounds that
  "nobody is reading it." Chapter 06's argument is that
  zero-audience-stage is *exactly* when the discipline of naming
  the audience matters most.

## Acceptance criteria

You have completed the exercise when:

- [ ] The two primary references from `resources.md` were read,
      and the one-paragraph comparison of founder-side and
      investor-side voice is at the top of the template file.
- [ ] The reusable template file
      (`investor-update-template.md`) matches the one-page
      three-section shape from chapter 06, with the discipline
      notes section reproducing the chapter's rules in your own
      words.
- [ ] A filled first update
      (`investor-update-[YYYY-MM].md`) is present for the
      current or most-recent month, in the template's shape.
- [ ] The filled update fits on one page (roughly 250–400 words
      in the body, not counting the numbers snapshot).
- [ ] Highlights each name a specific event or number; lowlights
      each name what happened + what you are doing about it;
      asks each name action + criterion + timing.
- [ ] The two-failure-mode teardown (highlights-only drift +
      vague asks) is done, with a short reflection on which was
      harder.
- [ ] The audience list is named by role, with one sentence per
      reader on why they are on the list.
- [ ] The folder is committed to your notes as
      `mod-004-exercise-06-investor-update/`.

## Common failure modes to avoid

- **Highlights-only first update.** The single most common
  first-update failure. If your first update has no lowlights or
  one-line lowlights with no "what you are doing about it," it
  is a marketing document, not a report. Chapter 06 is explicit:
  the update loses trust after two or three highlights-only
  months.
- **Asks written as social nicety.** "Any thoughts welcome" and
  "let me know if you can help" produce zero responses.
  Specific asks (role, company shape, timing) produce responses.
  Rewrite until every ask names a concrete action a reader
  could take.
- **Length inflation.** The template is one page. The first
  update is one page. Every future update is one page. If the
  update creeps to a page and a half by the third month, the
  cut-order is: highlights first (cut to three), then lowlights
  (cut to two), then asks (cut to two).
- **Batching the update with a broader "state of the company"
  memo.** The monthly update is one page. State-of-the-company
  memos, if they exist, are separate artifacts. Do not conflate.
- **Writing the update as if the audience is a stranger.** The
  monthly update is written for readers who already know what
  the company does. Do not re-explain the product, the market,
  or the team. The audience for that context is the
  founder-narrative (chapter 05); the update assumes it.

## What good looks like

A template file a founder can pick up on the first day of any
month for the next five years and use verbatim. A first update
that fits on one screen, reads in under 90 seconds, and leaves a
reader — a co-founder, a mentor, an eventual investor — with a
specific action they could take (from the asks section) and a
credible picture of the month (because the lowlights are honest
and the highlights are specific).

The most useful signal is that **the lowlights section makes the
founder slightly uncomfortable to send**. Comfortable lowlights
are usually not lowlights; they are highlights re-labelled. A
first update whose lowlights section required an internal
argument to write is usually a first update that will build
credibility fast.

The template you author here is the same template you use for
every future monthly update. The first update fires the monthly
cadence chapter 06 named; every subsequent update runs against
the same template, against the same audience list, on the same
day of the month. That is the whole discipline the module is
installing.
