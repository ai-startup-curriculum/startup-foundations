---
module: mod-001-how-startups-work
exercise: exercise-01
slug: startup-vs-not-startup-diagnostic
hours: 2
prereqs: [chapter-01-what-is-a-startup]
---

# Exercise 01 — Startup vs Not-a-Startup Diagnostic

## Problem statement

Chapter 01 installed a definition of a startup (a temporary organization
searching for a repeatable, scalable business model under uncertainty) and
four contrasts (small business, consulting project, lifestyle business,
research program). This exercise makes sure you can *apply* the definition
under load — quickly, honestly, and against real cases.

You will run the chapter-01 diagnostic against **six candidate businesses**,
classify each one, and write the reasoning. The point is not to get "right"
answers (the answer depends on details) — it is to force the reasoning to be
explicit and the four contrasts to become second nature.

## Requirements

1. Pick **six candidate businesses** to classify. At least four should come
   from the list below; you may substitute the remaining two with real
   businesses you know personally, or with well-documented public ones.

   Suggested candidates (pick at least four):

   - A profitable single-city artisanal coffee-roaster with 4 employees and
     one location that the founder wants to keep at one location forever.
   - A two-person software agency that builds custom Salesforce integrations
     for enterprise clients, charging by the project.
   - A newly-incorporated developer-tools company that has raised US$1.5M on
     a SAFE, has one product in closed beta, and is talking to 30 target
     customers a week.
   - A one-person independent Substack newsletter whose author makes a
     comfortable living from paid subscriptions and refuses sponsorships to
     keep editorial control.
   - A university research group building a novel protein-folding algorithm,
     funded on a 4-year NSF grant, with no commercialization plans.
   - A three-person biotech startup working from a university-adjacent lab,
     with $500k in seed funding and one drug candidate in preclinical
     testing.
   - A regional franchise operator that owns 12 quick-service restaurant
     locations and plans to open 4 more per year within the state.
   - A vertical SaaS company selling scheduling software to independent dog
     groomers, growing 6% week-over-week from a small user base, having
     raised a US$3M seed round.

2. For each candidate, run the **four-question diagnostic** from chapter 01
   and record the answers:
   - Is there already a proven business model to copy?
   - Does serving customer #10 still require founder hand-work?
   - Is the founder trading outcome size for lifestyle?
   - Is the goal knowledge rather than a scalable revenue business?

3. Produce a **classification** for each candidate — startup, small business,
   consulting project, lifestyle business, research program, or "not
   classifiable without more information."

4. For each candidate, write a **one-paragraph justification** (3–5
   sentences) explaining which of the four contrasts was decisive and why.
   If the classification depended on information you don't have, name the
   specific fact you would need to be sure.

5. Produce a **summary table** at the top of the deliverable in the shape
   below.

## Deliverable shape

A single Markdown file. Structure:

```markdown
# Startup vs Not-a-Startup — Diagnostic

## Summary table

| # | Candidate (short name) | Classification | Deciding contrast |
|---|---|---|---|
| 1 | ... | ... | ... |
| 2 | ... | ... | ... |
...

## 1. <Candidate 1 short name>

**Description:** <one-line description of the candidate>

**Four-question diagnostic:**
- Proven model to copy? ...
- Founder hand-work at customer #10? ...
- Trading outcome for lifestyle? ...
- Goal is knowledge? ...

**Classification:** ...

**Justification:** <one paragraph>

## 2. <Candidate 2>
...
```

Repeat sections 1–6 for all six candidates.

## Starter guidance

- **The four questions are ordered by decisiveness.** If a "yes" to the
  first question settles it (there is already a proven model — this is a
  small business), you don't need to work through the others. But *write
  them all anyway* for this exercise — the discipline is the point.
- **Ambiguous cases are the interesting ones.** The biotech example, the
  vertical SaaS example, and the franchise operator are all deliberately
  ambiguous. Write the ambiguity, don't hide it.
- **"Both" is often the honest answer at a moment in time.** A university
  research group can *become* a startup at the moment it spins out. A
  lifestyle business can become a startup the day the founder decides to
  raise money and scale. Note when a classification is conditional on the
  founder's future intent.
- **The four contrasts are not a moral ranking.** Consulting, lifestyle,
  and research are all excellent things to run. The classification tells
  you what *methodology* to apply, not whether the business is good.
- **Do not use Foundations tools where they don't apply.** If you classify
  something as a small business, you would not build it a runway model in
  the mod-005 sense — that would be category confusion. Say so
  explicitly in the justification if it applies.

## Acceptance criteria

You have completed the exercise when:

- [ ] Six candidates are classified, at least four from the suggested list.
- [ ] Each candidate has all four diagnostic questions answered explicitly.
- [ ] Each candidate has a one-paragraph justification naming the deciding
      contrast.
- [ ] The summary table at the top matches the per-candidate sections
      (same names, same classifications).
- [ ] At least one candidate is classified as ambiguous or conditional, with
      the specific missing fact named.
- [ ] For each candidate you would classify as *startup*, you have named
      which of the five searches from chapter 05 (problem, solution, market,
      business model, team) is the primary open one right now. (This is a
      cross-chapter check — do not skip it.)
- [ ] The file is committed to your notes with the filename
      `mod-001-exercise-01-startup-vs-not-startup.md`.

## Common failure modes to avoid

- Classifying everything as a startup because "the founder is ambitious."
  Ambition is not a classification criterion; scalable business model
  search is.
- Classifying an early-stage business as "not a startup" because it hasn't
  proven the model yet. That's the *whole point* of the startup phase —
  they haven't found it. The classification is about intent and structure,
  not about proof.
- Refusing to classify at all because "it depends." Force yourself to make
  the call, then name the caveat.
- Skipping the justification. The justification is the exercise.

## What good looks like

A completed diagnostic that a co-founder could read in five minutes and
walk away with a clear, defensible classification for each of the six
candidates plus the reasoning. If the co-founder disagrees with any
specific classification, they can point to the deciding contrast and
argue about *that*, rather than about vibes.

You will reuse this diagnostic for the rest of Foundations and for every
downstream pillar. It is the smallest test that stops you from applying
startup tooling to a non-startup.
