---
name: Daily Curation
schedule: daily
skill: .agents/skills/daily-curation/SKILL.md
---

# Daily Curation Automation

Run a daily compounding pass from the vault root.

## Prompt

Run the daily curation pass for this second brain.

Use `AGENTS.md` as the root contract and `.agents/skills/daily-curation/SKILL.md`
as the workflow. Preserve raw sources, curate durable knowledge into `wiki/`,
update `wiki/index.md` when navigation changes, and append meaningful work to
`wiki/log.md`.

Be conservative with broad reorganizations. If the category map no longer fits,
record the recommendation instead of moving large parts of the vault without
explicit approval.

