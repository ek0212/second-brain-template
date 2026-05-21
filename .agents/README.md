# Agent Instructions

This directory holds agent guidance that should not live in the always-loaded
root `AGENTS.md`.

## Rules

Use `.agents/rules/` for constraints that are always relevant or relevant to
specific paths.

Good examples:

- Wiki pages need frontmatter and sources.
- Raw material must be preserved.
- Schema files define the operating model.

## Skills

Use `.agents/skills/` for repeatable workflows and deeper procedural guidance.

Good examples:

- Ingest a raw note.
- Synthesize a topic across the vault.
- Maintain the wiki.
- Answer a question using curated pages first.

Prefer narrow skills over giant generic playbooks.

