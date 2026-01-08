# Commit, Branch, and PR Rules
- Keep commits and PRs scoped to the approved plan and architecture; exclude unrelated changes.
- Branch strategy: `main` is protected; feature branches (`feature/*`) for work; use `hotfix/*` or `release/*` if applicable.
- Conventional Commits required; allowed types: `feat`, `fix`, `chore`, `refactor`, `test`, `docs`, `ci`, `build`, `revert`. Prefer scope = top-level dir or package (e.g., `feat(policy): ...`).
- Ensure commits are small, logically grouped, and reference the work item or issue when provided.
- PRs must include: scope summary, lint/format/test evidence (commands + results), risk/rollback notes, and related issues.
- Do not merge or request merge with failing required checks or unresolved blocking review items.
- Obtain human approval before merging or deploying any change.
