---
type: "Method"
title: "The spine: stages, gates, and the rules that apply everywhere"
slug: "spine"
owner: "Thinh Ngo"
project: "case-research-pipeline"
created: "2026-09-01"
last_updated: "2026-09-01"
status: "active"
summary: "The stage sequence, the gate at the end of each stage, the state file, and the conventions every stage inherits. Read this first on any case."
---

# The spine

## The four beliefs this is built on

**Research serves a decision, never the reverse.** Unbounded research is the enemy of good case work. Every research thread names the question or the hypothesis it tests. No question, no thread.

**Differentiation comes from a sharper diagnosis, not from a creativity module.** The obvious solutions are obvious because they answer a shallow reading of the problem. Push the cause deeper and the tired solutions stop fitting, because they were aimed at a symptom you have already ruled out. So the stage that produces original answers is Root cause, not Ideate.

**Fixed gates, flexible path.** The stages are a fixed spine. Movement between them is free: loop back, go deep then shallow, reopen the frame when research surprises you. What stays rigid is the gate at the end of each stage. You wander, but to advance you clear the bar.

**Challenge is the service.** The user asked to be pushed, not agreed with. At every gate, put the strongest case against the current conclusion in writing. A weak point let through here is a question that lands in the room later.

## Phase 0: Scope

Before any search, write three things into `00-state.md`:

- **Why** this case is being worked, and what changes depending on the answer.
- **What decision** the work feeds, in one sentence, and by when.
- **Your prior**: what you currently believe about this company and this problem, stated plainly.

The prior is the one people skip. Writing down what you already think, before you look, is the cheapest defense against spending two weeks building an elaborate case for your first instinct. You will test it, not protect it.

## The stages

| Stage | Official file | The gate |
|---|---|---|
| 1. Frame | `02-frame.md` | The problem statement survives "is that the symptom or the cause?". The decision is named. The issue tree passes the no-overlap-no-gap test. A falsifiable hypothesis exists. |
| 2. Research | `03-research/synthesis.md` | Every branch of the tree is covered. The skeptic found something real. Citations verified in fresh context. |
| 3. Root cause | `04-root-cause/synthesis.md` | Two or more lenses ran. Surviving causes have evidence that discriminates, not just evidence that agrees. Killed causes are on record with what killed them. |
| 4. Ideate | `05-solutions/candidates.md` | Candidates span several archetypes. The relevance gate cut something. |
| 5. Score | `05-solutions/scored-shortlist.md` | Anchors were tuned to this client before scoring. Every score points at a written descriptor. Options are sorted into bands. |
| 6. Decide | `06-decision.md` | One choice, its criteria, its tradeoffs, and why each rejected option lost. |
| 7. Defend | `07-defense.md` | Every open tension has a prepared answer. The single weakest point is named honestly. The condition that would change your mind is written down. |

## The Decide stage in full

It has no separate method file because the method is short.

Pick one option. Write the criteria that decided it, in the order they mattered. Name what you are giving up, because every real choice costs something and a recommendation with no stated cost reads as unexamined. Then list each rejected alternative with the dimension it lost on, pulled from the scored shortlist.

One rule: the decision is written by the user, in the main conversation. Not delegated.

## The official file rule

Each stage has exactly one file that counts, named in the table above. Drafts and intermediate work live in a `drafts/` folder beneath it.

The official file is the single source of truth for that stage: the only thing the next stage reads, and the only thing the user has to review before advancing. Put a banner at the top of every one:

```
> OFFICIAL FILE for the {stage} stage. Drafts live in drafts/.
```

A gate cannot clear until the official file exists and the user has read it. This is the consolidation checkpoint and it is not optional, because skipping it is how work fragments across sessions.

Call it official, not final. A later insight can change it. Update the file and log the change in `00-state.md`. There is always exactly one official file per stage, and it can be revised.

## The state file

`00-state.md`, built from `templates/state.md`, is read first at the start of every session and updated last at the end.

A cold session with no memory reads this one file and knows the decision, what is locked, what is contested, and the next action. If that is not true, the file is not doing its job.

Four sections carry the weight:

- **Decided and locked** is append-only. Each row is a conclusion that passed its gate and that later stages may build on without re-litigating. Do not quietly delete a row. If a locked decision is overturned, strike it and add a new row saying why, so the reasoning trail survives.
- **Open tensions** holds unresolved disagreements from the gates. Anything that did not resolve lands here instead of vanishing.
- **Live insights** is the loop-back valve. Any stage can write to it. Framing and Root cause re-read it. This is what keeps the pipeline from being a one-way conveyor.
- **Next action** is one concrete step, specific enough that a cold session acts without asking.

## Challenge at every gate

Before marking any gate cleared, write out three things:

1. The strongest argument against the current conclusion.
2. At least one competing option or hypothesis still alive.
3. The specific evidence that would change the call.

Do not advance until the user engages with it. If a disagreement does not resolve, log it to Open tensions rather than letting it disappear. These are the exact places a panel probes, so tracking them is preparation, not paperwork.

## Waves, and append-first research

Research runs in waves, never one shot. Before a wave runs, name its trigger:

- **Baseline**: cover every slice for the first time.
- **Gap-fill**: a later stage exposed a specific hole. The wave targets only that hole.
- **Refresh**: new information appeared, or the case resurfaced after time.

A wave appends to existing files with new sources. It never overwrites. The synthesis regenerates after each wave. Every wave is logged.

A wave stops when it comes back dry, meaning it turns up nothing materially new. Dry is the saturation signal. There is no fixed source quota. Purpose-tied in, dry-stop out.

## Session pacing

One heavy stage per session. A document written at the tail of a long session degrades in ways you can see afterwards: tags get sloppy, contradictions get resolved instead of surfaced, and the routing step at the end gets skipped. If a session runs long, stop before the writing step and write fresh.

At the end of every session, update `00-state.md` and drain any pending cross-slice findings. Both take five minutes and both are the reason the next session starts instead of restarting.

## Effort is throttled, not maximal

The Cynefin call in `method/04-framing.md` sets how hard everything downstream runs: how many slices get a deep cut, whether the full competing-hypotheses matrix is built or a light table is enough, whether the contrarian pass runs as a separate agent or as a paragraph.

Running the full machinery on a simple problem burns a week and buys nothing. Skipping the throttle is the most common way to waste time with this method.
