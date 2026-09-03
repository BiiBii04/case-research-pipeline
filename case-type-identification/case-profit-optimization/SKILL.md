---
name: case-profit-optimization
description: >-
  Checklist and full solving framework for a profit-optimization (profitability) business case — profit is
  declining, or a proposed move needs a profitability check, and the ask is to find the root cause and recommend
  a fix — one of a family of case-type skills alongside `case-brand-communication` and `case-orchestrator` (with
  market entry, M&A, pricing, turnaround still planned). Use as soon as a brief is released, BEFORE committing
  to any framework — run the checklist first to test whether the brief is profit-optimization, a different type,
  or a mix. If confirmed, use the profit-tree (Profit = Revenue − Cost, MECE-decomposed to fit the industry) plus
  hypothesis-driven branch analysis and worked examples to build that part of the answer. Also trigger on any
  brief mentioning declining profit/margin, rising costs, a profitability check on a new product/market/store, an
  outsourcing or cost-benefit decision, or phrases like "profit is falling even though sales/units are stable."
---

# Profit Optimization Case — Checklist and Framework

This skill turns a case-solving method into something usable live, during a competition, under time pressure. It is one member of a planned family of case-type skills (`case-brand-communication`, `case-profit-optimization`, and later `case-market-entry`, `case-ma`, and others) that together cover the case types a team might draw. Read the "How this fits with other case-type skills" section below first if more than one case-type skill is loaded — it explains how to keep the final answer coherent instead of stapling together separate mini-answers.

The content here is an original, rewritten summary of standard case-interview and management-consulting methods (profit-tree/MECE decomposition, hypothesis-driven analysis, fixed vs. variable cost structuring). Keep this skill team-internal; don't redistribute outside the competition team.

**By design, this skill is company-agnostic.** It knows how to recognise a profit-optimization case and how to solve one — it does not know anything about any specific company, and doesn't reference any particular team's research files by name. That's deliberate: the checklist and framework need to work unchanged on whatever brief actually drops, for this competition or a future one, without being tuned (or biased) toward one team's prep material. If your team has built company-specific research for the current competition, keep the pointer to it in a separate, clearly-labelled file outside this skill (see Section 5) — don't fold it into this skill's own content.

## 1. Where "Profit Optimization" sits among case types

A 48-hour business case can land in several different problem families. Profit optimization is specifically about *why the money math stopped working* — profit is falling, or a proposed move's profit math needs checking — not about changing brand perception, entering a new market for strategic reasons, or restructuring the org.

| Case type | Core question | Primary tool |
|---|---|---|
| **Profit Optimization** | Why is profit falling (or would a proposed move be profitable), and what fixes it? | Profit tree (Revenue − Cost, MECE by industry) → branch analysis → root cause → recommendation |
| Brand Communication | How do we change perception/behaviour toward a brand through a campaign or message? | Issue → Objective → SoG → Winning Point → J2BD → Insight → Idea → IMC → Trade → KPI |
| Market Entry / Expansion | Should we enter a new market/segment/format, and how? | TAM/SAM/SOM, entry-mode analysis, go/no-go criteria |
| Growth Strategy | Where should the next unit of growth come from? | Ansoff matrix, portfolio/SoG-style analysis |
| Turnaround / Crisis | How do we stop the bleeding and stabilise after a shock? | Root-cause diagnosis, stakeholder triage, phased plan (a profit fix may be one workstream, not the whole answer) |
| Pricing | Is the price right, and how should it change? | Elasticity, competitor benchmarking, value-based pricing (narrower than profit optimization — pricing is one lever inside a profit tree, not the whole tree) |
| Operations / Supply Chain | How do we fix a cost, availability, or efficiency problem? | Process mapping, cost-driver analysis (often the follow-through once a profit tree points at a cost-side root cause) |
| M&A / Partnership | Should we buy, merge with, or partner with another player? | Synergy analysis, valuation, integration risk |

A live brief is rarely a pure type. "Retail margins are shrinking" could be a profit-optimization problem (a genuine cost/revenue root cause to diagnose), a pricing problem, or a brand-communication problem (footfall decline from perception, which then shows up as lower revenue), depending on what's actually driving it. The checklist below is how the team tells which one it's actually holding.

