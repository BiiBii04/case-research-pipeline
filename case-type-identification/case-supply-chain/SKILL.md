---
name: case-supply-chain
description: >-
  Checklist and full solving framework for a supply-chain / operations case — the brief is about how goods,
  materials, or inventory move (sourcing, production, warehousing, distribution, logistics), under everyday
  planning or a sudden disruption — one of a family of case-type skills alongside `case-brand-communication`,
  `case-profit-optimization`, and `case-orchestrator` (market entry, M&A, pricing, turnaround still planned).
  Use as soon as a brief is released, BEFORE committing to any framework — run the checklist first to test
  whether the brief is a supply-chain case, a different type, or a mix. If confirmed, use the
  Demand/Inventory/Supply diagnostic lens plus the qualitative-vs-quantitative split (crisis/disruption vs.
  planning/optimization) to build that part of the answer. Also trigger on stockouts, excess inventory, a
  supplier or logistics disruption, a factory-network or sourcing decision, a shipment-delay/fulfillment
  problem, or "the supply chain can't keep up with demand."
---

# Supply Chain Case — Checklist and Framework

This skill turns a case-solving method into something usable live, during a competition, under
time pressure. It is one member of a family of case-type skills (`case-brand-communication`,
`case-profit-optimization`, `case-supply-chain`, and later `case-market-entry`, `case-ma`, and others) that
together cover the case types a team might draw. Read the "How this fits with other case-type skills" section
below first if more than one case-type skill is loaded — it explains how to keep the final answer coherent
instead of stapling together separate mini-answers.

The content here is an original, rewritten summary of standard supply-chain-management and operations-research
methods (the supply-chain-surplus objective, the SCOR plan/source/make/deliver/return model, lean vs. agile
supply chains, XYZ inventory analysis, linear programming). Keep this skill team-internal; don't redistribute
outside the competition team.

**By design, this skill is company-agnostic.** It knows how to recognise a supply-chain case and how to solve
one — it does not know anything about any specific company, and doesn't reference any particular team's research
files by name. That's deliberate: the checklist and framework need to work unchanged on whatever brief actually
drops, for this competition or a future one, without being tuned (or biased) toward one team's prep material. If
your team has built company-specific research for the current competition, keep the pointer to it in a separate,
clearly-labelled file outside this skill (see Section 5) — don't fold it into this skill's own content.

## 1. Where "Supply Chain" sits among case types

A 48-hour business case can land in several different problem families. A supply-chain case is specifically
about *how the physical flow of goods and materials works* — sourcing, production, inventory, warehousing,
distribution, logistics — not about changing brand perception, checking whether the P&L math works, or deciding
whether to enter a new market.

| Case type | Core question | Primary tool |
|---|---|---|
| **Supply Chain / Operations** | Why can't the chain deliver goods/materials reliably or efficiently, and how do we fix it? | Demand/Inventory/Supply diagnostic → qualitative (disruption) or quantitative (optimization) solving path |
| Brand Communication | How do we change perception/behaviour toward a brand through a campaign or message? | Issue → Objective → SoG → Winning Point → J2BD → Insight → Idea → IMC → Trade → KPI |
| Profit Optimization | Why is profit falling (or would a proposed move be profitable), and what fixes it? | Profit tree (Revenue − Cost, MECE by industry) → branch analysis → root cause → recommendation |
| Market Entry / Expansion | Should we enter a new market/segment/format, and how? | TAM/SAM/SOM, entry-mode analysis, go/no-go criteria |
| Growth Strategy | Where should the next unit of growth come from? | Ansoff matrix, portfolio/SoG-style analysis |
| Turnaround / Crisis | How do we stop the bleeding and stabilise after a shock? | Root-cause diagnosis, stakeholder triage, phased plan (a supply-chain fix may be one workstream, not the whole answer) |
| Pricing | Is the price right, and how should it change? | Elasticity, competitor benchmarking, value-based pricing |
| M&A / Partnership | Should we buy, merge with, or partner with another player? | Synergy analysis, valuation, integration risk |

