---
name: case-research-pipeline
description: A staged, gated pipeline for solving company case studies, from scoping and problem framing through deep company research, root-cause diagnosis, solution generation, scored selection, and defense preparation. Use this whenever the user is working a business case study, a consulting-style company problem, a capstone or assignment that asks them to diagnose a company and recommend a solution, or anything where they hand over a case brief and need a rigorous, defensible answer rather than a quick take. Trigger it even when the user does not say "pipeline": phrases like "I have a case study", "help me solve this company's problem", "here is the client brief", "we need to find the root cause", "what should this company do", "research this company for me", or "I have to pitch a solution to a panel" should all pull this in. Drives the work in stages, challenges the user's reasoning at every gate, and keeps durable state so a fresh session can resume cold.
---

# Case research pipeline

This file is the map. The methods live in `method/`, and you read the relevant one when you enter a stage. Do not try to run a stage from memory of this file.

## Read first, always

`method/01-spine.md` holds the stages, the gates, the state file, and the rules that apply everywhere. Read it at the start of any case.

`method/02-evidence-rules.md` holds the tagging and sourcing rules. They apply to every word written in every stage, so read it before writing anything that will be cited.

## Then, per stage

| Stage | Read this | Produces |
|---|---|---|
| 0. Scope | `method/01-spine.md` | `00-state.md` |
| 1. Frame | `method/04-framing.md` | `02-frame.md` |
| 2. Research | `method/03-company-map.md` and `method/05-research.md` | `03-research/synthesis.md` |
| 3. Root cause | `method/06-root-cause.md` | `04-root-cause/synthesis.md` |
| 4. Ideate | `method/07-ideation.md` | `05-solutions/candidates.md` |
| 5. Score | `method/08-scoring.md` | `05-solutions/scored-shortlist.md` |
| 6. Decide | `method/01-spine.md`, the Decide section | `06-decision.md` |
| 7. Defend | `method/09-defense.md` | `07-defense.md` |

## Starting a case

1. Ask for the case brief and the rubric or judging criteria.
2. Create `cases/<slug>/` and copy `templates/state.md` to `00-state.md`.
3. Digest the brief and the criteria into `01-brief.md` as one clean file. If the brief is a PDF, convert it first and work from the markdown afterwards, so later sessions never reopen the PDF.
4. Run Phase 0 scoping, then enter the Frame stage.

If `00-state.md` already exists, this is a resume. Read it and orient from where the work stands. Do not restart.

## Tool routing

`method/10-tools.md` has the setup, the parameters, and the traps. Read it before the first research stage. The rules below are the summary, not the file.

- **Web research is Exa only.** `mcp__exa__web_search_exa` to find sources, `mcp__exa__web_fetch_exa` to read them. Do not fall back to a built-in web tool without saying so.
- **Read load-bearing sources in full.** Search results give you highlights, usually an abstract and a conclusion. Never build an argument on those. Fetch the source with a high character limit and read the body.
- **Flag paywalls before fetching.** If a source is likely behind one, stop and tell the user, who may have library access and can supply the PDF for direct reading. Never characterise a paywalled work from its abstract.
- **Fan out with sub-agents.** In the research stage, spawn one agent per company slice, in parallel, in a single message.
- **PDFs are read locally.** A long filing read from disk beats the same filing read through a fetch window.
- **Never fetch without setting `maxCharacters`.** It defaults to 3,000, which is about an abstract, and it truncates with no error. This is the most damaging default in the toolchain.

## What never gets delegated

Sub-agents gather, fetch and verify. They do not judge. These steps stay in the main conversation with the user:

- Assigning any `[F/I/A + NN%]` tag.
- The competing-hypotheses adjudication in the root-cause stage.
- The attack on your own leading conclusion.
- The scoring calls.
- Writing any official file.

The reason is in `method/02-evidence-rules.md`, section 1: agents report evidence, and evidence is not yet judgment.

## Output conventions

No em-dashes. Straight quotes only. Sentence-case headings. One paragraph per line, no hard wrapping. Lean on tables so files stay scannable.

Write answer-first. Lead with the finding, then the support, and make headings carry the message rather than label the topic. "Ground rent, not operating margin, is where the loss sits" is a heading. "Costs" is not.
