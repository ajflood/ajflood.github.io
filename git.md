# Git Cheat Sheet

See all branches and links `git remote show origin`

Track all remote branches `git fetch --all`

Checkout branch (even remotes) `git checkout <branchname>`

See the remote URL `git remote show origin`

Make and Checkout new branch `git checkout -b newbranch`

Push branch around: `git push <REMOTENAME> <BRANCHNAME>`

To link local to remote branch: `git push --set-upstream <REMOTENAME> <BRANCHNAME>`

Reset branch to last commit `git reset --hard HEAD`

Rebase: `git rebase <some_branch>` -> Appends new changes of current branch onto the end of <some_branch>

Working with submodules: 
* Add new submodule: `git submodule add some_repo@some_location` then to keep track of the upstream changes `git submodule init repo_name`
* Update submodule: `git submodule update`
* Remove submodule: `git submodule rm repo_name` Then remove modify .gitmodules to remove repo_name, remove the repo_name from .git/config, delete cached data with `git rm --cached repo_path`

Merging branches together: 
* git checkout branchMergingInto
* git merge branchMergingFrom

Tagging branch as archived, deleting locally, then deleting remotely:
```
 git tag archive/<branchname> <branchname>
 git branch -D <branchname>
 git branch -d -r origin/<branchname>
 git push --tags
 git push origin :<branchname>
```
