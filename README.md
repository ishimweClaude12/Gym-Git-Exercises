#Git Exercises Solutions
#Bundle 1

## Exercise 1

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises  
$ git init
Initialized empty Git repository in C:/Users/User/Desktop/TheGym/Git-Exercises/.git/

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (master)
$ git branch -M main

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)$ git add home.html

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)$ git commit -m "Add Home.html"
[main (root-commit) 1c04b6c] Add Home.html
1 file changed, 10 insertions(+)
create mode 100644 home.html

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)$ git add README.md

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)$ git commit -m " Add README.md"
[main 0fd719a] Add README.md
1 file changed, 0 insertions(+), 0 deletions(-)
create mode 100644 README.md

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)$ git status
On branch main
nothing to commit, working tree clean

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)$ git remote add origin https://github.com/ishimweClaude12/Gym-Git-Exercises.git

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)$ git push -u origin main
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 12 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (6/6), 650 bytes | 650.00 KiB/s, done.  
Total 6 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/ishimweClaude12/Gym-Git-Exercises.git

- [new branch] main -> main
  branch 'main' set up to track 'origin/main'.

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)$ git checkout -b dev
Switched to a new branch 'dev'

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (dev)
$ git checkout -b test
Switched to a new branch 'test'

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (test)$ git checkout dev
Switched to branch 'dev'

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (dev)
$ git branch -D test
Deleted branch test (was 0fd719a).

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (dev)
$

# Exercise 2

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)ises (main)
$ git add home.html

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git stash list
stash@{0}: WIP on main: 557abba Add Home.html

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git stash
Saved working directory and index state WIP on main: 557abba Add Home.html

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git add about.html

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git stash
Saved working directory and index state WIP on main: 557abba Add Home.html

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git add team.html

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git stash
Saved working directory and index state WIP on main: 557abba Add Home.html

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git stash list
stash@{0}: WIP on main: 557abba Add Home.html
stash@{1}: WIP on main: 557abba Add Home.html
stash@{2}: WIP on main: 557abba Add Home.html
stash@{3}: WIP on main: 557abba Add Home.html

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git stash pop stash@{2}
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
(use "git add <file>..." to update what will be committed)
(use "git restore <file>..." to discard changes in working directory)
modified: home.html

Untracked files:
(use "git add <file>..." to include in what will be committed)
about.html

no changes added to commit (use "git add" and/or "git commit -a")
Dropped stash@{2} (707d5e5575b84ce3cd7f27613342529c249e7c45)

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git stash pop stash@{1}
error: The following untracked working tree files would be overwritten by merge:
about.html
Please move or remove them before you merge.
Aborting
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
(use "git add <file>..." to update what will be committed)
(use "git restore <file>..." to discard changes in working directory)
modified: home.html

Untracked files:
(use "git add <file>..." to include in what will be committed)
about.html

no changes added to commit (use "git add" and/or "git commit -a")
The stash entry is kept in case you need it again.

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git commit -m "Commit Current Changes"
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
(use "git add <file>..." to update what will be committed)
(use "git restore <file>..." to discard changes in working directory)
modified: home.html

Untracked files:
(use "git add <file>..." to include in what will be committed)
about.html

no changes added to commit (use "git add" and/or "git commit -a")

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git add .

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git commit -m "Commit Current Changes"
[main 79b96ee] Commit Current Changes
2 files changed, 14 insertions(+)
create mode 100644 about.html

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git push
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 12 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 579 bytes | 579.00 KiB/s,
done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0  
remote: Resolving deltas: 100% (1/1), completed with 1
local object.
To https://github.com/ishimweClaude12/Gym-Git-Exercises.git
557abba..79b96ee main -> main

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git stash list
stash@{0}: WIP on main: 557abba Add Home.html
stash@{1}: WIP on main: 557abba Add Home.html
stash@{2}: WIP on main: 557abba Add Home.html

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git stash pop stash@{2}
Auto-merging about.html
CONFLICT (add/add): Merge conflict in about.html  
Auto-merging home.html
CONFLICT (content): Merge conflict in home.html  
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
(use "git restore --staged <file>..." to unstage)  
 modified: README.md
new file: team.html

