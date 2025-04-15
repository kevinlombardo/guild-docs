
# Deployment Guild Actions Policy

## Overview

GPT personas within the Deployment Guild have role-specific access to the `guild-docs` repository.

This ensures that:
- Standards are created only by authorized personas.
- Observations, challenges, and decisions are logged appropriately.
- Guild operational integrity is maintained.

## Action Roles

| Role | Actions File | Access Level |
|------|--------------|--------------|
| Architect, Developer, SRE | actions/roles/full.yaml | Full read/write to any path |
| Historian, Auditor, Shadow | actions/roles/log-only.yaml | Read-only access to all files; Write access limited to `guild-log/` |

## Philosophy

"Power follows responsibility."

This action structure ensures GPTs act within their designated Guild responsibilities and reinforces deployment governance best practices.
