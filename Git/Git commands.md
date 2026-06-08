# Common Git Commands

## Verify Git Version

```bash
git -V
# or
git --version
```

---

# Repository Creation

## Initialize a Repository

```bash
git init
```

Creates a new local Git repository.

## Clone a Repository

```bash
git clone <url>
```

Copies an existing repository to your local machine.

---

# Daily Workflow

## Check Repository Status

```bash
git status
```

Shows modified, staged, and untracked files.

## Add All Changes

```bash
git add .
```

Stages all modified files.

## Add Specific Files

```bash
git add <file.py> <file2.py>
```

Stages only selected files.

## Create a Commit

```bash
git commit -m "saving all changes what I've done so far"
```

Saves staged changes to the local repository.

## View Commit History

```bash
git log
```

Displays repository history.

---

# Synchronization with Remote Repositories

## Pull Changes

```bash
git pull origin main
```

Downloads and merges changes from the remote repository.

> Good practice: pull before pushing.

## Fetch Changes Without Merge

```bash
git fetch origin
```

Downloads remote changes without modifying your branch.

## Push Changes

```bash
git push origin main
```

Uploads local commits to the remote repository.

---

# Branch Management

## Show Local Branches

```bash
git branch
```

## Show Remote Branches

```bash
git branch -r
```

Example:

```bash
origin/HEAD -> origin/main
origin/main
```

## Create a New Branch

```bash
git checkout -b <branch_name>
```

Creates and switches to the new branch.

## Switch Branches

```bash
git checkout <branch_name>
```

## Delete a Branch

```bash
git branch -d <branch_name>
```

Force delete:

```bash
git branch -D <branch_name>
```

---

# Remote Management

## Show Configured Remotes

```bash
git remote -v
```

## Add a Remote

```bash
git remote add origin <url>
```

## Change Remote URL

```bash
git remote set-url origin <new_url>
```

---

# Stash (Temporary Work)

Useful when you need to switch branches quickly without committing.

## Save Changes

```bash
git stash
```

## Save Changes with a Message

```bash
git stash push -m "message"
```

## List Stashes

```bash
git stash list
```

## Restore Latest Stash

```bash
git stash pop
```

## Apply Without Removing

```bash
git stash apply
```

---

# Conflict Resolution

When conflicts occur during merge or rebase:

## Check Status

```bash
git status
```

Resolve conflicts manually, then:

```bash
git add .
git rebase --continue
```

## Cancel Rebase

```bash
git rebase --abort
```

---

# Safe Rollback

## Revert a Commit

```bash
git revert <commit_hash>
```

Creates a new commit that undoes a previous commit without rewriting history.

---

# Recovery Commands

## Show Full History Including Lost References

```bash
git reflog
```

## Move to a Previous State

```bash
git checkout <hash>
```

or

```bash
git reset --hard <hash>
```

Use `reset --hard` carefully because it discards local changes.

---

# Repository Cleanup

## Preview What Would Be Removed

```bash
git clean -n
```

## Remove Untracked Files

```bash
git clean -f
```

## Remove Untracked Files and Directories

```bash
git clean -fd
```

---

# Cherry-Pick

Bring a specific commit from another branch.

```bash
git cherry-pick <commit_hash>
```

---

# Tags (Releases)

## Create a Tag

```bash
git tag v1.0
```

## Create an Annotated Tag

```bash
git tag -a v1.0 -m "release 1.0"
```

## Push Tags

```bash
git push origin --tags
```

---

# Interactive Rebase

Clean up commit history before creating a Pull Request.

```bash
git rebase -i HEAD~5
```

Common actions:

- Reword commit messages
    
- Squash commits
    
- Remove commits
    

---

# Worktrees

Work with multiple branches simultaneously.

```bash
git worktree add ../another-folder branch_name
```

---

# Commit Signing

Sign commits using GPG.

```bash
git commit -S -m "message"
```

---

# Professional Workflow Example

```bash
git checkout -b feature/new-feature

git add .

git commit -m "feat: new functionality"

git pull --rebase origin main

git push origin feature/new-feature
```

Typical flow:

Feature Branch → Push → Pull Request → Review → Merge