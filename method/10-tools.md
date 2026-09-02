---
type: "Method"
title: "Tools: connecting Exa, the parameters that matter, and the traps"
slug: "tools"
owner: "Thinh Ngo"
project: "case-research-pipeline"
created: "2026-09-02"
last_updated: "2026-09-02"
status: "active"
summary: "How to connect the one research tool this method depends on, which parameters change the output, and the silent failures that make research look complete when it is not."
---

# Tools

## Provenance of the rules below

This file follows the same honesty discipline as the method it belongs to, so every rule carries where it came from:

- **[schema]** read directly off the tool definition this repo runs against. Reliable, and it changes when Exa changes the tool.
- **[docs]** from Exa's own documentation, retrieved 2026-09-02.
- **[convention]** a working rule adopted here, not independently tested. Treat as a default, not a finding.

This file is thinner than it should be, and that is stated on purpose. The version of this document worth having is one written from failures you hit yourself. Add to it when a search goes wrong, and say which category the new rule belongs to.

## Connecting Exa

The method depends on one tool. Without it, nothing in the research stage runs.

**Claude Code, the whole plugin** (MCP server plus Exa's own skills): [docs]

```bash
claude plugin install exa@claude-plugins-official
```

**Claude Code, MCP server only:** [docs]

```bash
claude mcp add --transport http exa https://mcp.exa.ai/mcp
```

**Any other client:** point it at `https://mcp.exa.ai/mcp`. [docs]

Confirm it worked by checking that tools named `mcp__exa__web_search_exa` and `mcp__exa__web_fetch_exa` are available. If they are not, restart the client. Some clients need a full restart to pick up a new MCP server. [docs]

### Authentication

The hosted server works anonymously, with rate limits. A `429` is the rate limit, not a bug, and the fix is your own key. [docs]

Get a key at `dashboard.exa.ai/api-keys`, then pass it as an `x-api-key` header, an `Authorization: Bearer` header, or on the URL as `?exaApiKey=...`. OAuth is the option Exa prefers and most clients prompt for it. [docs]

Never commit a key. `.gitignore` here already excludes `.env*` and `.mcp.json`.

### Optional tools worth enabling

Two tools are on by default. Two more are not, and both are useful for case work: [docs]

```
https://mcp.exa.ai/mcp?tools=web_search_exa,web_fetch_exa,web_search_advanced_exa
```

- `web_search_advanced_exa` gives category filters, domain restrictions, date ranges, and subpage crawling. Worth having for the Rules and Rivals slices, where you want one regulator's domain or one date window.
- `agent_run` runs a multi-step Exa Agent. It needs authentication and it bills by usage. This method does not use it, because the multi-step reasoning is supposed to happen in your sub-agents where you can see it.

Note that the `?tools=` list **replaces** the defaults rather than adding to them, so include every tool you want. [docs]

## The parameter that matters most

`web_fetch_exa` defaults `maxCharacters` to **3000**. [schema]

Three thousand characters is roughly an abstract. If you fetch a filing, a research paper or an annual report and do not set this, you get the opening and nothing else, and the agent reading it will write a confident summary of the first two pages as though it read the document.

This is the single most damaging default in the whole toolchain, because it fails silently. There is no error and no truncation notice. The output just looks like a short document.

**Rule: never call `web_fetch_exa` without setting `maxCharacters`.** [convention]

| What you are reading | Set it to |
|---|---|
| A news article or a short page | 10,000 |
| A long article, documentation, a report section | 50,000 |
| A full filing, an annual report, an academic paper | 100,000, and page through with more calls if the end looks cut |

The workspace rule this inherits from says to start at 50,000 for anything that will be cited. That is the floor for a load-bearing source, not a ceiling.

## Batching

`web_fetch_exa` takes `urls` as an array. [schema] Several URLs in one call is one call, not several. Batch every time you have more than one page to read.

## Searching well

`web_search_exa` defaults `numResults` to 10. [schema] Set it explicitly when you want fewer or more, so the cost is a decision rather than a default.

**Write the query as a description of the ideal page, not as keywords.** [docs, and the workspace convention] "Official annual report disclosing segment revenue by country for 2025" beats "annual report revenue country". The index is semantic, so a fuller sentence retrieves better than a denser one.

Category filters `category:people` and `category:company` search LinkedIn profiles and company pages. [schema] Useful for the People and Rivals slices.

**Search gives you highlights, not the document.** The highlights are an algorithm's pick, usually an abstract and a conclusion. They are fine for deciding what to read. They are never enough to carry a claim. Every load-bearing source gets a follow-up fetch. [convention, and the workspace rule]

## Reading long documents past truncation

Two separate truncation problems, and they are easy to confuse:

1. **Fetch truncation**, fixed by `maxCharacters` above.
2. **Local file truncation**, when a file-reading tool returns the first portion of a long PDF or markdown file and stops. The fix is to keep reading with offsets until the document is loaded.

Both fail without an error. Any agent instruction that involves reading source material must say explicitly that the agent continues until the whole document is loaded, because an agent that stops at the default will report as though it finished. [convention]

For long PDFs the user already has, reading locally from disk beats fetching. It is more reliable, it is free, and nothing gets silently cut.

## Paywalls

Before searching for or fetching a source likely behind a paywall, stop and ask the user. Many students and professionals have library access and can put the full PDF on disk, which reads better than any fetch. [convention]

**Never characterise a paywalled work from its abstract.** Mark it `abstract only` in the source list and treat it as unable to carry a claim, per `method/02-evidence-rules.md`.

## Cost

Exa bills by usage, and the spend is driven by how much you crawl rather than by how big the case is.

The levers, in order of size:

1. **Choose what to read in full.** Deep reading is the expensive part and it is also the point. The saving comes from picking fewer sources to read properly, never from reading many sources shallowly.
2. **Set `maxCharacters` deliberately**, both directions. Do not pay 100,000 characters for a press release.
3. **Batch fetches.**
4. **Set `numResults` explicitly** rather than taking 10 every time.

## Recording tool behaviour you discover

When something surprises you, add it here with its category, the date, and what it cost you. A rule with a story attached gets followed. A rule without one gets skipped.

| Date | What happened | The rule now |
|---|---|---|
| | | |
