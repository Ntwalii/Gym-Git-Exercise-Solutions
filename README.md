### Gym-Git-Exercise-Solutions

## Bundle 1

# Exercise 1
```
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
```
# Exercise 2
```
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
```

## Bundle 2
# Exercise 1

```
Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git checkout -b ft/bundle-2
Switched to a new branch 'ft/bundle-2'

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/bundle-2)
$ touch services.html

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/bundle-2)
$ git add .

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/bundle-2)
$ git commit -m "Services pagge created"
[ft/bundle-2 36df28f] Services pagge created
 1 file changed, 10 deletions(-)

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/bundle-2)
$ git push
fatal: The current branch ft/bundle-2 has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/bundle-2

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/bundle-2)
$ git push --set-upstream origin ft/bundle-2
Enumerating objects: 11, done.
Counting objects: 100% (11/11), done.
Delta compression using up to 4 threads
Compressing objects: 100% (8/8), done.
Writing objects: 100% (9/9), 840 bytes | 420.00 KiB/s, done.
Total 9 (delta 5), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (5/5), completed with 2 local objects.
To https://github.com/Ntwalii/git-exercises.git
   77db5bf..36df28f  ft/bundle-2 -> ft/bundle-2
branch 'ft/bundle-2' set up to track 'origin/ft/bundle-2'.

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/bundle-2)
$
```
# Exercise 2
```
$ git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/service-redesign)
$ git add .

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/service-redesign)
$ git commit -m "Services.html edit"
[ft/service-redesign 3e0dd1a] Services.html edit
 1 file changed, 10 insertions(+), 1 deletion(-)

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/service-redesign)
$ git push
fatal: The current branch ft/service-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/service-redesign

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/service-redesign)
$ git push --set-upstream origin ft/service-redesign
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 280 bytes | 280.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Ntwalii/git-exercises.git
   f758e79..fae53c6  ft/service-redesign -> ft/service-redesign
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/service-redesign)
$ git diff main
diff --git a/services.html b/services.html
new file mode 100644
index 0000000..b2a1cb7
--- /dev/null
+++ b/services.html
@@ -0,0 +1,10 @@
+<html lang="en">
+<head>
+    <meta charset="UTF-8">
+    <meta name="viewport" content="width=device-width, initial-scale=1.0">
+    <title>Document</title>
+</head>
+<body>
+    <h1>Initial change 2.1</h1>
+</body>
+</html>
\ No newline at end of file

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/service-redesign)
$ git merge ft/service-redesign
Already up to date.

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/service-redesign)
$ git merge main
CONFLICT (modify/delete): services.html deleted in main and modified in HEAD.  Version HEAD of services.html left in tree.
Automatic merge failed; fix conflicts and then commit the result.

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/service-redesign|MERGING)
$ git diff main
diff --git a/services.html b/services.html
new file mode 100644
index 0000000..b2a1cb7
--- /dev/null
+++ b/services.html
@@ -0,0 +1,10 @@
+<html lang="en">
+<head>
+    <meta charset="UTF-8">
+    <meta name="viewport" content="width=device-width, initial-scale=1.0">
+    <title>Document</title>
+</head>
+<body>
+    <h1>Initial change 2.1</h1>
+</body>
+</html>
\ No newline at end of file

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/service-redesign|MERGING)
$ git merge main
fatal: You have not concluded your merge (MERGE_HEAD exists).
Please, commit your changes before you merge.

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/service-redesign|MERGING)
$ git commit "Merge complete"
fatal: cannot do a partial commit during a merge.

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/service-redesign|MERGING)
$ git commit -m "Merge complete"
[ft/service-redesign e61dd7b] Merge complete

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/service-redesign)
$ git push
Enumerating objects: 1, done.
Counting objects: 100% (1/1), done.
Writing objects: 100% (1/1), 213 bytes | 213.00 KiB/s, done.
Total 1 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Ntwalii/git-exercises.git
   fae53c6..e61dd7b  ft/service-redesign -> ft/service-redesign

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/service-redesign)
$
```

