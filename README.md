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
## Bundle 3
# Exercise 1

```
Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/service-redesign)
$ git checkout -b team-page
Switched to a new branch 'team-page'

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (team-page)
$ ls
README.md  about.html  home.html  services.html

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (team-page)
$ touch team.html

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (team-page)
$ git add .

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (team-page)
$ git commit -m "Team page initialization"
[team-page f1606d5] Team page initialization
 1 file changed, 10 insertions(+)
 create mode 100644 team.html

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (team-page)
$ git push
fatal: The current branch team-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin team-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (team-page)
$ git push --set-upstream origin team-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 413 bytes | 413.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'team-page' on GitHub by visiting:
remote:      https://github.com/Ntwalii/git-exercises/pull/new/team-page
remote:
To https://github.com/Ntwalii/git-exercises.git
 * [new branch]      team-page -> team-page
branch 'team-page' set up to track 'origin/team-page'.

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (team-page)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git branch ft/contact-page

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git checkout ft/team-page
error: pathspec 'ft/team-page' did not match any file(s) known to git

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git checkout ft/team-page
error: pathspec 'ft/team-page' did not match any file(s) known to git

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git checkout ft/team-page
error: pathspec 'ft/team-page' did not match any file(s) known to git

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git checkout ft/team-page
error: pathspec 'ft/team-page' did not match any file(s) known to git

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git branch
  dev
  ft/bundle-2
  ft/contact-page
  ft/service-redesign
* main
  team-page

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git checkout team-page
Switched to branch 'team-page'
Your branch is up to date with 'origin/team-page'.

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (team-page)
$ git branch -M "ft/team-page"

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/team-page)
$ git log
commit f1606d5181c8f2f5bd8b564ef596409419339a12 (HEAD -> ft/team-page, origin/team-page)
Author: ntwalii <ntwaliaubin@gmail.com>
Date:   Mon Apr 22 19:47:24 2024 +0200

    Team page initialization

commit e61dd7bb7811247b495df07d0ccd68e1167f1d9a (origin/ft/service-redesign, ft/service-redesign)
Merge: fae53c6 efdfa29
Author: ntwalii <ntwaliaubin@gmail.com>
Date:   Mon Apr 22 19:35:27 2024 +0200

    Merge complete

commit efdfa29bb0aa4ff2464dd9b4fac1fd1074bfcb0d (origin/main, main, ft/contact-page)
Merge: 3044aa5 a94eabb
Author: ntwalii <ntwaliaubin@gmail.com>
Date:   Mon Apr 22 19:30:24 2024 +0200

    Merge branch 'main' of https://github.com/Ntwalii/git-exercises

commit 3044aa581a021410eeb58522620b87ee295afbfc
Author: ntwalii <ntwaliaubin@gmail.com>
Date:   Mon Apr 22 19:30:05 2024 +0200

    Deleting services.html

commit a94eabb9f1942d540522f548450ed8d7a10e1b58
Merge: bcf88cb ccd3743
Author: Aubin Ntwali <119161688+Ntwalii@users.noreply.github.com>
Date:   Mon Apr 22 19:28:30 2024 +0200

    Merge pull request #4 from Ntwalii/ft/bundle-2

    Ft/bundle 2

commit fae53c6caa5770e800da46d322c82388a9b2e82b
Author: ntwalii <ntwaliaubin@gmail.com>
Date:   Mon Apr 22 19:27:51 2024 +0200

    New push

commit f758e796756e4ea27aee1113e25dd0795aea7621
Merge: 4db239d b69ad46
Author: ntwalii <ntwaliaubin@gmail.com>
Date:   Mon Apr 22 19:26:53 2024 +0200

    Merged

:
commit f1606d5181c8f2f5bd8b564ef596409419339a12 (HEAD -> ft/team-page, origin/team-page)
Author: ntwalii <ntwaliaubin@gmail.com>
Date:   Mon Apr 22 19:47:24 2024 +0200

    Team page initialization

commit e61dd7bb7811247b495df07d0ccd68e1167f1d9a (origin/ft/service-redesign, ft/service-redesign)
Merge: fae53c6 efdfa29
Author: ntwalii <ntwaliaubin@gmail.com>
Date:   Mon Apr 22 19:35:27 2024 +0200

    Merge complete

commit efdfa29bb0aa4ff2464dd9b4fac1fd1074bfcb0d (origin/main, main, ft/contact-page)
Merge: 3044aa5 a94eabb
Author: ntwalii <ntwaliaubin@gmail.com>
Date:   Mon Apr 22 19:30:24 2024 +0200

    Merge branch 'main' of https://github.com/Ntwalii/git-exercises

commit 3044aa581a021410eeb58522620b87ee295afbfc
Author: ntwalii <ntwaliaubin@gmail.com>
Date:   Mon Apr 22 19:30:05 2024 +0200

    Deleting services.html

commit a94eabb9f1942d540522f548450ed8d7a10e1b58
Merge: bcf88cb ccd3743
Author: Aubin Ntwali <119161688+Ntwalii@users.noreply.github.com>
Date:   Mon Apr 22 19:28:30 2024 +0200

    Merge pull request #4 from Ntwalii/ft/bundle-2

    Ft/bundle 2

commit fae53c6caa5770e800da46d322c82388a9b2e82b
Author: ntwalii <ntwaliaubin@gmail.com>
Date:   Mon Apr 22 19:27:51 2024 +0200

    New push

commit f758e796756e4ea27aee1113e25dd0795aea7621
Merge: 4db239d b69ad46
Author: ntwalii <ntwaliaubin@gmail.com>
Date:   Mon Apr 22 19:26:53 2024 +0200

    Merged

commit 4db239d0786f9787198401921dcd9cc2d46db698
...skipping...

commit e43c2bedc77ae52bee952f2e864842e3af4b5704
Merge: efacc7c 4e21ed2
Author: Gloria Umutoni <124312203+gloriaumutoni@users.noreply.github.com>
Date:   Mon Apr 22 17:29:42 2024 +0200

    Merge pull request #2 from Ntwalii/ft/service-redesign

    Services page edit

commit 4e21ed2529777cac0cd975de36c5271b8218bc23
Author: ntwalii <ntwaliaubin@gmail.com>
Date:   Mon Apr 22 17:15:56 2024 +0200

    Services page edit

commit efacc7ca109dc1dd684ad31d51a32e04602e8777
Author: ntwalii <ntwaliaubin@gmail.com>
Date:   Mon Apr 22 17:05:41 2024 +0200

    Changes to services.html

commit abfc6679f154960e9da1ac38f93b0eb1c8191a06
Merge: 13b170d 77db5bf
Author: IGIRANEZA Josue <88510074+IGIRANEZAJosue@users.noreply.github.com>
Date:   Mon Apr 22 16:59:23 2024 +0200

    Merge pull request #1 from Ntwalii/ft/bundle-2

    Created a services.html

commit 77db5bf47dbeac00888cb9012622e5aa87ee07bc
Author: ntwalii <ntwaliaubin@gmail.com>
Date:   Mon Apr 22 16:52:46 2024 +0200

    Created a services.html

commit 13b170d9e434a9eca42b3073aaea79ef6f03d551
Author: ntwalii <ntwaliaubin@gmail.com>
Date:   Mon Apr 22 16:31:53 2024 +0200

    Added 2 new pages; about and home page

commit 7ac1b36f92809b86f3b4706e829c759083d63473 (dev)
Author: ntwalii <ntwaliaubin@gmail.com>
Date:   Mon Apr 22 15:34:21 2024 +0200

    Created a README

commit e43c2bedc77ae52bee952f2e864842e3af4b5704
Merge: efacc7c 4e21ed2
Author: Gloria Umutoni <124312203+gloriaumutoni@users.noreply.github.com>
Date:   Mon Apr 22 17:29:42 2024 +0200

    Merge pull request #2 from Ntwalii/ft/service-redesign

    Services page edit

commit 4e21ed2529777cac0cd975de36c5271b8218bc23
Author: ntwalii <ntwaliaubin@gmail.com>
Date:   Mon Apr 22 17:15:56 2024 +0200

    Services page edit

commit efacc7ca109dc1dd684ad31d51a32e04602e8777
Author: ntwalii <ntwaliaubin@gmail.com>
Date:   Mon Apr 22 17:05:41 2024 +0200

    Changes to services.html

commit abfc6679f154960e9da1ac38f93b0eb1c8191a06
Merge: 13b170d 77db5bf
Author: IGIRANEZA Josue <88510074+IGIRANEZAJosue@users.noreply.github.com>
Date:   Mon Apr 22 16:59:23 2024 +0200

    Merge pull request #1 from Ntwalii/ft/bundle-2

    Created a services.html

commit 77db5bf47dbeac00888cb9012622e5aa87ee07bc
Author: ntwalii <ntwaliaubin@gmail.com>
Date:   Mon Apr 22 16:52:46 2024 +0200

    Created a services.html

commit 13b170d9e434a9eca42b3073aaea79ef6f03d551
Author: ntwalii <ntwaliaubin@gmail.com>
Date:   Mon Apr 22 16:31:53 2024 +0200

    Added 2 new pages; about and home page

commit 7ac1b36f92809b86f3b4706e829c759083d63473 (dev)
Author: ntwalii <ntwaliaubin@gmail.com>
Date:   Mon Apr 22 15:34:21 2024 +0200

    Created a README

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/team-page)
$ git checkout ft/contact-page
Switched to branch 'ft/contact-page'

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/contact-page)
$ git cherry-pick ft/team-page
[ft/contact-page 8128868] Team page initialization
 Date: Mon Apr 22 19:47:24 2024 +0200
 1 file changed, 10 insertions(+)
 create mode 100644 team.html

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/contact-page)
$ ls
README.md  about.html  home.html  team.html

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/contact-page)
$ touch contact.html

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/contact-page)
$ git add .

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/contact-page)
$ git commit -m "Contact page initialization"
[ft/contact-page ca639ca] Contact page initialization
 1 file changed, 10 insertions(+)
 create mode 100644 contact.html

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/contact-page)
$ git push
fatal: The current branch ft/contact-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/contact-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/contact-page)
$ git push --set-upstream origin ft/contact-page
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 4 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 673 bytes | 673.00 KiB/s, done.
Total 5 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
remote:
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/Ntwalii/git-exercises/pull/new/ft/contact-page
remote:
To https://github.com/Ntwalii/git-exercises.git
 * [new branch]      ft/contact-page -> ft/contact-page
branch 'ft/contact-page' set up to track 'origin/ft/contact-page'.

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/contact-page)
$ git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/faq-page)
$ touch faq.html

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/faq-page)
$ git add .

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/faq-page)
$ git commit -m "Faq page init"
[ft/faq-page ce84cf5] Faq page init
 1 file changed, 10 insertions(+)
 create mode 100644 faq.html

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/faq-page)
$ git push
fatal: The current branch ft/faq-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/faq-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/faq-page)
$ git push --set-upstream origin ft/faq-page
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 226 bytes | 226.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/Ntwalii/git-exercises/pull/new/ft/faq-page
remote:
To https://github.com/Ntwalii/git-exercises.git
 * [new branch]      ft/faq-page -> ft/faq-page
branch 'ft/faq-page' set up to track 'origin/ft/faq-page'.

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/faq-page)
$ git checkout -b ft/team-page
fatal: a branch named 'ft/team-page' already exists

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/faq-page)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/team-page'.

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/team-page)
$ git revert f1606d5181c8f2f5bd8b564ef596409419339a12
[ft/team-page 37d7e86] Revert "Team page initialization"
 1 file changed, 10 deletions(-)
 delete mode 100644 team.html

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/team-page)
$ git push
fatal: The upstream branch of your current branch does not match
the name of your current branch.  To push to the upstream branch
on the remote, use

    git push origin HEAD:team-page

To push to the branch of the same name on the remote, use

    git push origin HEAD

To choose either option permanently, see push.default in 'git help config'.

To avoid automatically configuring upstream branches when their name
doesn't match the local branch, see option 'simple' of branch.autoSetupMerge
in 'git help config'.


Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/team-page)
$ git push origin HEAD
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 254 bytes | 254.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/Ntwalii/git-exercises/pull/new/ft/team-page
remote:
To https://github.com/Ntwalii/git-exercises.git
 * [new branch]      HEAD -> ft/team-page

```
# Exercise 2

