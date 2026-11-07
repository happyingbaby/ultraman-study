# Domain Docs

## Before exploring, read these

- `CONTEXT.md` at the repo root: existing project requirements and domain vocabulary. Preserve it as the current source of project context.
- `GLOSSARY.md` at the repo root: resolved domain terms, when available.
- `docs/adr/`: read decisions relevant to the area being explored.

If the glossary or ADR files do not exist, proceed silently. Do not flag their absence or create empty placeholders. The `/domain-modeling` skill creates them lazily when terms or decisions are resolved.

## File structure

This is a single-context repo. Use one root `GLOSSARY.md` and root `docs/adr/` for architectural decisions. Do not create a `GLOSSARY-MAP.md` or per-context directories for this layout.

## Use the glossary's vocabulary

Use the terms defined in `GLOSSARY.md` when naming domain concepts in issues, proposals, hypotheses, or tests. Until the glossary exists, use the vocabulary already recorded in `CONTEXT.md`. Avoid synonyms the domain documentation explicitly rejects.

If a needed concept is missing, reconsider whether it belongs to the domain or note the gap for `/domain-modeling`. Do not invent a resolved definition.

## Flag ADR conflicts

If a proposal contradicts an existing ADR, explicitly identify the ADR and explain why it should be reconsidered rather than silently overriding it.