A live brief is rarely a pure type. "Our stores keep running out of stock during Tet" could be a supply-chain
problem (a genuine sourcing/inventory/logistics root cause to diagnose), a profit-optimization problem (if the
ask is really "how much is this costing us and is a fix worth it"), or a turnaround problem (if stockouts are
one symptom among several in a bigger crisis), depending on what's actually being asked. The checklist below is
how the team tells which one it's actually holding.

## 2. Checklist — is this a supply-chain case?

Run this in the first 15-20 minutes after the brief drops, out loud, as a group. Score it loosely — the more
left-column boxes get ticked, the more confidently the team can commit to this framework.

**Signals it IS a supply-chain case**
- The brief centres on the physical movement of goods or materials — sourcing, manufacturing, warehousing,
  inventory levels, shipping/logistics, distribution — rather than what to sell, how to talk about it, or
  whether the price is right.
- A stockout, excess-inventory, or fulfillment-delay problem is described, with no real question about product,
  price, or messaging behind it.
- The brief describes a disruption to the flow of goods — a supplier failure, a logistics bottleneck, a
  pandemic/natural-disaster/political-conflict shock — and asks how to keep operations running.
- The brief is a planning/optimization ask about the physical network itself: where to locate a factory or
  warehouse, how to allocate production or shipments across multiple sites, how much safety stock to hold.
- Data given (if any) is operational — order volumes, inventory levels, shipment/delay rates, supplier lead
  times, production capacity — rather than brand-perception survey data or a P&L.
- The deliverable it's fishing for sounds like "keep the chain running/efficient" or "optimize this operational
  decision," not a campaign, a profitability verdict, or a market-entry recommendation.

**Signals it's something else (redirect to the matching skill)**
- The ask is really "how much is this problem costing us, and is a fix worth it" — the case wants a cost-benefit
  number more than an operational redesign → Profit Optimization; a supply-chain root cause can still be *the*
  answer inside a profit tree's cost branch, but the deliverable there is a dollar figure, not a process fix.
- Root complaint is that the audience doesn't know about, trust, or feel good about the brand → Brand
  Communication; a supply issue that's purely a symptom (e.g. "we look unreliable") with the fix being a
  communications response, not an operational one.
- Multiple things are collapsing at once — finances, leadership, stakeholders, *and* operations — and the
  disruption is only one workstream among several → Turnaround/Crisis; don't stretch this framework to cover
  the whole case if operations is one piece of a bigger stabilisation plan.
- "Should we open a new factory/warehouse in province X" as a *strategic market-entry* question (new geography,
  new customer base) rather than a network-optimization question (where to place a node to best serve existing
  demand) → Market Entry.
- The brief only asks "is the price right" with no operational-flow question behind it → Pricing.

**When it's mixed:** many real prompts blend types — e.g. a turnaround case where fixing a broken supply chain
is one lever among several, or a profit-optimization case whose cost branch traces straight back to a sourcing
or inventory problem. Scope this framework to the specific sub-question that's actually about how goods move,
say explicitly which parts of the case use which framework, and don't force the Demand/Inventory/Supply lens
onto a case that's really about perception, the P&L, or strategic fit.

## 3. How this fits with other case-type skills

**If `case-orchestrator` is loaded, it now owns this logic centrally.** It reads the whole brief, segments it
into sub-questions, classifies each one against every case-type skill's checklist, and integrates every
sub-framework's output into one coherent case structure tied to a shared objective. Load `case-orchestrator`
first and let it hand off to this skill for any confirmed supply-chain sub-question, rather than re-deriving the
classification here. The rest of this section is this skill's own standalone fallback logic, for the case
`case-orchestrator` isn't loaded and this skill is being used on its own.

