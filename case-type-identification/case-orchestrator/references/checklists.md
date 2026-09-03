# Condensed Case-Type Checklists

Fast first-pass scoring only — see `SKILL.md` Section 3 for why these are deliberately condensed, and why the
sibling skill's own checklist always wins if the two ever disagree. Score loosely: the more signals tick for a
type, the more confidently that sub-question can be assigned it. Run this for every sub-question the brief
segments into, not just once for the whole brief.

## Master taxonomy

| Case type | Core question | Primary tool | Dedicated skill? |
|---|---|---|---|
| **Brand Communication** | How do we change perception/behaviour toward a brand through a campaign or message? | Issue → Objective → SoG → Winning Point → J2BD → Insight → Idea → IMC → Trade → KPI | Yes — `case-brand-communication` |
| **Profit Optimization** | Why is profit falling (or would a proposed move be profitable), and what fixes it? | Profit tree (Revenue − Cost, MECE by industry) → branch analysis → root cause → recommendation | Yes — `case-profit-optimization` |
| **Operations / Supply Chain** | Why can't the chain deliver goods/materials reliably or efficiently, and how do we fix it? | Demand/Inventory/Supply diagnostic lens → qualitative (disruption) or quantitative (optimization) solving path | Yes — `case-supply-chain` |
| **M&A / Partnership** | Should we buy, merge with, invest in, or partner with another company, and on what terms? | Porter's Five Forces (objective) → SWOT/Strategic Fit → Synergy tree → DCF valuation → go/no-go | Yes — `case-ma` |
| **New Product Launch** | Should we launch this new product/feature, what should it look like, and how do we bring it to market? | STP → Whitespace × Strength positioning → Proposition/Positioning → 6Ps go-to-market → revenue/P&L goal | Yes — `case-product-launch` |
| **Finance / Investment** | Is this business financially healthy, and is a specific investment (build it ourselves, joint-venture, or acquire) worth the capital it needs? | P&L read (Financial Performance → Revenue Breakdown → Cost Structure) → Payback Period / Investment Value / ROIC | Yes — `case-investment` |
| **Market Entry / Expansion** | Should we enter a new market/segment/format, and how? | 3Cs + Market + Financials → Market Sizing → entry-mode fit → go/no-go | Yes — `case-market-entry` |
| Growth Strategy | Where should the next unit of growth come from? | Ansoff matrix, portfolio/SoG-style analysis | Not yet built |
| Turnaround / Crisis | How do we stop the bleeding and stabilise after a shock? | Root-cause diagnosis, stakeholder triage, phased plan | Not yet built |
| Pricing | Is the price right, and how should it change? | Elasticity, competitor benchmarking, value-based pricing | Not yet built |

When a sub-question scores into one of the "not yet built" rows, there's no full framework to hand off to (see
`SKILL.md` Step 5) — use that row's "Primary tool" as the starting point for general structuring instead.

## Condensed signals per type

**Brand Communication** — signals it fires:
- Centres on awareness, perception, image, trust, or sentiment toward a specific brand — not product spec,
  price, or distribution.
- Ask is to build/fix/relaunch/defend a campaign, message, positioning, or communication plan.
- Gap between reality and perception ("the product is strong but nobody knows/believes it").
- A specific, nameable target audience whose *mind* needs to change.
- Mentions media, channels, KOLs, social platforms, PR, advertising, or in-store communication materials.
- A launch/relaunch underperformed specifically on awareness or trial (not distribution, price, or quality).

**Profit Optimization** — signals it fires:
- States profit/margin/earnings is falling, especially alongside a related metric (units, revenue, share)
  that's stated as flat or growing.
- Explicitly rules out major external shocks ("no significant change in the market or competitors") —
  points inward, to cost structure or product mix.
- Framed as "find the root cause and recommend a fix," not "build a campaign" or "should we enter."
- A proposed move (new product/store/outsourcing decision) needs a profitability or cost-benefit check, with no
  new capital/investment decision or financial-health read as the actual test (if it is, see Finance/Investment).
- Numbers are central and precise — revenue, cost, price, volume figures given or clearly obtainable.