## 2. Checklist — is this a profit optimization case?

Run this in the first 15-20 minutes after the brief drops, out loud, as a group. Score it loosely — the more left-column boxes get ticked, the more confidently the team can commit to this framework.

**Signals it IS profit optimization**
- The brief states profit, margin, or earnings is falling — especially when it also states a *related* metric (units sold, revenue, market share) has stayed flat or even grown, which is the classic profitability-case setup.
- The brief explicitly rules out major external shocks ("no significant change in the market or from competitors") — a strong signal the cause is internal (cost structure, product mix, an operational change) rather than market-driven.
- The ask is framed as "find the root cause and recommend a fix," not "build a campaign" or "should we enter."
- The brief describes a proposed move (new product, new store, an outsourcing decision) and asks whether it will be profitable, or is worth it on a cost-benefit basis.
- The deliverable it's fishing for sounds like a diagnosis plus a short-/long-term recommendation — not a communication plan, a market-sizing recommendation, or a deal structure.
- Numbers are central to the brief — revenue, cost, price, volume figures are given or clearly obtainable, and the case rewards precise arithmetic.

**Signals it's something else (redirect to the matching skill)**
- Root complaint is that the audience doesn't know about, trust, or feel good about the brand → Brand Communication; profit may be the symptom, but the fix is a message/campaign, not a cost or revenue-mix change.
- "Should we open in province X / launch format Y" as a *strategic* fit question (not just "would it be profitable") → Market Entry; use TAM/SAM/SOM and entry-mode logic as the spine.
- Financial collapse, executive scandal, supply failure, regulatory shutdown → Turnaround/Crisis; a profit fix may be one component, not the primary deliverable.
- The brief only asks "is the price right" with no broader cost/revenue-structure question → Pricing is the narrower, more specific tool to reach for first, even though it lives inside a profit tree.
- Acquiring, partnering, or divesting a business unit → M&A.

**When it's mixed:** many real prompts blend types — e.g. a turnaround case where fixing the cost structure is one lever among several, or a brand-communication case where the ultimate ask is phrased as "and by how much would this improve profit." Scope this framework to the specific sub-question that's actually about the revenue/cost math, say explicitly which parts of the case use which framework, and don't force a full profit-tree breakdown onto a case that's really about perception or strategic fit.

## 3. How this fits with other case-type skills

**If `case-orchestrator` is loaded, it now owns this logic centrally.** It reads the whole brief, segments it into sub-questions, classifies each one against every case-type skill's checklist, and integrates every sub-framework's output into one coherent case structure tied to a shared objective. Load `case-orchestrator` first and let it hand off to this skill for any confirmed profit-optimization sub-question, rather than re-deriving the classification here. The rest of this section is this skill's own standalone fallback logic, for the case `case-orchestrator` isn't loaded and this skill is being used on its own.

The plan is for this skill to sit alongside siblings for other case types (brand communication, market entry, M&A, pricing, turnaround, etc.), each with its own checklist and framework. When more than one is available:

1. **Run every available checklist against the brief before committing to one.** Real briefs blend types more often than they're pure.
2. **If exactly one lens fires strongly**, use that skill's framework as the backbone of the whole answer.
3. **If more than one lens fires (a mixed case)**, don't let each framework run in isolation and get stapled together at the end. Nominate one owner for the shared throughline — one SCQ (Situation-Complication-Question) and one overarching Objective that every sub-framework's output has to tie back to. Each specialized section should open by naming which sub-question it's answering and close by connecting back to that shared Objective, so the final answer reads as one solution arrived at from multiple angles, not several disconnected mini-decks.
4. **If nothing fires clearly**, don't force this framework. Say so, and fall back to general business-case structuring (root cause → objective → options → recommendation) rather than distorting the case to fit a template that doesn't match.

