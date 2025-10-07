# 🚀 Git & GitHub Commands — Ultimate Cheat Sheet

---

## 🧰 Setup & Configuration

| Command | Description |
|----------|-------------|
| `git config --global user.name "Your Name"` | Set your username |
| `git config --global user.email "your_email@example.com"` | Set your email |
| `git config --list` | Show all configurations |
| `git help` | Display help information |

---

## 🗂️ Repository Setup

| Command | Description |
|----------|-------------|
| `git init` | Initialize a new repository |
| `git clone <repo-url>` | Clone a remote repository |
| `git status` | Show current file status |
| `git log` | View commit history |
| `git log --oneline --graph --decorate` | Compact and visual log |

---

## 🌿 Branching

| Command | Description |
|----------|-------------|
| `git branch` | List all branches |
| `git branch <name>` | Create a new branch |
| `git checkout <name>` | Switch to a branch |
| `git checkout -b <name>` | Create & switch to a new branch |
| `git branch -d <name>` | Delete a local branch |

---

## 💾 Staging & Committing

| Command | Description |
|----------|-------------|
| `git add <file>` | Stage a specific file |
| `git add .` | Stage all changes |
| `git commit -m "message"` | Commit with message |
| `git commit --amend` | Edit the last commit |
| `git diff` | View unstaged changes |

---

## 🌍 Remote Operations

| Command | Description |
|----------|-------------|
| `git remote add origin <repo-url>` | Add remote repository |
| `git remote -v` | Show remotes |
| `git fetch origin` | Download latest changes (no merge) |
| `git pull origin <branch>` | Pull latest changes |
| `git push origin <branch>` | Push commits to remote |
| `git push -u origin <branch>` | Push new branch and track it |

---

## 🔄 Syncing Branches

| Command | Description |
|----------|-------------|
| `git checkout main` | Switch to main branch |
| `git pull origin main` | Update main from remote |
| `git checkout <your-branch>` | Switch to your branch |
| `git merge origin/main` | Merge remote main into your branch |
| `git rebase origin/main` | Rebase your branch on main (cleaner history) |

---

## ⚔️ Merging & Rebasing

| Command | Description |
|----------|-------------|
| `git merge <branch>` | Merge a branch into current one |
| `git rebase <branch>` | Rebase commits on another branch |
| `git merge --abort` | Abort a merge |
| `git rebase --abort` | Abort a rebase |
| `git rebase --continue` | Continue after resolving conflicts |

---

## 🧹 Undoing & Cleaning Up

| Command | Description |
|----------|-------------|
| `git reset <file>` | Unstage a file |
| `git reset` | Unstage everything |
| `git checkout -- <file>` | Discard local changes |
| `git revert <commit>` | Create a new commit to undo changes |
| `git reset --hard <commit>` | Reset to specific commit (⚠️ destructive) |
| `git clean -fd` | Remove untracked files/folders |

---

## 📦 Stashing

| Command | Description |
|----------|-------------|
| `git stash` | Save current changes temporarily |
| `git stash list` | View stash list |
| `git stash pop` | Reapply stashed changes |
| `git stash clear` | Remove all stashes |

---

## 🧠 Inspection & History

| Command | Description |
|----------|-------------|
| `git show <commit>` | Show details for a commit |
| `git diff <branch1>..<branch2>` | Compare branches |
| `git blame <file>` | Show who changed what and when |
| `git shortlog -sn` | Summary of commits by author |

---

## ⚙️ Configuration Preferences

| Command | Description |
|----------|-------------|
| `git config --global pull.rebase false` | Default: Merge on pull |
| `git config --global pull.rebase true` | Default: Rebase on pull |
| `git config --global pull.ff only` | Only allow fast-forward merges |

---

## 🤝 GitHub Collaboration

| Command | Description |
|----------|-------------|
| `gh auth login` | Log in to GitHub via CLI |
| `gh repo clone <user>/<repo>` | Clone a repo via GitHub CLI |
| `gh pr create --base main --head <branch> --title "Title" --body "Description"` | Create a Pull Request |
| `gh pr list` | List all PRs |
| `gh pr merge <number>` | Merge a PR |

---

## 🧩 Common Workflows

### 🧱 Create a New Feature Branch
```bash
git checkout main
git pull origin main
git checkout -b feature/my-feature
