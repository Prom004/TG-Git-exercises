# EXERCISES

## BUNDLE 1

### Exercises 1

```
$ mkdir GYM-Exercises

Promise@DESKTOP-54LQL0B MINGW64 ~ (master)
$ git init
Reinitialized existing Git repository in C:/Users/Promise/.git/

Promise@DESKTOP-54LQL0B MINGW64 ~ (master)
$ git branch

Promise@DESKTOP-54LQL0B MINGW64 ~ (master)
$ git branch -M main

Promise@DESKTOP-54LQL0B MINGW64 ~ (main)
$ git add README.md
warning: in the working copy of 'README.md', LF will be replaced by CRLF the next time Git touches it


Promise@DESKTOP-54LQL0B MINGW64 ~ (main)
$ git remote add origin https://github.com/Prom004/TG-Git-exercises.git



Promise@DESKTOP-54LQL0B MINGW64 ~ (main)
$ git commit -a -m "Updated ReadMe.md"
[main (root-commit) 7d44663] Updated ReadMe.md
 1 file changed, 6 insertions(+)
 create mode 100644 README.md



Promise@DESKTOP-54LQL0B MINGW64 ~ (main)
$ git push -u origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 260 bytes | 65.00 KiB/s, done. 
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/Prom004/TG-Git-exercises.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

Promise@DESKTOP-54LQL0B MINGW64 ~ (main)
$ git branch dev

Promise@DESKTOP-54LQL0B MINGW64 ~ (main)
$ git branch
  dev
* main

Promise@DESKTOP-54LQL0B MINGW64 ~ (main)
$ git checkout dev
Switched to branch 'dev'

Promise@DESKTOP-54LQL0B MINGW64 ~ (dev)
$ git branch test

Promise@DESKTOP-54LQL0B MINGW64 ~ (dev)
$ git branch -d test
Deleted branch test (was 7d44663).

Promise@DESKTOP-54LQL0B MINGW64 ~ (dev)
$ git checkout main
M       README.md
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

Promise@DESKTOP-54LQL0B MINGW64 ~ (main)
$ git push
Everything up-to-date

Promise@DESKTOP-54LQL0B MINGW64 ~ (dev)
$ git branch
* dev
  main
```
### EXERCISES 2

```bash
Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (main)
$ git add home.html

Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (main)
$ git stash
Saved working directory and index state WIP on mainll be replaced by CRLF : 6602c44 Updated ReadMe
                                                   : 6602c44 Updated ReadM

Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises 
(main)
$ git add about.html
warning: in the working copy of 'about.html', LF will be replaced by CRLF the next time Git touches it
Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises 
(main)
$ git stash
Saved working directory and index state WIP on main: 1b0fbe8 trial


Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (main)
$ git stash list
stash@{0}: WIP on main: 1b0fbe8 trial
stash@{1}: WIP on main: 1b0fbe8 trial
stash@{2}: WIP on main: 1b0fbe8 trial

Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (main)
$ git stash pop stash@{1}
On branch main
Your branch is ahead of 'origin/main' by 3 commits.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html

Dropped stash@{1} (712269913e961e53bf029ac9a1145914e7e2c909)

Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (main)
$ git stash pop stash@{1}
On branch main
Your branch is ahead of 'origin/main' by 3 commits.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Dropped stash@{1} (6c2ce713ac61621568c86d58302815d06d82563a)

Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (main)
$ git commit -m "Stash usage"
[main ae142bd] Stash usage
 2 files changed, 23 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html

Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (main)
$ git stash pop
On branch main
Your branch is ahead of 'origin/main' by 4 commits.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

Dropped refs/stash@{0} (6e6c53928307722b9bc71be2827905f90029b82f)

Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (main)
$ git reset
Unstaged changes after reset:
M       README.m


## BUNDLE 2

### Exercise 1
```bash
Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (main)
$ git branch ft/bundle-2
```
```bash
Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (main)
$ git branch
  dev
  ft/bundle-2
* main
```

```bash
Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (main)
$ git checkout ft/bundle-2
M       README.md
Switched to branch 'ft/bundle-2'
```

```bash
Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (ft/bundle-2)
$ git add services.html
warning: in the working copy of 'services.html', LF will be replaced by CRLF the next time Git touches it
```

```bash
Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (ft/bundle-2)
$ git status
On branch ft/bundle-2
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   services.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)  
        modified:   README.md
```

```bash
Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (ft/bundle-2)
$ git commit -m "New files added"
[ft/bundle-2 9fa511a] New files added
 1 file changed, 89 insertions(+)
 create mode 100644 services.html
