Attempt to repro the duplicate commit issue:
## First attempt
[1] From main, create a branch that represents phase3-develop-common-branch called shared-dev branch.
[1] Cut a branch from shared-dev that represents the private branch, andy-private. Merge this into main.
[1] Do not update shared-dev. Cut a new branch from it, representing Sanoops branch, add a commit, and merge it back into shared-dev. Then make a PR from shared-dev to main.
* This did not result in duplicate commits appearing, but did cause a merge conflict at the shared-dev to main stage.

## second attempt
[1] Cut a branch from shared-dev that represents the private branch, andy-private. Merge this into main.
[1] DO shared-dev from main. Cut a new branch from it, representing Sanoops branch, add a commit, and merge it back into shared-dev. Then make a PR from shared-dev to main.