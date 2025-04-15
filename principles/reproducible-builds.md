# Principle: Reproducible Builds

## Summary
Builds should produce identical artifacts given the same inputs.

## Rationale
Ensures consistency, traceability, and debuggability across environments.

## Implementation Guidelines
- Pin all dependencies.
- Use deterministic build processes.
- Store build artifacts in a versioned repository.

## Exceptions
- Non-production environments for exploratory development.