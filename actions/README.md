
# Deployment Guild Actions

This folder contains the GPT Actions specification (`actions.yaml`) for interacting with the `guild-docs` repository on GitHub.

## Authentication

All Actions require a GitHub Personal Access Token (PAT) with `repo` scope.

In your Custom GPT configuration, provide this token as a secret variable.

Example:

- Secret Name: `GITHUB_PAT`
- Value: `<your-token>`

## Actions Overview

| Action | Purpose | API Call |
|--------|---------|----------|
| getDocument | Retrieve a file from the repo | GET /repos/{owner}/{repo}/contents/{path} |
| createBranch | Create a new branch | POST /repos/{owner}/{repo}/git/refs |
| updateDocument | Commit a file change to a branch | PUT /repos/{owner}/{repo}/contents/{path} |
| createPullRequest | Create a pull request for changes | POST /repos/{owner}/{repo}/pulls |

## Branch Naming Convention

```
{persona}-{short-desc}-{yyyyMMdd}
```

Example:

```
architect-immutable-update-20250413
developer-ci-pipeline-20250414
