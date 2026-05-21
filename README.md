# Second Brain Template

This repository is a generic template for an Obsidian-compatible second brain.
It is designed to preserve messy source material first, then gradually turn it
into concise, linked wiki pages.

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

## Structure

```text
AGENTS.md
.agents/
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
- `.agents/rules/` contains path-scoped constraints.
- `.agents/skills/` contains repeatable workflows.
- `schema/` contains the human-readable source of truth for how the vault works.
- `raw/unprocessed/` is the inbox for source material.
- `raw/processed/` stores reviewed originals.
- `wiki/` contains curated pages.
- `attachments/` is for shared supporting files when they are not bundled with a raw source.

## Starting A New Vault

1. Copy this template into a new folder.
2. Edit `schema/category-map.md` for the new vault's domains.
3. Keep `AGENTS.md` small and stable.
4. Add path-specific guidance to `.agents/rules/`.
5. Add repeatable procedures to `.agents/skills/`.
6. Put new source material into `raw/unprocessed/`.
7. Ask an agent to use the ingest workflow when you are ready to curate.

