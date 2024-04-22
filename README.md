### Gym-Git-Exercise-Solutions

## Bundle 1

# Exercise 1

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises
$ git init
Initialized empty Git repository in C:/Users/HP/Desktop/Personal/The Gym/Git Exercises/.git/

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (master)
$ git branch -M main

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ code README.md

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ ls
README.md

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md

nothing added to commit but untracked files present (use "git add" to track)

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git add .

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   README.md


Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git commit -m "Created a README"
[main (root-commit) 7ac1b36] Created a README
 1 file changed, 5 insertions(+)
 create mode 100644 README.md

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git remote add origin https://github.com/Ntwalii/git-exercises.git

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git status
On branch main
nothing to commit, working tree clean

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git push --set-upstream origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 254 bytes | 127.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Ntwalii/git-exercises.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git checkout -b dev
Switched to a new branch 'dev'

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (dev)
$ git checkout -b test
Switched to a new branch 'test'

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (test)
$ git checkout dev
Switched to branch 'dev'

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (dev)
$ git branch -d test
Deleted branch test (was 7ac1b36).

# Exercise 2

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ vi home.html

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ ls
README.md  home.html

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git add .

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git stash
Saved working directory and index state WIP on main: 7ac1b36 Created a README

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git add .

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git stash
Saved working directory and index state WIP on main: 7ac1b36 Created a README

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ ls
README.md  about.html

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git stash
No local changes to save

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git add .\
> .
fatal: ..: '..' is outside repository at 'C:/Users/HP/Desktop/Personal/The Gym/Git Exercises'

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git add .

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html


Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git stash
Saved working directory and index state WIP on main: 7ac1b36 Created a README

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ ls
README.md

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git add .

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git stash
Saved working directory and index state WIP on main: 7ac1b36 Created a README

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git stash pop
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped refs/stash@{0} (f5a3ab6f2ef68016c53774d6f8c4c50ef99f65c5)

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ ls
README.md  team.html

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git add .

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git stash
Saved working directory and index state WIP on main: 7ac1b36 Created a README

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git stash list
stash@{0}: WIP on main: 7ac1b36 Created a README
stash@{1}: WIP on main: 7ac1b36 Created a README
stash@{2}: WIP on main: 7ac1b36 Created a README
stash@{3}: WIP on main: 7ac1b36 Created a README

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git stash pop stash@{2}
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{2} (d3de1085a0384e2641279e86831b5ecb73e1c348)

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ ls
README.md  about.html

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git stash list
stash@{0}: WIP on main: 7ac1b36 Created a README
stash@{1}: WIP on main: 7ac1b36 Created a README
stash@{2}: WIP on main: 7ac1b36 Created a README

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git stash pop stash@{2}
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Dropped stash@{2} (e315586c8e356c462a4cbc5d882c8308884bb684)

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ ls
README.md  about.html  home.html

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git commit -m "Added 2 new pages; about and home page"
[main 13b170d] Added 2 new pages; about and home page
 2 files changed, 20 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 532 bytes | 532.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/Ntwalii/git-exercises.git
   7ac1b36..13b170d  main -> main

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git stash pop
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped refs/stash@{0} (175dc6e8560be63689b4cdc34985cffa0c09a067)

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git reset --help

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git reset --hard
HEAD is now at 13b170d Added 2 new pages; about and home page



