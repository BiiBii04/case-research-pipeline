---
type: "Method"
title: "Research: waves, parallel agents, and the skeptic"
slug: "research"
owner: "Thinh Ngo"
project: "case-research-pipeline"
created: "2026-09-01"
last_updated: "2026-09-01"
status: "active"
summary: "How a research wave runs: the fan-out across the eight company slices, the agent contract, the three-tier funnel, and citation verification. Produces 03-research/synthesis.md."
---

# Research

## Purpose

Build the evidence base the diagnosis will stand on. The official file is `03-research/synthesis.md`: one consolidated overview of every slice, with the slices ranked by how strongly each bears on the problem. That ranking is what tells the root-cause stage where to dig first.

**Inputs:** `02-frame.md` for the hypothesis and the depth allocation, `method/03-company-map.md` for the slices, `method/02-evidence-rules.md` for everything about how claims get written.

## Folder layout

```
03-research/
  <slice>/
    draft.md        what the agent wrote for this slice
    inbound/
      pending/      findings routed here by other slices
      archive/      absorbed
  consolidated/     category roll-ups (scratch)
  synthesis.md      OFFICIAL: all slices, ranked
  wave-log.md       every wave, its trigger, what it added
  _sources.md       every source, with its two-axis grade
```

## The wave model

Before a wave runs, write its trigger in `wave-log.md`. Baseline, gap-fill, or refresh. A wave with no named trigger is browsing.

A wave appends to existing drafts with new sources. It never overwrites, because the thing you overwrite is always the thing you needed three weeks later.

After each wave, regenerate `synthesis.md`. A wave stops when it comes back dry.

## The fan-out

Spawn the slices in parallel, in a single message so they run concurrently. One agent per slice, plus the skeptic.

### The agent contract

Every agent gets:

- The slice it owns, and the ownership boundary from `method/03-company-map.md`, so it knows what to route rather than absorb.
- The governing hypothesis. For the skeptic, the instruction to break it.
- The relevant part of `02-frame.md`, and its depth allocation.
- The rules it must follow: Exa only, read load-bearing sources in full at a high character limit, grade every source on both axes, read long files past truncation.
- Where to write: `03-research/<slice>/draft.md`.

Every agent returns:

- A distilled draft, not a raw dump. Distillation inside the agent is what keeps the main conversation from drowning in full text.
- Its graded sources.
- One line on what it could not find, and where it looked. That line is what turns a gap into a target for the next wave instead of a silence.

### How an agent should work inside its slice

Not one batch of searches. A loop, up to three rounds:

1. **Reason.** Name the biggest open gap in this slice right now.
2. **Search.** Two Exa searches and one batched fetch, aimed at that gap.
3. **Reflect.** Record what closed, grade the sources, and test the stop rule.

Stop when you can no longer name a specific unexplored source or angle, when returns are clearly diminishing, or at the three-round cap. That is a named-gap test, not a quality floor: a genuinely thin slice stops honestly at a low grade rather than padding itself.

Round one is the ordinary search anyone would run. The depth comes from rounds two and three, aimed only at what round one left open.

## The skeptic

One agent, no subject, one job: find evidence the governing hypothesis is wrong.

Give it the hypothesis and tell it to break it. Grade what it brings back with the same rigour as everything else, or the whole exercise is theatre.

If it returns nothing, do not treat that as confirmation. Re-run it with a sharper target. A hypothesis nobody could dent in one pass is usually a hypothesis nobody attacked properly.

## The three-tier funnel

1. **Drafts**: raw per-slice output.
2. **Consolidated**: drafts grouped by category and rolled up.
3. **Synthesis**: one official overview.

**Re-ground at the write step.** Compression drifts away from what sources actually said, and a summary of a summary of a summary is fiction with citations attached. When writing `synthesis.md`, go back to the graded sources and check the claims, rather than summarising the summaries.

The synthesis also ranks the slices by how strongly each bears on the problem, with a sentence of justification per slice. That ranking is the handoff to the diagnosis.

## Routing before the wave closes

At the end of the wave, run the routing walk from `method/03-company-map.md`: name all eight slices, and for each ask what you found that it owns. Drop entries into the destination queues. Drain backflow into already-written slices in the same session.

This is the step everyone skips, and skipping it is how a correction lands in one file and not in the three others that repeat the same wrong number.

## Citation verification

Before `synthesis.md` is marked official, run a verification agent in fresh context. Its only job is to confirm each citation exists and says what the synthesis claims.

Fresh context is the point. An agent that did the writing believes its own sources.

Triage what gets re-checked rather than checking everything: a claim earns verification when it is load-bearing **and** it is single-sourced, old, time-sensitive, or of unclear origin.

Per claim, the verifier returns a verdict of confirmed, refuted, or partial, plus the original record it checked against. Use `templates/verification-report.md`.

Two patterns worth stealing:

- **Check against the working system, not the description of it.** A claim about an advantage is not tested against the company's own account of it. It is tested against what rivals actually do today.
- **Positive controls on any absence.** See `method/02-evidence-rules.md`, rule 7.

## The gate

1. **Coverage.** Does the synthesis cover every branch of the issue tree, or are there silent gaps? A gap that nobody wrote down is indistinguishable from a topic with nothing in it.
2. **Disconfirmation.** Did the skeptic actually find something, or go through the motions?
3. **Verification.** Have the load-bearing citations been checked in fresh context?
4. **Tags and scopes.** Does every load-bearing claim carry a tag you assigned, and does every figure carry whose, when, and on what basis?

Anything unresolved goes to Open tensions, or triggers a gap-fill wave.
