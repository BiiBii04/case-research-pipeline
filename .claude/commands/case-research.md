---
description: Start or resume a company case study through the full pipeline, from scoping to defense preparation.
---

# /case-research

Run the case research pipeline for: **$ARGUMENTS**

If no company or case was named, ask for one before doing anything else.

## Step 1. Check that Exa is connected

Look for tools named `mcp__exa__web_search_exa` and `mcp__exa__web_fetch_exa`.

If they are missing, stop and print this, then wait:

> This pipeline needs the Exa MCP server, and it is not connected. Install it with one of:
>
> ```bash
> claude plugin install exa@claude-plugins-official
> claude mcp add --transport http exa https://mcp.exa.ai/mcp
> ```
>
> Restart Claude Code afterwards, then run `/case-research` again. Full setup notes are in `method/10-tools.md`.

Do not continue without it. Every research stage depends on it, and falling back to a built-in web tool produces work that fails this method's own sourcing rules.

## Step 2. Resume, or start

Check whether `cases/<slug>/00-state.md` exists for this case.

**If it exists, this is a resume.** Read that file and nothing else first. It tells you the stage, what is locked, what is contested, and the next action. Report where the work stands in three or four lines, confirm the next action with the user, then continue from there. Do not restart and do not re-derive settled conclusions.

**If it does not exist, this is a new case.** Continue to step 3.

## Step 3. Set up

1. Ask for the case brief and the rubric or judging criteria. If either is a PDF, convert it to markdown in the case folder first and work from the markdown afterwards, so later sessions never reopen the PDF.
2. Create `cases/<slug>/` and copy `templates/state.md` to `cases/<slug>/00-state.md`.
3. Write `01-brief.md`: the client, the stated ask, the constraints, and the criteria the work will be judged against, as one clean digest.

## Step 4. Phase 0, scope

Before any search, get three things into `00-state.md`, asking the user directly for each:

- **Why** this case is being worked, and what changes depending on the answer.
- **The decision** it feeds, in one sentence, and by when.
- **The user's prior**: what they already believe about this company and this problem.

Push on the prior if they skip it or keep it vague. It is the cheapest defense against spending the whole case building support for a first instinct, and it is the one people avoid writing down.

## Step 5. Run the stages

Read `method/01-spine.md` now if you have not. Then work the stages in order, reading the method file for each stage as you enter it. The routing table is in `SKILL.md`.

Three things that apply throughout:

- **One heavy stage per session.** Stop before the writing step if the session has run long, and write fresh next time.
- **Every gate ends with a challenge.** Write the strongest argument against the current conclusion, name a live alternative, and state the evidence that would change the call. Do not advance until the user engages with it. Log anything unresolved to Open tensions.
- **Tags and judgment stay with the user.** Sub-agents gather and verify. They never assign a confidence tag, never adjudicate the competing hypotheses, and never write an official file. `method/02-evidence-rules.md` explains why.

## Step 6. Close the session

Whenever work stops, before anything else:

1. Update `00-state.md`: where we are, what got locked, the next action, any new open tension.
2. Drain any pending cross-slice findings in `03-research/*/inbound/pending/`.
3. Tell the user in two lines what moved and what the next action is.

A session that ends without this costs the next session twenty minutes of rediscovery.