**Operations / Supply Chain** — signals it fires:
- Centres on the physical movement of goods or materials — sourcing, production, inventory, warehousing,
  logistics, distribution — not what to sell, how to talk about it, or whether the price is right.
- A stockout, excess-inventory, or fulfillment-delay problem, with no real product/price/messaging question
  behind it.
- A disruption to the flow of goods (supplier failure, logistics bottleneck, pandemic/disaster/political shock)
  where the ask is how to keep operations running.
- A planning/optimization ask about the physical network itself — factory/warehouse location, production or
  shipment allocation, safety-stock levels.
- Data given (if any) is operational — order volumes, inventory levels, shipment/delay rates, supplier lead
  times, production capacity — not brand-perception data or a P&L.
- Dedicated skill: `case-supply-chain`. Watch the overlap with Profit Optimization (a supply-chain root cause is
  often what's moving a profit tree's cost branch — the test is whether the deliverable is a dollar figure
  (Profit Optimization) or a redesigned/stabilised process (Supply Chain)) and with Turnaround/Crisis (a
  disruption is only Supply Chain if operations is the whole case, not one workstream among several).

**M&A / Partnership** — signals it fires:
- The brief names two companies (or a company and an unnamed "target"/"candidate") and asks whether one should
  buy, merge with, invest in, or partner with the other.
- The ask is explicitly about deal terms — a purchase price, a valuation, an ROI/payback target, or "is this
  deal worth it."
- Financial or operating data is given for *both* companies (revenue, growth rate, cost structure, market
  position), not just one.
- The deliverable sounds like "should we do this deal, and at what price/terms," not a campaign, a cost
  diagnosis on the existing business, or a go-to-market plan for a new product.
- A financial-buyer angle is present (a private equity or investment fund evaluating an acquisition purely for
  return), or the brief mentions synergies, strategic fit, due diligence, integration risk, or a specific
  acquisition structure (buying shares vs. buying assets).
