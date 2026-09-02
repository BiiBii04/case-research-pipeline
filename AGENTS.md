---
type: "Reference"
title: "Agent entry point for the case-research-pipeline repo"
slug: "agents"
owner: "Thinh Ngo"
project: "case-research-pipeline"
created: "2026-09-02"
last_updated: "2026-09-02"
status: "active"
summary: "What this repo is, which file to read depending on why you are here, and the rules that apply to any edit."
---

# Agent entry point

## What this repo is

A **method**, written in markdown. There is no code, no build, no tests, and nothing to run. Every file here is instructions for how to work a company case study.

Two different reasons to be here, and they lead to different files.

## If you are here to use the method on a real case

Read `SKILL.md` first. It routes you to the right method file for whichever stage you are on.

Then `method/01-spine.md` for the stages and gates, and `method/02-evidence-rules.md` before writing anything that will be cited.

The case's own working files go in `cases/<slug>/`, which is gitignored. **Never commit case material.** This repo holds the method, not the work done with it.

## If you are here to change the method

Read `CONTRIBUTING.md`. It has the branch convention, what a pull request has to explain, and the four questions used to decide between two competing approaches.

The short version: `main` is what everyone has agreed on, every idea gets its own `approach/<name>-<topic>` branch, and comparison happens in a draft pull request.

## Two ways to install this

They are different, and picking the wrong one is the usual reason something does not work.

**To develop the method:** clone anywhere, `cd` in, run `claude`. You get this file, `CLAUDE.md`, and the `/case-research` command. This is the mode for editing the method itself.

```bash
git clone https://github.com/BiiBii04/case-research-pipeline.git
cd case-research-pipeline
claude
```

**To use the method on cases in other projects:** clone into the Claude Code skills directory. The skill then loads on its own whenever a case-shaped request appears, in any project.

```bash
git clone https://github.com/BiiBii04/case-research-pipeline.git \
  ~/.claude/skills/case-research-pipeline
```

In this second mode the `/case-research` command is not registered, because project commands only load from the directory Claude Code was opened in. That is expected, and the skill still triggers from its description.

## The tool this depends on

Exa, connected as an MCP server. Setup is in `method/10-tools.md`, along with the parameter defaults that will quietly ruin research if left alone. Read that file before running the research stage for the first time.

Web research is Exa only. Do not fall back to a built-in web tool without saying so in the output.

## Rules for any edit you make here

- **No em-dashes.** Commas, periods, colons, or a new sentence.
- **Straight quotes only.**
- **Sentence-case headings.**
- **One paragraph per line.** No hard wrapping inside a paragraph, because it makes diffs unreadable.
- **Answer first.** The heading carries the message, not the topic label.
- Every file in `method/` and `templates/` opens with a YAML frontmatter block. Copy the shape from a neighbour and bump `last_updated`.
- Do not add code, scripts or build tooling. If a rule needs a script to be followed, the rule is wrong.

## The one thing not to get wrong

This method exists because research fails quietly: the searches work, the prose reads well, and the conclusion is wrong. Every rule here blocks a specific failure of that kind.

So when you edit, do not smooth a rule into something more agreeable. If a rule seems annoying, that is usually the rule doing its job. Change it only when you can name the failure it was blocking and explain why that failure no longer applies.
