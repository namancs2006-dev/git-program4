HI@DESKTOP-90KBJMH MINGW64 ~
$ cd "~C:\Users\HI\git commands"
bash: cd: ~C:\Users\HI\git commands: No such file or directory

HI@DESKTOP-90KBJMH MINGW64 ~
$ cd "C:\Users\HI\git commands~"
bash: cd: C:\Users\HI\git commands~: No such file or directory

HI@DESKTOP-90KBJMH MINGW64 ~
$ cd "C:\Users\HI\git commands"

HI@DESKTOP-90KBJMH MINGW64 ~/git commands
$ git clone "https://github.com/namancs2006-dev/git-program4.git"
Cloning into 'git-program4'...
remote: Enumerating objects: 12, done.
remote: Counting objects: 100% (12/12), done.
remote: Compressing objects: 100% (8/8), done.
remote: Total 12 (delta 2), reused 2 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (12/12), 555.53 KiB | 5.55 MiB/s, done.
Resolving deltas: 100% (2/2), done.

HI@DESKTOP-90KBJMH MINGW64 ~/git commands
$ git status
fatal: not a git repository (or any of the parent directories): .git

HI@DESKTOP-90KBJMH MINGW64 ~/git commands
$ ^C

HI@DESKTOP-90KBJMH MINGW64 ~/git commands
$ cd git-program4

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ code .


HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   stash_demo/mystash.txt

no changes added to commit (use "git add" and/or "git commit -a")

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git diff
diff --git a/stash_demo/mystash.txt b/stash_demo/mystash.txt
index 379d91b..339833b 100644
--- a/stash_demo/mystash.txt
+++ b/stash_demo/mystash.txt
@@ -1 +1,2 @@
 print('hello world')
+//changing a simple line and understanding it with the help of git diff
\ No newline at end of file

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ ^C

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git add stash_demo/mystash.txt

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   stash_demo/mystash.txt


HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git diff

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ ^C

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git diff --staged
diff --git a/stash_demo/mystash.txt b/stash_demo/mystash.txt
index 379d91b..339833b 100644
--- a/stash_demo/mystash.txt
+++ b/stash_demo/mystash.txt
@@ -1 +1,2 @@
 print('hello world')
+//changing a simple line and understanding it with the help of git diff
\ No newline at end of file

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ ^C

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   stash_demo/mystash.txt

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   stash_demo/mystash.txt


HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ ^C

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git diff --staged
diff --git a/stash_demo/mystash.txt b/stash_demo/mystash.txt
index 379d91b..339833b 100644
--- a/stash_demo/mystash.txt
+++ b/stash_demo/mystash.txt
@@ -1 +1,2 @@
 print('hello world')
+//changing a simple line and understanding it with the help of git diff
\ No newline at end of file

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ ^C

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git diff
diff --git a/stash_demo/mystash.txt b/stash_demo/mystash.txt
index 339833b..7e07a42 100644
--- a/stash_demo/mystash.txt
+++ b/stash_demo/mystash.txt
@@ -1,2 +1,3 @@
 print('hello world')
-//changing a simple line and understanding it with the help of git diff
\ No newline at end of file
+//changing a simple line and understanding it with the help of git diff^M
+this is second line of code
\ No newline at end of file

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ ^C

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git diff HEAD
diff --git a/stash_demo/mystash.txt b/stash_demo/mystash.txt
index 379d91b..7e07a42 100644
--- a/stash_demo/mystash.txt
+++ b/stash_demo/mystash.txt
@@ -1 +1,3 @@
 print('hello world')
+//changing a simple line and understanding it with the help of git diff^M
+this is second line of code
\ No newline at end of file

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ ^C

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   stash_demo/mystash.txt

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   stash_demo/mystash.txt


HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ ^C

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git restore --staged stash_demo/mystash.txt

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   stash_demo/mystash.txt

no changes added to commit (use "git add" and/or "git commit -a")

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ ^C

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git diff
diff --git a/stash_demo/mystash.txt b/stash_demo/mystash.txt
index 379d91b..7e07a42 100644
--- a/stash_demo/mystash.txt
+++ b/stash_demo/mystash.txt
@@ -1 +1,3 @@
 print('hello world')
+//changing a simple line and understanding it with the help of git diff^M
+this is second line of code
\ No newline at end of file

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ ^C

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git restore stash_demo/mystash
error: pathspec 'stash_demo/mystash' did not match any file(s) known to git

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git restore stash_demo/mystash.txt

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git diff

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ ^C

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   stash_demo/mystash.txt

