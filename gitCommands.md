```bash
git init
```

- create a repository inside your current folder

---

```bash
git status
```

- view current state of your project

---

```bash
git log
```

- see details of the commits that were made

---

```bash
git reflog
```

- show the project history

---

```bash
git remote -v
```

- show information about the repository(the remote that was cloned)

---

```bash
git branch <new-branch>
```

- create a new branch

---

```bash
git checkout <branch-name>
```

- go to that branch

---

```bash
git branch -a
```

- list all branches in the repo

---

```bash
git add <file-name>
git add *
```

- add this file to the staging area

---

```bash
git reset <file-name>
```

- remove file from staging area

---

```bash
git diff
```

- show changes made to the code

---

```bash
git commit -m "message"
```

- commit your staged changes with a message

---

```bash
git pull origin master
```

- pull changes from the repo
- origin: name of the remote repo
- master: branch to add file to

---

```bash
git fetch
```

- fetch the latest info about the repo
- doesn't change your local files, just updates the tracking data on the .git folder

---

```bash
git push origin master
```

- push your changes to the master branch
- origin: remote name
- master: branch to add your changes to, can be any other branch

---

```bash
git merge <branch-name>
```

- merge changes from another branch to current branch
- merge: add all files/changes from one branch to another

---

```bash
git branch --merged
```

- show all branches that have been merged

---

```bash
git checkout <file-name>
```

- remove changes from file before staging

---

```bash
git commit --ammend
```

- add a file to previous commit after you already made the commit to the repo
- commit hash changes, change git history if you pushed to remote

---

```bash
git commit --amend -m "message"
```

- change previous commit message
- hash changes, change git history if you pushed to remote

---

```bash
git log --stat
```

- show previous commits and their changes

---

```bash
git cherry-pick <commit-hash>
```

- make a new commit based on another commit
  -it doesn't delete the commit that is used as base

---

```bash
git reset <flag> <hash>
```

- return to the point in the repo when you made the commit, all commits made after the one specified with the hash are removed

_flags_

- --soft: delete commits after the one used on the hash, but keep the changes on the staging area

- default(noflag): delete commits after the one used as the hash, keep the changes on the working directory but not on the staging area

- --hard: delete commits after the one used as the hash, all tracked files go back to the state they were in on the hash commit(lose changes), untracked files stay on the working directory - not changed

---

```bash
git clean -df
```

- remove untracked directories and files from working directory

---

```bash
git revert <hash>
```

- creates a new commit that completely reverts(undo) the specified commit
- 'unmake' commits without changing the git history
