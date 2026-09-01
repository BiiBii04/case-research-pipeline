---
type: "Method"
title: "Evidence rules: the tags, the grades, and the honesty checks"
slug: "evidence-rules"
owner: "Thinh Ngo"
project: "case-research-pipeline"
created: "2026-09-01"
last_updated: "2026-09-01"
status: "active"
summary: "The F/I/A confidence tag, two-axis source grading, and the twelve rules that stop research from being confidently wrong. Applies to every stage."
---

# Evidence rules

Research fails quietly. The searches work, the prose reads well, and the conclusion is wrong, because a brochure got treated as fact, a stale page got treated as current, or one unverified number got repeated until it looked corroborated. This file is the guard rail set. Every rule in it exists because someone hit the failure it prevents.

These rules apply everywhere, in every stage. Read this before writing anything that will be cited.

## 1. The claim tag: [F / I / A + NN%]

Every load-bearing claim carries a tag.

| Tag | Meaning | Example |
|---|---|---|
| `[F/NN%]` | **Fact**, checked against an original record | `The company owns land at 63 branches [F/95%]` |
| `[I/NN%]` | **Inference**, your reasoning from evidence | `The loss most likely sits in ground rent [I/70%]` |
| `[A/NN%]` | **Assumption**, unproven, but the read collapses without it | `The 2025 mix holds through 2026 [A/50%]` |

`NN%` is your confidence. **You assign it yourself, at the moment you write the sentence.** Never let a research agent or a verification agent set the final tag. Agents report evidence. Evidence is not yet judgment, and the adjudication is what makes the document defensible.

**Split tags are allowed and usually more honest.** A company survey supports `[F/90% that it is claimed, I/60% that it is representative]`. A judgment stacked on solid signals supports `[F/85% on the signals, I/70% on the conclusion]`.

Calibration guide:

| Situation | Tag |
|---|---|
| Several independent original sources agree | F at 90 to 97 |
| One original source, nothing contradicting it after you went looking | F at 85 to 90 |
| A company's own unaudited figure | F at 80 to 90 **that it is claimed**; whether the figure is true is a separate, lower judgment |
| Well-evidenced reasoning of your own | I at 65 to 85 |
| An inference you want to put above 85 | Stop and go find the record that would make it a fact |
| A load-bearing assumption you cannot test from outside | A at 40 to 60, and it belongs in a visible "what must be true" list, not buried in a paragraph |

The point is not bookkeeping. The point is that typing `[A/50%]` forces you to notice you are standing on an assumption, at the moment you write it, rather than the night before the pitch.

## 2. No fact without a citation

Every fact carries an in-text link that opens, and every file ends with a reference list. A claim you cannot trace is a lead, not a fact, and it gets labelled as one.

Corollary that catches people: **gathered output is an unverified baseline even when it is cited.** A citation at the gathering stage proves where a claim came from, not that it is true. Verification is what upgrades a claim.

Never invent a source. If nothing turns up, write `[source needed]` and leave it visible.

## 3. Two-axis source grading: [R·C]

Every source that carries weight gets two independent grades.

**Reliability (R): the source itself, regardless of the claim.**

| Grade | Meaning |
|---|---|
| R1 | Authoritative: regulator records, official filings, peer-reviewed work, primary data |
| R2 | Credible: established outlets, industry bodies, reputable research firms |
| R3 | Practitioner: trade press, expert blogs, company documentation |
| R4 | Weak: self-published, promotional, unattributed |

**Credibility (C): the specific claim you are taking from it.**

| Grade | Meaning |
|---|---|
| C1 | Corroborated: two or more independent sources agree |
| C2 | Consistent: fits the other evidence, not directly confirmed |
| C3 | Uncorroborated: single source, plausible |
| C4 | Contested: sources disagree |

Two axes catch the two cases one blended score hides: a trustworthy outlet making a weak claim, and a modest outlet reporting a solid original fact.

Two hard rules come with the grades:

1. **A source that is the sole origin of a figure caps at C3**, no matter how many outlets repeat it. Ten articles quoting one survey is one source.
2. **Reliability is relative to the claim type.** A company's own documentation is close to authoritative for "what this company says about itself" and much weaker for "what is true about the market". A source used outside its competence gets capped down.

