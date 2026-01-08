---
name: coding
description: Implement the approved architecture and plan while following coding standards, guardrails, and review outcomes.
---

## Purpose
Apply code changes aligned with the plan and policies, with concise summaries and test results.

## Inputs
- Approved plan and architecture decisions
- Applicable policies (`guardrails`, `coding_standards`, `commit_pr_rules`, `testing_policy`)
- Selected review outcomes and constraints

## Steps
1. Load the approved plan, architecture, and policies.
2. Implement changes scoped to the plan; avoid scope creep.
3. Keep code clear, small, and testable; document non-obvious logic concisely.
4. Validate against inputs and expected behavior; prepare tests per policy.
5. Summarize changes, files touched, and testing performed.

## Outputs
- Code changes aligned with the plan and policies, plus summaries and test results.

## Failure modes
- Altering scope or architecture without approval
- Skipping required tests or violating policies
- Introducing nondeterministic or unsafe behavior
