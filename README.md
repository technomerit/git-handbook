# Git Handbook by TECHNO MERIT
Comprehensive Git Command Reference for Everyday Development

---

## 🔥 Most Commonly Used Git Commands

### 1. git clone
Clone a public repository to your local machine.
```bash
git clone https://github.com/username/repo-name.git local-folder-name
```

### 2. git init
Initialize a new Git repository in your current directory.
```bash
git init
```

### 3. git status
Check the current status of your working directory — which files are modified, staged, or untracked.
```bash
git status
```

### 4. git add
Stage (save) all the changes in your repository.
```bash
git add --all
```

Stage a specific file:
```bash
git add filename
```

### 5. git diff
Show differences between working directory and last commit.
```bash
git diff
```

Compare two commits:
```bash
git diff commit1 commit2
```

### 6. git commit
Commit your staged changes with a message.
```bash
git commit -m "your message"
```

Amend last commit message (if not pushed yet):
```bash
git commit --amend -m "new message"
```
# 💬 Commit Message Conventions

Clear and **consistent commit messages** make your Git history easier to read, track, and collaborate on. Here are common types of commit messages:

---

## Commit Message Types

1.  **Basic Commit**
    ```
    Update README with new instructions
    ```
2.  **Feature / New Functionality**
    ```
    feat: add user login API
    ```
3.  **Bug Fix**
    ```
    fix: resolve login crash when password is empty
    ```
4.  **Refactoring**
    ```
    refactor: optimize database query performance
    ```
5.  **Documentation**
    ```
    docs: update README with GitHub workflow
    ```
6.  **Style / Formatting**
    ```
    style: fix indentation and remove extra spaces
    ```
7.  **Testing**
    ```
    test: add unit tests for login API
    ```
8.  **Chore / Maintenance**
    ```
    chore: update npm packages to latest version
    ```

---

## Example of Good Commit Messages

* `feat: add search functionality to product page`
* `fix: correct null pointer error in user profile`
* `docs: update contributing guide with branch naming rules`
* `style: remove unused imports and fix indentation`

### 7. git push
Push your committed changes to a remote repository.
```bash
git push origin master
```

Set upstream (first-time setup):
```bash
git push -u origin master
```

After setting upstream once:
```bash
git push
```

Force push (override remote conflicts):
```bash
git push -f origin master
```

### 8. git pull
Fetch and merge changes from a remote repository.
```bash
git pull
```

---

## ⚙️ Configuration Commands

### 9. git config
Set your username and email globally (used for all commits).
```bash
git config --global user.email "youremail@example.com"
git config --global user.name "yourusername"
```

List all configuration settings:
```bash
git config --list
```

---

## 🌿 Branch & Navigation Commands

### 10. git branch
List, create, or delete branches.
```bash
git branch          # List all branches
git branch new-name # Create a new branch
git branch -d name  # Delete a branch
```

### 11. git checkout
Switch between branches or commits.

Move to an existing branch:
```bash
git checkout branch-name
```

Create and switch to a new branch:
```bash
git checkout -b new-branch
```

Switch to a specific commit:
```bash
git checkout commit-id
```

Return to master/main branch:
```bash
git checkout master
```

### 12. git merge
Merge another branch into the current one.
```bash
git merge branch-name
```

### 13. git rebase
Reapply commits on top of another branch (used for cleaner commit history).
```bash
git rebase branch-name
```

---

## 🌐 Remote Repository Commands

### 14. git remote add origin
Add a remote repository to your local project.
```bash
git remote add origin https://github.com/username/repo-name.git
```

### 15. git remote remove origin
Remove an existing remote origin.
```bash
git remote remove origin
```

### 16. git fetch
Download changes from remote without merging.
```bash
git fetch
```

---

## 📜 History & Inspection Commands

### 17. git log
View recent commits with commit IDs, authors, timestamps, and messages.
```bash
git log
```

Compact one-line view:
```bash
git log --oneline
```

View specific file history:
```bash
git log filename
```

---

## 🧹 Undo & Recovery Commands

### 18. git restore
Restore modified files to their last committed state.
```bash
git restore
```

Restore a specific file:
```bash
git restore filename
```

### 19. git reset
Undo uncommitted changes completely (warning: destructive).
```bash
git reset --hard
```

Then, restore the latest version from remote:
```bash
git pull
```

### 20. git clean
Delete all untracked files and directories.
```bash
git clean -fd
```

### 21. git stash
Temporarily store uncommitted changes (useful when switching branches).
```bash
git stash
```

Apply stashed changes later:
```bash
git stash pop
```

List all stashed changes:
```bash
git stash list
```

### 22. git revert
Undo a specific commit safely without rewriting history.
```bash
git revert commit-id
```

---

## 📦 File Management Commands

### 23. git rm
Remove tracked files from repo and working directory.
```bash
git rm filename
```

### 24. git mv
Rename or move files within a repository.
```bash
git mv oldname newname
```

---

## 🏷️ Tagging Commands

### 25. git tag
Mark specific commits (useful for versioning).
```bash
git tag v1.0
git tag -a v1.0 -m "Initial release"
```

Push tags to remote:
```bash
git push origin --tags
```

---

## ✅ Summary of Common Workflow

```bash
# 1. Clone or initialize
git clone <repo-url>
# or
git init

# 2. Make changes, then stage and commit
git status
git add --all
git commit -m "update message"

# 3. Push to remote
git push
# or set upstream for the first time
git push -u origin master

# 4. Pull new updates
git pull
```

---

---

© TECHNO MERIT — Owned and operated by [High Codex Digital](https://highcodex.com)

## 📄 License

This Git Handbook is licensed under the MIT License.  
See the [LICENSE](./LICENSE) file in this repository for full license text.
