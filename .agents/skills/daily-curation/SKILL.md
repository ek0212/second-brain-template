# Daily Curation

Use this skill for the recurring maintenance pass that keeps the second brain
compounding.

## Workflow

1. Read `AGENTS.md`, `schema/wiki-schema.md`, `schema/category-map.md`, and `wiki/index.md`.
2. Inspect `raw/unprocessed/` for new source material.
3. If new source material exists, process a manageable batch with `.agents/skills/ingest-note/`.
4. Search for wiki pages that are missing sources, missing index entries, or have unresolved `Open Questions`.
5. Check whether recent sources should update existing pages instead of creating new ones.
6. Improve cross-links when proper nouns, projects, places, concepts, or decisions recur.
7. Update `wiki/index.md` when navigation changes.
8. Append meaningful work, skipped work, and recommendations to `wiki/log.md`.

## Priority Order

1. Preserve raw sources.
2. Curate high-signal new material.
3. Update existing pages before creating new pages.
4. Improve links and index entries.
5. Record open questions and maintenance recommendations.

## Batch Limits

Keep daily passes modest. If there is too much raw material to process safely,
process the highest-signal batch and record what remains in `wiki/log.md`.

## Log Entry Format

```markdown
## YYYY-MM-DD

- Processed:
- Updated:
- Moved:
- Open questions:
- Next pass:
```

