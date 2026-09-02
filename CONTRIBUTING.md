---
type: "Reference"
title: "Working on this repo: branch model, review, and house style"
slug: "contributing"
owner: "Thinh Ngo"
project: "case-research-pipeline"
created: "2026-09-02"
last_updated: "2026-09-02"
status: "active"
summary: "How two people work separate approaches on this method and compare them without stepping on each other."
---

# Working on this repo

Two people, two approaches, one method. This file is the convention so that comparing them later is easy.

## The branch model

`main` is what both of us have agreed on. Nothing lands there until we have talked about it.

Everything else happens on your own branch:

```
approach/<your-name>-<what-you-are-changing>
```

For example `approach/thinh-lighter-scoring` or `approach/minh-merge-frame-and-research`.

One branch per idea, not one branch per person. If you want to try two different things, make two branches, because a branch carrying two unrelated ideas cannot be half-accepted.

## Getting set up

This repo is a Claude Code skill, so clone it where Claude Code will find it:

```bash
git clone https://github.com/BiiBii04/case-research-pipeline.git \
  ~/.claude/skills/case-research-pipeline
cd ~/.claude/skills/case-research-pipeline
git checkout -b approach/<your-name>-<topic>
```

Whatever branch is checked out is the version Claude Code loads. That is the point: check out your branch, run a real case through it, and see what breaks.

## Before you open a pull request

Open it as a **draft**. A draft PR is the comparison surface: it shows the diff file by file, and either of us can leave a comment on a specific line during a call. It does not have to be finished to be useful.

In the PR description, answer three questions in a paragraph each:

1. **What did you change, and where.** Which method files, which rules.
2. **What failure were you fixing.** Name the thing that went wrong, ideally something you hit on a real case rather than something that felt untidy.
3. **What does this cost.** Every change to a method makes something else harder. Say what.

The third one is the useful one. A change with no stated cost has usually not been thought through, and it is the question we should each be asking the other.

## House style

The method files are prose, and they get read under time pressure. Match what is already there:

- No em-dashes. Commas, periods, colons, or a new sentence.
- Straight quotes only.
- Sentence-case headings.
- One paragraph per line. No hard wrapping inside a paragraph, because it makes diffs unreadable.
- Answer first. The heading carries the message: "Ground rent, not margin, is where the loss sits" beats "Costs".
- Lean on tables. A rule that fits in a table row is easier to follow than the same rule in a paragraph.

Every method and template file opens with a YAML frontmatter block. Copy the shape from a neighbouring file and bump `last_updated` when you change one.

## What does not get committed

`cases/` is ignored. Your own case research, client material and working notes stay on your machine. This repo holds the method, not the work done with it.

Also ignored: `.env`, `.mcp.json`, and anything else carrying a key.

## Deciding between two approaches

When we compare, argue on these, in this order:

1. **Does it prevent a failure that actually happened?** Not one we imagined.
2. **Does it survive a lazy user?** A rule that only works when someone is being careful is not a rule, it is a hope. The good rules force the work rather than request it.
3. **What does it cost in time on a real case?** Every gate added is a gate someone will skip at 1am the night before a deadline.
4. **Can a stranger follow it?** If a rule needs one of us in the room to explain it, it needs rewriting, not defending.

If we cannot agree, the method has an answer for that: log it as an open tension, keep both readings written down, and let the next real case settle it.
