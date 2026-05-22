# Second Brain Agent Contract

This repository is an Obsidian-compatible second brain. It preserves raw source
material, then gradually curates it into concise, linked wiki pages that
compound over time.

## Source Of Truth

- `schema/` contains the durable rules, templates, category map, and workflows.
- `.agents/automations/` contains portable automation definitions.
- `.agents/rules/` contains path-scoped constraints.
- `.agents/skills/` contains task-specific workflows.
- `AGENTS.md` should stay small. Do not turn it into a mini-wiki of the vault.

## Knowledge Lifecycle

- New source material starts in `raw/unprocessed/`.
- Reviewed source material moves to `raw/processed/`.
- Durable synthesis lives in `wiki/`.
- Good answers and maintenance discoveries should be filed back into `wiki/` when durable.
- Supporting files live near their source bundle when possible.
- Shared attachments may live in `attachments/`.

## Hard Rules

- Preserve raw material. Do not rewrite originals for style.
- Search existing wiki pages before creating a near-duplicate.
- Prefer concise curated pages over copied raw dumps.
- Use Obsidian wikilinks for internal wiki references.
- Cite processed raw sources from curated pages.
- Update `wiki/index.md` when creating, renaming, merging, or retiring curated pages.
- Update `wiki/log.md` after meaningful curation or maintenance work.
- Update `schema/` before making major structural changes.
- Always inspect current files before relying on summaries.

## Routing

- Use `.agents/skills/ingest-note/` for processing raw notes.
- Use `.agents/skills/synthesize-topic/` for building or refreshing topic pages.
- Use `.agents/skills/maintain-wiki/` for duplicates, stale pages, broken links, and structure checks.
- Use `.agents/skills/answer-from-vault/` for answering questions from the vault.
- Use `.agents/skills/daily-curation/` for scheduled compounding passes.
- Use `.agents/automations/daily-curation.md` as the portable daily automation definition.
