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
<<<<<<< HEAD
=======

>>>>>>> 35a0a5a048c77117186fff92e84b1cfbc736364a
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
M       README.md
<<<<<<< HEAD



=======
```
>>>>>>> 35a0a5a048c77117186fff92e84b1cfbc736364a
