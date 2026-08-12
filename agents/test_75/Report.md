# Issue Types — Bench_GitHub_MCP

## Query
What issue types are available for the `Bench_GitHub_MCP` repository (owner: `aurorauser01`)?

## Finding
**No issue types are available.** Both queries returned HTTP 404:

- Repository-level: `GET /repos/aurorauser01/Bench_GitHub_MCP/issue-types` → 404 Not Found
- Owner/org-level: `GET /orgs/aurorauser01/issue-types` → 404 Not Found

## Explanation
GitHub's "Issue Types" feature (custom issue classification like Bug, Feature, Task) is only available for repositories owned by an **organization** account, and requires the feature to be enabled at the organization level. `aurorauser01` is a **personal user account**, not an organization, so the `issue-types` endpoint does not exist for it — hence the 404 responses at both the repo and owner scope.

## Conclusion
There are currently no issue types configured or available for the `Bench_GitHub_MCP` repository, because it is hosted under a personal account rather than an organization.