**Specifically with `case-brand-communication`:** the two skills share the same SCQ framing tool for restating the problem, which makes handoff easy — but they diverge immediately after that. A profit-optimization sub-question decomposes into a numbers tree (Revenue/Cost); a brand-communication sub-question decomposes into a people/perception chain (Issue → Objective → Insight → Idea). A brief that's "profit is falling because a campaign underperformed on trial" is a brand-communication case whose success metric happens to be phrased in profit terms — don't mistake the phrasing for the case type. Conversely, a brief that's "should we accept this profitability-costed marketing spend" is a profit-optimization case that happens to mention marketing — the deliverable is a cost-benefit number, not a campaign.

As sibling skills get added, keep them in the same `case-<type>` naming pattern (e.g. `case-market-entry`, `case-ma`) so they're easy to spot as one family.

## 4. The framework, step by step

The roadmap below is a summary. This public copy does not include the full worked framework detail, the fixed-cost-vs-variable-cost drill, or worked examples (kept out deliberately, see the repo README) — read it as a checklist and step outline, not a complete how-to.

**A. WHAT — confirm the problem, build the profit tree.** 1. Re-state the issue with SCQ (note explicitly if external shocks are ruled out) → 2. Build the universal first layer, Profit = Revenue − Cost → 3. Hypothesize and confirm an industry-specific second layer for both Revenue and Cost → 4. Narrow with exclusion questions to figure out which branch actually moved.

**B. ROOT CAUSE — analyze the branch(es).** 5. Revenue branch: check volume vs. price vs. mix, then (only if needed) drill into market-level causes → 6. Cost branch: identify which cost category is out of line, whether fixed or variable, and why (supplier, self-inflicted, regulatory, input scarcity, other market shift).

**C. SOLUTION — conclude and recommend.** 7. State the root cause in 2-3 sentences with 2-3 supporting explanations → 8. Give short-term and long-term recommendations, organized by category → 9. (Optional, for extra credit) add one strategic recommendation beyond the direct fix.

Each stage depends on the one before it — don't propose a fix before the branch analysis has actually isolated where the number moved, and don't skip the exclusion questions in a rush to calculate, since a wrong branch choice wastes the clock on the wrong analysis.

Worked examples are not included in this public copy.

## 5. What information each step needs

If the checklist confirms profit optimization (in full or in part), here's what the framework asks for at each step. This list is deliberately generic — it names the *kind* of data each step needs, not a specific team's files, so it stays valid regardless of which company or competition it's applied to.

| Framework step | Data it needs |
|---|---|
| SCQ restatement | The brief's own stated facts — what changed, what's confirmed unchanged (market, competitors) |
| Revenue-tree hypothesis | General knowledge of how the *industry* segments revenue (by product line, size, channel, customer type) — not pre-built; comes from case-solver knowledge plus confirmation with the brief/exhibits |
| Cost-tree hypothesis | General knowledge of the industry's typical cost structure (production/selling/support; fixed/variable split) — same, built live and confirmed, not pre-researched |
| Exclusion questions | Whatever the brief/exhibits state about revenue and cost trends — not pre-buildable, this is case-specific interaction |
| Branch analysis — revenue | Price, volume, and product-mix figures for the period in question; market/competitor/regulatory context if the anomaly isn't purely internal |
| Branch analysis — cost | Cost-category breakdown (fixed/variable, by sub-category), cost trend over the period, and context on any supplier/input/regulatory driver |
| Regulatory check on any cost-side finding | Whether a cited cost increase traces to a new law, tax, or compliance requirement — worth having general regulatory-landscape research on hand if the competition's industry is regulation-heavy |
| Recommendation | Category revenue/cost benchmarks if available, to sanity-check whether a proposed fix is realistic in scale |

**Before the clock starts on an actual case, check your own team's prep against this list** — for each row, do you already have this data, or will it have to come live from the brief? Most of this framework's inputs (the industry-specific tree shapes, the branch numbers) are *never* pre-buildable — they only exist once the real brief and its exhibits land — so this is a lighter-prep case type than brand communication: the main pre-work that transfers is general industry/regulatory knowledge, not company-specific figures.

If your team keeps a research index for the current competition (which company, which files, which framework step each one covers), treat it as a separate document alongside this skill, not part of it — that keeps this skill reusable for a future competition without editing, and keeps this skill's *classification logic* independent of any one team's research, which may be incomplete or unverified in places.

