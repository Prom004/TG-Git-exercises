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

```
Promise@DESKTOP-54LQL0B MIN~/TG-Giises (main)
ain)
$ git add home.html
warning: in the working copy of 'home.html', LF will be replaced by CRLF the next time Git touches it

Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (main)
Saved working directory and index state WIP on main: 497c7e2 Initial commit                 F will be replaced by C

Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exerc main: 497c7e2 Initial ises (main)
$ git add home.html
fatal: pathspec 'home.html' did not match any ises (main)
file


Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (main)
$ git add about.html
warning: in the working copy of 'about.html', 
LF will be replaced by CRLF the next time Git 
touches it

Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (main)
$ git stash
Saved working directory and index state WIP on main: 497c7e2 Initial commit


Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (main)
$ git add team.html
warning: in the working copy of 'team.html', LF will be replaced by CRLF the next time Git touches it

Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (main)
$ git stash
Saved working directory and index state WIP on main: 497c7e2 Initial commit

Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (main)
$ git stash list
stash@{0}: WIP on main: 497c7e2 Initial commitstash@{1}: WIP on main: 497c7e2 Initial commitstash@{2}: WIP on main: 497c7e2 Initial commit
Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (main)
$ git stash pop stash@{1}
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{1} (37f6d78d0b8619143303c098d3f54389747bba34)

Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (main)
$ git stash pop stash@{1}
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Dropped stash@{1} (b89c61c42594138f5a12860bbc15313ab6d2b92d)

Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (main)
$ git commit -m "use of stash"
[main 8d90b35] use of stash
 2 files changed, 29 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html

Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (main)
$ git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 927 bytes | 231.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/Prom004/TG-Git-exercises.git
   497c7e2..8d90b35  main -> main

Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (main)
$ git stash pop
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped refs/stash@{0} (2a061a6d9d7ac9c6dfdf4ce05fffc1f7e875d54d)

Promise@DESKTOP-54LQL0B MINGW64 ~/TG-Git-exercises (main)
$ git reset
```