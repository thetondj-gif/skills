# AGENTS.md — Shared Skills

Before estate-wide work, read the current Google Drive bootstrap `README_START_HERE` (`17WIrwqwC1z8MBzotqVO1n-sHDCFkFBL_Wk6CcHT8GkI`) and `AGENT_START_HERE_CURRENT` (`1V4TQ4c5eAD-R-ZEqHDz0cS6wJfb5urWshhmrUaPGuDk`). Never use the archived PRE-2026-08-30 startup files as authority.

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

## Mandatory agent ingestion

These skills are not registry-only metadata. Any agent or worker performing substantive Deus work must load the applicable `SKILL.md` contents into its working context before execution.

- Always load `deus-outcome-first/SKILL.md`.
- Load `deus-source-and-manuals-first/SKILL.md` for repository, infrastructure, configuration, integration, audit or repair work.
- Load `deus-capability-assembly/SKILL.md` whenever capability/tool/workflow/model selection or composition is involved.
- Load `deus-goal-resume-contract/SKILL.md` for multi-step, delegated, resumable or long-running work.
- Load `deus-learning-promotion/SKILL.md` after substantive execution when a reusable lesson, repair route, workflow or skill improvement may have been learned.

Loading means reading the actual shared skill file, not merely seeing its registry record, title or summary. Workers should receive only the relevant skill set plus the baseline to avoid unnecessary context expansion.

For complex work, prefer the smallest relevant subset rather than injecting all five into every prompt. `deus-outcome-first` is the default behavioural baseline; the others are retrieved by task need.
