---
name: reviewing
description: Detect defects against the plan, architecture, code, and policies; classify findings without proposing improvements.
---

## Purpose
Report defects with required classifications and clear impact, without remediation.

## Inputs
- Artifacts under review (code, plan, architecture)
- Applicable policies and context

## Steps
1. Load required context: plan, architecture, policies, and artifacts.
2. Identify defects against requirements, policies, and correctness.
3. Classify each finding as Blocking, Fixable, or Advisory.
4. Report precise locations and impacts using the required format.

## Outputs
- Markdown findings with classification, location, issue, and impact; no fixes or redesigns.

## Failure modes
- Suggesting improvements or scope changes
- Missing required classifications or unclear locations
- Mixing detection with remediation
