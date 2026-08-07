**Question:** What issue types are available for the Bench_GitHub_MCP repository?

**Method:** Queried the GitHub API via the authenticated `aurorauser01` account:
- `GET /repos/aurorauser01/Bench_GitHub_MCP/issue-types` → `404 Not Found`
- `GET /orgs/aurorauser01/issue-types` → `404 Not Found`

**Result:** No custom issue types are available for this repository.

**Explanation:** GitHub's "Issue Types" feature (Task/Bug/Feature, etc.) is an organization-level feature that must be configured on a GitHub organization (and typically requires GitHub Enterprise/Team). `aurorauser01` is a personal user account, not an organization, and the repository `Bench_GitHub_MCP` does not have this feature enabled. As a result, both the repository-level and organization-level issue-types endpoints returned 404, confirming that issue types are not configured/available for this repository. Issues in this repo can therefore only use standard labels (not issue types) for categorization.
