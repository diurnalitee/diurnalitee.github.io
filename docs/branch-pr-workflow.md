## Branch & PR Workflow

I tend to loosely follow a simplified GitFlow-style workflow.

### Main Branches

* `main`
  * The "stable" branch. Should always contain production-ready code
  * Only ever updated via reviewed and discussed PRs
* `develop`
  * Integration branch for ongoing work
  * All feature branches merge into here first, before then being merged into `main`.

This system ensures that there is always a stable branch, even if a PR unexpectedly breaks something after a merge into `develop`.

### Feature Workflow

Typical flow for working on something:

```text
develop -> feature branch -> PR -> develop
```

1. Create a branch from `develop`
2. Work on feature/bugfix/whatever
3. Open a PR targeting `develop`
4. Get it reviewed and merged and you're done :)

Releases or major milestones can then be merged from `develop` into `main`!

### PR Review Cadence

I like to have a scheduled moment to review PRs in batches, usually once per week (e.g. every Friday). Smaller or urgent PRs can be reviewed earlier if needed.  
It's important not to let PRs sit too long. Stale PRs can get really painful to review if the code starts becoming out-of-date.

### Branch Cleanup & Squashing Commits

After a PR is merged, the feature branch should be deleted. This keeps the repo clean and avoids confusion with outdated branches.

To squash or not to squash, there are two valid approaches. I choose depending on context:

#### Squash merge (default):

* Keeps develop / main history clean and readable
* Ideal for messy or iterative commit histories
* Results in one clear commit per PR

#### Regular merge (preserve commits):

* Useful when commit history is meaningful (e.g. step-by-step system development)
* Helps when debugging or understanding how something evolved

TL;DR, In general: **Only keep the commit history if it adds value!**
