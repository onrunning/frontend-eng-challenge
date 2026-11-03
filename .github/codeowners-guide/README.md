# Set up code ownership

Every managed On repository needs an owning team to review changes. Repositories without CODEOWNERS will be archived.

If this repository is no longer maintained, please let us know so we can archive it.

The [CODEOWNERS template](../CODEOWNERS) is blank: all rules are commented out, so it assigns no owners. Complete it before merging.

1. Replace `REPOSITORY_TEAM` with your team's GitHub slug and uncomment the `*` fallback and `/.github/` rules. The team must be visible and have explicit write access to this repository.
2. Add component or shared-tooling overrides if needed. Replace the example paths and team slugs, then remove unused examples. Keep the review-governance rules last.
3. Check the file for errors in GitHub and merge it into the default branch. Enable **Require review from Code Owners** in branch protection or an applicable ruleset to make owner approval mandatory.

Use `.github/CODEOWNERS`, without a `.md` extension. Paths are case-sensitive, and the last matching rule replaces earlier owners. When a rule lists multiple owners, approval from any one is sufficient.

Update ownership when teams or responsibilities change. See [GitHub's CODEOWNERS documentation](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-code-owners) for syntax and review behavior.
