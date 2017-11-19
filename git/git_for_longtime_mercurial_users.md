# https://medium.com/@tmvvr/git-for-longtime-mercurial-users-c41f37352fca
## Notes
* Git/Hg rosetta stone - https://github.com/sympy/sympy/wiki/Git-hg-rosetta-stone
* In Git a branch is just a pointer to a single commit.

# https://www.mercurial-scm.org/wiki/GitConcepts
* Each clone of the repo is a branch, this works the same in git and hg. This
  is often referred to as a *heavy branch*.
* Git has lightweight branches, these are simply references to commits, that
  move up with each new commit. This is similar to the bookmark concept in hg.
There is no equivalent to the hg named branches in git.
* Git has the concept of a *index* or *staging* area. This allows you to control working copy status information and determine which files/changes get included in the next commit.

# Useful commands
```bash
# Revert changes
git reset --hard
# strip current commit
git reset --hard HEAD~1
# Stage all untracked files for commit
git add -A
# remove file from the index (e.g. a file staged for addition)
git rm --cached test
# commit all changes to know files
git commit -a
```