The plan is for this skill to sit alongside siblings for other case types (brand communication, profit
optimization, market entry, M&A, pricing, turnaround, etc.), each with its own checklist and framework. When
more than one is available:

1. **Run every available checklist against the brief before committing to one.** Real briefs blend types more
   often than they're pure.
2. **If exactly one lens fires strongly**, use that skill's framework as the backbone of the whole answer.
3. **If more than one lens fires (a mixed case)**, don't let each framework run in isolation and get stapled
   together at the end. Nominate one owner for the shared throughline — one SCQ (Situation-Complication-Question)
   and one overarching Objective that every sub-framework's output has to tie back to. Each specialized section
   should open by naming which sub-question it's answering and close by connecting back to that shared
   Objective, so the final answer reads as one solution arrived at from multiple angles, not several
   disconnected mini-decks.
4. **If nothing fires clearly**, don't force this framework. Say so, and fall back to general business-case
   structuring (root cause → objective → options → recommendation) rather than distorting the case to fit a
   template that doesn't match.

**Specifically with `case-profit-optimization`:** these two overlap the most, because a supply-chain root cause
often *is* what's moving the cost side of a profit tree. The test is what the final recommendation looks like —
a profit-optimization case wants a diagnosed cost/revenue root cause and a dollar-denominated fix; a
supply-chain case wants a redesigned or stabilised operational process (a sourcing strategy, an inventory
policy, a network layout). "Margins are falling because of a sourcing disruption" can be either, depending on
whether the deliverable is "quantify the profit hit and recommend a fix" (profit optimization, with the supply
chain as the cost branch's root cause) or "redesign how we source to prevent this" (supply chain, with the
profit impact as supporting evidence, not the main deliverable).

**Specifically with `case-brand-communication`:** the two skills share the same SCQ framing tool for restating
the problem — but a brand-communication sub-question decomposes into a people/perception chain (Issue →
Objective → Insight → Idea), while a supply-chain sub-question decomposes into the Demand/Inventory/Supply
operational lens. A brief that's "customers think we're unreliable because of stockouts" can be a
brand-communication case (the deliverable is a trust-rebuilding message) that happens to be triggered by an
operational cause — don't mistake the trigger for the case type.

As sibling skills get added, keep them in the same `case-<type>` naming pattern (e.g. `case-market-entry`,
`case-ma`) so they're easy to spot as one family.

## 4. The framework, step by step

The roadmap below is a summary. This public copy does not include the full worked framework detail — the
Demand/Inventory/Supply strategy menu, both case-format processes, or the linear-programming/Excel Solver
technique — or worked examples (kept out deliberately, see the repo README) — read it as a checklist and step
outline, not a complete how-to.

**A. Ground the case in the objective and the diagnostic lens.** 1. Anchor on the Supply Chain Surplus
objective (Customer Value − Supply Chain Cost) — every recommendation should trace back to protecting or
growing this, not just cutting cost → 2. Diagnose which of the three levers is actually the problem: Demand
(volatile/mis-forecast), Inventory (efficiency vs. responsiveness conflict), or Supply (sourcing/network
disruption or dependency risk) — a real brief is often one or two of these, not all three.

**B. Identify the case format, because it changes the toolkit.** 3. Decide qualitative or quantitative: is this
a crisis/disruption with limited data calling for a hypothesis-driven response, or a planning/optimization ask
with a full data set calling for a data-driven or mathematical answer? This single call determines which
sub-process to run next.

**C. Solve in the matching format.** 4a. *Qualitative*: Define Problem (SCQ) → Structure the Problem (issue
tree off the Demand/Inventory/Supply lens) → Recommendation (weighted decision matrix across candidate
solutions) → Risk Management (likelihood × impact, organized by Plan/Source/Make/Deliver/Return). 4b.
*Quantitative*: if the case hands over a dashboard/data set, read it critically across pages/tables before
proposing a fix — don't react to the first chart in isolation; if the case is a pure optimization problem
(production mix, transportation/network allocation), formulate a linear-programming model (decision variables,
objective function, constraints) and solve it, e.g. with Excel Solver.

