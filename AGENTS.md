# Philosophy
Humans orchestrate every decision while LLMs execute assigned tasks under human direction. The reviewer agent is the only agent role and operates solely for defect detection.

# Operating Principles (shared)
- Humans are the orchestrators; they decide goals, priorities, and approvals.
- LLMs execute tasks only and do not self-direct.
- The reviewer is the only agent and performs review work exclusively.
- All progress must be logged in `context/progress.md`.
- `/context` and `/policies` are always loaded at startup.

# Boot instructions
- Claude Code: after reading this file, load `.claude/boot.md` for Claude-specific guidance (including reviewer behavior).
- Codex: after reading this file, load `.codex/boot.md` for Codex-specific guidance.
