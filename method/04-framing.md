---
type: "Method"
title: "Frame: carve the problem, set the effort level, write a guess that can be wrong"
slug: "framing"
owner: "Thinh Ngo"
project: "case-research-pipeline"
created: "2026-09-01"
last_updated: "2026-09-01"
status: "active"
summary: "Scout sweep, issue tree, the Cynefin throttle, stated ask versus real problem, and the governing hypothesis. Produces 02-frame.md."
---

# Frame

## Purpose

Turn a raw case into a sharp frame before any deep research runs. Everything downstream inherits this, so a lazy frame poisons the whole pipeline.

This is also where the anti-cliché engine starts up. The better the problem is defined here, the faster the obvious solutions stop fitting later.

**Input:** `01-brief.md`, the digested brief and judging criteria. Read it fully first.

## 1. Scout, then carve

Do not carve the problem into branches while blind.

Run a quick, broad, shallow pass first. Read the brief closely and do a light Exa scan to learn the terrain: the industry, the obvious forces, what has happened around this company recently. The goal is orientation, not depth. A page of notes is enough.

Then carve. Carving before any evidence is the weakness this step exists to fix.

## 2. Build the issue tree

Break the problem into branches, and hold the split to two tests:

- **No overlap.** No two branches cover the same ground. A split that double-counts sends two agents to research one thing.
- **No gap.** Together the branches cover the whole problem. A split with a hole sends nobody to research the part that matters.

Write the tree out explicitly in the frame file. A tree you can see is a tree someone can argue with, and someone should.

## 3. Cynefin triage: this sets the throttle

Classify the problem, because this decides how hard everything downstream runs.

| Domain | What it means | How the pipeline runs |
|---|---|---|
| **Clear** | Known problem, known answer, best practice applies | Run very light. The value is in execution, not diagnosis. |
| **Complicated** | Cause and effect are knowable, an expert could diagnose it | Fewer slices cut deep, light competing-hypotheses table, contrarian pass as a paragraph |
| **Complex** | Cause and effect only make sense in hindsight, the system is tangled | All eight slices, full evidence matrix, contrarian pass as a separate fresh-context agent |
| **Chaotic** | No stable patterns to research | Stabilise and reframe before researching anything |

Record the call, and record what it implies: how many slices get a deep cut, and which analysis machinery runs in full.

This is the effort governor. It is how the work stays proportional to the case instead of running everything at maximum for a simple problem, and skipping it is the most common way to waste a week here.

## 4. Separate the stated ask from the real problem

The brief says what the client thinks they want. That is rarely the problem.

Name both, side by side: the stated ask, and your read of the underlying problem. Then write the decision this whole pipeline exists to make, in one sentence, and lock it into `00-state.md`.

If the decision changes later, that is a major event. It invalidates downstream work and it gets logged, not quietly absorbed.

## 5. Write the governing hypothesis

One sentence saying what you think the real cause is, written so it could be proven wrong.

"Costs are too high" cannot be proven wrong and is useless. "The loss sits in ground rent rather than in operating margin" can be checked against a filing, and checking it either way moves the case forward.

List two or three competing explanations still alive alongside it. Those become the columns of the evidence matrix in the root-cause stage, so writing them now saves work later.

The hypothesis is frozen for the length of a research wave, so the fan-out has a steady aim. It is revisable between waves when the skeptic surfaces something that kills it. Frozen in a wave, revisable between waves, and every revision logged.

## 6. Set the research depth per slice

The eight slices in `method/03-company-map.md` all run. The frame decides which get a deep cut and which get one pass.

Write that allocation into the frame file. An agent given "research the Machine slice" with no depth guidance will either skim it or spend the whole budget on it.

## The gate

Before marking Frame cleared, put these in writing:

1. **Is the problem statement the symptom or the cause?** Push until it is plausibly the cause, or until it is explicitly labelled as a hypothesis to be tested.
2. **Does the tree overlap or leave a gap?** Name the branch you are least sure about.
3. **Is the hypothesis falsifiable, or is it mush?** If you cannot say what evidence would kill it, rewrite it.
4. **Is the Cynefin call honest, or did it get set to Complex because that feels more serious?** Over-classifying is the expensive mistake.

Log anything unresolved to Open tensions in `00-state.md`.

## Output: 02-frame.md

```
> OFFICIAL FILE for the Frame stage. Drafts live in drafts/.

# Frame: {case name}

## Lay of the land
{scout notes: the terrain, the forces, what has happened recently}

## Issue tree
{the decomposition, as a nested list, with the no-overlap and no-gap check stated}

## Cynefin call
{domain, plus what it implies for depth and for which machinery runs}

## Stated ask versus real problem
{both, side by side}

## The decision to be made
{one sentence}

## Governing hypothesis
{one falsifiable statement}

## Competing explanations still alive
{two or three, these become matrix columns later}

## Research allocation
{which of the eight slices get a deep cut, which get one pass, and why}
```