Each stage depends on the one before it — don't jump to a recommendation before the Demand/Inventory/Supply
diagnosis has actually located where the problem lives, and don't run the wrong case-format process (a
crisis case doesn't have a clean data set to optimize against; a planning case shouldn't be solved by
improvised hypothesis alone when real data is sitting in front of the team).

Worked examples are not included in this public copy.

## 5. What information each step needs

If the checklist confirms a supply-chain case (in full or in part), here's what the framework asks for at each
step. This list is deliberately generic — it names the *kind* of data each step needs, not a specific team's
files, so it stays valid regardless of which company or competition it's applied to.

| Framework step | Data it needs |
|---|---|
| Supply Chain Surplus framing | The brief's own stated facts on what customers value and what the chain currently costs to deliver it |
| Demand/Inventory/Supply diagnosis | Whatever the brief/exhibits state about demand patterns, inventory levels, and supply reliability — not pre-buildable, this is case-specific |
| Qualitative vs. quantitative call | How much data the brief actually hands over, and whether the situation is a described disruption or a steady-state planning ask |
| Qualitative — issue tree | General knowledge of how a supply chain in the *relevant industry* typically breaks down (own manufacturing vs. outsourced, single vs. multi-region sourcing, etc.) — built live and confirmed against the brief |
| Qualitative — decision matrix | Whatever criteria the brief's requirements imply (speed of deployment, cost, resource availability, risk reduction) — case-specific, not pre-buildable |
| Qualitative — risk management | The Plan/Source/Make/Deliver/Return structure is reusable; the actual risks and mitigations come from the brief's specifics |
| Quantitative — dashboard reading | Whatever data tables/charts the case provides — order volumes, inventory levels, shipment/delay rates, by category/region/time |
| Quantitative — LP formulation | Cost/profit-per-unit figures, capacity or demand constraints, and any extra business rules stated in the brief — all case-specific inputs, not pre-buildable |
| Recommendation | Category/industry operational benchmarks if available, to sanity-check whether a proposed fix is realistic in scale |

**Before the clock starts on an actual case, check your own team's prep against this list** — for each row, do
you already have this data, or will it have to come live from the brief? Like profit optimization, this is a
lighter-prep case type than brand communication: the diagnostic lens and both case-format processes are
reusable regardless of company, so the main pre-work that transfers is general operations/logistics knowledge
(and, if the team expects a quantitative case, comfort with Excel Solver), not company-specific figures.

If your team keeps a research index for the current competition (which company, which files, which framework
step each one covers), treat it as a separate document alongside this skill, not part of it — that keeps this
skill reusable for a future competition without editing, and keeps this skill's *classification logic*
independent of any one team's research, which may be incomplete or unverified in places.

## 6. The case-solving process, if it's a supply-chain case

