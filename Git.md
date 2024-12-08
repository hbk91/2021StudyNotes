---
title: "Git"
author: "Aman Jindal"
description: "Notes"
---

## **Common Git Commands**

| **Command**                | **Description**                                                                 |
|-----------------------------|---------------------------------------------------------------------------------|
| `git init`                 | Initializes a new Git repository in the current directory.                      |
| `git clone [url]`          | Clones a repository from the specified URL to your local machine.               |
| `git status`               | Displays the state of the working directory and staging area.                   |
| `git add [file]`           | Adds a file to the staging area for the next commit.                            |
| `git commit -m "[message]"`| Commits the staged changes with a descriptive message.                          |
| `git push`                 | Pushes the committed changes to the remote repository.                          |
| `git pull`                 | Fetches and merges changes from the remote repository to the local repository.  |
| `git branch`               | Lists all branches in the repository or creates a new branch.                   |
| `git checkout [branch]`    | Switches to the specified branch.                                               |
| `git merge [branch]`       | Merges the specified branch into the current branch.                            |
| `git log`                  | Shows the commit history for the current branch.                                |
| `git diff`                 | Displays changes between commits, branches, or the working directory.           |
| `git reset [file]`         | Unstages a file from the staging area without removing its changes.             |
| `git rm [file]`            | Removes a file from the working directory and stages the removal.               |
| `git stash`                | Temporarily saves changes without committing them.                              |
| `git stash pop`            | Restores the most recently stashed changes and removes them from the stash list.|
| `git remote -v`            | Displays the URLs of remote repositories.                                       |
| `git tag [tag_name]`       | Creates a tag for a specific commit.                                            |
| `git fetch`                | Downloads objects and refs from another repository without merging.             |

## **Pulling from `origin` Variants**

| **Command**                      | **Description**                                                                                  |
|-----------------------------------|--------------------------------------------------------------------------------------------------|
| `git pull origin`                | Pulls the latest changes from the current branch of the `origin` remote.                        |
| `git pull origin [branch]`       | Pulls the latest changes from the specified branch of the `origin` remote (e.g., `main`).       |
| `git fetch origin`               | Fetches changes from the `origin` remote without merging them.                                  |
| `git merge origin/[branch]`      | Merges the fetched changes from the specified branch into the current branch.                   |
| `git pull --rebase origin [branch]` | Fetches changes from the `origin` remote and applies your local changes on top (rebases).       |

## **Pulling from a Specific Branch**

| **Command**                             | **Description**                                                                                          |
|------------------------------------------|----------------------------------------------------------------------------------------------------------|
| `git pull origin [branch]`              | Pulls changes from a specific branch on the `origin` remote to the current branch.                       |
| `git checkout [branch]`                 | Switches to the specific branch to ensure the changes are pulled into the correct branch.                |
| `git fetch origin [branch]`             | Fetches changes from a specific branch on the `origin` remote without merging them into the local branch.|
| `git merge origin/[branch]`             | Merges fetched changes from a specific branch into the current branch.                                   |
| `git pull --rebase origin [branch]`     | Rebases the current branch on top of the changes from a specific branch on the `origin` remote.          |
| `git pull origin [source_branch]:[target_branch]` | Pulls changes from a source branch on the remote and merges into a local target branch.                  |


