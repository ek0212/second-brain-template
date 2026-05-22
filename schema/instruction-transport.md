# Instruction Transport

This vault uses a layered instruction system so agents can keep the wiki alive
without loading every detail into every session.

## Layers

```text
AGENTS.md
  -> small always-loaded contract
.agents/rules/
  -> path-scoped constraints
.agents/skills/
  -> task-specific workflows
.agents/automations/
  -> recurring workflow definitions
schema/
  -> human-readable operating model
raw/
  -> preserved source material
wiki/
  -> maintained synthesis
wiki/index.md
  -> navigation map
wiki/log.md
  -> curation history
```

## Responsibilities

`AGENTS.md` answers: What must every agent know every session?

`.agents/rules/` answers: What constraints apply when touching these paths?

`.agents/skills/` answers: What procedure should run for this kind of task?

`.agents/automations/` answers: What recurring agent work should happen without
waiting for a one-off prompt?

`schema/` answers: What is the durable, human-readable operating model?

`raw/` answers: What source material exists and what has been reviewed?

`wiki/` answers: What does the vault currently know?

## Compounding Flow

1. Source material enters `raw/unprocessed/`.
2. An ingest skill turns durable pieces into `wiki/` pages.
3. Path rules keep page shape, source citation, and index updates consistent.
4. Good answers and maintenance discoveries are filed back into `wiki/`.
5. The daily curation automation checks for new sources, weak links, stale pages, and missed updates.
6. `wiki/index.md` and `wiki/log.md` make the next agent pass easier.

The system is working when every useful pass reduces future rediscovery.

