---
type: "Method"
title: "Score: five dimensions, anchors tuned to this client, results read as bands"
slug: "scoring"
owner: "Thinh Ngo"
project: "case-research-pipeline"
created: "2026-09-01"
last_updated: "2026-09-01"
status: "active"
summary: "Turning surviving candidates into a defensible ranking, plus an attack note per finalist that doubles as defense preparation. Produces 05-solutions/scored-shortlist.md."
---

# Score

## The principle

The dimensions below do not share a unit. Feasibility and originality are not commensurable, and adding raw scores would hide the exact tradeoff a panel will probe.

So this is not a black-box weighted average. Every dimension is scored against a written descriptor, the order of operations puts relevance and feasibility ahead of cleverness, and originality carries a small weight so it can break a tie but never rescue a weak option or sink a strong one.

The whole point is that a score is attackable. A 2 on feasibility has to point at a specific descriptor and a specific reason, so that anyone can argue with the standard rather than with a hunch.

## Step 0. Tune the anchors to this case

Generic anchors are toothless. Before scoring anything, rewrite each level descriptor against this client's real constraints and the actual judging criteria.

"Feasibility 4" means nothing. "Feasibility 4 for a client with no in-house data team and a six-month window" bites.

Write the tuned anchors into the scoring file, so the scores are reproducible and the standard is visible to anyone who disagrees.

Spend two minutes here. Skipping it is how scoring quietly becomes a vibe with numbers stapled on.

## Step 1. The relevance gate, again

Binary, not scored. Does it attack the root cause, yes or no? A no does not proceed.

It was already applied at ideation. It runs again here because candidates get reshaped between the two stages, and a candidate that drifted off target during sharpening is easy to miss.

## Step 2. Score the survivors

One to five on each dimension, against the tuned anchors.

| Dimension | Default weight | What it measures |
|---|---|---|
| Impact on the root cause | 30% | Does it move the actual driver, and by how much |
| Desirability | 20% | Do the client and the end users want it, and will they adopt it |
| Viability | 20% | Is it economically and strategically sustainable for this business |
| Feasibility | 15% | Can this client actually implement it under real constraints |
| Originality | 15% | Is it non-obvious and defensible, or a play any similar firm already runs |

Weights are editable per case. If the client cares more about implementation risk than novelty, raise feasibility, and say in the file that you did and why.

Weighted score is the sum of level times weight, divided by 100, so it stays on the one to five scale.

### Level anchors, as a starting structure

Tune all of these in step 0.

**Impact on the root cause**
- 5: Removes or neutralises the cause. The effect is structural and lasting.
- 4: Substantially reduces it. Something remains.
- 3: Addresses a real contributor, but not the main driver.
- 2: Touches a symptom near the cause. Cosmetic or short-lived.
- 1: No credible mechanism connects it to the cause.

**Desirability**
- 5: Both the client and the end users want it, with evidence of demand.
- 4: The main stakeholder wants it, mild friction elsewhere.
- 3: Acceptable, but nobody is enthusiastic. Adoption needs pushing.
- 2: A key stakeholder group actively resists.
- 1: Cuts against stakeholder incentives. Likely rejected.

**Viability**
- 5: A self-sustaining case that fits the business model and the strategy.
- 4: Positive on reasonable assumptions, pays back inside the horizon.
- 3: Breaks even, or depends on optimistic assumptions.
- 2: Weak. Needs ongoing subsidy or strains the model.
- 1: No sustainable economics.

**Feasibility**
- 5: Built with existing resources inside the horizon. Precedent exists.
- 4: Needs one new capability or partnership, and it is attainable.
- 3: Needs several new capabilities or real investment. Non-trivial.
- 2: Needs a capability the client lacks and cannot easily get.
- 1: Not implementable under realistic constraints.

**Originality**
- 5: A similar firm would not have got here. A real edge or a genuine insight.
- 4: Recognisable, with an angle competitors miss.
- 3: Fairly common, applied unusually well.
- 2: A standard play most firms would consider.
- 1: Textbook. The client has almost certainly tried it.

## Step 3. The cliché gate on the top scorers

Run it on the leaders only, because it is the question a panel asks first.

Would a company this size already have considered this? If yes, why has it not worked, or what makes ours different? No answer, no place at the top.

This is also why a 1 or a 2 on originality is a warning rather than a death sentence. A common play with a sharp answer to this question is a fine recommendation.

## Step 4. Read the result as bands

Do not read the weighted total to one decimal and crown a winner. That is precision the method does not have, and a panel will find the seam.

Sort the survivors into three bands: clearly strong, contested, clearly weak. The weighted total only separates options **inside** the strong band. The written justification carries the decision; the arithmetic organises it.

Document every rejected option and the dimension it lost on. "Did you consider X?" then has a real answer, with a number and a reason attached.

## Output: 05-solutions/scored-shortlist.md

The tuned anchors, then the table:

| Solution | Impact | Desirability | Viability | Feasibility | Originality | Weighted | Band |
|---|---|---|---|---|---|---|---|
| {name} | {1-5} | {1-5} | {1-5} | {1-5} | {1-5} | {score} | strong / contested / weak |

Then an attack note per finalist:

- The strongest argument a hostile audience makes against this solution.
- Its lowest-scoring dimension, and the specific reason for that score.
- What evidence would raise that score, and whether it is gettable before the deadline.

The attack notes are the bridge to the Defend stage. Every weakness named here is a question already pre-empted there.
