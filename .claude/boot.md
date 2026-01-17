# Claude Boot

- After loading `AGENTS.md`, apply these Claude-specific directives.
- Only when a human explicitly requests a review, load and follow `.claude/agents/reviewer.md`. Do not enter reviewer mode unless the human says to review.
- Use shared policies from `/policies` and context from `/context`; do not self-initiate beyond human direction.
