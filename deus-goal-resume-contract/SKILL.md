---
name: deus-goal-resume-contract
description: Persist task intent, state, evidence, failures and next action so interrupted or delegated work resumes from verified state instead of restarting.
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
# Deus Goal and Resume Contract

## Required state
Every substantial task should be representable as:
- goal
- success_criteria
- authority_and_approval_boundaries
- current_state
- completed_steps
- failed_steps_and_retry_history
- evidence_and_receipts
- pending_approvals
- source_files_and_refs
- model_tool_workflow_route
- unresolved_questions
- next_safe_action
- verification_status

## Resume rule
On resume, reconstruct state from canonical receipts/project state first. Do not replay the whole conversation or repeat completed work. Revalidate volatile facts, credentials, deployments and external state before continuing.

## Delegation rule
Subagents receive the same goal contract plus only the context needed for their workstream. Their output is evidence to be checked, not automatic completion.

## Completion
Close the contract only when success criteria are evidenced, or preserve the exact blocker and smallest safe next action.
