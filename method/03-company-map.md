---
type: "Method"
title: "The company map: eight slices, their boundaries, and how findings get routed"
slug: "company-map"
owner: "Thinh Ngo"
project: "case-research-pipeline"
created: "2026-09-01"
last_updated: "2026-09-01"
status: "active"
summary: "The fixed decomposition the research stage fans out on, so every fact has exactly one home and cross-slice findings get routed instead of lost."
---

# The company map

## Why the topic list is fixed

A company is too large to research as one question, and inventing a fresh topic list for every case has two failure modes. Topics overlap, so two agents research the same thing and produce two slightly different versions of one fact. Or topics leave a hole, and nobody researches the part that turns out to matter.

So the decomposition is fixed. Eight slices, chosen to cover a business of any shape, each declaring what it owns and what its neighbours own. Every fact then has exactly one home, which is what makes contradictions findable: two files claiming the same fact is a structural bug you can see.

The frame decides how deep each slice is cut. It does not decide which slices exist.

## The eight slices

| # | Slice | The question it answers | Where the sharp findings usually are |
|---|---|---|---|
| 1 | **Bet** | What is the company betting on, why now, and what has to be true for the bet to work? | The assumptions nobody inside the company states out loud any more |
| 2 | **Entity** | What is this thing? Ownership, structure, history, footprint, and where the money comes from and goes. | The gap between the entity people describe and the entity on the filings |
| 3 | **Offer** | What does it actually sell, and how does that differ from what it markets? | Anywhere the marketing layer and the shipping layer disagree |
| 4 | **Customers** | Who buys, why, what job are they really hiring it for, and how many are there? | The buyer the company thinks it has versus the buyer it has |
| 5 | **Rivals** | Who else is in the ring, and where is this company exposed? | Advantages that are asserted rather than demonstrated |
| 6 | **Machine** | How does it physically run? Supply chain, network, assets, systems, the operational plumbing. | Constraints that are structural and therefore not fixable by a campaign |
| 7 | **Rules** | What regulation, licensing, tax and policy does it sit inside? | Constraints the company treats as fixed that are not, and the reverse |
| 8 | **People** | Who runs it, who is being hired, and what does that pattern signal? | Where the org chart contradicts the stated strategy |

## The ninth agent: the skeptic

Alongside the eight runs one agent with no subject of its own. Its only job is to find evidence that the governing hypothesis is wrong.

Without it, research becomes an expensive way of agreeing with yourself: you look for support, you find support, and the fact that would have killed your story never gets searched for. **A skeptic that comes back with nothing is a warning sign, not a clean bill of health.** It usually means the instruction was too vague or the agent went through the motions. Re-run it with a sharper target.

## Slices 6 and 7 are the ones people drop

Most published research templates were written for young software companies, where the interesting questions are the bet, the product, the buyers and the moat. Machine and Rules barely matter there.

For an asset-heavy, regulated, or physically distributed business, they are where the answer usually lives. A retailer's problem is often in its supply chain or its property position. A financial services problem is often in a licensing rule. If you drop those slices because a template did not have them, you will spend your case describing a marketing problem that is actually a logistics problem.

The Cynefin call from framing decides depth per slice. It does not license deleting one.

## Where "what is happening right now" lives

There is no separate timeline slice. Each slice carries a short "what changed recently" section, and Entity owns the overall timeline.

The timing read is a separate thing from the event, and it belongs where the event does. A funding round is an Entity fact. Reading that round as pre-emptive positioning is an Entity inference. A competitor's round is a Rivals fact, even if you found it while researching something else.

## Ownership boundaries

Every slice file opens with a header:

```
**Owns (single source of truth):** the facts this file is the home for.
**Does not own:** each adjacent slice, and which file owns it instead.
```

This does three jobs. It stops any one file bloating into an everything-document. It makes contradictions findable. And it forces the routing step below, because when a boundary is explicit, a finding that belongs elsewhere is recognisable at the moment you find it.

Boundary calls that come up constantly:

| Finding | Owner | Not |
|---|---|---|
| A rival's funding or expansion | Rivals | Entity, even though it is a corporate fact |
| The company's own funding | Entity | Rivals |
| A leader's public claim about the product | Offer owns whether the claim is true | People owns that they said it and what that signals |
| A tax or licensing constraint that shapes the network | Rules owns the constraint | Machine owns what it does to operations |
| A supplier relationship that is also a shareholding | Entity owns the shareholding | Machine owns the supply dependency |

When in doubt, ask which file a reader would open to look this up. That file owns it.

## Routing findings between slices

After a slice is written, walk **all eight slices by name** and ask, for each: what did I find that this other slice owns?

The walk has to name every slice out loud. The same boundaries that keep files clean also hide cross-findings from a lazy self-scan, which is why a general "anything else?" does not work.

Each net-new finding becomes one small file in the destination slice's queue:

```
03-research/<slice>/inbound/
├── pending/    one file per routed finding, waiting to be absorbed
└── archive/    absorbed, moved here after integration
```

One file per finding: a headline, one or two sentences, the citation, and which slice sent it. Nobody edits somebody else's entry. Absorbing is a move from `pending/` to `archive/`, which doubles as the audit trail.

Apply the drop test before routing: if the destination slice's own research would obviously find this anyway, do not route it.

Two paths:

- **Forward**, when the destination slice is not written yet. The entry waits and gets absorbed when that slice starts.
- **Backflow**, when the destination is already written. Drain it at the end of the same session: absorb it into the owning section, merge the reference list, assign the tag yourself, move the file to `archive/`.

Keep a one-line log of every backflow in `00-state.md`. It is the record that answers "did that correction actually land everywhere?", which is a question you will ask.

## The People boundary

Public professional signal only.

**In scope:** the public org structure, hiring patterns and what they suggest, published talks and posts, stated professional history once verified.

**Out of scope:** guessed-at private psychology presented as a finding, personal life, anything that reads as surveillance rather than research.

The test: if this person read the file, would it look like serious professional work, or would it put them on guard? Research that fails that test is worse than useless, because it damages the relationship the research was meant to serve.
