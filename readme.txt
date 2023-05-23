kevin@kevinlaptop MINGW64 ~/desktop/git (master)
$ ll
total 10195
-rw-r--r-- 1 kevin 197609       61 May 18 11:40 1.py
-rw-r--r-- 1 kevin 197609       21 May 17 16:22 2.py
-rw-r--r-- 1 kevin 197609       56 May 18 10:58 boss.py
drwxr-xr-x 1 kevin 197609        0 May 18 10:36 dev/
-rw-r--r-- 1 kevin 197609        0 May 17 16:22 etl.sql
-rw-r--r-- 1 kevin 197609 10434042 May 18 11:57 flights.csv
-rw-r--r-- 1 kevin 197609        0 May 20 11:24 readme.txt

kevin@kevinlaptop MINGW64 ~/desktop/git (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   readme.txt


kevin@kevinlaptop MINGW64 ~/desktop/git (master)
$ git restore --staged readme.txt

kevin@kevinlaptop MINGW64 ~/desktop/git (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        readme.txt

nothing added to commit but untracked files present (use "git add" to track)

kevin@kevinlaptop MINGW64 ~/desktop/git (master)
$ ll
total 10195
-rw-r--r-- 1 kevin 197609       61 May 18 11:40 1.py
-rw-r--r-- 1 kevin 197609       21 May 17 16:22 2.py
-rw-r--r-- 1 kevin 197609       56 May 18 10:58 boss.py
drwxr-xr-x 1 kevin 197609        0 May 18 10:36 dev/
-rw-r--r-- 1 kevin 197609        0 May 17 16:22 etl.sql
-rw-r--r-- 1 kevin 197609 10434042 May 18 11:57 flights.csv
-rw-r--r-- 1 kevin 197609        0 May 20 11:24 readme.txt

kevin@kevinlaptop MINGW64 ~/desktop/git (master)
$ git add A
fatal: pathspec 'A' did not match any files

kevin@kevinlaptop MINGW64 ~/desktop/git (master)
$ git add -A

kevin@kevinlaptop MINGW64 ~/desktop/git (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   readme.txt


kevin@kevinlaptop MINGW64 ~/desktop/git (master)
$
