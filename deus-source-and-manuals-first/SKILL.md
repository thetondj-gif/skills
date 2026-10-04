---
name: deus-source-and-manuals-first
description: Inspect canonical source, manuals, schemas and current implementation before changing a system; preserve provenance and reject stale assumptions.
version: 1.0.0
license: MIT
metadata:
  deus:
    scope: estate-wide
    source_repo: thetondj-gif/hermes-agent
    source_upstream: NousResearch/hermes-agent
    source_ref: 8b66a51036c1e20920a17cdd049fdf55c968d683
    source_license: MIT
    adaptation: Deus Intus operating logic; no Hermes runtime dependency
---
# Deus Source and Manuals First

## Procedure
1. Identify the canonical implementation and current owner/source of truth.
2. Read the relevant README, AGENTS.md, SKILL.md, API/tool schema, configuration and recent implementation evidence before editing.
3. Prefer first-party/current documentation over remembered syntax.
4. Resolve IDs, paths, branches, schemas and authority boundaries from evidence; never invent them.
5. Compare discovered instructions with current Deus doctrine. Deus authority boundaries win over donor-runtime assumptions.
6. Preserve source repository, path, ref/SHA, licence, dependencies and modification status for imported capability logic.
7. Execute against the current interface, then verify the result independently.

## Failure handling
If documentation conflicts with runtime behaviour, record the conflict as candidate learning; prove the correct route with a repeat test before promoting it to a reusable recipe.
