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