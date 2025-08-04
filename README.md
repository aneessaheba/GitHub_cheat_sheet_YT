# Git & GitHub Command Cheat Sheet
[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/Vwg2m6h4ySo/0.jpg)](https://youtu.be/Vwg2m6h4ySo)

This repository contains a handy cheat sheet of essential Git and GitHub commands with practical examples.

## Getting Started

### 1. Create a Repository on GitHub
Go to [GitHub](https://github.com), click on **New Repository**, give it a name (e.g., `my-first-repo`), and create it.

### 2. Clone the Repository
```bash
git clone https://github.com/your-username/my-first-repo.git
cd my-first-repo
````

## Working with Files

### 3. Check Repository Status

```bash
git status
```

### 4. Add Files and Commit

```bash
echo "Hello GitHub" > README.md
git add README.md
git commit -m "Initial commit with README"
```

### 5. Push Changes to GitHub

```bash
git push origin main
```

## Branching and Merging

### 6. Create and Work on a Branch

```bash
git checkout -b feature-1
echo "Feature 1" > feature.txt
git add feature.txt
git commit -m "Add feature 1 file"
git push --set-upstream origin feature-1
```

### 7. Merge Branch into Main

```bash
git checkout main
git pull origin main
git merge feature-1
git push origin main
```

## Branch Management

### 8. View All Branches

```bash
git branch        # Local branches
git branch -r     # Remote branches
```

## Undoing Changes

### 9. Revert or Reset to Previous Version

```bash
git log                      # Get the commit hash
git revert <commit-hash>     # Safe revert (creates a new commit)
git reset --hard <commit-hash> # Dangerous reset (erases history)
```

## Syncing with GitHub

### 10. Pull Latest Changes

```bash
git pull origin main
```

## Summary of Common Commands

| Action                 | Command                          |
| ---------------------- | -------------------------------- |
| Clone repo             | `git clone <url>`                |
| Check status           | `git status`                     |
| Add files              | `git add .`                      |
| Commit changes         | `git commit -m "message"`        |
| Push to GitHub         | `git push origin main`           |
| Pull from GitHub       | `git pull origin main`           |
| Create branch          | `git branch new-branch`          |
| Switch branch          | `git checkout branch-name`       |
| Create + switch branch | `git checkout -b new-branch`     |
| Merge branches         | `git merge branch-name`          |
| View log               | `git log`                        |
| Revert commit          | `git revert <commit-hash>`       |
| Reset to commit        | `git reset --hard <commit-hash>` |

## Tips

* Always pull before you push to avoid conflicts.
* Use branches for different features or experiments.
* Use `git log` often to track commit history.