Weight findings by grade, never by the order they came back in. The first result is not the best result.

## 4. Conflicts are surfaced, never quietly resolved

When two sources disagree on a number, a date, or a fact: both values and both sources go in the file, marked as a conflict. Resolve it only when an original record settles it, and then say so in the text.

Surfacing the conflict is part of the deliverable. A file that reads too clean has usually laundered its contradictions, and the reader has no way to know.

## 5. Claimed versus actual

The most useful distinction in company research. Keep two layers apart: what the company says it does, and what it demonstrably does.

The company's own materials are the best possible source for the first, and a poor one for the second. What actually happens is answered by different evidence: filings, asset registers, live documentation, named customers, third-party records, the physical footprint.

Expect the two layers to disagree. **Where they disagree is very often the most valuable finding in the whole case.**

## 6. Every figure carries its scope

A number without its scope is a trap, and it is the single most common way a case blows up under questioning.

Every figure gets three labels attached at the moment it is written down:

- **Whose**: which entity. The parent group, one country, one segment, one site.
- **When**: which period, and whether it is a point in time or a range.
- **On what basis**: continuing operations or including what was sold, audited or self-reported, like-for-like or including new openings.

The failure this prevents is specific. A group-level figure sitting in a country-level file, unlabelled, will eventually be read as the country's number by someone reading fast. A training programme covering 20,000 people across a group, put next to a country headcount of 14,454, is impossible on its face and will be caught in the room rather than in the draft.

Where two figures for the same thing exist on different bases, both go in, both labelled, per rule 4.

## 7. The absence ban: no negative finding without a positive control

"We could not find it" is a statement about your search, not about the world.

Before publishing an absence, demonstrate that your method finds things that are definitely there. "The company appears on no industry roster, and the rosters we checked do list its named competitors" is a publishable finding. Without the second clause it is a failed search waiting to embarrass you.

## 8. Freshness is not what it looks like

Search-index dates reflect when a page was published or crawled, not when its content was true. A stale page re-crawled yesterday looks current.

For anything time-sensitive, go to the record itself: the register, the live documentation, the current filing, fetched directly.

## 9. Identity and name checks before attribution

Before attributing a finding to a person, name and role and organisation must all match. Common names contaminate searches and corporate groups recycle the same people across entities. One misattributed quote poisons a whole file.

The same applies to companies. Watch for name collisions with unrelated firms, places, or products, and record known collisions early so every later search excludes them.

## 10. Read sources in full, past truncation

File-reading and fetching tools truncate long documents silently. An agent reporting on the first fraction of a long filing produces findings that look complete and are not.

Every agent instruction that involves reading source material must say so explicitly: continue reading with offsets until the whole document is loaded. For long PDFs, read locally from disk rather than through a fetch window.

## 11. State your prior, then hunt against it

Your hypothesis goes in writing before the gathering starts, and one agent in every research wave is dedicated to disconfirming it. Grade the disconfirming evidence with the same rigour as the supporting evidence, or the whole exercise is theatre.

The hypothesis is frozen for the length of a wave, so the research has a steady aim. You update it between waves, in writing, never silently mid-search.

## 12. Derived documents go stale faster than you think

Translations, summaries, slide text and paste-ready versions are all derived from an original file. The moment the original changes, the derived copy is wrong and nothing in it says so.

Three rules:

- Every derived file names its source file and the date it was derived from.
- A warning about an unresolved number goes **at the line where the number appears**, not only in a banner at the top. A reader meets the number three screens below a banner they already scrolled past.
- A stale derived file is more dangerous than no derived file, because its staleness notice only lists what somebody remembered to write in it. When in doubt, regenerate rather than patch.

## Before any official file is marked official

Run a verification pass in fresh context. Its only job is to confirm each citation exists and says what the file claims it says. Fresh context matters: an agent that did the writing believes its own sources.

Then run this list:

1. Does every load-bearing claim carry a tag, assigned by you?
2. Does every figure carry whose, when, and on what basis?
3. Is every conflict shown rather than smoothed over?
4. Does any negative finding have a positive control behind it?
5. Are single-origin numbers capped at C3, however many places repeat them?
6. Is anything in here sourced only from what the subject says about itself, presented as what is actually true?
