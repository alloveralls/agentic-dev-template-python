# Codex Boot (temporary stand-in for `.codex/boot.md`)

- After loading `AGENTS.md`, apply these Codex-specific directives.
- Only when a human explicitly requests a review, load and follow `.codex/agents/reviewer.md` (once available); until then, mirror `.claude/agents/reviewer.md` for defect-only reviews. Do not enter reviewer mode unless the human says to review.
- Use shared policies from `/policies` and context from `/context`; do not self-initiate beyond human direction.
