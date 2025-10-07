<h1 align="center">🚀 Git & GitHub Commands — Ultimate Developer Cheat Sheet</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Git-Tool-orange?logo=git" />
  <img src="https://img.shields.io/badge/GitHub-Platform-black?logo=github" />
  <img src="https://img.shields.io/badge/Status-Active-success?style=flat-square" />
  <img src="https://img.shields.io/badge/Maintained-Yes-brightgreen?style=flat-square" />
</p>

<p align="center">📘 Your all-in-one Git & GitHub command reference — clean, visual, and developer-friendly.</p>

---

## 🧰 Setup & Configuration

| 🔧 Command | 📝 Description |
|------------|----------------|
| `git config --global user.name "Your Name"` | Set your username |
| `git config --global user.email "you@example.com"` | Set your email |
| `git config --list` | View all configuration settings |
| `git help` | Get help for any Git command |

---

## 📁 Repository Basics

| 📦 Command | 📝 Description |
|------------|----------------|
| `git init` | Initialize a new Git repository |
| `git clone <repo-url>` | Clone an existing repository |
| `git status` | Show working directory status |
| `git log --oneline --graph --decorate` | Visual commit history |

---

## 🌿 Branch Management

| 🌱 Command | 📝 Description |
|------------|----------------|
| `git branch` | List all branches |
| `git branch <branch>` | Create a new branch |
| `git checkout <branch>` | Switch to a branch |
| `git checkout -b <branch>` | Create & switch to a new branch |
| `git branch -d <branch>` | Delete a branch |

---

## 💾 Staging & Committing

| 💡 Command | 📝 Description |
|------------|----------------|
| `git add <file>` | Stage a file |
| `git add .` | Stage all changes |
| `git commit -m "message"` | Commit staged files |
| `git commit --amend` | Modify the last commit |
| `git diff` | Show unstaged changes |

---

## 🌍 Remote Repositories

| 🌐 Command | 📝 Description |
|------------|----------------|
| `git remote add origin <url>` | Add remote repository |
| `git remote -v` | List remotes |
| `git fetch origin` | Fetch remote updates (no merge) |
| `git pull origin <branch>` | Pull latest changes |
| `git push origin <branch>` | Push commits to remote |
| `git push -u origin <branch>` | Push new branch & track it |

---

## 🔁 Syncing Branches

| 🔄 Command | 📝 Description |
|------------|----------------|
| `git checkout main` | Switch to main |
| `git pull origin main` | Update local main |
| `git checkout <branch>` | Switch to your branch |
| `git merge origin/main` | Merge remote main into branch |
| `git rebase origin/main` | Rebase your branch on main |

---

## ⚔️ Merging & Rebasing

| ⚙️ Command | 📝 Description |
|------------|----------------|
| `git merge <branch>` | Merge a branch |
| `git rebase <branch>` | Rebase on another branch |
| `git merge --abort` | Cancel merge |
| `git rebase --abort` | Cancel rebase |
| `git rebase --continue` | Continue after fixing conflicts |

---

## 🧹 Undoing & Cleaning

| 🧽 Command | 📝 Description |
|------------|----------------|
| `git reset <file>` | Unstage file |
| `git checkout -- <file>` | Discard changes |
| `git revert <commit>` | Revert a specific commit |
| `git reset --hard <commit>` | Reset branch to specific commit ⚠️ |
| `git clean -fd` | Delete untracked files |

---

## 📦 Stashing

| 🪣 Command | 📝 Description |
|------------|----------------|
| `git stash` | Save current work temporarily |
| `git stash list` | List all stashes |
| `git stash pop` | Restore last stash |
| `git stash clear` | Delete all stashes |

---

## 🧠 Inspect & Review

| 🔍 Command | 📝 Description |
|------------|----------------|
| `git show <commit>` | Show commit details |
| `git diff <branch1>..<branch2>` | Compare two branches |
| `git blame <file>` | See who modified each line |
| `git shortlog -sn` | Show commit count per author |

---

## ⚙️ Preferences

| ⚖️ Command | 📝 Description |
|------------|----------------|
| `git config --global pull.rebase false` | Default: merge on pull |
| `git config --global pull.rebase true` | Default: rebase on pull |
| `git config --global pull.ff only` | Only allow fast-forward pulls |

---

## 🤝 GitHub CLI (Optional)

| 💬 Command | 📝 Description |
|------------|----------------|
| `gh auth login` | Log into GitHub |
| `gh repo clone <user>/<repo>` | Clone using GitHub CLI |
| `gh pr create --base main --head <branch>` | Create pull request |
| `gh pr list` | List PRs |
| `gh pr merge <number>` | Merge a PR |

---

## 🧩 Common Workflows

### ✨ Start a New Feature
```bash
git checkout main
git pull origin main
git checkout -b feature/my-feature
