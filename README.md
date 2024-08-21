# Git Conflict Resolution Exercise

Welcome to the Git Conflict Resolution Exercise! This repository is designed to help you practice handling conflicts that arise when merging, rebasing, and squashing branches in Git.

## Overview

In this exercise, you'll work with a repository that has multiple branches, each containing changes that will intentionally conflict with each other. Your task is to resolve these conflicts as you merge, rebase, and squash commits across branches.

## Branches

The repository contains the following branches:

- **`main`**: The main branch where all changes will eventually be merged.
- **`feature-A`**: A feature branch with changes that conflict with those in the `main` branch.
- **`feature-B`**: Another feature branch with different conflicting changes in the same files as `feature-A` and `main`.
- **`feature-C`**: A branch with additional changes that will introduce more complex conflicts when rebasing or merging.

## Exercise Instructions

### 1. Merging with Conflicts

- **Goal**: Merge `feature-A` into `main` and resolve the conflicts.
- **Steps**:
  1. Check out the `main` branch.
  2. Merge `feature-A` into `main`.
  3. Resolve the conflict in `README.md` and any other conflicting files.
  4. Commit the resolved merge and push to the remote repository.

### 2. Rebasing with Conflicts

- **Goal**: Rebase `feature-B` onto the `main` branch and resolve the conflicts.
- **Steps**:
  1. Check out the `feature-B` branch.
  2. Rebase `feature-B` onto `main`.
  3. Resolve the conflict in `README.md` and any other conflicting files.
  4. Complete the rebase and push the branch to the remote repository.

### 3. Squashing Commits with Conflicts

- **Goal**: Squash the commits in `feature-C` into a single commit and merge it into `main`, resolving conflicts along the way.
- **Steps**:
  1. Check out the `feature-C` branch.
  2. Use interactive rebase to squash the commits into one.
  3. Check out the `main` branch.
  4. Merge the squashed `feature-C` branch into `main`.
  5. Resolve any conflicts and push the final merged branch to the remote repository.

## Conflict Resolution Tips

- Use `git status` to see which files have conflicts.
- Open the conflicting files in your favorite text editor and manually resolve the conflicts. Look for lines marked with `<<<<<<<`, `=======`, and `>>>>>>>`.
- After resolving conflicts, use `git add <file>` to mark the conflicts as resolved.
- If you're stuck, don't hesitate to use `git rebase --abort` or `git merge --abort` to undo the operation and start over.

## Getting Started

To get started, clone this repository to your local machine:

```bash
git clone <repository-url>
cd git-training
```

Once you've cloned the repository, follow the instructions in each exercise section to practice resolving conflicts.