Unmerged paths:
(use "git restore --staged <file>..." to unstage)  
 (use "git add <file>..." to mark resolution)
both added: about.html
both modified: home.html

The stash entry is kept in case you need it again.

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
(use "git restore --staged <file>..." to unstage)  
 modified: README.md
new file: team.html

Unmerged paths:
(use "git restore --staged <file>..." to unstage)  
 (use "git add <file>..." to mark resolution)
both added: about.html
both modified: home.html

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git add .

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
(use "git restore --staged <file>..." to unstage)  
 modified: README.md
modified: about.html
modified: home.html
new file: team.html

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git restore team.html

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
(use "git restore --staged <file>..." to unstage)  
 modified: README.md
modified: about.html
modified: home.html
new file: team.html

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git restore --stage team.html

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
(use "git restore --staged <file>..." to unstage)  
 modified: README.md
modified: about.html
modified: home.html

Untracked files:
(use "git add <file>..." to include in what will be committed)
team.html

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git stash list
stash@{0}: WIP on main: 557abba Add Home.html
stash@{1}: WIP on main: 557abba Add Home.html
stash@{2}: WIP on main: 557abba Add Home.html

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git stash
Saved working directory and index state WIP on main: 79b96ee Commit Current Changes

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git checkout dev
Switched to branch 'dev'
Your branch is up to date with 'origin/dev'.

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (dev)
$ git stash list
stash@{0}: WIP on main: 79b96ee Commit Current Changes
stash@{1}: WIP on main: 557abba Add Home.html
stash@{2}: WIP on main: 557abba Add Home.html
stash@{3}: WIP on main: 557abba Add Home.html

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (dev)
$ git stash pop stash@{3}
error: The following untracked working tree files would be overwritten by merge:
team.html
Please move or remove them before you merge.
Aborting
On branch dev
Your branch is up to date with 'origin/dev'.

Untracked files:
(use "git add <file>..." to include in what will be committed)
team.html

nothing added to commit but untracked files present (use "git add" to track)
The stash entry is kept in case you need it again.

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (dev)
$ git switch main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
(use "git add <file>..." to include in what will be committed)
team.html

nothing added to commit but untracked files present (use "git add" to track)

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git add team.html

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git stash
Saved working directory and index state WIP on main: 79b96ee Commit Current Changes

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git checkout dev
Switched to branch 'dev'
Your branch is up to date with 'origin/dev'.

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (dev)
$ git stash pop stash@{3}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
(use "git restore --staged <file>..." to unstage)  
 new file: about.html

Dropped stash@{3} (104ccea43bec58dac107edfa4467818ecd00a9c3)

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (dev)
$ git switch main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$

# Bundle 2

## Exercise 1

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git branch
dev

- main

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git checkout -b ft/bundle-2
Switched to a new branch 'ft/bundle-2'

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/bundle-2)
$ git status
On branch ft/bundle-2
Changes not staged for commit:
(use "git add <file>..." to update what will be committed)
(use "git restore <file>..." to discard changes in working directory)
modified: README.md

Untracked files:
(use "git add <file>..." to include in what will be committed)
services.html

no changes added to commit (use "git add" and/or "git commit -a")

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/bundle-2)
$ git add services.html

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/bundle-2)
$ git commit -m "Add Services page"
[ft/bundle-2 0a23864] Add Services page
1 file changed, 10 insertions(+)
create mode 100644 services.html

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/bundle-2)
$ git push
fatal: The current branch ft/bundle-2 has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/bundle-2

To have this happen automatically for branches without
a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/bundle-2)
$ git push --set-upstream origin ft/bundle-2
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 455 bytes | 455.00 KiB/s,
done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0  
remote: Resolving deltas: 100% (1/1), completed with 1
local object.
remote:
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote: https://github.com/ishimweClaude12/Gym-Git-Exercises/pull/new/ft/bundle-2
remote:
To https://github.com/ishimweClaude12/Gym-Git-Exercises.git

- [new branch] ft/bundle-2 -> ft/bundle-2  
  branch 'ft/bundle-2' set up to track 'origin/ft/bundle-2'.

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/bundle-2)
$

## Exercise 2
