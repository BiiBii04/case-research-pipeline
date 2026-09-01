---
type: "Research dossier"
title: "{company}: {slice} slice"
slug: "{company-slug}-{slice}"
owner: "{your name}"
project: "{project}"
created: "{YYYY-MM-DD}"
last_updated: "{YYYY-MM-DD}"
status: "draft"
slice: "{bet | entity | offer | customers | rivals | machine | rules | people}"
wave: "{n}"
---

# {company}: {slice}

**Owns (single source of truth):** {the facts this file is the home for}

**Does not own:** {each adjacent slice, and which file owns it instead. Be specific: "competitor funding rounds, owned by rivals.md" beats "other stuff".}

**Tag legend:** `[F/NN%]` fact checked against an original record. `[I/NN%]` inference from evidence. `[A/NN%]` assumption the read depends on. Percentage is the author's confidence, assigned at write time. Source grades are `[R1-R4 · C1-C4]`, reliability and corroboration. Full definitions in `method/02-evidence-rules.md`.

---

## The short version

{Three to five sentences. The findings that would change what someone does, first. Not a description of what is in the file.}

## {Section: a question this slice answers}

{Answer first, then the support. Headings carry the message: "Ground rent, not margin, is where the loss sits" beats "Costs".}

{Every load-bearing claim carries a tag and an in-text citation. Every figure carries whose, when, and on what basis.}

## Surfaced conflicts

> Both values, both sources. Resolved only when an original record settles it, and then say so.

| The disagreement | Source A | Source B | Status |
|---|---|---|---|
| {what} | {value, citation} | {value, citation} | {carried, or resolved in favour of X because Y} |

## What must be true

> The assumptions this slice's read depends on, pulled out of the prose so they are visible. Anything tagged `[A/...]` belongs here.

| Assumption | Tag | How it could be tested |
|---|---|---|
| {statement} | {[A/NN%]} | {what would settle it} |

## Open questions

{What this slice could not answer, and where you looked. A gap nobody wrote down is indistinguishable from a topic with nothing in it. These become gap-fill wave triggers.}

## Routed out

| To slice | The finding | Date |
|---|---|---|
| {slice} | {one line} | {YYYY-MM-DD} |

## Absorbed in

| From slice | The finding | Date |
|---|---|---|
| {slice} | {one line} | {YYYY-MM-DD} |

## Sources

| # | Source | Grade | Read depth |
|---|---|---|---|
| 1 | {author or org, title, date, URL} | {R2 · C1} | {read in full / read excerpts / abstract only} |

> Read depth is recorded honestly. Only sources read in full, or substantially in excerpt, may carry a claim.
