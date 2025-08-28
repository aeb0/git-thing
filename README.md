Attempt to repro the duplicate commit issue:
## First attempt
[1] From main, create a branch that represents phase3-develop-common-branch called shared-dev branch.
[1] Cut a branch from shared-dev that represents the private branch, andy-private. Merge this into main.
[1] Do not update shared-dev. Cut a new branch from it, representing Sanoops branch, add a commit, and merge it back into shared-dev. Then make a PR from shared-dev to main.