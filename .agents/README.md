# Agent Instructions

This directory holds agent guidance that should not live in the always-loaded
root `AGENTS.md`.

The goal is progressive disclosure: load the smallest stable contract first,
then pull in rules, skills, and automation definitions only when they matter.

## Automations

Use `.agents/automations/` for portable definitions of recurring agent work.

Good examples:

- Daily curation pass.
- Weekly link and stale-page review.
- Monthly source audit.

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
