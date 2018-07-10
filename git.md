# Git Cheat Sheet

See the remote URL `git remote show origin`

Make and Checkout new branch `git checkout -b newbranch`

Push branch around: `git push  <REMOTENAME> <BRANCHNAME>`

To link local to remote branch: `git push --set-upstream <REMOTENAME> <BRANCHNAME>`

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