no changes added to commit (use "git add" and/or "git commit -a")

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git add stash_demo/mystash.txt

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git commit -m "practice git reset"
[main 965740e] practice git reset
 1 file changed, 1 insertion(+)

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git log --oneline -3
965740e (HEAD -> main) practice git reset
2b6a50e (origin/main, origin/HEAD) Add files via upload
ad64402 (tag: v1.0) added feature work

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ ^C

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git reset --soft HEAD~1

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   stash_demo/mystash.txt


HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ ^C

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git log --oneline -3
2b6a50e (HEAD -> main, origin/main, origin/HEAD) Add files via upload
ad64402 (tag: v1.0) added feature work
e4b249d (tag: v2.0) Add files via upload

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ ^C

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git commit -m "Practice git mixed commit"
[main 4776e54] Practice git mixed commit
 1 file changed, 1 insertion(+)

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git log --oneline-3
fatal: unrecognized argument: --oneline-3

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git log --oneline -3
4776e54 (HEAD -> main) Practice git mixed commit
2b6a50e (origin/main, origin/HEAD) Add files via upload
ad64402 (tag: v1.0) added feature work

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ ^C

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git reset --mixed HEAD~1
Unstaged changes after reset:
M       stash_demo/mystash.txt

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   stash_demo/mystash.txt

no changes added to commit (use "git add" and/or "git commit -a")

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git diff
diff --git a/stash_demo/mystash.txt b/stash_demo/mystash.txt
index 379d91b..b19c178 100644
--- a/stash_demo/mystash.txt
+++ b/stash_demo/mystash.txt
@@ -1 +1,2 @@
 print('hello world')
+This is my rest practice
\ No newline at end of file

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ ^C

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git log --oneline -3
2b6a50e (HEAD -> main, origin/main, origin/HEAD) Add files via upload
ad64402 (tag: v1.0) added feature work
e4b249d (tag: v2.0) Add files via upload

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ ^C

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   stash_demo/mystash.txt

no changes added to commit (use "git add" and/or "git commit -a")

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git diff
diff --git a/stash_demo/mystash.txt b/stash_demo/mystash.txt
index 379d91b..c3c86f8 100644
--- a/stash_demo/mystash.txt
+++ b/stash_demo/mystash.txt
@@ -1 +1,3 @@
 print('hello world')
+This is my rest practice ^M
+this is my another session for hard reset.
\ No newline at end of file

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git reset --hard HEAD
HEAD is now at 2b6a50e Add files via upload

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git diff

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ ^C

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git reflog
2b6a50e (HEAD -> main, origin/main, origin/HEAD) HEAD@{0}: reset: moving to HEAD
2b6a50e (HEAD -> main, origin/main, origin/HEAD) HEAD@{1}: reset: moving to HEAD
~1
4776e54 HEAD@{2}: commit: Practice git mixed commit
2b6a50e (HEAD -> main, origin/main, origin/HEAD) HEAD@{3}: reset: moving to HEAD
~1
965740e HEAD@{4}: commit: practice git reset
2b6a50e (HEAD -> main, origin/main, origin/HEAD) HEAD@{5}: clone: from https://g
ithub.com/namancs2006-dev/git-program4.git

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ ^C

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git reset --hard 4776e54
HEAD is now at 4776e54 Practice git mixed commit

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git log --oneline -3
4776e54 (HEAD -> main) Practice git mixed commit
2b6a50e (origin/main, origin/HEAD) Add files via upload
ad64402 (tag: v1.0) added feature work

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git branch recovery

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git branch
* main
  recovery

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git log --oneline --decorate -3
4776e54 (HEAD -> main, recovery) Practice git mixed commit
2b6a50e (origin/main, origin/HEAD) Add files via upload
ad64402 (tag: v1.0) added feature work

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ ^C

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git blame stash_demo/mystash.txt
2b6a50e6 (namancs2006-dev 2026-01-03 12:40:00 +0530 1) print('hello world')
4776e548 (naman           2026-08-25 11:45:33 +0530 2) This is my rest practice

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ ^C

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ git log --oneline --decorate --all
4776e54 (HEAD -> main, recovery) Practice git mixed commit
2b6a50e (origin/main, origin/HEAD) Add files via upload
ad64402 (tag: v1.0) added feature work
e4b249d (tag: v2.0) Add files via upload

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ ^C

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ touch GIT_LEARNING.md

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$ ls
 GIT_LEARNING.md   Links/  'Screenshot (2).png'   feature.txt   stash_demo/

HI@DESKTOP-90KBJMH MINGW64 ~/git commands/git-program4 (main)
$