- Dedicated skill: `case-ma`. Watch the overlap with Profit Optimization (an M&A synergy estimate shares the
  Revenue/Cost MECE instinct with a profit tree — the test is whether the recommendation is a go/no-go on a
  *second* company plus a price (M&A), or a diagnosed fix on the *existing* business (Profit Optimization)) and
  with Supply Chain (acquiring a supplier is M&A only if the deliverable is a valuation/deal call, not one
  operational option among several being weighed against multi-sourcing or postponement) and with New Product
  Launch (an acquisition whose real point is "what should this new product be and how do we launch it," with
  the deal itself incidental, belongs to New Product Launch instead) and with Finance/Investment (if no one
  specific target is named and the ask is really "compare buying vs. building this capability ourselves purely
  on the numbers," that's Finance/Investment; once a specific target's own strategic fit and price are the
  test, it's M&A).

**New Product Launch** — signals it fires:
- The brief describes introducing something new: a brand-new product, a re-launch/improvement of an existing
  one, or a new feature on an existing product/app/service.
- The ask is about *whether* to launch, *what* the product/feature should be, or *how* to bring it to market —
  not a deal with a second company, a cost diagnosis of the existing business, or a perception/behaviour
  campaign for something already on the market.
- The brief gives, or explicitly asks the team to identify, an unmet customer need or pain point the new
  product is meant to solve.
- The deliverable sounds like "should we launch this, what should it look like, who's it for, and how do we
  take it to market" — a Product Concept plus a go-to-market plan.
- A revenue or P&L goal-setting ask is tied specifically to the *new* product/feature, not the existing
  business's overall profit trend.
- Dedicated skill: `case-product-launch`. Watch the overlap with Brand Communication (a new product's
  Proposition is a narrower, product-specific cousin of a full brand Positioning — this skill owns the
  sub-question if a new product is actually launching, even though its Promotion piece borrows
  communication-mix thinking; Brand Communication owns it if nothing new is being introduced) and with Market
  Entry (if the *market* choice is still open, that's Market Entry with launch detail as supporting content; if
  the market is a given and the ask is what to build and how to launch it there, this skill owns it) and with
  M&A (see the M&A entry above).

**Finance / Investment** — signals it fires:
- The brief hands over multi-period P&L-style financial data for one company and asks the team to evaluate its
  financial performance, trend, or health — not to diagnose and fix a specific existing profit problem.
- The brief describes a specific capital-allocation decision (building new capacity, expanding production, or
  entering a project via primary investment, joint venture, or acquisition) and the ask is explicitly whether
  it's financially worth it.
- The deliverable is framed around Payback Period, ROI/ROIC, an investment/valuation figure, or a forward-
  looking multi-year P&L build for a not-yet-existing investment or product line.
- The ask compares the *economics* of different ways to pursue the same capital decision (build it ourselves
  vs. joint-venture vs. acquire) purely on the numbers, without one specific acquisition target's own strategic-
  fit story being the point.
- Numbers are central, detailed, and multi-period — revenue, cost, margin, investment cost, discount rate,
  contract length, given or clearly derivable from the brief.
- Dedicated skill: `case-investment`. Watch the overlap with Profit Optimization (see that entry above) and
  with M&A (see the M&A entry above) and with Market Entry (a market-entry-flavored setup — "which country
  should we expand into" — is still Finance/Investment if the actual test is the Payback/ROIC math on the entry
  investment rather than a qualitative market-attractiveness/entry-mode-fit judgment call).

**Market Entry / Expansion** — signals it fires:
- The brief asks whether a company should enter a new geography, segment, channel, or format — framed as a
  strategic-fit and attractiveness question, not purely "would it be profitable" (Profit Optimization wearing
  an entry costume) or purely "what's the payback/ROI number" (Finance/Investment).
- The deliverable sounds like "should we enter, and if so how" — a go/no-go plus a recommended entry approach,
  not a deal-specific valuation, a campaign, or a product concept.
- The brief needs (or explicitly asks for) a market-size estimate for the new market/segment.
- An entry-mode choice is in play — organic/greenfield build, joint venture, acquisition, or franchise — as a
  genuinely open question, not one already settled by the brief.
- The brief gives (or asks the team to reason about) competitor landscape, customer fit, and company-readiness
  information specific to the *new* market, not just the company's existing home market.
- Dedicated skill: `case-market-entry`. Watch the overlap with New Product Launch (if the market choice is still
  open, Market Entry leads with Product Launch detail as supporting content; if the market is a given and the
  ask is what to build and how to launch it there, New Product Launch owns it) and with Finance/Investment (see
  that entry above) and with M&A (acquisition is one entry-mode option on Market Entry's menu until a specific
  target is named, at which point M&A owns the sub-question).

**Growth Strategy** — signals it fires:
- Asks broadly "where should growth come from" without already pointing at one lever (new market, new
  product, new segment, deeper penetration) — an Ansoff-shaped question.

**Turnaround / Crisis** — signals it fires:
- A shock has already happened — financial collapse, executive scandal, supply failure, regulatory shutdown —
  and the ask is to stabilise, not just improve.
- Multiple workstreams are implied at once (comms, cost, ops, stakeholders) rather than one clean lever.

**Pricing** — signals it fires:
- The ask is narrowly "is the price right, and how should it change" with no broader cost/revenue-structure
  question behind it. If cost structure is also in play, this is really profit optimization with pricing as
  one branch, not a standalone pricing case.

## The phrasing trap (see `SKILL.md` Step 3)

A sub-question's stated metric and its actual case type are not the same thing. Before assigning a type, ask
what the *final recommendation* looks like — a campaign/message, a cost or revenue number, a go/no-go on
entering somewhere, a deal structure, a go-to-market plan, a financial-health read or investment appraisal, a
stabilisation plan — rather than which words the brief used to phrase the problem. "Profit fell because of a
weak campaign" is brand communication measured in profit terms; "should we approve this marketing spend" is
profit optimization that happens to mention marketing; "should we acquire this startup's product" can be M&A
(the deal terms are the test) or New Product Launch (what to build and how to launch it is the test, and the
acquisition is just the mechanism); "should we expand into this country" can be Market Entry (a qualitative
go/no-go on the market itself is the test) or Finance/Investment (the payback/ROIC math on the required capital
is the test, and the market-selection narrative is just the setup).
