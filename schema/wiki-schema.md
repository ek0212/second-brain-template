# Wiki Schema

This repository is a second brain maintained from raw notes, exports, documents,
conversations, and other source material. The goal is not to perfectly file
everything on the first pass. The goal is to preserve sources, then gradually
curate them into reliable, useful pages.

The vault is intended to work well in Obsidian. Optimize for readable filenames,
wikilinks, backlinks, aliases, tags, and a useful graph.

## Layers

- `raw/unprocessed/` contains newly added source material that has not been reviewed.
- `raw/processed/` contains original source material after review.
- `wiki/` contains curated pages written from raw material and direct knowledge.
- `schema/` contains maintenance instructions, templates, category definitions, and workflow notes.
- `.agents/` contains agent-facing rules and task workflows.

## Curated Pages

Curated pages should be short, clear, and useful. They should not copy every raw
detail unless the detail is durable and worth finding again.

Use this default frontmatter:

```yaml
---
aliases: []
tags: []
status: draft
sources: []
---
```

Use `status` values:

- `draft` for newly synthesized pages that may need review.
- `stable` for pages that feel reliable.
- `stale` for pages likely outdated.

Use tags sparingly for cross-cutting qualities, not for the main category.

## Raw Material

Raw material can be messy, duplicated, emotional, generated, obsolete, or unclear.
That is acceptable. Preserve it as evidence.

Do not rewrite raw notes for style or category fit. If cleanup, summarization,
deduplication, or synthesis is useful, create or update a curated page in `wiki/`,
move the reviewed source to `raw/processed/`, and cite it from the curated page.

## Cross-References

The wiki should become interlinked over time.

Use cross-references when:

- a source affects more than one topic
- a topic appears in several contexts
- a page summarizes or updates an older page
- a page depends on a person, place, project, decision, routine, or source described elsewhere
- a raw note should inform multiple curated pages

Prefer links over duplication:

```markdown
See also: [[Related Page]]
```

Use aliases when the displayed text should differ:

```markdown
See also: [[Related Page|display text]]
```

For pages with several related notes, add a short section near the bottom:

```markdown
## Related

- [[Related Page]] - why it matters here.
- [[Another Page]] - how it connects.
```

## Index

`wiki/index.md` is the content-oriented catalog of the curated wiki. Update it
when curated pages are created, renamed, merged, or retired.

The index should list useful hubs and important pages. It does not need to list
every tiny note unless that is useful for the vault.

