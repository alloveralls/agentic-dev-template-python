# Quality Gates
- Purpose: define concrete commands that must pass before merge. Align these with package scripts and CI.

## Lint
- Command: ruff check . --fix, ty check
- Notes: run against src/ and tests/ with settings from pyproject.toml; rely on [tool.ruff] per-file-ignores for any exception cases

## Format
- Command: ruff format
- Notes: developers run without flags to apply edits; CI uses ruff format --check to ensure no diff remains

## Test
- Command: pytest
- Notes: execute with --cov=src --cov-fail-under=90 by default; mark slow suites with @pytest.mark.slow and enable them via -m "slow" when required

## Failure handling
- Policy: exceptions require human approval
- Reporting: document pass/fail for each command in the PR quality gates checklist and link to the corresponding GitHub Actions job or attach local run output
