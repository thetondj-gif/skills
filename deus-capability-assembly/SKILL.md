---
name: deus-capability-assembly
description: Resolve, rank and compose existing skills, MCPs, workflows, models, APIs and compute into a task-specific execution route without adding orchestration.
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
# Deus Capability Assembly

## Inputs
Outcome, constraints, current estate state, authority level, available capability inventory.

## Assembly algorithm
1. Search the Capability Compiler/shared registry semantically by required capability, not product name alone.
2. Rank candidates by fit, verification evidence, locality/ownership, cost, freshness, licence, dependencies and failure history.
3. Reuse a single capability when it satisfies the outcome; compose only when needed.
4. Keep routing, scheduling, memory, MCP and database authority in their existing canonical layers.
5. Use thin adapters where interfaces differ.
6. Execute the route and capture which capabilities and versions were actually used.
7. Verify outputs independently and feed successful combinations to the learning-promotion process.

## Gap rule
Only declare a capability gap after current tools, connected plugins/MCPs, installed services, workflows, registry sources, GitHub, Hugging Face and relevant specialist sources have been checked. Build new only as the final option.
