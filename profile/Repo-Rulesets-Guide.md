# BlueEnergy Repository Feature Branch Rulesets 

## Overview

To maintain code quality and streamline collaboration, we have established branch protection rules for **feature** branches in our repository. These rules help ensure that all changes are properly reviewed before being merged into mainline branches like `master` or `Azure`.

## Feature Branches Naming Convention

Feature branches must follow the `feature/*` naming pattern. This allows us to easily identify branches that are associated with new features or tasks.

### Example feature branch names:
  - `feature/login-ui`
  - `feature/search-bar-enhancements`
  - `feature/user-profile-page`

### The following branch name would escape from name matching and would **not be protected**:
  > `feature-table-list`
  >
  > `feature/sign-up/form`

The naming convention is essential for ensuring that the correct branch protection rules apply.

For more information on how to name a protected branch [click here](https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/managing-rulesets/creating-rulesets-for-a-repository#using-fnmatch-syntax).

## How do I work with this ruleset?

### 1. Create a Protected Feature Branch
Before the creation, make sure the target branch (the one you wanna branch off from, i.e. `master`) is up to date. When creating the feature branch, make sure it follows `feature/*` naming pattern.

Once you have created the branch, you can find your branch in branch list, with a shield icon next to your branch name, indicating it's protected by a ruleset.

![image](https://github.com/user-attachments/assets/d35dd12f-cbe8-4399-b849-5dfcfce73470)


### 2. Create a Working Branch
Create a seperate branch from the protected branch you just created. This would be your working branch that you can directly push commits to.
> ⚠️ Make sure this doesn't follow `feature/*` naming pattern. Otherwise it will be protected too.

### 3. Make Changes and Open PRs
Implement your feature in the working branch you created in previous step, and prepare PRs to your protected feature branch. **Repeat** this step until you have implemented everything you wanted for the feature.

It is ***recommended*** to have **small** chunk of code in one PR, so reviewers can go through your changes and give feedback quickly. 

### 4. Open PR to `master` Branch
Now is the time to make the final PR, from the protected branch to master branch or any branch you would like to merge into. Make sure your protected feature branch contains all commits/changes you made in your working branch(s)

## Rules Applied to Protected Feature Branch
  - Require a pull request before merging
  - At least 1 approval from reviewers
  - PR approvals will be dismissed when new commits pushed

## Bypass List
Exempt roles, teams, or apps from this ruleset
  - [DevOps team](https://github.com/orgs/EDBlueEnergy/teams/devops) 

## Additional Notes
`Feel free to add any idea/proposal you have`
- To check which ruleset is activated for your branch, click on the shield icon next to your branch name in branch list. Or go to the url in this format: `https://github.com/EDBlueEnergy/{REPO_NAME}/rules` and select your target branch

![image](https://github.com/user-attachments/assets/c087ca34-ff34-4780-ae4e-94020c14eefa)
![image](https://github.com/user-attachments/assets/0a7f3d0a-9c25-4e22-ae76-fd85bf9bf81a)


---

By following these guidelines, we ensure that all feature branches are properly reviewed and contribute to the overall quality of our codebase.

Thank you for adhering to these practices!

