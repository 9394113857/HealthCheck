# Git Workflow Commands Documentation

## Project: HealthCheck

This document contains all commonly used Git commands for managing branches, merging code, pushing changes, deleting branches, and maintaining the repository.

---

# 1. Check Git Commit History

## Command: View Complete Git History Graph

```bash
git log --oneline --graph --all --decorate
```

### Purpose:
- Shows all commits from all branches.
- Displays branch relationships.
- Helps understand merge history.

---

# 2. Check Available Branches

## Command: List Branches

```bash
git branch
```

### Purpose:
- Shows all local branches.
- Displays the current active branch with `*`.

---

# 3. Check Main Branch History

## Command:

```bash
git log --oneline main
```

### Purpose:
- Displays commit history of the main branch.
- Helps verify latest commits.

---

# 4. Check Feature Branch History

## Command:

```bash
git log --oneline raghu
```

### Purpose:
- Displays commit history of raghu branch.
- Used before merging branches.

---

# 5. Merge Feature Branch Into Main Branch

## Command:

```bash
git merge raghu --allow-unrelated-histories
```

### Purpose:
- Merges raghu branch into main.
- `--allow-unrelated-histories` allows merging branches with different root commits.

---

# 6. Save Merge Commit in Vim Editor

When Git opens Vim after merge:

## Commands:

```text
Press ESC

:wq

Press Enter
```

### Purpose:
- Saves the merge commit message.
- Exits Vim editor.

---

# 7. Add Changed Files

## Command:

```bash
git add .
```

### Purpose:
- Adds all modified files to staging area.
- Prepares files for commit.

---

# 8. Check Repository Status

## Command:

```bash
git status
```

### Purpose:
- Shows modified files.
- Shows staged files.
- Shows branch synchronization status.

Example:

```
nothing to commit, working tree clean
```

---

# 9. Verify Merge Commit

## Command:

```bash
git log --oneline --decorate --graph main -10
```

### Purpose:
- Shows latest 10 commits of main branch.
- Confirms merge was successful.

Example:

```
Merge branch 'raghu'
```

---

# 10. Push Changes To GitHub

## Command:

```bash
git push origin main
```

### Purpose:
- Uploads local main branch changes to GitHub.
- Updates remote repository.

---

# 11. Check Git Credential Helper

## Command:

```bash
git config --global credential.helper
```

### Purpose:
- Shows configured Git credential manager.
- Helps troubleshoot authentication issues.

---

# 12. Remove Incorrect Credential Helper

## Command:

```bash
git config --global --unset credential.helper
```

### Purpose:
- Removes invalid credential helper configuration.

---

# 13. Check Current Repository Status

## Command:

```bash
git status
```

### Purpose:
- Confirms current branch.
- Checks clean working tree.

---

# 14. View Complete Branch Graph

## Command:

```bash
git log --oneline --graph --decorate --all
```

### Purpose:
- Displays complete branch structure.
- Shows commits and branch pointers.

---

# 15. Switch To Main Branch

## Command:

```bash
git checkout main
```

### Purpose:
- Moves from current branch to main branch.

---

# 16. Delete Local Branch

## Command:

```bash
git branch -d raghu
```

### Purpose:
- Deletes local raghu branch after merge.
- Keeps repository clean.

---

# 17. Delete Remote Branch

## Command:

```bash
git push origin --delete raghu
```

### Purpose:
- Deletes raghu branch from GitHub remote repository.

---

# 18. Download Latest Remote Information

## Command:

```bash
git fetch origin
```

### Purpose:
- Downloads latest remote branch information.
- Does not modify local files.

---

# 19. Pull Latest Changes

## Command:

```bash
git pull
```

### Purpose:
- Downloads and merges latest changes from remote repository.

---

# 20. Create New Feature Branch

## Command:

```bash
git checkout -b feature/new-feature
```

### Purpose:
- Creates a new branch.
- Automatically switches to that branch.

Example:

```
main
 |
 |
feature/new-feature
```

---

# 21. Push New Feature Branch

## Command:

```bash
git push -u origin feature/new-feature
```

### Purpose:
- Uploads new branch to GitHub.
- Sets upstream tracking.

---

# 22. Complete Git Development Workflow

```
Clone Repository
        |
        |
Create Feature Branch
        |
        |
Develop Code
        |
        |
git add .
        |
        |
git commit
        |
        |
git push feature branch
        |
        |
Create Pull Request
        |
        |
Merge Into Main
        |
        |
git push origin main
        |
        |
Delete Old Branch
```

---

# 23. Daily Git Commands

## Check Status

```bash
git status
```

Purpose:
- Check repository condition.

---

## Add Changes

```bash
git add .
```

Purpose:
- Stage all changes.

---

## Commit Changes

```bash
git commit -m "commit message"
```

Purpose:
- Save changes with description.

---

## Push Changes

```bash
git push origin main
```

Purpose:
- Upload commits to GitHub.

---

## Pull Changes

```bash
git pull
```

Purpose:
- Download latest changes.

---

# 24. Recommended Git Branch Strategy

```
main
 |
 |
feature/login
 |
 |
feature/api-update
 |
 |
feature/new-model
```

Workflow:

1. Create feature branch.
2. Develop changes.
3. Commit changes.
4. Push branch.
5. Merge into main.
6. Delete old branch.

---

# 25. Repository Maintenance Commands

## See Remote Repository

```bash
git remote -v
```

Purpose:
- Shows connected GitHub repository.

---

## Show Current Branch

```bash
git branch --show-current
```

Purpose:
- Displays active branch name.

---

## See All Branches Including Remote

```bash
git branch -a
```

Purpose:
- Shows local and remote branches.

---

## Remove Deleted Remote Branch References

```bash
git fetch --prune
```

Purpose:
- Cleans deleted remote branch references.

---

# End Of Git Documentation

Project: HealthCheck

Maintained under:

docs/GIT_WORKFLOW_COMMANDS.md