```

```bash
Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (ft/bundle-2)
$ git push
fatal: The current branch ft/bundle-2 has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/bundle-2

To have this happen automatically for branches without a tracking        
upstream, see 'push.autoSetupRemote' in 'git help config'.
```

```bash
Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (ft/bundle-2)
$ git push --set-upstream origin ft/bundle-2
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 8 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 1.61 KiB | 411.00 KiB/s, done.
Total 6 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 1 local object.     
remote: This repository moved. Please use the new location:
remote:   https://github.com/Prom004/TG-Git-exercises.git
remote:
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:   
remote:      https://github.com/Prom004/TG-Git-exercises/pull/new/ft/bundle-2
remote:
To https://github.com/Prom004/TG-Git-Exercises.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
branch 'ft/bundle-2' set up to track 'origin/ft/bundle-2'.
```


### EXERCISES 2
```bash
Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (main)
$ git checkout main
M       README.md
Already on 'main'
Your branch is up to date with 'origin/main'.
```
```bash
Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (main)
$ git branch ft/service-redesign
```

```bash
Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (main)
$ git commit -a -m "Updates on the new branch"
[main 1fa6567] Updates on the new branch
 2 files changed, 5 insertions(+), 1 deletion(-)
```

```bash
Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (main)
$ git push
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 482 bytes | 120.00 KiB/s, done.
Total 4 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.        
remote: This repository moved. Please use the new location:
remote:   https://github.com/Prom004/TG-Git-exercises.git
To https://github.com/Prom004/TG-Git-Exercises.git
   326eaae..1fa6567  main -> main
```

```bash
Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (main)
$ git branch
  dev
  ft/bundle-2
  ft/service-redesign
* main
```

```bash
Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (main)
$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
```

```bash
Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (ft/service-redesign)     
$ git add services.html
```

```bash
Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (ft/service-redesign)     
$ git commit -a -m "Updates"
[ft/service-redesign 00be4f8] Updates
 1 file changed, 1 insertion(+), 1 deletion(-)
```

```bash
Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (ft/service-redesign)     
$ git push --set-upstream origin ft/service-redesign
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 294 bytes | 147.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.        
remote: This repository moved. Please use the new location:
remote:   https://github.com/Prom004/TG-Git-exercises.git
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/Prom004/TG-Git-exercises/pull/new/ft/service-redesign
remote:
To https://github.com/Prom004/TG-Git-Exercises.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.
```

```bash
Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (ft/service-redesign)     
$ git checkout main
Switched to branch 'main'
Your branch is behind 'origin/main' by 2 commits, and can be fast-forwarded. 
  (use "git pull" to update your local branch)
```

```bash
Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (main)
$ git add services.html
```

```bash
Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (main)
$ git add .
warning: in the working copy of '.vscode/settings.json', LF will be replaced 
by CRLF the next time Git touches it
```

```bash
Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (main)
$ git commit -a -m "Updated Services"
[main 60bf3e7] Updated Services
 1 file changed, 3 insertions(+)
 create mode 100644 .vscode/settings.json
```

```bash
Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (main)
$ git push origin main
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (6/6), 639 bytes | 639.00 KiB/s, done.
Total 6 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 1 local object.
remote: This repository moved. Please use the new location:
remote:   https://github.com/Prom004/TG-Git-exercises.git
To https://github.com/Prom004/TG-Git-Exercises.git
   1522dda..f73955a  main -> main
```

```bash
Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (main)
$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.
```

```bash
Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (ft/service-redesign)     
$ git diff main
diff --git a/.vscode/settings.json b/.vscode/settings.json
deleted file mode 100644
index 6f3a291..0000000
--- a/.vscode/settings.json
+++ /dev/null
@@ -1,3 +0,0 @@
-{
-    "liveServer.settings.port": 5501
```

```bash
Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (ft/service-redesign)     
$ git checkout ft/service-redesign
Already on 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.
```

```bash
Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (ft/service-redesign)     
$ git merge main
Updating 00be4f8..f73955a
Fast-forward
 .vscode/settings.json | 3 +++
 README.md             | 4 ++++
 services.html         | 2 +-
 3 files changed, 8 insertions(+), 1 deletion(-)
 create mode 100644 .vscode/settings.json
```

```bash
Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (ft/service-redesign)     
$ git push origin ft/service-redesign
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote: This repository moved. Please use the new location:
remote:   https://github.com/Prom004/TG-Git-exercises.git
To https://github.com/Prom004/TG-Git-Exercises.git
   00be4f8..f73955a  ft/service-redesign -> ft/service-redesign
```

