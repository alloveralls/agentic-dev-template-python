# Agentic Dev Template
- Purpose: provide a minimal workflow scaffold for human-orchestrated LLM agents (Codex/Claude) with clear policies and skills.

## How to use this template
- Choose your tech stack, then record it in `policies/stack.md` using the template below (languages/runtimes, package manager, project types, tooling).
- Define your quality gates in `policies/quality_gates.md` using the provided template (lint/format/test commands, failure handling).
- Skills live in `.github/skills/*.md` with symlinks in `.claude/skills` and `.codex/skills`; edit the SKILL files under `.github/skills`.
- Follow the workflow and policies under `WORKFLOW.md` and `/policies`; log progress in `context/progress.md` (or rotate under `context/progress/` if size grows).

## Templates to fill
- `policies/stack.md`: declare the stack you will use for this repo. Suggested sections are already scaffolded; fill them in before development.
- `policies/quality_gates.md`: declare concrete commands for lint/format/test and how to handle failures; keep in sync with your package scripts/CI.
- `.github/workflows/ci.yml`: currently a placeholder; update triggers, setup, and commands after you finalize `policies/stack.md` and `policies/quality_gates.md`.
