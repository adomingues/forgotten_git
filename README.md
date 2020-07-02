# forgotten git

All the git commands I keep googling.


## discard uncommited changes in a file

```bash
git checkout hello.html
```
Source: https://githowto.com/undoing_local_changes


## create branch with uncommited changes

```bash
git checkout -b new_branch
```
Source: https://stackoverflow.com/questions/1394797/move-existing-uncommitted-work-to-a-new-branch-in-git


## How can I reset or revert a file to a specific revision?

```bash
git checkout c5f567 -- file1/to/restore file2/to/restore
```
Source: https://stackoverflow.com/a/215731/1274242

## Merging and branching

1. create new branch

```bash
git checkout -b hotfix
```

2. Do something and commit.

3. change to master and merge

```bash
git checkout master
git merge hotfix
```

4. (optional) Delete branch

```bash
git branch -d hotfix
```

Source: https://git-scm.com/book/en/v2/Git-Branching-Basic-Branching-and-Merging

## create a branch from a specific commit

This is helful to to debbug or test changes that occoured at a particular commit which is well in the past.

```bash
git checkout -b fread_commit bef92a83
```
