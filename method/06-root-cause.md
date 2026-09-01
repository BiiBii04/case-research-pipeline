---
type: "Method"
title: "Root cause: test the explanations against each other, then attack the winner"
slug: "root-cause"
owner: "Thinh Ngo"
project: "case-research-pipeline"
created: "2026-09-01"
last_updated: "2026-09-01"
status: "active"
summary: "Diagnostic lenses, the competing-hypotheses matrix, and the mandatory contrarian pass. This is the stage that kills the obvious solutions. Produces 04-root-cause/synthesis.md."
---

# Root cause

## Purpose

Move from "here is everything we found" to "here is what is actually driving this, and here is why the alternatives are not."

This stage is the hinge of the pipeline and the real source of original answers. When the true cause is named and the surface-level causes are explicitly ruled out, the obvious solutions die here, because they were aimed at things you have just dismissed with evidence.

**Inputs:** `03-research/synthesis.md` for the ranked evidence, `02-frame.md` for the hypothesis and its rivals.

## 1. Run at least two lenses

One lens tunnels. Run two or more in `drafts/` and see whether they land in the same place. Pick by fit:

- **Tree drill-down.** Keep splitting down the highest-impact branch until you reach something a client could act on. Good when the problem decomposes cleanly.
- **Five whys.** Ask why repeatedly down a causal chain. Good for process and operational failures.
- **Fishbone.** Sort candidate causes into categories, such as people, process, technology, market and regulation, then check whether a whole category went unexamined. Good when you suspect you are missing a kind of cause rather than a specific one.

Divergence between lenses is a signal, not a failure. If the tree says supply chain and the five whys says incentives, that gap is information, and the file has to explain it rather than pick a favourite quietly.

How many lenses and how deep follows the Cynefin call. Complicated cases may need a tree and a check. Complex cases get everything below.

## 2. The competing-hypotheses matrix

This is the core move, and it runs against instinct.

The ordinary approach is to pick your favourite explanation and look for support. That approach cannot fail, which is exactly the problem: support can be found for almost any story, so finding it tells you nothing.

Instead:

1. **List every explanation still in play.** From the frame, plus anything research surfaced. Include the boring ones and include the client's own theory.
2. **Build the matrix.** Rows are the key pieces of evidence from the synthesis. Columns are the explanations. In each cell, mark whether that evidence is consistent, inconsistent, or not applicable.
3. **Weight by how much a row discriminates.** Evidence consistent with every explanation tells you nothing, no matter how striking it is. Evidence consistent with one and inconsistent with the rest is what carries the decision. Flag those rows.
4. **The survivor is the explanation with the least evidence against it**, not the one with the most evidence for it.

That last inversion is the whole technique. An explanation can have a pile of support and still be dead, because one fact flatly contradicts it, and the ordinary way of working never goes looking for that fact.

For a Complicated case, a light table is enough. For a Complex case, build it out fully. It is expensive and it is the thing that makes the diagnosis defensible.

## 3. The contrarian pass is mandatory

Before locking the leading cause, argue against it on purpose.

Write the strongest possible case that your leading cause is wrong and one of the rejected explanations is right. Not a token objection. The version a hostile expert would make.

For a Complex case, run this as an agent in fresh context, so it is not anchored to the analysis that produced the leading cause.

If the leading cause survives a real attack, it is solid. If it does not, the ranking was premature and you go back to step 2.

## 4. Converge, and write down the dead

Name the surviving cause or causes, each with the evidence that carried it, specifically the rows that discriminated.

Then document every explanation you killed and exactly what killed it.

This is not paperwork. It is the single best answer to "but isn't the real problem X?", because instead of thinking on your feet you are reading: we tested X, here is the evidence inconsistent with it, here is where it failed.

## The gate

1. Did two or more lenses run, and did they converge or diverge? If they diverged, is that explained rather than smoothed over?
2. Does each surviving cause rest on evidence that discriminates, not just evidence that agrees?
3. Did the leading cause survive a genuine attack, or a polite one?
4. **Are the surface-level causes on the killed list?** The ones the obvious solutions would address. If those are still alive, the obvious solutions are still in play, and there is nowhere for an original answer to come from.

Anything unresolved goes to Open tensions.

## Output: 04-root-cause/synthesis.md

```
> OFFICIAL FILE for the Root cause stage. Drafts live in drafts/.

# Root cause: {case name}

## The verdict
{the cause or causes, in one or two sentences, first}

## How we got here
{which lenses ran, what each showed, and how they related}

## The evidence matrix
{explanations as columns, key evidence as rows, discriminating rows flagged}

## Why the alternatives lost
{each killed explanation, and the evidence that killed it}

## The contrarian pass
{the strongest argument against the verdict, and why it did not hold}

## What this constrains
{one line: the kind of solution that could actually address this cause. This is the brief for the next stage.}
```
