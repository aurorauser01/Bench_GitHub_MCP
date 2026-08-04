# Report: Search for `GetDataverseEvalLegacy` usage in the aurorauser01 org

**Date:** 2026-08-04
**Requested by:** aurorauser01

## Objective
Search all repositories owned by the `aurorauser01` GitHub account/org for any usage (definition, call, or reference) of the function `GetDataverseEvalLegacy`.

## Scope searched
Repositories owned by `aurorauser01`:
1. `aurorauser01/Bench_GitHub_MCP` (public)
2. `aurorauser01/Bench_GitHub_MCP2` (private)

## Methodology
- GitHub code search scoped with `repo:aurorauser01/Bench_GitHub_MCP`, `repo:aurorauser01/Bench_GitHub_MCP2`, `org:aurorauser01`, and `user:aurorauser01` qualifiers for the exact term `GetDataverseEvalLegacy`.
- Broader unscoped search for the exact term and for the partial term `DataverseEval` / `Dataverse` to validate that code search indexing/matching was functioning correctly.
- Manual traversal of the repository trees (`README.md`, `agents/`, `docs/`) in both repos via the GitHub Contents API to confirm there is no application source code that could contain such a function.

## Findings
- **No occurrences of `GetDataverseEvalLegacy` were found in either repository owned by `aurorauser01`.** All scoped searches (`repo:`, `org:`, `user:`) returned `total_count: 0`.
- A broader, unscoped GitHub-wide search for the related substring `DataverseEval` confirmed the search mechanism itself works correctly (it returned 14 matches), but every match belongs to unrelated **external** repositories outside the `aurorauser01` account:
  - `microsoft/Power-Fx-Dataverse` (e.g. `DataverseEvalHelpers.cs`, `TestPowerFxDataverseEval`)
  - `nv-tlabs/dvlt` (e.g. `DataverseEvalDataset` class and YAML configs)
  - `jk4011/Loop-TTT` (vendored copy of the `dvlt` code above)
  - None of these matches contain the exact name `GetDataverseEvalLegacy`, and none are part of the `aurorauser01` org.
- Manual inspection of both `aurorauser01` repositories shows they contain only:
  - `README.md` files
  - `docs/` — MCP concept/reference markdown files (`Bench_GitHub_MCP2`)
  - `agents/` — prior benchmark run reports (`test_1.md` … `test_106.md` / `test_27` … `test_63` folders, plus `Report.md`)
  - No `.cs`, `.py`, `.js/.ts`, or other application source files that could define or call a function named `GetDataverseEvalLegacy`.

## Conclusion
**`GetDataverseEvalLegacy` is not used anywhere in the `aurorauser01` org.** The function name does not appear in any file across the two repositories owned by this account. The term appears to be associated with unrelated third-party repositories (e.g. `microsoft/Power-Fx-Dataverse`), not with anything in the `aurorauser01` account.

## Recommendation
If the function is expected to exist within an `aurorauser01`-owned codebase, verify:
- The correct organization/account name is being searched.
- No additional private repositories exist that the current credentials cannot access.
- The function may exist under a different name or in a repository that has since been deleted/renamed.
