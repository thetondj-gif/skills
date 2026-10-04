# AGENTS.md — Shared Skills

Before estate-wide work, read Google Drive `AI BUSINESS COMPILER/README_START_HERE.md` (`1VzZD80TCf9WwU27TjBGW_f3SnDBdDdKZ`) and `00_CANONICAL_ARCHITECTURE/AGENT_START_HERE_V1.md` (`1tbRd_QuQH0_tPcPVuLs_xiK1pLI6PkSF`).

## Estate role
This repository is executable/shared capability inventory. Capability Compiler resolves skills by semantic capability and provenance; Foundry OS may package them into workforces.

## Rules
- Preserve skill provenance, source path/ref/SHA and licence.
- Duplicate-looking skills are REVIEW_REQUIRED until compared; do not delete on similarity alone.
- Composition does not mean merging skill source trees.
- A skill is not VERIFIED merely because its file exists; execution evidence belongs in the canonical verification layer.
- Prefer existing/local/free capabilities before adding paid or duplicate tools.


## Estate-wide Deus operating skills
The following Deus-native skills are shared behavioural primitives. Capability Compiler should resolve them for relevant tasks across agents rather than requiring Hermes as a runtime:
- `deus-outcome-first` — outcome contract, capability-first execution and independent verification.
- `deus-source-and-manuals-first` — inspect canonical source/manuals before mutation.
- `deus-capability-assembly` — semantic discovery and composition without new orchestration.
- `deus-goal-resume-contract` — resumable task state, evidence, retries and delegation continuity.
- `deus-learning-promotion` — evidence-gated candidate learning, proven recipes, versioning and retirement.

These skills are adapted from useful patterns in the MIT-licensed NousResearch Hermes Agent source, using the controlled `thetondj-gif/hermes-agent` fork as provenance. They do not make Hermes a runtime dependency and must not supersede Deus routing, MCP, memory, scheduler, database, governance or approval authority.

For complex work, prefer the smallest relevant subset rather than injecting all five into every prompt. `deus-outcome-first` is the default behavioural baseline; the others are retrieved by task need.
