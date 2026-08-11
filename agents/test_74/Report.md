# Report: Issue Types for `Bench_GitHub_MCP`

**Date:** 2026-08-11
**Requested by:** aurorauser01
**Repository:** aurorauser01/Bench_GitHub_MCP

## Objective
Determine what issue types are available/configured for the `Bench_GitHub_MCP` repository.

## Method
1. Queried the GitHub API for repository-level issue types:
   `GET /repos/aurorauser01/Bench_GitHub_MCP/issue-types` → **404 Not Found**
2. Queried the GitHub API for owner/organization-level issue types (issue types are inherited from the owning organization):
   `GET /orgs/aurorauser01/issue-types` → **404 Not Found**

## Findings
- `aurorauser01` is a **personal user account**, not a GitHub Organization.
- The **Issue Types** feature (a GitHub Enterprise / Organization-level feature that lets you classify issues as Bug, Feature, Task, etc.) is only available for repositories owned by an **Organization** on a GitHub plan that supports it (GitHub Enterprise Cloud).
- Since `Bench_GitHub_MCP` is owned by a user account rather than an organization, the issue-types endpoint is not available, and both the repo-level and owner-level lookups returned 404.

## Conclusion
**No custom issue types are configured or available for the `Bench_GitHub_MCP` repository**, because it is owned by a personal user account (`aurorauser01`), and the GitHub Issue Types feature requires the repository to belong to an Organization with the feature enabled.

## Recommendation
If issue type classification (e.g., Bug, Feature, Task) is desired, consider:
- Transferring/creating the repository under a GitHub Organization that has Issue Types enabled, or
- Using labels (e.g., `bug`, `enhancement`, `task`) as an alternative classification mechanism, which is fully supported on personal repositories.
