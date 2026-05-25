# Adapt This Template

Use this file when creating a new second brain from the template.

The template is meant to work for many kinds of base folders:

- research projects
- school notes
- wedding planning
- household administration
- health records
- creative writing
- company or team knowledge
- personal life archives

Do not preserve the starter categories just because they exist. Preserve the
transport mechanism and adapt the domain model.

## What Should Stay Stable

- `AGENTS.md` stays short and carries the full agent rule set.
- `.agents/skills/` holds repeatable workflows.
- `.agents/automations/` holds recurring workflow definitions.
- `schema/` is the human-readable operating model.
- `raw/unprocessed/` is the inbox.
- `raw/processed/` is the reviewed source archive.
- `wiki/` is the maintained synthesis layer.
- `wiki/index.md` is the navigation map.
- `wiki/log.md` records meaningful curation.

## What Should Change

- The folders inside `wiki/`.
- The category descriptions in `schema/category-map.md`.
- Any domain-specific skills in `.agents/skills/`.
- The daily automation prompt details if the vault has special review needs.

## Adaptation Workflow

1. Inspect the target folder and existing files.
2. Identify the vault's real purpose and reopening patterns.
3. Replace the starter categories in `schema/category-map.md`.
4. Create matching folders under `wiki/`.
5. Update `wiki/index.md` to match those folders.
6. Add narrow skills for repeated workflows in this domain.
7. Keep `AGENTS.md` short; only extend it when a rule truly applies every session, otherwise put it in a skill.

## Good Adaptation Test

A user should be able to say:

```text
Use this second-brain template for this folder and adapt it to the domain.
```

The agent should know to keep the lifecycle, instruction transport, and daily
compounding loop, while replacing the category map to fit the folder.

