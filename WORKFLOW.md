# Development Workflow
Assumed roles: Codex handles planning/architecture; Claude Code handles implementation/testing; Codex handles review.

1. Planning by Codex using `planning` skill
2. Architecture by Codex using `architecture` skill
3. Reviewer pass (Codex) covering planning/architecture (detection-only)
4. Human selects which Fixable items to address
5. Fixable-only correction by Codex (planning/architecture), if any
6. Implementation by Claude Code using `coding` skill
7. Testing by Claude Code using `testing` skill
8. Reviewer pass (Codex) covering coding/testing (detection-only)
9. Human selects Fixable items
10. Fixable-only correction by Claude Code, if any
11. Testing by Claude Code

Reviewer passes occur once per stage (once for planning/architecture, once for coding/testing). Fixable corrections are allowed once per stage. Blocking causes workflow rollback. No additional re-review beyond the single pass per stage.
