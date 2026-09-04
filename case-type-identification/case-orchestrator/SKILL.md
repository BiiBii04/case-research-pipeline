---
name: case-orchestrator
description: >-
  Run this FIRST, before case-brand-communication, case-profit-optimization, case-supply-chain,
  case-ma, case-product-launch, case-investment, case-market-entry, or any future case-type skill,
  the moment a business case brief is released — this is the front door, not an alternative to
  those skills. Reads the brief once, writes the overall Situation-Complication-Question, segments
  it into its actual sub-questions, and scores each against every case-type checklist to see which
  framework(s) genuinely apply — including mixed briefs where different sub-questions need
  different frameworks, the normal case. Hands off to the matching skill(s) to solve, then
  integrates every sub-answer into one coherent case tied to a shared objective, instead of
  disconnected mini-answers stapled together. Use whenever a brief needs classifying, scoping, or
  triaging before solving — "what kind of case is this," "is this a mixed case," "which framework
  applies to which part," "how do these sub-questions fit together."
---

# Case Orchestrator — Classify, Scope, and Integrate

This skill is the front door for a live case brief. It doesn't solve the case itself — it figures out *which*
framework(s) the case actually needs, which sub-question each one owns, and how to weave their outputs back into
one answer. It exists because real briefs are rarely a pure type, and a team that picks a framework in the first
five minutes and never revisits that choice usually ends up either force-fitting a mismatched framework onto part
of the brief, or answering each sub-question in isolation and stapling the results together at the end — both
read as weaker, less coherent answers to a grader than one that visibly reasoned about case type first.

**Read this whole file before the clock starts on a real brief** — it's short by design so the team can run it
live under time pressure, not study it in advance.

## 1. What this skill owns, and what it hands off

`case-brand-communication`, `case-profit-optimization`, `case-supply-chain`, `case-ma`, `case-product-launch`,
`case-investment`, and `case-market-entry` each carry their own "how this fits with other case-type skills"
section, written as a fallback for when they're
used standalone. Once this skill is loaded alongside them, it owns that integration logic centrally — the
sibling skills' own sections still work (so any one of them is safe to use alone if this one somehow isn't
loaded), but this file is the one source of truth for classification and integration when more than one
case-type skill is in play.

What this skill does NOT do: it does not re-derive or replace any sibling's actual framework (the ten-step
brand-communication method, the profit-tree method, the Demand/Inventory/Supply supply-chain method, the M&A
five-step Objective→Fit→Synergy→Valuation→Alternative method, the four-step product-launch method, the
Finance/Investment case's P&L-read and investment-appraisal formulas, the Market Entry four-step process).
Those live
in the sibling skills' own `SKILL.md` + `references/`, and once a sub-question's type is confirmed, solving it
means reading and following that sibling skill in full — not working from this skill's condensed checklist,
which is deliberately too short to solve anything (see Section 3).

## 2. The process

Run this as a group in the first 15-20 minutes after the brief drops, same time budget the sibling skills assume
for their own Section 2 checklists — this replaces running each sibling's checklist separately, not adds to it.

**Step 1 — Read the whole brief, then write the overall SCQ.** One person reads it aloud, cover to cover,
before anyone proposes a framework — don't let the first reaction anchor the room. Write a brief-level
Situation-Complication-Question and, in one sentence, what the brief is ultimately asking the team to
deliver. This becomes the shared throughline every sub-answer ties back to in Step 6.

**Step 2 — Segment into sub-questions.** List every distinct ask or deliverable the brief actually contains.
Most competition briefs have one to three. A brief with one ask is not automatically a "pure" case — check
Step 3 anyway, since a single ask can still blend signals (e.g. "recommend how to restore profit" can be a
profit-optimization case OR a brand-communication case whose success metric is phrased in profit terms — see
the phrasing trap below).

**Step 3 — Score each sub-question against the condensed checklists.** Read `references/checklists.md` — it
holds a fast-scoring version of every case type's signals, including the seven with a full sibling skill built
(brand communication, profit optimization, supply chain, M&A, product launch, finance/investment, market
entry) and the ones that don't have a dedicated skill yet (growth strategy, turnaround/crisis, pricing). Score loosely, same style as
the sibling skills' own Section 2 — the more signals tick, the more confidently that sub-question can be
assigned that type.

**Watch for the phrasing trap:** a sub-question's *metric* and its *case type* are different things. "Profit
is falling because a campaign underperformed on trial" is a brand-communication case whose outcome happens to
be measured in profit — the deliverable is a campaign, not a cost-benefit number. "Should we approve this
marketing spend on a cost-benefit basis" is a profit-optimization case that happens to mention marketing — the
deliverable is a number, not a campaign. "Should we acquire this company's product line" can be an M&A case
(the deliverable is a valuation and deal terms) or a product-launch case wearing an acquisition costume (the
deliverable is really what to build and how to launch it, and the acquisition is just how the IP changed
hands). When in doubt, ask: *what does the final recommendation actually look like* — a message/campaign, a
cost/revenue number, a market-entry go/no-go, a deal structure, a go-to-market plan, etc. — not which words the
brief used to state the problem.

