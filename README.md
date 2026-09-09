# Lab 03: Git and GitHub

This repository documents my practice with 
local Git, GitHub, branches, and pull requests.

## README Responses

### 1.1 After initialization
```text
ls -la
atomi@LAPTOP-1APKAE2C:~/csci338/lab03-exercises$ ls -la
total 12
drwxr-xr-x 3 atomi atomi 4096 Sep  3 09:58 .
drwxr-xr-x 6 atomi atomi 4096 Sep  3 09:58 ..
drwxr-xr-x 6 atomi atomi 4096 Sep  3 09:58 .git
```

### 1.2 First git status

```text
atomi@LAPTOP-1APKAE2C:~/csci338/lab03-exercises$ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md

nothing added to commit but untracked files present (use "git add" to track)
```

### 1.3 After the first commit

```text
atomi@LAPTOP-1APKAE2C:~/csci338/lab03-exercises$ git status
On branch main
nothing to commit, working tree clean
```

### 1.4 git log
```text
atomi@LAPTOP-1APKAE2C:~/csci338/lab03-exercises$ git log --oneline
0f5b3c6 (HEAD -> main) Create lab README
```

### 1.5 git diff

Paste the `git status` and `git diff` commands and their output.

```text
atomi@LAPTOP-1APKAE2C:~/csci338/lab03-exercises$ git status
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
```
```text
atomi@LAPTOP-1APKAE2C:~/csci338/lab03-exercises$ git diff
diff --git a/README.md b/README.md
index 0934033..2b084c6 100644
--- a/README.md
+++ b/README.md
@@ -1,5 +1,8 @@
 # Lab 03: Git and GitHub

+This repository documents my practice with ^M
+local Git, GitHub, branches, and pull requests.^M
+^M
 ## README Responses

 ### 1.1 After initialization
@@ -30,14 +33,23 @@ nothing added to commit but untracked files present (use "git add" to track)
 ### 1.3 After the first commit


+atomi@LAPTOP-1APKAE2C:~/csci338/lab03-exercises$ git status^M
+On branch main^M
+nothing to commit, working tree clean^M


 ### 1.4 git log

+atomi@LAPTOP-1APKAE2C:~/csci338/lab03-exercises$ git log --oneline^M
+0f5b3c6 (HEAD -> main) Create lab README^M


 ### 1.5 git diff

 Paste the `git status` and `git diff` commands and their output.

+^M
+^M
 How does this `git status` differ from the one in **1.2**?

 ### 1.6 Git command reflections
```

How does this `git status` differ from the one in **1.2**?
```text
the new one shows that README has been changed, and commits have been done
```

### 1.6 Git command reflections

In one or two sentences each, what does each command do?

- `git init`
```text
turns the current directory into a Git repository
```
- `git status`
```text
tells what files (if any) are changed/new compared to most recent commit in repo
```
- `git add`
```text
stages files to be committed
```
- `git commit`
```text
commits staged files to the repo
```
- `git log`
```text
command shows commit history
```
- `git diff`
```text
shows most recent changes in files compared to most recent commit
```

### 1.7 Repository link
```text
https://github.com/bcjenkins1/lab03-exercises
```

### 1.8 Comparing approaches

In your own words:

- How does the nested-loop approach check for a duplicate?
  ```text
  The loop compares each number with every number that comes after it
  ```

- How does the set-based approach check for a duplicate?
  ```text
  it buts everything into a HashSet and a set can't contain duplicates, so they're automatically removed
  ```

- What is the runtime and memory trade-off of each?
  ```test
  Runtime, Memory
  Loop: O(n^2), O(1)
  Memory: O(n), O(n)
  ```


### 1.9 Pull request merge options

In your own words, what does each GitHub merge option do?

- Create a merge commit
- Squash and merge
- Rebase and merge

```test

```