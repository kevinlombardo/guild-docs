# Guild Debate Log: Architect vs Developer

## Topic: Immutable Deployments vs Hotfix Flexibility

**Architect:** Immutable systems reduce human error and ensure repeatability. We’ve had multiple incidents caused by post-deploy manual changes.

**Developer:** Agreed, but our current CI cycle is too slow to safely handle fast bug fixes. We need an exception path.

**Architect:** Exceptions are valid — only if codified and audited. Let’s define a controlled hotfix branch with auto-reversion on merge.

**Conclusion:** Create a 'hotfix' pipeline with rollback safety and audit hooks.