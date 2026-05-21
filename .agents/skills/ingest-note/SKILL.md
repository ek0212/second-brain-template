# Ingest Note

Use this skill when processing new raw notes, imported documents, transcripts,
clips, exports, or conversation summaries.

## Workflow

1. Inspect `raw/unprocessed/`.
2. Read the relevant source material.
3. Decide whether the source should remain raw-only or deserves curated extraction.
4. Search `wiki/` for related pages, duplicate titles, people, places, projects, and recurring topics.
5. Create a new curated page only if no suitable page exists.
6. Prefer updating an existing page over creating a near-duplicate.
7. Move reviewed source material to `raw/processed/`.
8. Add the processed source path to the curated page frontmatter.
9. Add wikilinks to related pages where useful.
10. Update `wiki/index.md` if a curated page was created, renamed, merged, or became important.

## Output

Summarize:

- Which raw files were processed.
- Which wiki pages were created or updated.
- Which sources were moved to `raw/processed/`.
- Any open questions or uncertain categorization.