A suggested run of show once the checklist confirms this case type and the clock starts. Rescale the timing to
the actual deadline, but keep the order — each step depends on the one before it. Timings assume the
**qualitative** path; if the case is quantitative, expect more time in the "Diagnose the data" and "Model/solve"
rows and less in "Structure the problem," since the work shifts from hypothesis-building to data work and (if
it's an optimization sub-type) formulating and running the model.

| Time (of ~10 working hrs) | Step | What the team does |
|---|---|---|
| First 20 min | Confirm case type | Run the Section 2 checklist as a group. Agree explicitly: "this is a supply-chain case, scoped to [X]." Decide qualitative or quantitative. Assign roles (Issue/Diagnosis lead, Data/Dashboard lead, Solution lead, Risk/QA lead). |
| 20-60 min | SCQ + Surplus framing | Write the SCQ. State explicitly what "customer value" and "supply chain cost" mean for this brief, so every later recommendation has something concrete to tie back to. |
| 60-150 min | Demand/Inventory/Supply diagnosis | Work through the three-lever diagnostic against the brief's facts/exhibits. Decide which lever(s) actually need full analysis — don't analyze all three exhaustively by default. |
| 150-210 min | Structure (qualitative) / Diagnose the data (quantitative) | Qualitative: build the issue tree off the confirmed lever(s). Quantitative: work through the provided dashboard/data set across every page/table before concluding anything from one chart alone; if it's an optimization sub-type, formulate the mathematical model. |
| 210-360 min | Solution development | Qualitative: brainstorm and score candidate solutions on the Section 4a decision matrix. Quantitative: run Excel Solver (or the equivalent) and sanity-check the result; or finalize the data-driven recommendation. |
| 360-420 min | Risk / Evaluation | Qualitative: build the Plan/Source/Make/Deliver/Return risk table with mitigations. Quantitative: stress-test the result against a changed assumption (what if demand/costs move) and note the sensitivity. |
| 420-480 min | Recommendation | Draft the final recommendation, explicitly tied back to protecting/growing the Supply Chain Surplus, not just minimizing cost. |
| Remaining time | Synthesis & rehearsal | Compress onto one cheat-sheet page: the diagnostic tree, the chosen lever(s), the recommendation, the top 1-2 risks. Rehearse the arc: SCQ → diagnosis → structure/data → solution → risk → recommendation. Time-box Q&A prep — expect challenges on why a lever was ruled out, and (for quantitative cases) on the model's assumptions. |

## 7. Common failure modes to avoid

- **Optimizing cost alone and calling it done.** The objective is Supply Chain *Surplus* — Customer Value minus
  Cost — not cost minimization by itself. A recommendation that cuts cost but quietly erodes what the customer
  actually gets (availability, speed, quality) hasn't actually protected the surplus.
- **Analyzing all three levers (Demand/Inventory/Supply) exhaustively instead of diagnosing first.** Wastes the
  clock; use the brief's own signals to narrow down which lever is actually broken before going deep.
- **Running the wrong case-format process.** Forcing a full Excel Solver optimization onto a disruption/crisis
  case with limited data (or, in the other direction, improvising a hypothesis-driven answer when the case
  handed over a full data set worth actually analyzing) wastes the case's own structure.
- **Reacting to one chart in a quantitative dashboard instead of cross-referencing.** A single metric in
  isolation (e.g. "orders dropped") can look like a demand problem when the real story only shows up by
  checking it against another page (e.g. inventory levels also collapsing at the same time) — read across the
  whole data set before concluding.
- **A recommendation with no risk/evaluation pass.** A fix that isn't stress-tested against "what could go
  wrong" or "does this number still hold if an assumption shifts" reads as incomplete, not just risky.
- **Treating this as the whole answer when the brief is actually mixed.** If part of the brief is really about
  the P&L, perception, or strategic fit, don't stretch the Demand/Inventory/Supply lens to cover it — hand that
  part to the matching skill (see Section 3).

## 8. One-page decision flow (first few minutes)

1. Read the brief once, cover to cover, before discussing — don't let the first person's guess anchor the room.
2. Underline every noun/verb about the physical movement of goods ("stockout," "supplier," "warehouse,"
   "shipment," "lead time," "delay") vs. a perception/behaviour change, a P&L/cost-benefit ask, or a
   strategic-fit question.
3. Score the case against the Section 2 checklist as a group — out loud, fast, don't overthink individual boxes.
4. If it's a supply-chain case: decide qualitative or quantitative (Section 4b), open your team's prepped
   operational/industry research, assign roles, start the Section 6 timeline.
5. If it's mixed: agree which sub-question gets this treatment and which gets a different framework (see
   Section 3), and say so explicitly in the final answer.
6. If it's clearly something else entirely: set this skill aside and use the matching case-type skill instead.
