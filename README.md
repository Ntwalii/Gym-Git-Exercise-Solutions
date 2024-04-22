### Gym-Git-Exercise-Solutions

## Bundle 1

# Exercise 1

### Git Exercises

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



