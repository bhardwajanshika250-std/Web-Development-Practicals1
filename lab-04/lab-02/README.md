# Lab 2: Pushing and Cloning a Repository

## 1. Practical Aim
To create a local bare repository, push commits to it, clone it into a new directory, and verify commit logs.

## 2. Theoretical Background
- **Bare Repository (`--bare`):** A repository containing Git history and metadata without a working directory. Used primarily as a central remote endpoint to share/receive commits.
- **Git Remote (`git remote add`):** Maps a friendly name (like `origin`) to a repository path or URL.
- **Git Push (`git push`):** Sends committed local changes to a remote repository branch.
- **Git Clone (`git clone`):** Copies an existing Git repository, creating a working copy with complete history.
- **Git Log (`git log --oneline`):** Displays commit history in a concise single-line format.

## 3. Pre-requisites & Tools Used
- Git version 2.56.0+
- Visual Studio Code (Terminal)
- Windows OS File Directory Structure

## 4. Step-by-Step Procedure
1. Created a local bare repository next to the main directory using `git init --bare ../html-remote`.
2. Added the bare repository as remote origin using `git remote add origin ../html-remote`.
3. Verified remote links with `git remote -v`.
4. Pushed local branch commits to the remote origin using `git push origin master` (or `main`).
5. Navigated up one directory and cloned the remote repository into a new folder named `html-copy` using `git clone html-remote html-copy`.
6. Changed directory into `html-copy` and verified commit history with `git log --oneline`.

## 5. Command Log / Source Code
```bash
# Task 1: Bare repository and remote setup
git init --bare ../html-remote
git remote add origin ../html-remote
git remote -v

# Task 2: Push commits to origin
git push origin master

# Task 3: Clone remote and verify logs
cd ..
git clone html-remote html-copy
cd html-copy
git log --oneline
6. Screenshots & Output Evidence
Task 1 Output: ![Task 1 Remote Setup](images/task1.png)

Task 2 Output: ![Task 2 Git Push](images/task2.png)

Task 3 Output: ![Task 3 Git Clone & Log](images/task3.png)

7. Key Learning Outcomes
Understood how local remote bare repositories function without GitHub/Cloud servers.

Learned how to manage remote connections, branch pushing, and clone verification in Git.

8. Common Errors & Troubleshooting
fatal: not a git repository: Fixed by initializing git in the project root (git init) and completing initial commits before setting remote links.

git config missing: Fixed by setting global user name and email.

9. Viva / Interview Questions
Q: What is the difference between git init and git init --bare?

A: git init creates a working repository with code files editable directly. git init --bare creates only Git history/metadata without source files, intended to act as a remote host.

Q: What does git log --oneline do?

A: It prints commit hashes and commit messages in a single line per commit for quick log viewing.

10. Submission Checklist
[x] Task 1 execution & - **Task 1 Output:** ![Task 1 Remote Setup](images/task1.png)
- **Task 2 Output:** ![Task 2 Git Push](images/task2.png)
- **Task 3 Output:** ![Task 3 Git Clone & Log](images/task3.png)
