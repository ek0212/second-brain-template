# Ingest Workflow

Use this workflow when turning source material into curated wiki pages.

1. Read the source note in `raw/unprocessed/`.
2. Decide whether it should remain raw-only or deserves curated extraction.
3. Search `wiki/` for related pages and near-duplicate titles.
4. Choose the best existing page to update, or create a new page if needed.
5. Preserve the original source.
6. Move reviewed source material to `raw/processed/`.
7. Link the curated page back to the processed raw source.
8. Add wikilinks to related pages where useful.
9. Update `wiki/index.md` if a curated page was created or became important.
10. Add uncertainties under `Open Questions`.

## Raw-Only Sources

Some sources do not need immediate curation. If a source is reviewed but remains
raw-only, move it to `raw/processed/` and optionally add a short note explaining
why it was preserved without synthesis.