```
Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/contact-page)
$ git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/faq-page)
$ touch faq.html

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/faq-page)
$ git add .

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/faq-page)
$ git commit -m "Faq page init"
[ft/faq-page ce84cf5] Faq page init
 1 file changed, 10 insertions(+)
 create mode 100644 faq.html

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/faq-page)
$ git push
fatal: The current branch ft/faq-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/faq-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/faq-page)
$ git push --set-upstream origin ft/faq-page
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 226 bytes | 226.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/Ntwalii/git-exercises/pull/new/ft/faq-page
remote:
To https://github.com/Ntwalii/git-exercises.git
 * [new branch]      ft/faq-page -> ft/faq-page
branch 'ft/faq-page' set up to track 'origin/ft/faq-page'.

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/faq-page)
$ git checkout -b ft/team-page
fatal: a branch named 'ft/team-page' already exists

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/faq-page)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/team-page'.

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/team-page)
$ git revert f1606d5181c8f2f5bd8b564ef596409419339a12
[ft/team-page 37d7e86] Revert "Team page initialization"
 1 file changed, 10 deletions(-)
 delete mode 100644 team.html

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/team-page)
$ git push
fatal: The upstream branch of your current branch does not match
the name of your current branch.  To push to the upstream branch
on the remote, use

    git push origin HEAD:team-page

To push to the branch of the same name on the remote, use

    git push origin HEAD

To choose either option permanently, see push.default in 'git help config'.

To avoid automatically configuring upstream branches when their name
doesn't match the local branch, see option 'simple' of branch.autoSetupMerge
in 'git help config'.


Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/team-page)
$ git push origin HEAD
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 254 bytes | 254.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/Ntwalii/git-exercises/pull/new/ft/team-page
remote:
To https://github.com/Ntwalii/git-exercises.git
 * [new branch]      HEAD -> ft/team-page

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/team-page)
$ git chheckout -b ft/home-page-redesign
git: 'chheckout' is not a git command. See 'git --help'.

The most similar command is
        checkout

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/team-page)
$ git checkout -b ft/home-page-redesign
Switched to a new branch 'ft/home-page-redesign'

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/home-page-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git commit -a -m "New changes in main"
[main 839aceb] New changes in main
 1 file changed, 1 insertion(+)

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git push
To https://github.com/Ntwalii/git-exercises.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/Ntwalii/git-exercises.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git pull
remote: Enumerating objects: 1, done.
remote: Counting objects: 100% (1/1), done.
remote: Total 1 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (1/1), 903 bytes | 180.00 KiB/s, done.
From https://github.com/Ntwalii/git-exercises
   efdfa29..a4d569c  main       -> origin/main
Merge made by the 'ort' strategy.
 services.html | 10 ++++++++++
 1 file changed, 10 insertions(+)
 create mode 100644 services.html

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git push
Enumerating objects: 9, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 556 bytes | 556.00 KiB/s, done.
Total 5 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 2 local objects.
To https://github.com/Ntwalii/git-exercises.git
   a4d569c..f4ea61e  main -> main

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git checkout ft/home-page-redesign
Switched to branch 'ft/home-page-redesign'

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/home-page-redesign)
$ git rebase
There is no tracking information for the current branch.
Please specify which branch you want to rebase against.
See git-rebase(1) for details.

    git rebase '<branch>'

If you wish to set tracking information for this branch you can do so with:

    git branch --set-upstream-to=<remote>/<branch> ft/home-page-redesign


Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/home-page-redesign)
$ git rebase main
Successfully rebased and updated refs/heads/ft/home-page-redesign.

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/home-page-redesign)
$ git commit -a -m "Rebased"
[ft/home-page-redesign f1418e6] Rebased
 1 file changed, 1 insertion(+)

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/home-page-redesign)
$ git push
fatal: The current branch ft/home-page-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/home-page-redesign

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/home-page-redesign)
$ git push --set-upstream origin ft/home-page-redesign
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 4 threads
Compressing objects: 100% (7/7), done.
Writing objects: 100% (7/7), 909 bytes | 454.00 KiB/s, done.
Total 7 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/home-page-redesign' on GitHub by visiting:
remote:      https://github.com/Ntwalii/git-exercises/pull/new/ft/home-page-redesign
remote:
To https://github.com/Ntwalii/git-exercises.git
 * [new branch]      ft/home-page-redesign -> ft/home-page-redesign
branch 'ft/home-page-redesign' set up to track 'origin/ft/home-page-redesign'.

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/home-page-redesign)
```
# Bundle 4

##Exercise 1

```
Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (ft/home-page-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git remote add git-copy https://github.com/Ntwalii/Git-Exercise-repo-2.git

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git commit -a -m "Changes to homepage"
[main 0a71f10] Changes to homepage
 1 file changed, 1 insertion(+)

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 322 bytes | 322.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Ntwalii/git-exercises.git
   f4ea61e..0a71f10  main -> main

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$ git push git-copy
Enumerating objects: 69, done.
Counting objects: 100% (69/69), done.
Delta compression using up to 4 threads
Compressing objects: 100% (65/65), done.
Writing objects: 100% (69/69), 11.85 KiB | 1.08 MiB/s, done.
Total 69 (delta 32), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (32/32), done.
To https://github.com/Ntwalii/Git-Exercise-repo-2.git
 * [new branch]      main -> main

Ntwali@DESKTOP-CP6B3NG MINGW64 ~/Desktop/Personal/The Gym/Git Exercises (main)
$
```
