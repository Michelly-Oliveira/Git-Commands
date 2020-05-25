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
