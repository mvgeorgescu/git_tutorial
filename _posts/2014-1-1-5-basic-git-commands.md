---
layout: slide
title: Basic Git Commands
---

---

<section markdown="1">

Git provides a set of powerful commands for managing version-controlled projects efficiently. These commands form the backbone of everyday Git usage and are essential for any developer working with Git. Let's explore some of the most commonly used Git commands:

## git init: Initializing a Repository

- `git init` creates a new Git repository in the current directory, turning it into a Git project.
- It initializes an empty repository with a .git directory where Git stores metadata and the version history of the project.

## git status: Checking the Status of the Repository

- `git status` provides information about the current state of the repository.
- It shows which files have been modified, staged, or untracked, helping you keep track of changes in your project.
- `git status` is a useful command for understanding what needs to be committed or staged.

## git log: Viewing the Commit History

- `git log` displays the commit history of the repository, showing the list of commits in reverse chronological order.
- It includes details such as commit hashes, authors, timestamps, and commit messages.
- You can use options like `--oneline`, `--graph`, and `--decorate` to customize the output format.
</section>

<section markdown="1">
## git add: Adding Changes to the Staging Area

- `git add <file>` stages changes in the specified file, preparing them to be committed.
- You can also use `git add .` or `git add -A` to stage all changes in the working directory.
- The staging area allows you to selectively choose which changes to include in the next commit.

## git commit: Committing Changes to the Repository

- `git commit` records staged changes to the repository, creating a new commit.
- Each commit has a unique identifier (SHA-1 hash), author, timestamp, and commit message describing the changes made.
- The commit message should be descriptive and succinct, explaining the purpose of the changes.
</section>

<section markdown="1">
## git branch: Managing Branches

- `git branch` lists existing branches in the repository.
- You can create a new branch using `git branch <branch_name>` and switch to it using `git checkout <branch_name>` or `git switch <branch_name>`.
- Deleting a branch is done with `git branch -d <branch_name>`.

## git merge: Integrating Changes

- `git merge` combines changes from one branch into another.
- It integrates the changes while preserving the commit history of both branches.
- Merging is commonly used to incorporate feature branches into the main branch (e.g., master).
</section>

