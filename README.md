# README
## Student Task Tracker
A simple project to track daily tasks and student assignments.

kevin@KevinNguyenPC UCRT64 ~
$ mkdir student-task-tracker

kevin@KevinNguyenPC UCRT64 ~
$ cd student-task-tracker

kevin@KevinNguyenPC UCRT64 ~/student-task-tracker
$ git init
Initialized empty Git repository in C:/Users/kevin/student-task-tracker/.git/

kevin@KevinNguyenPC UCRT64 ~/student-task-tracker (main)
$ git config --global user.name "Kevin Nguyen"

kevin@KevinNguyenPC UCRT64 ~/student-task-tracker (main)
$ git config --global user.email "kevintrongkhangnguyen@gmail.com"

kevin@KevinNguyenPC UCRT64 ~/student-task-tracker (main)
$ git list
git: 'list' is not a git command. See 'git --help'.

The most similar commands are
        bisect
        rev-list

kevin@KevinNguyenPC UCRT64 ~/student-task-tracker (main)
$ git config --global core.editor "code --wait"

kevin@KevinNguyenPC UCRT64 ~/student-task-tracker (main)
$ git config --list
diff.astextplain.textconv=astextplain
filter.lfs.clean=git-lfs clean -- %f
filter.lfs.smudge=git-lfs smudge -- %f
filter.lfs.process=git-lfs filter-process
filter.lfs.required=true
http.sslbackend=schannel
core.autocrlf=true
core.fscache=true
core.symlinks=false
pull.rebase=false
credential.helper=manager
credential.https://dev.azure.com.usehttppath=true
init.defaultbranch=master
user.name=Kevin Nguyen
user.email=kevintrongkhangnguyen@gmail.com
init.defaultbranch=main
core.editor=code --wait
core.repositoryformatversion=0
core.filemode=false
core.bare=false
core.logallrefupdates=true
core.symlinks=false
core.ignorecase=true

kevin@KevinNguyenPC UCRT64 ~/student-task-tracker (main)
$ ls -a
./  ../  .git/

kevin@KevinNguyenPC UCRT64 ~/student-task-tracker (main)
$ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md

nothing added to commit but untracked files present (use "git add" to track)

kevin@KevinNguyenPC UCRT64 ~/student-task-tracker (main)
$ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md
        tasks.txt

nothing added to commit but untracked files present (use "git add" to track)

kevin@KevinNguyenPC UCRT64 ~/student-task-tracker (main)
$ git add README.md tasks.txt

kevin@KevinNguyenPC UCRT64 ~/student-task-tracker (main)
$ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   README.md
        new file:   tasks.txt


kevin@KevinNguyenPC UCRT64 ~/student-task-tracker (main)
$ git commit -m "Add project documentation and task list"
[main (root-commit) 828de93] Add project documentation and task list
 2 files changed, 8 insertions(+)
 create mode 100644 README.md
 create mode 100644 tasks.txt

kevin@KevinNguyenPC UCRT64 ~/student-task-tracker (main)
$ git status
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   tasks.txt

no changes added to commit (use "git add" and/or "git commit -a")

kevin@KevinNguyenPC UCRT64 ~/student-task-tracker (main)
$ git add tasks.txt

kevin@KevinNguyenPC UCRT64 ~/student-task-tracker (main)
$ git commit -m "Update task list with an extra task"
[main 25894b5] Update task list with an extra task
 1 file changed, 2 insertions(+), 1 deletion(-)

kevin@KevinNguyenPC UCRT64 ~/student-task-tracker (main)
$ git log --oneline
25894b5 (HEAD -> main) Update task list with an extra task
828de93 Add project documentation and task list

kevin@KevinNguyenPC UCRT64 ~/student-task-tracker (main)
$ touch .gitignore

kevin@KevinNguyenPC UCRT64 ~/student-task-tracker (main)
$ code .gitignore

kevin@KevinNguyenPC UCRT64 ~/student-task-tracker (main)
$ touch app.log .env

kevin@KevinNguyenPC UCRT64 ~/student-task-tracker (main)
$ git add .gitignore

kevin@KevinNguyenPC UCRT64 ~/student-task-tracker (main)
$ git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   .gitignore

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .env
        app.log


kevin@KevinNguyenPC UCRT64 ~/student-task-tracker (main)
$ git commit -m "Add rules for ignored files"
[main 988a4d4] Add rules for ignored files
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 .gitignore

kevin@KevinNguyenPC UCRT64 ~/student-task-tracker (main)
$ git status
On branch main
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .env
        app.log

nothing added to commit but untracked files present (use "git add" to track)

kevin@KevinNguyenPC UCRT64 ~/student-task-tracker (main)
$ git remote add origin https://github.com/TRNG-2493/Kevin-Nguyen.git
kevin@KevinNguyenPC UCRT64 ~/student-task-tracker (main)
$ git pull origin main --allow-unrelated-histories
From https://github.com/TRNG-2493/Kevin-Nguyen
 * branch            main       -> FETCH_HEAD
Merge made by the 'ort' strategy.

kevin@KevinNguyenPC UCRT64 ~/student-task-tracker (main)
$ git push -u origin main
Enumerating objects: 12, done.
Counting objects: 100% (12/12), done.
Delta compression using up to 16 threads
Compressing objects: 100% (10/10), done.
Writing objects: 100% (11/11), 1.18 KiB | 1.18 MiB/s, done.
Total 11 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), done.
To https://github.com/TRNG-2493/Kevin-Nguyen.git
   9820659..0e1a441  main -> main
branch 'main' set up to track 'origin/main'.

kevin@KevinNguyenPC UCRT64 ~/student-task-tracker (main)
$ git clone https://github.com/TRNG-2493/Kevin-Nguyen.git student-task-tracker-copy
Cloning into 'student-task-tracker-copy'...
remote: Enumerating objects: 24, done.
remote: Counting objects: 100% (24/24), done.
remote: Compressing objects: 100% (15/15), done.
remote: Total 24 (delta 2), reused 11 (delta 2), pack-reused 0 (from 0)
Receiving objects: 100% (24/24), done.
Resolving deltas: 100% (2/2), done.

kevin@KevinNguyenPC UCRT64 ~/student-task-tracker (main)
$ rm -rf student-task-tracker-copy

kevin@KevinNguyenPC UCRT64 ~/student-task-tracker (main)
$ cd ..

kevin@KevinNguyenPC UCRT64 ~
$ git clone https://github.com/TRNG-2493/Kevin-Nguyen.git student-task-tracker-copy
Cloning into 'student-task-tracker-copy'...
remote: Enumerating objects: 24, done.
remote: Counting objects: 100% (24/24), done.
remote: Compressing objects: 100% (15/15), done.
remote: Total 24 (delta 2), reused 11 (delta 2), pack-reused 0 (from 0)
Receiving objects: 100% (24/24), done.
Resolving deltas: 100% (2/2), done.

kevin@KevinNguyenPC UCRT64 ~
$ cd student-task-tracker-copy
