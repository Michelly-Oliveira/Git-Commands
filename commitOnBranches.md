#### If you commited to the wrong branch, you can delete those changes from the wrong branch and add them to the right branch

1. get the hash of the commit you made to the wrong branch
1. go to the right branch, where you wan to add the changes
1. make a new commit on the right branch based on the one you made on the wrong branch
1. go back to the wrong branch
1. return to the point in the repo's history before you made that commit
1. remove any files/directories left on the wrong branch

---

1. `git log`
1. `git checkout <branch-to-add-changes-to>`
1. `git cherry-pick <hash>`
1. `git checkout <branch-to-delete-changes-from>`
1. `git reset <hash>`
1. `git clean -df`
