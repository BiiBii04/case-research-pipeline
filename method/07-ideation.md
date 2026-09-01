---
type: "Method"
title: "Ideate: options across six archetypes, filtered before they are scored"
slug: "ideation"
owner: "Thinh Ngo"
project: "case-research-pipeline"
created: "2026-09-01"
last_updated: "2026-09-01"
status: "active"
summary: "Generating solution candidates aimed at the diagnosed cause, spread across six kinds of answer, then cut by two filters. Produces 05-solutions/candidates.md."
---

# Ideate

## Purpose

Generate options aimed squarely at the root cause, spread wide enough to escape the obvious, then filter them before they reach scoring.

Keep the ambition of this stage honest. Most of the originality was already banked in the diagnosis. What happens here is narrower: make sure you do not tunnel on one kind of answer, and do not settle for something the client has already tried.

**Input:** `04-root-cause/synthesis.md`. Every candidate must trace to a cause named there.

## Generate across the six archetypes

The default failure is three flavours of the same idea, and it is almost always three technology ideas.

Force breadth by generating at least one candidate for each archetype that plausibly fits:

| Archetype | The move |
|---|---|
| **Technology** | A tool, a platform, automation |
| **Process** | Change how the work flows, not what tool runs it |
| **Business model** | Change how value is captured, or who pays |
| **Partnership** | Solve it through somebody else's capability instead of building it |
| **Behavioural** | Change the incentives or the decisions of people, not the systems |
| **Rules or structure** | Use a standard, a contract, a legal form, or an organisational change |

Not every archetype fits every case. Consciously checking each one is what surfaces the option nobody at the client had considered, and it costs two minutes.

## When the obvious answers crowd in

Three techniques that reliably shake something loose:

- **Cross-industry analogy.** How was a structurally similar problem solved somewhere else? Transfer the mechanism, not the surface. Copying the mechanism of how airlines handle perishable inventory is useful. Saying "be the Netflix of X" is not.
- **Constraint inversion.** Name something everyone treats as fixed, then ask what becomes possible if it is not. Half the time the constraint turns out to be a habit.
- **Jobs to be done.** What is the client really hiring a solution to do? Solutions that serve the underlying job beat solutions that serve the stated request, and the gap between those two is often the whole case.

## Two filters, before anything is scored

### The relevance gate, binary

For each candidate: does it attack the named root cause, yes or no?

A no is dropped, or sharpened until it becomes a yes. This stays a gate rather than a scored dimension on purpose. If relevance were tradeable, a clever but off-target idea could bank points elsewhere and float up the ranking. Relevance is the floor every survivor has already cleared.

If nothing gets cut here, the gate was not applied. Generating five ideas that all conveniently pass usually means they were generated to pass.

### The cliché gate

For each survivor: **would a company this size already have considered this? If yes, why has it not worked for them, or what makes ours materially different?**

A candidate that cannot answer gets cut or sharpened until it can.

This is the first question a panel asks, so answering it here is rehearsal rather than paperwork. And note what the gate is actually testing. A common-looking play that survives with a sharp answer is completely fine. Being unusual is not the goal. Having an answer is.

## The gate

1. Do the candidates span several archetypes, or are they variations on one?
2. Did the relevance gate actually cut anything?
3. Can every survivor answer the cliché question in one sentence?

## Output: 05-solutions/candidates.md

```
> OFFICIAL FILE for the Ideate stage. Drafts live in drafts/.

# Solution candidates: {case name}

## Candidates
{for each: name, archetype, the cause it targets, two lines on how it works, and its answer to the cliché question}

## Cut, and why
{candidates that failed the relevance gate, with the reason}
```

Survivors go to `method/08-scoring.md`.
