
# 🚀 Git & GitHub Tutorial: Day 1 to Day 20

Welcome to my **20-Day Git and GitHub Learning Journey!** 🎯

This tutorial is designed for beginners who want to learn Git and GitHub from scratch. Each day includes simple explanations, commands, examples, and practice tasks.

## 📚 Learning Goals

- Understand Git and GitHub.
- Install and configure Git.
- Create and manage repositories.
- Track changes and create commits.
- Learn branching and merging.
- Upload projects to GitHub.
- Clone, pull, and push repositories.
- Learn basic collaboration and troubleshooting.

---

## 📅 Day 1: Introduction to Git and GitHub

**Git:** A version control system that tracks changes in files.

> DURGA BHAVANI

**GitHub:** An online platform for hosting Git repositories and collaborating with developers.

**Key Difference:**
- Git manages version history.
- GitHub hosts repositories online.

**Practice:** Create a GitHub account and explore the Git website.

---

## 📅 Day 2: Installing Git

Download Git from: https://git-scm.com/downloads

Check the installation:

```bash
git --version
```

**Practice:** Install Git and check your version.

---

## 📅 Day 3: Configure Git

Set your name and email:

```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

View your configuration:

```bash
git config --global --list
```

**Practice:** Configure your Git identity.

---

## 📅 Day 4: Create Your First Repository

Create a folder:

```bash
mkdir git-practice
cd git-practice
```

Initialize Git:

```bash
git init
```

Check the repository:

```bash
git status
```

**Practice:** Create your own Git repository.

---

## 📅 Day 5: Create and Track Files

Create a file named `README.md`.

Add it to staging:

```bash
git add README.md
```

Check the status:

```bash
git status
```

**Practice:** Create a text file and stage it.

---

## 📅 Day 6: First Commit

A commit saves a checkpoint of your staged changes.

```bash
git commit -m "Initial commit"
```

**Practice:** Create your first commit.

---

## 📅 Day 7: Git Status and Diff

Check your changes:

```bash
git status
git diff
git diff --staged
```

- `git status` shows the current repository state.
- `git diff` shows unstaged changes.
- `git diff --staged` shows staged changes.

**Practice:** Edit a file and inspect the differences.

---

## 📅 Day 8: View Commit History

View your commit history:

```bash
git log
```

View a shorter version:

```bash
git log --oneline
```

**Practice:** Make two commits and review your history.

---

## 📅 Day 9: Modify and Update Files

Edit your README file and save the changes:

```bash
git add README.md
git commit -m "Update README"
```

**Practice:** Add a new section to your README.

---

## 📅 Day 10: Git Ignore

Create a `.gitignore` file to exclude certain untracked files.

Example:

```gitignore
__pycache__/
*.pyc
.env
.venv/
```

**Note:** Never commit passwords, API keys, or other secrets.

**Practice:** Create a `.gitignore` file and test it.

---

## 📅 Day 11: Introduction to Branches

Branches allow you to develop features separately.

List branches:

```bash
git branch
```

Create a branch:

```bash
git branch feature
```

Switch branches:

```bash
git switch feature
```

Or create and switch in one command:

```bash
git switch -c feature
```

**Practice:** Create a branch named `feature-about`.

---

## 📅 Day 12: Commit Changes on a Branch

Make a change on your feature branch.

```bash
git add README.md
git commit -m "Add feature information"
```

Switch back to your main branch:

```bash
git switch main
```

**Practice:** Make a commit on a separate branch.

---

## 📅 Day 13: Merge Branches

Merge your feature branch into `main`:

```bash
git switch main
git merge feature
```

If your default branch is named `master`, use `master` instead.

**Practice:** Create a feature branch and merge it.

---

## 📅 Day 14: Resolve Merge Conflicts

Merge conflicts occur when Git cannot automatically combine changes.

Typical steps:

1. Open the conflicted file.
2. Find the conflict markers.
3. Choose or combine the required changes.
4. Remove the conflict markers.
5. Stage and commit the resolved file.

```bash
git add README.md
git status
git commit -m "Resolve merge conflict"
```

**Practice:** Resolve a conflict in a test repository.

---

## 📅 Day 15: Create a GitHub Repository

1. Sign in to https://github.com/.
2. Click **New repository**.
3. Enter a repository name.
4. Choose public or private visibility.
5. Create the repository.
6. Copy its HTTPS URL.

**Practice:** Create a repository named `git-20-day-tutorial`.

---

## 📅 Day 16: Connect Git to GitHub

Add your GitHub repository as a remote:

```bash
git remote add origin https://github.com/YOUR-USERNAME/git-20-day-tutorial.git
```

Check the remote:

```bash
git remote -v
```

Push your main branch:

```bash
git push -u origin main
```

Replace the example username and repository name with your own.

**Practice:** Upload your local project to GitHub.

---

## 📅 Day 17: Clone a Repository

Clone a repository to your computer:

```bash
git clone https://github.com/OWNER/REPOSITORY.git
```

Open the cloned folder:

```bash
cd REPOSITORY
```

**Practice:** Clone your GitHub repository.

---

## 📅 Day 18: Pull and Push

Download and integrate remote changes:

```bash
git pull
```

Upload your local commits:

```bash
git push
```

**Practice:** Edit your README on GitHub, pull the changes locally, and push a new local commit.

---

## 📅 Day 19: Undo Common Mistakes

Unstage a file without deleting its changes:

```bash
git restore --staged README.md
```

Discard unstaged edits to a tracked file:

```bash
git restore README.md
```

**Warning:** The second command discards unstaged edits to that file.

Create a new commit that reverses an earlier commit:

```bash
git revert COMMIT_ID
```

**Practice:** Practise these commands in a test repository.

---

## 📅 Day 20: Final Mini Project 🎯

Create a Git Learning Journal.

### Project Structure

```text
git-learning-journal/
├── README.md
├── day1.md
├── day2.md
├── day3.md
└── .gitignore
```

### Tasks

- [ ] Initialize a Git repository.
- [ ] Create your learning notes.
- [ ] Track files using `git add`.
- [ ] Save changes using `git commit`.
- [ ] Review changes using `git diff`.
- [ ] View history using `git log`.
- [ ] Create and merge a branch.
- [ ] Create a GitHub repository.
- [ ] Push your code to GitHub.
- [ ] Clone your repository.
- [ ] Practise pulling remote changes.

**Final Goal:** Complete the project and publish your learning journey on GitHub!

---

## ⚡ Git Command Cheat Sheet

| Command | Purpose |
|---|---|
| `git init` | Initialize a repository |
| `git status` | Check repository status |
| `git add .` | Stage changes under the current directory |
| `git commit -m "message"` | Save a commit |
| `git diff` | View unstaged changes |
| `git log --oneline` | View commit history |
| `git branch` | List branches |
| `git switch -c branch-name` | Create and switch branches |
| `git merge branch-name` | Merge a branch |
| `git clone URL` | Clone a repository |
| `git pull` | Integrate remote changes |
| `git push` | Upload local commits |
| `git remote -v` | View remote repositories |

---

## 🔗 Useful Resources

- [Git Official Website](https://git-scm.com/)
- [Git Documentation](https://git-scm.com/docs)
- [Pro Git Book](https://git-scm.com/book/en/v2)
- [GitHub Documentation](https://docs.github.com/)
- [GitHub Skills](https://skills.github.com/)

---

## 🎉 Conclusion

Congratulations on completing this 20-day Git and GitHub tutorial!

Keep practising, write meaningful commit messages, protect your private information, and use Git regularly in your projects.

**Happy Coding! 💻**
