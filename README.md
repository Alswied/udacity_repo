# Udacity Repo
This is a repository to gain familiarity with Git and GitHub.

---

## Common Git Commands

### Repository Initialization
- `git init`: Create a new, brand-new repository.
- `git clone <repo_url>`: Clone or copy an existing repository.

---

### Staging and Committing Changes
- `git status`: Check the status of the repository.
- `git add <file1> <file2> ... <fileN>`: Add files from the working directory to the staging index.
  - Add all files in one command: `git add .`
- `git rm --cached <file>`: Remove the file from the staging index (file is not deleted).
- `git commit`: Take files from the staging index and save them in the repository.
- `git commit -m "message"`: Save staged changes with a commit message directly in the terminal.
- `git commit --amend`: Alter the most recent commit.

---

### Viewing Changes and Logs
- `git diff`: Display the differences between two versions of a file.
- `git show <commit_id>`: Display information about a specific commit.
- `git log`: Display information about existing commits.
  - Filter commits by message: `git log --grep="bug"`
  - Filter commits by author: `git log --author="AuthorName"`
  - Show all branches and commits: `git log --oneline --decorate --graph --all`
- `git log --oneline origin/main`: Check what is on remote.

---

### Tags
- `git tag <tag_name>`: Add a label to a commit.
  - Annotated tag: `git tag -a v1.0`
  - Tag a specific commit: `git tag -a v1.0 <commit_id>`
  - Delete a tag: `git tag -d v1.0`

---

### Branching
- `git branch <branch_name>`: Create a new branch.
- `git branch`: List all branches.
- `git branch -d <branch_name>`: Delete a branch.
- `git branch -M main`: Rename the current branch to `main`.

---

### Switching Branches
- `git checkout <branch_name>`: Switch to a specific branch.
- `git checkout -b <new_branch>`: Create and switch to a new branch.
- `git checkout -b <new_branch> <start_point>`: Create a new branch starting at a specific commit.

---

### Merging and Rebasing
- `git merge <branch_name>`: Merge changes from another branch into the current branch.
  - Undo a merge: `git reset --hard HEAD^`
- `git rebase -i HEAD~<n>`: Rebase the last `n` commits interactively.
  - Options:
    - `p` or `pick`: Keep the commit as is.
    - `r` or `reword`: Edit the commit message.
    - `e` or `edit`: Edit the commit content.
    - `s` or `squash`: Combine this commit with the previous one.
    - `f` or `fixup`: Combine this commit with the previous one and discard the commit message.
    - `d` or `drop`: Delete the commit.

---

### Undoing Changes
- `git revert <commit_id>`: Reverse a specific commit.
- `git reset`: Delete a commit.
  - `git reset --mixed`: Move the last commit to the working directory.
  - `git reset --soft`: Move the last commit to the staging area.
  - `git reset --hard`: Permanently delete the last commit.

---

### Remote Repositories
- `git remote add <name> <url>`: Link your local repository to a remote repository.
- `git remote -v`: Verify the remote repository link.
- `git remote remove <name>`: Remove a remote repository.
- `git remote rename <old_name> <new_name>`: Rename a remote repository.

---

### Pushing and Pulling Changes
- `git push origin <branch>`: Push local commits to the remote branch.
- `git pull origin <branch>`: Download and merge changes from the remote branch.
- `git fetch origin <branch>`: Download updates from the remote branch without merging.
- `git push -u origin <branch>`: Push the branch and set it as the default upstream branch.

---

### Forking and Cloning
- `git fork`: Create a copy of a remote repository under your account.
  - **Difference between Forking and Cloning**:
    - **Forking**: Creates a duplicate copy of the remote repository under your account.
    - **Cloning**: Creates a local copy of a remote repository on your machine.

---

### Miscellaneous Commands
- `git reflog`: View a log of all references (kept for 30 days).
- `git shortlog`: Display an alphabetical list of commit authors and their commit messages.
  - Options:
    - `-s`: Show just the number of commits.
    - `-n`: Sort the list numerically.

