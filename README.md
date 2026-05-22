# Second Brain Template

This repository is a generic template for an Obsidian-compatible second brain.
It is designed to preserve messy source material first, then gradually turn it
into concise, linked wiki pages that compound over time.

The template is intentionally domain-agnostic. A vault created from it could be
for research, school, wedding planning, a company, a creative project, health
records, family history, or any other knowledge domain. The categories should
change. The transport mechanism should stay stable.

## Core Idea

Use the same lifecycle in every vault:

```text
new source material
  -> raw/unprocessed/
  -> reviewed by a person or agent
  -> durable synthesis in wiki/
  -> original preserved in raw/processed/
  -> index and related links updated
```

The folder names are stable, but the categories inside `wiki/` should be
customized for each vault.

## What Makes It Work

The important reusable system is not the starter taxonomy. It is the way context
moves through the vault:

```text
AGENTS.md
  -> points agents to stable source-of-truth files
.agents/rules/
  -> applies path-specific constraints while files are edited
.agents/skills/
  -> runs repeatable workflows such as ingest, synthesis, and maintenance
schema/
  -> stores the durable operating model humans can inspect and revise
raw/
  -> preserves source material
wiki/
  -> accumulates maintained synthesis
wiki/index.md and wiki/log.md
  -> keep navigation and change history alive
```

This is the compounding loop: every ingest, maintenance pass, and useful answer
should leave the wiki slightly easier to use next time.

## Structure

```text
AGENTS.md
.agents/
  automations/
  rules/
  skills/
attachments/
raw/
  unprocessed/
  processed/
schema/
wiki/
  index.md
```

- `AGENTS.md` is the small always-loaded contract for agents.
- `.agents/automations/` contains portable automation definitions.
- `.agents/rules/` contains path-scoped constraints.
- `.agents/skills/` contains repeatable workflows.
- `schema/` contains the human-readable source of truth for how the vault works.
- `raw/unprocessed/` is the inbox for source material.
- `raw/processed/` stores reviewed originals.
- `wiki/` contains curated pages.
- `attachments/` is for shared supporting files when they are not bundled with a raw source.

## Starting A New Vault

1. Copy this template into a new folder.
2. Read `schema/adapt-this-template.md`.
3. Edit `schema/category-map.md` for the new vault's domain.
4. Keep `AGENTS.md` small and stable.
5. Add path-specific guidance to `.agents/rules/`.
6. Add repeatable procedures to `.agents/skills/`.
7. Configure a daily curation automation from `.agents/automations/daily-curation.md`.
8. Put new source material into `raw/unprocessed/`.
9. Ask an agent to use the ingest workflow when you are ready to curate.

## Bootstrap Prompt

Use a prompt like this when pointing an agent at a new folder:

```text
Use this second-brain template for this folder. Adapt the category map and wiki
index to the folder's domain, but preserve the raw/unprocessed -> raw/processed
-> wiki lifecycle, AGENTS.md contract, .agents rules, .agents skills, and daily
curation automation pattern. Keep AGENTS.md small. Put domain-specific behavior
in schema, rules, skills, or automation definitions.
```