**Step 4 — Resolve conflicts.** If a sub-question ticks signals for more than one type, don't split hairs on
the checklist score — use the phrasing-trap test above (what does the recommendation actually look like), and
if it's still genuinely ambiguous, treat it as belonging to whichever type's deliverable the brief spends more
words describing. Say the call out loud and move on; a fast, explicit, slightly-imperfect call beats a debate
that eats into solving time.

**Step 5 — Hand off.** For each confirmed sub-question type:
- If a dedicated `case-<type>` skill exists (`case-brand-communication`, `case-profit-optimization`,
  `case-supply-chain`, `case-ma`, `case-product-launch`, `case-investment`, `case-market-entry`, and any
  later siblings), **load that skill's full
  `SKILL.md` now** and follow its own checklist confirmation, its framework, and its own references as needed.
  Don't solve from this skill's condensed checklist — it isn't built to be sufficient for that (see Section 3).
- If the confirmed type has no dedicated skill yet, there's no framework to load — fall back to general
  business-case structuring (root cause → objective → options → recommendation), using the "primary tool"
  column in `references/checklists.md`'s taxonomy table as a starting point for what that structuring should
  emphasize.

**Step 6 — Integrate.** Once every sub-question has an answer, assemble them using the template in
`references/output-structure.md`: one shared Overall SCQ and Objective at the top (from Step 1), each
sub-question's framework output underneath with an explicit tie-back to that shared objective, and a final
integrated recommendation that reads as one decision reached from multiple angles — not a sequence of mini-decks.
`references/worked-mixed-example.md` walks this whole process end to end on a constructed mixed brief.

**Step 7 — If nothing fires clearly** on a sub-question even after Step 3-4, say so explicitly rather than
forcing the nearest-fitting framework, and fall back to general business-case structuring for that piece —
same fallback as Step 5's no-dedicated-skill case.

## 3. Why the checklists here are condensed, not authoritative

`references/checklists.md` exists purely for fast first-pass scoring across every case type in one place. It is
deliberately **not** a copy of any sibling skill's full Section 2 — it's short enough to scan across many types
in a few minutes, and correspondingly too thin to be the last word on any single type. Two consequences:

- **The sibling skill's own `SKILL.md` is always authoritative for its own type.** If this file's condensed
  entry for, say, profit optimization ever seems to disagree with `case-profit-optimization/SKILL.md`'s own
  Section 2, the sibling skill wins — treat that as a sign this file has drifted and needs a manual update.
- **This file will go stale as sibling skills evolve** unless it's updated alongside them. There's no
  automated sync — when a `case-<type>` skill's Section 2 checklist changes, or a new `case-<type>` sibling is
  added, revisit `references/checklists.md` by hand.

This is the deliberate trade-off behind holding condensed copies at all instead of only ever calling out live to
each sibling skill: classification gets faster (one file to scan instead of loading N full skills just to find
out which ones are even relevant), at the cost of a small maintenance duty when siblings change. Full solving
still always calls out to the real sibling skill (Step 5) — nothing about a case ever gets *solved* from the
condensed copy.

## 4. Common failure modes to avoid

- **Solving from the condensed checklist instead of handing off.** The checklist is for classification only —
  always load the full sibling skill before actually building that part of the answer.
- **Mistaking the brief's metric for its case type.** See the phrasing trap in Step 3 — always ask what the
  recommendation itself looks like.
- **Force-fitting a mixed brief into one type.** If two sub-questions genuinely need two frameworks, don't
  pick one and let it swallow the other for the sake of simplicity — that's exactly the failure mode this
  skill exists to prevent.
- **Stapling instead of integrating.** Two correct sub-answers presented back-to-back with no shared
  throughline still reads as two mini-decks to a grader. Step 6 and `references/output-structure.md` exist to
  stop that — every sub-answer needs an explicit sentence tying it back to the one shared objective.
- **Skipping Step 1's full read.** Segmenting into sub-questions before anyone has read the whole brief risks
  missing a sub-question that's implied rather than stated outright, or anchoring on the first person's guess.
- **Treating a single-ask brief as automatically pure.** Even one explicit ask can blend signals — run Step 3
  on it anyway rather than skipping straight to a framework.

## 5. One-page decision flow (first few minutes)

1. Read the brief once, cover to cover, before discussing.
2. Write the overall SCQ and the one-sentence "what is this brief ultimately asking for."
3. List the sub-questions (Step 2).
4. Score each sub-question against `references/checklists.md` (Step 3), watching for the phrasing trap.
5. For each confirmed type: load the matching `case-<type>` skill if one exists, or fall back to general
   structuring if it doesn't (Step 5).
6. Once every sub-question has an answer, assemble them with `references/output-structure.md` (Step 6).
7. If a sub-question never resolves clearly, say so and fall back to general structuring for that piece (Step 7)
   rather than forcing the nearest framework.
