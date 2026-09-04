# Worked Example — a Mixed Brief End to End

A constructed, company-agnostic brief showing the full Section 2 process from `SKILL.md`, including a filled-in
`output-structure.md` template at the end. This is deliberately generic — no real company, so it stays valid as
a training example regardless of which competition it's used to prep for.

## The constructed brief

> "A regional grocery retailer's like-for-like sales and gross margin have both declined for two consecutive
> quarters. Foot traffic across comparable stores in the same category has held roughly steady over the same
> period, and the retailer has made no major changes to its store network, staffing, or supplier base. Internal
> surveys, however, show a rising share of shoppers now describe the retailer as 'the expensive option' compared
> to a fast-growing discount rival, even though the retailer's average basket prices have not materially changed.
> The board wants to know why profitability is slipping and what to do about both the numbers and the
> perception problem before the next results announcement."

## Step 1 — Overall SCQ

- **Situation:** A regional grocery retailer has seen like-for-like sales and margin decline for two quarters
  while category foot traffic has stayed roughly flat and no major operational changes have occurred.
- **Complication:** Shoppers increasingly perceive the retailer as expensive relative to a discount rival, even
  though actual prices haven't materially moved — so the perception gap doesn't fully explain the margin
  decline on its own, and something else may be moving under the hood.
- **Question:** Why is profitability slipping, and what should the retailer do about both the financial
  problem and the perception problem before the next results announcement?

**What the brief is ultimately asking for:** a diagnosis of the margin decline plus a plan to close the
perception gap — explicitly two deliverables, not one.

## Step 2 — Segment into sub-questions

1. **Why is margin declining** when traffic and prices are both roughly stable? (a numbers question)
2. **Why do shoppers perceive the retailer as expensive** when prices haven't changed, and what should be done
   about it before the announcement? (a perception question)

## Step 3 — Score each sub-question

**Sub-question 1** against `checklists.md`: states margin is falling (✓) alongside a related metric — foot
traffic — stated as roughly flat (✓); no major external/operational change stated (✓, points inward); framed
as "why is profitability slipping" — a root-cause ask (✓). **Fires strongly: Profit Optimization.**

**Sub-question 2** against `checklists.md`: centres on perception/image, not product or price (✓, note prices
haven't moved — ruling out a real pricing case); a specific target audience (shoppers) whose *belief* needs to
change (✓); gap between reality (prices unchanged) and perception (seen as expensive) (✓, this is exactly the
brand-communication "signals it fires" pattern). **Fires strongly: Brand Communication.**

**Phrasing-trap check:** sub-question 2 could look like a Pricing case at a glance ("expensive" is a price
word) — but the brief explicitly states prices haven't materially changed, so there's no actual price lever to
analyze. The final recommendation here has to be a perception/message fix, not a price change — that's what
makes it Brand Communication, not Pricing.

## Step 4 — Resolve conflicts

No real conflict here — each sub-question fired cleanly on one type. (A harder version of this brief might have
had sub-question 1's margin decline actually caused by discounting to chase the perception problem, which would
make the two sub-questions interdependent — flag that kind of link for the Integrated Recommendation even when
classification itself is clean.)

## Step 5 — Hand off

- Sub-question 1 → load `case-profit-optimization/SKILL.md` in full. Build the profit tree (Revenue − Cost),
  run the exclusion questions, and note that the brief has already ruled out the classic external-shock and
  traffic-decline explanations — pointing the branch analysis toward cost structure or product mix rather than
  volume.
- Sub-question 2 → load `case-brand-communication/SKILL.md` in full. Since prices haven't moved but perception
  has, the Insight step should dig into *why* shoppers formed that belief (e.g. a rival's aggressive promotional
  visibility, a change in what's easy to compare at shelf, a category-wide narrative) rather than assuming it's
  really about price.

## Step 6 — Integrate (filled-in `output-structure.md`)

```markdown
# Case Structure — Regional Grocery Retailer: Margin Decline + Value Perception

## Overall SCQ
Situation: Like-for-like sales and margin have declined for two quarters while category foot traffic held
roughly steady and no major operational changes occurred.
Complication: Shoppers increasingly see the retailer as "the expensive option" versus a discount rival, despite
prices not materially changing — so perception alone doesn't explain the full margin story.
Question: Why is profitability slipping, and what closes both the financial gap and the perception gap before
the next results announcement?

## Overall Objective
Restore margin to its prior trajectory and close the value-perception gap with the discount rival, in a way
that reinforces rather than undercuts the financial fix — before the next results announcement.

## Sub-question 1 — Margin decline — Case type: Profit Optimization (case-profit-optimization)
[Profit tree output: e.g. root cause isolated to a cost-side branch — say, rising input or shrink costs
outpacing revenue, given traffic and price were both ruled out. Short-term recommendation: address the
specific cost driver. Long-term: renegotiate or restructure the affected cost line.]

**Ties back to the Overall Objective because:** fixing the cost driver restores the margin headroom needed to
fund the perception fix in Sub-question 2, without resorting to a price cut that would reinforce the "expensive"
narrative.

## Sub-question 2 — Value perception — Case type: Brand Communication (case-brand-communication)
[Framework output: e.g. Insight shows the "expensive" belief is driven by the rival's louder promotional
visibility rather than actual price gaps; Big Idea reframes value beyond headline price (e.g. total-basket
value, loyalty economics); IMC/Trade plan emphasizes in-store and channel signals where the comparison actually
happens.]

**Ties back to the Overall Objective because:** the campaign is explicitly built to close the perception gap
without competing on price — protecting the margin just recovered in Sub-question 1 rather than spending it
away on discounting.

## Integrated Recommendation
Fix the cost-side root cause first (Sub-question 1) to restore margin headroom, then fund and launch a
perception campaign (Sub-question 2) that reframes value on non-price terms — sequenced so the campaign doesn't
have to be paid for by a price cut, and the price cut is never on the table at all, which is itself the answer
to why the "expensive" perception shouldn't be met with a price response.
```

## What this example demonstrates

- Two sub-questions, two case types, no overlap in *type* — but real interdependence in the *recommendation*,
  which the Integrated Recommendation section is what surfaces. Classification being clean doesn't mean
  integration is trivial.
- Each sub-answer's tie-back sentence does real work — it's not filler, it's the sentence that turns "two
  correct answers" into "one coherent case."
