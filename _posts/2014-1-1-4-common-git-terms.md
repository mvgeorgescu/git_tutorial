---
layout: slide
title: Common Terms in Git
---

---

<section markdown="1" style="text-align: left;">

## Core Terminology and Concepts

- **Repository:** A collection of files and their history.
  - Local Repository: Exists on a local machine.
  - Remote Repository: Hosted on a remote server.
- **Commit:** A snapshot of changes to the repository.
- **Branch:** A parallel version of the repository.
  - Allows for independent work.
- **Merge:** Combines changes from one branch into another.
- **Pull Request:** Mechanism for submitting contributions.
  - Facilitates code review and discussion.
</section>

<section markdown="1">

## Local Repository vs. Remote Repository:

- **Local Repository:**
  - A copy of the project's entire history and files stored on your computer.
  - Resides in a hidden `.git` directory within your project directory.

- **Remote Repository:**
  - A version of your project hosted on a remote server (e.g., GitHub, GitLab, Bitbucket).
  - Serves as a central point for collaboration, allowing team members to share changes and collaborate on the project.
</section>

<section markdown="1">

## Committing Changes

- A commit in Git is a snapshot of the project at a specific point in time.
- It records changes to files in the repository.
- Each commit has a unique identifier (SHA-1 hash), author, timestamp, and commit message describing the changes made.
- Commits are the building blocks of Git's version control system, enabling you to track changes and revert to previous states of the project if needed.
</section>

<section markdown="1">

## Branching and Merging

### Branching:
- Branching in Git allows you to diverge from the main line of development (often called the master branch) and work on new features, bug fixes, or experiments without affecting the main codebase.

### Creating a Branch:
- You can create a new branch using the `git branch` command and switch to it using `git checkout` or `git switch`.

### Merging:
- Merging combines changes from one branch into another.
- It integrates the changes while preserving the commit history of both branches.
</section>

<section markdown="1">

### Working Directory

- The working directory is where you modify files in your project.
- It contains the actual files of the project, as well as any changes you have made since the last commit.
- Git monitors changes in the working directory and tracks them as modifications to be staged and committed.
</section>

<section markdown="1">

### Staging Area (Index):

The staging area, also known as the index, is an intermediate area between your working directory and the repository.
It acts as a holding area where you can stage changes before committing them to the repository.
This allows you to selectively choose which changes to include in the next commit, giving you more control over the commit process.
</section>

<section markdown="1">

### HEAD

- HEAD is a pointer to the current branch or commit in Git.
- It represents the state of your working directory and is typically used to refer to the latest commit on the current branch.
- When you switch branches or check out a specific commit, Git updates the HEAD to point to the corresponding branch or commit.

To view the current HEAD in Git, you can use the following command:
```bash
git rev-parse HEAD
```
</section>

