---
module: mod-001-how-startups-work
exercise: exercise-05
slug: three-failure-post-mortems-teardown
hours: 2
prereqs: [chapter-06-failure-post-mortems-and-the-graph, chapter-03-graham-heuristics]
---

# Exercise 05 — Three Failure Post-Mortems — Teardown

## Problem statement

Chapter 06 argued that failure post-mortems are the honest source and that
each failure can be classified onto the seven-layer graph — problem,
solution, market, business model, GTM, capital structure, team. This
exercise makes you do it: read three real failure post-mortems and
classify them on both the seven-layer graph and the cluster taxonomy of
Graham's 18 mistakes (chapter 03).

The output should sharpen the classification vocabulary and, more
importantly, give you a working prior for *which failures cluster where*
across many companies.

## Requirements

1. **Pick three failure post-mortems to read.** All three must be primary
   sources — either the failed founder's own writeup or a substantive
   investor writeup (e.g., a Founder Collective mortema). Do not use
   third-party summary articles.

   Requirements for the selection:
   - **At least one from a startup that failed at the problem or
     solution layer.** These are typically early failures — the product
     existed, the users didn't want it.
   - **At least one from a startup that failed at the market, business
     model, or GTM layer.** These are typically later failures — the
     product existed, users wanted it, but the money didn't work out or
     the distribution never opened.
   - **At least one from a startup that failed at the capital-structure
     or team layer.** These are the failures the founder often
     underplays but the investor writeup exposes.

   Suggested starting places (each of these has published, primary-source
   post-mortems):
   - The CB Insights "Startup Failure Post-Mortems" collection —
     <https://www.cbinsights.com/research/startup-failure-post-mortem/>
     (curated links to hundreds of founder-written writeups).
   - The Founder Collective "Mortemas" writeups —
     <https://foundercollective.com> (search their blog for the mortemas
     series).
   - Individual founder-written post-mortems from failed startups such as
     Everpix, Pebble, Quibi, Homejoy, Juicero, and many others — search
     for "[company name] post-mortem" and prefer the founder's own
     account.

   <!-- needs-research: verify the CB Insights and Founder Collective landing-page URLs at exercise-authoring time; both firms restructure their content periodically. If a URL 404s, do a fresh search for the current landing page. -->

2. **For each of the three post-mortems, produce a teardown** with the
   following sections:

   - **Company at a glance.** Name, one-line description of what they
     did, year founded → year shut down, roughly how much they raised
     (if publicly known), team size at peak, and how you found the
     post-mortem.
   - **The founder's stated cause of failure.** In 2–3 sentences,
     summarize what the founder or the writeup says killed the company.
     Quote the sharpest sentence directly.
   - **Surface classification (graph layer).** Which of the seven graph
     layers does the failure most obviously map onto? Justify in one
     sentence.
   - **Root-cause tracing.** Follow the chain of because-becauses to
     the deepest cause. Usually the surface failure sits on top of one
     or two upstream failures. Trace 2–3 levels deep. This is the most
     important part of the teardown.
   - **18-mistakes cluster mapping.** From the five clusters in chapter
     03 (team, problem/solution, process, commercial, capital), which
     one(s) does this failure match? Name the specific mistake(s) from
     Graham's list if you can identify them.
   - **What Foundations tooling would have caught this early.** In one
     paragraph: if the founder had run the search-status inventory from
     exercise 04, the growth compass from exercise 02, or the diagnostic
     from exercise 01, at what point would each have flagged the
     failure? If the tooling would not have caught it, say so and name
     what would.

3. **Produce a cross-teardown synthesis.** In 300–500 words after the
   three individual teardowns:
   - Which graph layer(s) appeared in more than one teardown? Is that a
     coincidence of your sample or a pattern?
   - Which of Graham's 18 mistakes appeared in more than one teardown?
   - Where did the founder's *stated* cause of failure diverge from the
     *root cause* you traced? This is the most useful pattern to
     identify — founders systematically underrate certain classes of
     failure in their own writeups.
   - What is the one thing you would change in how you spend your week
     — as a founder or a prospective founder — based on the three
     teardowns?

## Deliverable shape

A single Markdown file, structured as follows:

```markdown
# Three Failure Post-Mortems — Teardown

## Teardown 1: <Company Name>

### Company at a glance
...

### The founder's stated cause of failure
...

### Surface classification (graph layer)
...

### Root-cause tracing
1. Surface: ...
2. Because: ...
3. Because: ...
4. Root: ...

### 18-mistakes cluster mapping
...

### What Foundations tooling would have caught this early
...

## Teardown 2: <Company Name>
...

## Teardown 3: <Company Name>
...

## Cross-teardown synthesis
<300–500 words>

## References
- Post-mortem 1: <URL and author>
- Post-mortem 2: ...
- Post-mortem 3: ...
```

Total length: 1500–2500 words including the three teardowns.

## Starter guidance

- **Prefer founder-written post-mortems where possible.** The founder was
  in the room; a third-party summary was not. Investor writeups
  (Founder Collective mortemas) are the second-best source because the
  investor was close to the room. Third-party retrospectives are
  weakest — they tend to over-emphasize whichever narrative caught on.
- **Diversify across sectors and eras.** Three failures all from
  early-2010s consumer social will teach you one thing three times.
  Try to pick from different sectors (consumer, SaaS, hardware,
  marketplace) and different eras.
- **The stated cause is a starting point, not the answer.** Founders
  often attribute failure to whichever cause protects their next thing.
  A founder about to raise a new fund will attribute failure to bad
  market timing; a founder about to become an operator will attribute
  it to execution. Note this bias where you see it.
- **Root-cause tracing is not "everything caused everything."** Force
  yourself to a single chain of 2–3 links. If you cannot name the
  chain, the teardown isn't done.
- **The Foundations-tooling section is a stress test on the module.**
  If Foundations tooling would not have caught the failure, that is
  useful data — say so and name what would have.

## Acceptance criteria

You have completed the exercise when:

- [ ] Three primary-source post-mortems are read.
- [ ] The three cover at least one problem/solution failure, at least
      one market/business-model/GTM failure, and at least one
      capital-structure/team failure.
- [ ] Each teardown has all six sub-sections filled.
- [ ] Each root-cause tracing goes at least 2 levels deep with an
      identified root.
- [ ] The 18-mistakes cluster mapping references specific mistakes from
      Graham's list where identifiable.
- [ ] The cross-teardown synthesis identifies at least one recurring
      pattern and one systematic founder bias.
- [ ] All three post-mortems are cited with URL and author in the
      references section.
- [ ] The file is committed as
      `mod-001-exercise-05-three-post-mortems-teardown.md`.

## Common failure modes to avoid

- Using three post-mortems that all failed for the same reason.
  Diversify.
- Using summary articles instead of primary sources. The primary source
  is what makes the exercise honest.
- Accepting the founder's stated cause at face value. Trace deeper.
- Skipping the Foundations-tooling section. It is the part that closes
  the loop back to the rest of the module.
- Writing three unrelated book reports rather than a comparative
  teardown. The cross-teardown synthesis is where the compounding value
  is.

## What good looks like

A teardown that a fellow learner could read and use as a warning-signs
catalogue. The individual teardowns should be specific enough that the
learner recognizes the shape of the failure; the synthesis should be
general enough that they can carry the pattern into their own work.

You will reuse the seven-layer classification and the 18-mistakes cluster
mapping in project-003 (`Two-Slide Startup Diagnostic — What Stage Am I,
and What Kills Me First`), where the "kill-me-first" slide draws directly
on the pattern set built here.
