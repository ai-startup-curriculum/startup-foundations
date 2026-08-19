---
module: mod-001-how-startups-work
exercise: exercise-04
slug: the-search-model-of-founder-work
hours: 2
prereqs: [chapter-05-founder-work-as-search]
---

# Exercise 04 — The Search Model of Founder Work

## Problem statement

Chapter 05 decomposed Blank's "search for a repeatable and scalable
business model" into five sub-searches — problem, solution, market,
business model, team — and argued that a founder's most useful weekly
question is *which of these is currently binding?*

This exercise makes you apply the search model to one real (or realistic)
startup and produce a **search-status inventory**: what is open, what has
evidence, what is being neglected, and what is being run in the wrong
order.

The output is a working artifact you should be able to keep updating; it
is essentially the search-tracker version of a project status page.

## Requirements

1. **Pick one startup.** Options in order of preference:
   - Your own startup, if you're actively working on one.
   - A well-documented public startup at the seed or Series A stage (an
     early Y Combinator batch member, an early Stripe / Airbnb / Notion /
     Figma before their IPO, etc.). Pick one you can find substantial
     public writing about.
   - A realistic hypothetical startup you compose for this exercise. If
     you go this route, write a one-paragraph fact sheet at the top of
     the deliverable — company name, product, target user, current stage,
     current cash on hand, team size, months of operation, current
     week-over-week growth rate if applicable.

2. **Produce the search-status inventory table** with one row per
   sub-search:

   | Search | Status | Evidence | Binding this week? | Owner | Next test |
   |---|---|---|---|---|---|
   | Problem | | | | | |
   | Solution | | | | | |
   | Market | | | | | |
   | Business model | | | | | |
   | Team | | | | | |

   For each row:
   - **Status.** One of: `not started`, `open — no evidence`, `open —
     partial evidence`, `open — strong evidence`, `closed (validated)`,
     `closed (invalidated — pivoted)`. Be specific about which.
   - **Evidence.** One or two sentences on the concrete evidence backing
     the status. "We think" or "we feel" is not evidence. Named
     customers, dated conversations, revenue numbers, deployed MVPs,
     signed contracts, retention numbers, etc.
   - **Binding this week?** Yes / no. If yes, this is the search the
     founder's week should be organized around.
   - **Owner.** Which specific person on the team is running this search.
     "The team" is not an owner. "The founder" is only an owner if it is
     literally the founder alone.
   - **Next test.** One sentence naming the specific experiment or
     conversation that would move the search forward this week or next.

3. **Write the diagnosis section.** In 200–400 words, answer:
   - Which search *should* be binding right now given the stage of the
     startup (use the stage → search table in chapter 05)?
   - Which search *actually* has the founder's attention this week?
   - If those are different, why? And what should change?
   - Are any downstream searches being run before an upstream one has
     evidence? (E.g., is business-model work happening before the market
     search has evidence?) If so, name the specific mismatch.
   - Are any searches genuinely closed, or are they "closed" only in the
     sense that the founder stopped asking?

4. **Write the "what would evidence look like" section.** For at least
   the currently-binding search, describe in 3–5 sentences the exact
   evidence that would let you mark that search `closed (validated)`.
   Be specific: numbers, customer names, conversation counts, product
   usage patterns. This is the acceptance criterion for the search.

5. **Cross-reference with growth.** In one paragraph, answer: which of
   the five searches is your current weekly growth rate (or absence of
   one) most diagnostic of? Refer back to the annotation you produced in
   exercise 02.

## Deliverable shape

A single Markdown file. Suggested structure:

```markdown
# Search-Status Inventory — <Startup Name>

## Startup at a glance
<one paragraph — product, users, stage, cash, team size, months, growth if applicable>

## Inventory table
<the six-column table with all five sub-searches filled>

## Diagnosis
<200–400 words>

## Evidence that would close the currently-binding search
<3–5 sentences>

## What growth is telling us
<one paragraph, cross-referenced with exercise 02>
```

Total length: 600–1200 words plus the table.

## Starter guidance

- **Be honest, not aspirational.** If the "market" search has been open
  for eight months with no evidence, write that. The value of this
  artifact is that it tells you what you're avoiding, not what you're
  proud of.
- **The five searches usually have several open at once.** That's
  normal. What matters is that at any moment, one is *binding* — the
  founder's attention should be on it above all others, because closing
  it unlocks the next one.
- **Team is always partially open.** Even the best team is one departure
  away from becoming a problem. Do not mark team `closed`; the honest
  status is usually `open — strong evidence` at best.
- **"Closed" does not mean "solved forever."** It means "current
  evidence supports the hypothesis and we can move on." A closed search
  can re-open when new evidence contradicts it. Note in the diagnosis
  section if any historically-closed search is drifting back open.
- **Evidence must be nameable.** "We spoke to lots of customers" is not
  evidence. "We spoke to 22 target customers between May and July, 17 of
  whom described the problem in similar language" is. Force yourself to
  the specific.
- **The Next test column is the operating value of this artifact.** If
  every row has a plausible Next test, you have an operating plan for the
  next few weeks. If several rows say "not sure," those are the searches
  where the founder needs to design an experiment.

## Acceptance criteria

You have completed the exercise when:

- [ ] One specific startup is chosen and the fact sheet is written.
- [ ] The inventory table has all five sub-searches filled with all six
      columns populated.
- [ ] Each `Evidence` cell names concrete evidence (or explicitly says
      there is none).
- [ ] Exactly one search is marked `Binding this week? Yes` in the
      table. (More than one means you haven't picked the binding one.)
- [ ] The diagnosis section addresses stage-fit mismatch, ordering
      mismatch, and whether any "closed" searches are actually just
      neglected.
- [ ] The evidence-that-would-close-the-binding-search section is
      specific and testable within weeks, not months.
- [ ] The growth cross-reference paragraph is present.
- [ ] The file is committed as
      `mod-001-exercise-04-search-status-inventory.md`.

## Common failure modes to avoid

- Marking three or four searches as binding this week. If everything is
  binding, nothing is. Pick one.
- Filling `Evidence` with vibes ("looks strong," "getting good signal").
  Force specifics.
- Skipping the ordering-mismatch check. Founders love to work on the
  interesting search (usually solution or business model) instead of the
  binding one (usually problem, at the stage when problem is binding).
  The exercise is designed to expose that.
- Treating the artifact as a one-shot. Keep it in your notes and update
  it weekly. It works with the mod-004 operating loop.
- Choosing a public company that already exited. You need a company
  where the searches are or were live, so you can honestly assess.
  Post-hoc reconstruction of a mature company's search history is a
  different exercise.

## What good looks like

A search-status inventory that a co-founder could read in three minutes
and know exactly what the founder's week should be organized around,
where the weakest evidence is, and which experiment would move the
company forward the fastest. If the current stage and the currently-binding
search disagree, the diagnosis section names the disagreement and
recommends the fix.

You will reuse this inventory shape in mod-004's operating loop, where the
weekly plan is essentially "advance the binding search this week."
