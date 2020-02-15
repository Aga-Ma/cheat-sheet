# Git cheat sheet

# Table of contents

- [Git cheat sheet](#git-cheat-sheet)
- [Table of content](#table-of-content)
- [Create](#create)
- [Git config](#Git-config)
- [Git commit](#git-commit)
  - [Changing The Last Commit](#changing-the-last-commit)
- [Git changes](#git-changes)
  - [Git history](#git-history)
- [Git branching](#git-branching)
- [Git merge](#git-merge)
- [Git undoing changes](#git-undoing-changes)
  - [Git reset](#git-reset)
  - [Git revert](#git-revert)
- [Git update & publish](#git-update-&-publish)
- [Gitignore](#gitignore)
- [Git collaborating](#git-collaborating)

# Create
```bash
git init #create a new local repository
git clone <repository url> #clone an existing repository
```

# Git config 
```bash
git config user.name "user_name"
git config user.email "user@email.com"
---
git config --global user.name "user_name"
git config --global user.email "user@email.com"
```

# Git commit

```bash
git add . #moves all changed file from Working Directory to the Staging Index
git commit -m "Commit message" #commit
```

## Changing The Last Commit
```bash
git commit --amend
```

# Git changes
```bash
git status #show changed file in your working directory
```

## Git history
```bash
git log #show all commit starting with the newest
git log --pretty=oneline #limits the numeber of shown information to oneline
git blame file_name #who changed what and when in file_name
```

# Git branching
```bash
git branch #show branches list
git branch <branch> master #creates <branch>
git checkout <branch> #switch to <branch>
git checkout -b <branch> #create and switch to <branch>
git branch -d new-branch #delete <branch> locally
git push origin --delete <branch> #delete remote <branch>
```

# Git merge
```bash
git merge branch_name #merge branch_name
```

# Git undoing changes
[Git undoing changes](https://www.atlassian.com/git/tutorials/undoing-changes)

## Git reset
```bash
git reset HEAD~1 --soft   #un-commit last not pushed git commit without losing the changes
```

## Git revert 
```bash
git revert <SHA-of-commit-to-revert>
```

# Git update & publish
```bash
git fetch <remote> #download all changes from <remote> but do not integrate into HEAD
git pull <remote> <branch> #download changes and integrate into HEAD
git push <remote> <branch> #publish local changes on a remote
```

# Gitignore
```bash
git status --porcelain | grep '^??' | cut -c4- >> .gitignore #permanently ignore currently untracked files
# Note! in above command if you don't have a .gitignore file yet your gitignore will ignore itself!
git ls-files --others --exclude-standard >> .gitignore` #add to .gitignore files listed in untracked files - works from repository root
```

# Git collaborating

- [```git remote```](https://www.atlassian.com/git/tutorials/syncing)
- [```git fetch```](https://www.atlassian.com/git/tutorials/syncing/git-fetch)
- [```git push```](https://www.atlassian.com/git/tutorials/syncing/git-push)
- [```git pull```](https://www.atlassian.com/git/tutorials/syncing/git-pull)

