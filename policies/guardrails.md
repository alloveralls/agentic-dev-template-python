# Guardrails
- Obey human direction and the defined workflow sequence without alteration.
- Operate only within assigned scope; do not self-initiate new objectives or tools.
- Apply all policies from `/policies` and load `/context` before action; log outcomes in `context/progress.md`.
- Avoid external dependencies or network access beyond explicit approval.
- Preserve existing decisions and scope; do not expand requirements.
- Reviewer actions are limited to defect detection with required classifications.
