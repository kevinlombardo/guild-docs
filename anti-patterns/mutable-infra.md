# Anti-Pattern: Mutable Infrastructure

## Summary
Infrastructure is changed manually after deployment.

## Why It's Bad
Leads to configuration drift, untraceable changes, and fragile environments.

## Real Examples
- Hotfixing a server in production without updating IaC.
- Manual database schema edits outside of migration scripts.