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

### 1.6 Git command reflections

In one or two sentences each, what does each command do?

- `git init`
- `git status`
- `git add`
- `git commit`
- `git log`
- `git diff`

### 1.7 Repository link

### 1.8 Comparing approaches

In your own words:

- How does the nested-loop approach check for a duplicate?
- How does the set-based approach check for a duplicate?
- What is the runtime and memory trade-off of each?

### 1.9 Pull request merge options

In your own words, what does each GitHub merge option do?

- Create a merge commit
- Squash and merge
- Rebase and merge