## 6. The case-solving process, if it's profit optimization

A suggested run of show once the checklist confirms this case type and the clock starts. Rescale the timing to the actual deadline (this framework is naturally faster than a 10-step brand-communication case, so expect more slack time for numbers-checking and rehearsal), but keep the order — each step depends on the one before it.

| Time (of ~10 working hrs) | Step | What the team does |
|---|---|---|
| First 20 min | Confirm case type | Run the Section 2 checklist as a group. Agree explicitly: "this is a profit-optimization case, scoped to [X]." Assign roles (Issue/Tree lead, Revenue-branch lead, Cost-branch lead, Numbers/QA lead). |
| 20-60 min | SCQ + profit tree, layer 1 | Write the SCQ, flagging explicitly whether external shocks are ruled out. Build the universal Profit = Revenue − Cost layer. |
| 60-150 min | Industry-specific tree | Hypothesize the industry's revenue and cost sub-structure. Cross-check hypotheses against whatever industry/regulatory research the team has prepped. Confirm against the brief's exhibits. |
| 150-210 min | Exclusion questions + branch choice | Work through the Section 4 exclusion questions using the brief's data. Decide which branch(es) need full analysis. |
| 210-360 min | Branch analysis | Do the arithmetic on the chosen branch(es): volume/price/mix for revenue, category/fixed-variable/trend for cost. Cross-check every number twice — this framework is graded heavily on arithmetic precision. |
| 360-420 min | Root cause + explanations | State the root cause in 2-3 sentences. Draft 2-3 supporting explanations for *why* it happened. |
| 420-480 min | Recommendations | Draft short-term and long-term recommendations by category. Add one strategic bonus recommendation if time allows. |
| Remaining time | Synthesis & rehearsal | Compress onto one cheat-sheet page: tree diagram, the isolated root cause, the recommendation categories. Rehearse the arc: SCQ → tree → branch analysis → root cause → recommendation. Time-box Q&A prep — expect challenges on arithmetic assumptions and on why a branch was excluded first. |

## 7. Common failure modes to avoid

- **Building a generic tree instead of an industry-specific one.** A textbook Profit = Revenue − Cost tree with no industry-specific second layer signals the team didn't actually think about the business — always hypothesize and confirm a tree shaped to the real industry.
- **Skipping the exclusion questions and analyzing both branches exhaustively by default.** Wastes the clock; ask first, then choose where to dig.
- **Debating what a cost "is" instead of how it behaves.** Fixed vs. variable is a function of the business model, not an inherent property of the cost line.
- **A root cause with no qualitative "why."** Finding that a number moved isn't the end — keep asking "why" until reaching an actionable, addressable cause, not just a restated symptom.
- **Vague comparative language left unquantified.** "Costs went up a lot" isn't an answer — turn it into a number before using it in the conclusion.
- **A recommendation with no link back to the root cause.** Every recommendation should trace directly to the diagnosed cause; a generic "improve efficiency" line reads as padding, not analysis.
- **Treating this as the whole answer when the brief is actually mixed.** If part of the brief is really about perception or strategic fit, don't stretch the profit tree to cover it — hand that part to the matching skill (see Section 3).

## 8. One-page decision flow (first few minutes)

1. Read the brief once, cover to cover, before discussing — don't let the first person's guess anchor the room.
2. Underline every number and every verb that implies a financial change ("falling," "declining," "increasing," "shrinking") vs. a perception/behaviour change ("perceive," "trust," "aware," "choose") or a structural/strategic one ("expand," "acquire," "restructure").
3. Score the case against the Section 2 checklist as a group — out loud, fast, don't overthink individual boxes.
4. If it's profit optimization: open your team's prepped industry/regulatory research (see Section 5), assign roles, start the Section 6 timeline.
5. If it's mixed: agree which sub-question gets this treatment and which gets a different framework (see Section 3), and say so explicitly in the final answer.
6. If it's clearly something else entirely: set this skill aside and use the matching case-type skill instead.
