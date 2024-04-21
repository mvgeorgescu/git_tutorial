---
layout: slide
title: Basic Git Commands
---

---

<section markdown="1">


### git init: Initializing a Repository

- `git init` creates a new Git repository in the current directory.
- It initializes an empty repository with a .git directory where Git stores metadata and the version history of the project.

### git status: Checking the Status of the Repository

- `git status` provides information about the current state of the repository.
- It shows which files have been modified, staged, or untracked, helping you keep track of changes in your project.

{% highlight bash %}
➜ git status
On branch main
Your branch is ahead of 'origin/main' by 4 commits.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
{% endhighlight %}

</section>


<section markdown="1">
### git log: Viewing the Commit History

- `git log` displays the commit history of the repository, showing the list of commits in reverse chronological order.
- It includes details such as hashes, authors, timestamps, and commit messages.
- You can use options like `--oneline` and `--graph` to customize the output format.
</section>

<section markdown="1">
{% highlight bash %}
* d069ae6 (HEAD -> 20240402_updates, origin/20240402_updates) add PR assets
* 3336de4 update content
* 84da7ba update git ignore
* 91c7eb1 remove ds_store
* 1e796dc update dependencies
* 63bbc48 add branching diagram
* a75cc19 (origin/main, origin/HEAD, main) added commit history img
* 2b2206b alignment test
* 7dade26 r-stack test
* c3d6afd center image test
* dd186de added branching image
{% endhighlight %}
</section>

<section markdown="1">

### git add: Adding Changes to the Staging Area

- `git add <file>` stages changes in the specified file, preparing them to be committed.
- You can also use `git add .` or `git add -A` to stage all changes in the working directory.
- The staging area allows you to selectively choose which changes to include in the next commit.

### git commit: Committing Changes to the Repository

- `git commit` records staged changes to the repository, creating a new commit.
- Each commit has a unique identifier (SHA-1 hash), author, timestamp, and commit message describing the changes made.
- The commit message should be descriptive and succinct, explaining the purpose of the changes.
</section>

<section markdown="1">
![commit_history](https://raw.githubusercontent.com/mvgeorgescu/git_tutorial/main/assets/images/commit_history.png){:style="display:block; margin-left:auto; margin-right:auto; width:65%;"}
</section>

<section markdown="1">

### git branch: Managing Branches

- `git branch` lists existing branches in the repository.
- You can create a new branch using `git branch <branch_name>` and switch to it using `git checkout <branch_name>` or `git switch <branch_name>`.
- Deleting a branch is done with `git branch -d <branch_name>`.

### git merge: Integrating Changes

- `git merge` combines changes from one branch into another.
- It integrates the changes while preserving the commit history of both branches.
- Merging is commonly used to incorporate feature branches into the main branch (e.g., master).
</section>

