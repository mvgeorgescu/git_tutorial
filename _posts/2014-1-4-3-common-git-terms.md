---
layout: slide
title: Common Terms in Git / GitHub
---

---

<section markdown="1">

### Core Terminology and Concepts

<ul>
  <li><strong>Repository (Repo):</strong> 
    <ul>
      <li>A collection of files and their history.
        <ul>
          <li><em>Local Repository:</em> Exists on a local machine.</li>
          <li><em>Remote Repository:</em> Hosted on a remote server.</li>
        </ul>
      </li>
    </ul>
  </li>
  <li><strong>Commit:</strong> 
    <ul>
      <li>A snapshot of changes to the repository.</li>
    </ul>
  </li>
  <li><strong>Branch:</strong> 
    <ul>
      <li>A parallel version of the repository.
        <ul>
          <li>Allows for independent work.</li>
        </ul>
      </li>
    </ul>
  </li>
  <li><strong>Merge:</strong> 
    <ul>
      <li>Combines changes from one branch into another.</li>
    </ul>
  </li>
  <li><strong>Pull Request:</strong> 
    <ul>
      <li>Mechanism for submitting contributions.
        <ul>
          <li>Facilitates code review and discussion.</li>
        </ul>
      </li>
    </ul>
  </li>
</ul>

</section>

<section markdown="1">

### Local Repository vs. Remote Repository:

- **Local Repository:**
  - A copy of the project's entire history and files stored on your computer.
  - Resides in a hidden `.git` directory within your project directory.

- **Remote Repository:**
  - A version of your project hosted on a remote server (e.g., GitHub, GitLab, Bitbucket).
  - Serves as a central point for collaboration, allowing team members to share changes and collaborate on the project.

*It is entirely possible to run Git with only a local repository, without needing a remote repository.*
</section>

<section markdown="1">

### Committing Changes

- A commit in Git is a snapshot of the project at a specific point in time.
- It records changes to files in the repository.
- Each commit has a unique identifier (SHA-1 hash), author, timestamp, and commit message describing the changes made.
- Commits are the building blocks of Git's version control system, enabling you to track changes and revert to previous states of the project if needed.

<br>

![commit_diagram](https://raw.githubusercontent.com/mvgeorgescu/git_tutorial/main/assets/images/commit_history_diagram.png){:style="display:block; margin-left:auto; margin-right:auto"}
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
![branching](https://www.nobledesktop.com/image/gitresources/git-branches-merge.png){:style="display:block; margin-left:auto; margin-right:auto"}
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

