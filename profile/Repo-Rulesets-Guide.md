# Blue Repository Rulesets 

## Overview

To maintain code quality and streamline collaboration, we have established branch protection rules for **feature** branches in our repository. These rules help ensure that all changes are properly reviewed before being merged into mainline branches like `master` or `Azure`.

### Feature Branches Naming Convention

Feature branches must follow the `feature/*` naming pattern. This allows us to easily identify branches that are associated with new features or tasks.

Example feature branch names:
- `feature/login-ui`
- `feature/search-bar-enhancements`
- `feature/user-profile-page`

This naming convention is essential for ensuring that the correct branch protection rules apply.

### Rules Applied to Protected Feature Branch
  - Require a pull request before merging
  - At least 1 approval from reviewers
  - PR approvals will be dismissed when new commits pushed

### Why This Rule Exists

- **Code Quality**: Peer reviews help maintain a high standard of code quality.
- **Knowledge Sharing**: Reviews allow team members to stay informed about different parts of the codebase.
- **Bug Prevention**: Having a second set of eyes reduces the chance of bugs being introduced into the main branch.

### Bypass List
Exempt roles, teams, or apps from this ruleset
  - DevOps team

### Additional Notes

- If no reviewer is available, please reach out to your team or the designated code reviewer for assistance.
- If multiple team members are required to review, this can be added in the PR's reviewer section.

---

By following these guidelines, we ensure that all feature branches are properly reviewed and contribute to the overall quality of our codebase.

Thank you for adhering to these practices!