---

This organized structure makes it easier to find specific commands and understand their purpose. Let me know if you need further refinements!# Udacity Repo
This is a repository to gain familiarity with Git and GitHub.

---

## Common Git Commands

### Repository Initialization
- `git init`: Create a new, brand-new repository.
- `git clone <repo_url>`: Clone or copy an existing repository.

---

### Staging and Committing Changes
- `git status`: Check the status of the repository.
- `git add <file1> <file2> ... <fileN>`: Add files from the working directory to the staging index.
  - Add all files in one command: `git add .`
- `git rm --cached <file>`: Remove the file from the staging index (file is not deleted).
- `git commit`: Take files from the staging index and save them in the repository.
- `git commit -m "message"`: Save staged changes with a commit message directly in the terminal.
- `git commit --amend`: Alter the most recent commit.

---

### Viewing Changes and Logs
- `git diff`: Display the differences between two versions of a file.
- `git show <commit_id>`: Display information about a specific commit.
- `git log`: Display information about existing commits.
  - Filter commits by message: `git log --grep="bug"`
  - Filter commits by author: `git log --author="AuthorName"`
  - Show all branches and commits: `git log --oneline --decorate --graph --all`

---

### Tags
- `git tag <tag_name>`: Add a label to a commit.
  - Annotated tag: `git tag -a v1.0`
  - Tag a specific commit: `git tag -a v1.0 <commit_id>`
  - Delete a tag: `git tag -d v1.0`

---

### Branching
- `git branch <branch_name>`: Create a new branch.
- `git branch`: List all branches.
- `git branch -d <branch_name>`: Delete a branch.
- `git branch -M main`: Rename the current branch to `main`.

---

### Switching Branches
- `git checkout <branch_name>`: Switch to a specific branch.
- `git checkout -b <new_branch>`: Create and switch to a new branch.
- `git checkout -b <new_branch> <start_point>`: Create a new branch starting at a specific commit.

---

### Merging and Rebasing
- `git merge <branch_name>`: Merge changes from another branch into the current branch.
  - Undo a merge: `git reset --hard HEAD^`
- `git rebase -i HEAD~<n>`: Rebase the last `n` commits interactively.
  - Options:
    - `p` or `pick`: Keep the commit as is.
    - `r` or `reword`: Edit the commit message.
    - `e` or `edit`: Edit the commit content.
    - `s` or `squash`: Combine this commit with the previous one.
    - `f` or `fixup`: Combine this commit with the previous one and discard the commit message.
    - `d` or `drop`: Delete the commit.

---

### Undoing Changes
- `git revert <commit_id>`: Reverse a specific commit.
- `git reset`: Delete a commit.
  - `git reset --mixed`: Move the last commit to the working directory.
  - `git reset --soft`: Move the last commit to the staging area.
  - `git reset --hard`: Permanently delete the last commit.

---

### Remote Repositories
- `git remote add <name> <url>`: Link your local repository to a remote repository.
- `git remote -v`: Verify the remote repository link.
- `git remote remove <name>`: Remove a remote repository.
- `git remote rename <old_name> <new_name>`: Rename a remote repository.

---

### Pushing and Pulling Changes
- `git push origin <branch>`: Push local commits to the remote branch.
- `git pull origin <branch>`: Download and merge changes from the remote branch.
- `git fetch origin <branch>`: Download updates from the remote branch without merging.
- `git push -u origin <branch>`: Push the branch and set it as the default upstream branch.

---

### Forking and Cloning
- `git fork`: Create a copy of a remote repository under your account.
  - **Difference between Forking and Cloning**:
    - **Forking**: Creates a duplicate copy of the remote repository under your account.
    - **Cloning**: Creates a local copy of a remote repository on your machine.

---

### Miscellaneous Commands
- `git reflog`: View a log of all references (kept for 30 days).
- `git shortlog`: Display an alphabetical list of commit authors and their commit messages.
  - Options:
    - `-s`: Show just the number of commits.
    - `-n`: Sort the list numerically.

---