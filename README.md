# Git Exercises Solutions

# Bundle 1

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

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/bundle-2)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git pull
Already up to date.

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git checkout -b ft/service-redesign
fatal: a branch named 'ft/service-redesign' already exists

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/service-redesign)
$ git add .

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/service-redesign)
$ git commit -m "Add services page"
[ft/service-redesign 7e61bc1] Add services page
1 file changed, 10 insertions(+)
create mode 100644 services.html

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/service-redesign)
$ git push
fatal: The current branch ft/service-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/service-redesign

To have this happen automatically for branches without
a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/service-redesign)
$ git push --set-upstream origin ft/service-redesign
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 459 bytes | 459.00 KiB/s,
done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0  
remote: Resolving deltas: 100% (1/1), completed with 1
local object.
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote: https://github.com/ishimweClaude12/Gym-Git-Exercises/pull/new/ft/service-redesign
remote:
To https://github.com/ishimweClaude12/Gym-Git-Exercises.git

- [new branch] ft/service-redesign -> ft/service-redesign
  branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/service-redesign)
$ git switch main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git add .

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git commit -m "Change Services page"
[main f83c479] Change Services page
1 file changed, 1 insertion(+), 1 deletion(-)

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 353 bytes | 353.00 KiB/s,
done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0  
remote: Resolving deltas: 100% (2/2), completed with 2
local objects.
To https://github.com/ishimweClaude12/Gym-Git-Exercises.git
faa7498..f83c479 main -> main

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/service-redesign)
$ git diff

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/service-redesign)
$ git merge main
Auto-merging services.html
CONFLICT (add/add): Merge conflict in services.html  
Automatic merge failed; fix conflicts and then commit the result.

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/service-redesign|MERGING)
$ git status
On branch ft/service-redesign
Your branch is up to date with 'origin/ft/service-redesign'.

All conflicts fixed but you are still merging.
(use "git commit" to conclude merge)

Changes to be committed:
modified: README.md
modified: services.html

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/service-redesign|MERGING)
$ git add .

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/service-redesign|MERGING)
$ git commit -m "Merge conflicts"
[ft/service-redesign 7051d67] Merge conflicts

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/service-redesign)
$ git push
Everything up-to-date

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/service-redesign)
$

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/service-redesign|MERGING)
$ git commit -m "Merge conflicts"
[ft/service-redesign 7051d67] Merge conflicts

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/service-redesign)
$ git push
Everything up-to-date

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
(use "git add <file>..." to update what will be committed)
(use "git restore <file>..." to discard changes in working directory)
modified: README.md

no changes added to commit (use "git add" and/or "git commit -a")

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git add README.md

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git commit -m "Add Terminal History - Bundle 2 - Exercise 2"
[main 70b2703] Add Terminal History - Bundle 2 - Exercise 2
1 file changed, 124 insertions(+)

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 1.08 KiB | 1.08 MiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0  
remote: Resolving deltas: 100% (1/1), completed with 1
local object.
To https://github.com/ishimweClaude12/Gym-Git-Exercises.git
f83c479..70b2703 main -> main

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$

- History restored

# Bundle 3

## Exercise 1

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/team-page)
$ git add .

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/team-page)
$ git commit -m "Add Team page"
[ft/team-page 0624abb] Add Team page
2 files changed, 18 insertions(+), 3 deletions(-) create mode 100644 team.html

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/team-page)
$ git push
fatal: The current branch ft/team-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/team-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help
config'.

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/team-page)
$ git push --set-upstream origin ft/team-page  
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 12 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 635 bytes | 635.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote: https://github.com/ishimweClaude12/Gym-Git-Exercises/pull/new/ft/team-page
remote:
To https://github.com/ishimweClaude12/Gym-Git-Exercises.git

- [new branch] ft/team-page -> ft/team-page
  branch 'ft/team-page' set up to track 'origin/ft/team-page'.

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/team-page)
$ git checkout main
Switched to branch 'main'
Your branch is behind 'origin/main' by 3 commits,
and can be fast-forwarded.
(use "git pull" to update your local branch)

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/contact-page)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/team-page)
$ git log
commit 0624abbab8b1962cdc5c2715ba6a76474e01074e (HEAD -> ft/team-page, origin/ft/team-page)
Author: Claude Ishimwe <dpqb12haikuo@gmail.com>  
Date: Wed Aug 2 10:56:28 2023 +0200

    Add Team page

commit 70b27039c706c9a6b8af0c4aa7d010ba0df59d11 (main, ft/contact-page)
Author: Claude Ishimwe <dpqb12haikuo@gmail.com>  
Date: Tue Aug 1 20:06:59 2023 +0200

    Add Terminal History - Bundle 2 - Exercise 2

commit f83c4792c3ab6b812522bcc6947721bf12c6c017  
Author: Claude Ishimwe <dpqb12haikuo@gmail.com>  
Date: Tue Aug 1 19:54:15 2023 +0200

    Change Services page

commit faa74986b2e0bea163fc29ff65fa66193fd5f2f8 (ft/bundle-2)
Author: Claude Ishimwe <dpqb12haikuo@gmail.com>  
Date: Tue Aug 1 16:46:45 2023 +0200

    Add README Changes on Bundle 2

commit 382ca111a1197fcc6c71db1e4090570a52e14af5  
Merge: 8da8e87 0a23864
Author: ishoborabyose <52440263+ishoborabyose@users.noreply.github.com>
Date: Tue Aug 1 16:18:07 2023 +0200

    Merge pull request #2 from ishimweClaude12/ft/bundle-2

    Bundle 2- Exercise 1  - Add Services page

commit 0a238648c72176ac7a13f7f665a5cc3257d95984 (origin/ft/bundle-2)
Author: Claude Ishimwe <dpqb12haikuo@gmail.com>  
Date: Tue Aug 1 10:46:42 2023 +0200

    Add Services page

commit 8da8e8768df5763be9c414def195ce06f5724e99  
Author: Claude Ishimwe <dpqb12haikuo@gmail.com>  
Date: Mon Jul 31 08:58:19 2023 +0200

    Add: Terminal History

commit 79b96ee674217e28d7dfebff7724a86626da4371  
Author: Claude Ishimwe <dpqb12haikuo@gmail.com>  
Date: Mon Jul 31 08:34:41 2023 +0200

    Commit Current Changes

commit 557abba92ad303868d73ad8a25ffde8f295e2c4b  
Author: Claude Ishimwe <dpqb12haikuo@gmail.com>  
Date: Mon Jul 31 08:07:55 2023 +0200

    Add Home.html

commit 24b085a3660f8a63c9f9dc9a19b3b468450f234b  
Merge: 0fd719a 35d1d1e
Author: Claude <77576560+ishimweClaude12@users.noreply.github.com>
Date: Mon Jul 31 08:04:41 2023 +0200

    Merge pull request #1 from ishimweClaude12/dev
    README Bundle 1 - Exercise 1

commit 35d1d1e9c1eacec303cb2707d3cb8620c96fb0b3 (origin/dev, dev)
Author: Claude Ishimwe <dpqb12haikuo@gmail.com>  
Date: Mon Jul 31 08:03:10 2023 +0200

    README Bundle 1 - Exercise 1

commit 0fd719ada67e036e6ca2db9e822298497d2caea2  
Author: Claude Ishimwe <dpqb12haikuo@gmail.com>  
Date: Mon Jul 31 07:58:33 2023 +0200

     Add README.md

commit 1c04b6c43dbf5e9bb24141929e4d269132c4e0ba  
Author: Claude Ishimwe <dpqb12haikuo@gmail.com>  
Date: Mon Jul 31 07:57:42 2023 +0200

    Add Home.html

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/team-page)
$ git checkout ft/contact-page
Switched to branch 'ft/contact-page'

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/contact-page)
$ git log
commit 70b27039c706c9a6b8af0c4aa7d010ba0df59d11 (HEAD -> ft/contact-page, main)
Author: Claude Ishimwe <dpqb12haikuo@gmail.com>  
Date: Tue Aug 1 20:06:59 2023 +0200

    Add Terminal History - Bundle 2 - Exercise 2

commit f83c4792c3ab6b812522bcc6947721bf12c6c017  
Author: Claude Ishimwe <dpqb12haikuo@gmail.com>  
Date: Tue Aug 1 19:54:15 2023 +0200

    Change Services page

commit faa74986b2e0bea163fc29ff65fa66193fd5f2f8 (ft/bundle-2)
Author: Claude Ishimwe <dpqb12haikuo@gmail.com>  
Date: Tue Aug 1 16:46:45 2023 +0200

    Add README Changes on Bundle 2

commit 382ca111a1197fcc6c71db1e4090570a52e14af5  
Merge: 8da8e87 0a23864
Author: ishoborabyose <52440263+ishoborabyose@users.noreply.github.com>
Date: Tue Aug 1 16:18:07 2023 +0200

    Merge pull request #2 from ishimweClaude12/ft/bundle-2

    Bundle 2- Exercise 1  - Add Services page

commit 0a238648c72176ac7a13f7f665a5cc3257d95984 (origin/ft/bundle-2)
Author: Claude Ishimwe <dpqb12haikuo@gmail.com>  
Date: Tue Aug 1 10:46:42 2023 +0200

    Add Services page

commit 8da8e8768df5763be9c414def195ce06f5724e99  
Author: Claude Ishimwe <dpqb12haikuo@gmail.com>  
Date: Mon Jul 31 08:58:19 2023 +0200

    Add: Terminal History

commit 79b96ee674217e28d7dfebff7724a86626da4371  
Author: Claude Ishimwe <dpqb12haikuo@gmail.com>  
Date: Mon Jul 31 08:34:41 2023 +0200

    Commit Current Changes

commit 557abba92ad303868d73ad8a25ffde8f295e2c4b  
Author: Claude Ishimwe <dpqb12haikuo@gmail.com>  
Date: Mon Jul 31 08:07:55 2023 +0200

    Add Home.html

commit 24b085a3660f8a63c9f9dc9a19b3b468450f234b  
Merge: 0fd719a 35d1d1e
Author: Claude <77576560+ishimweClaude12@users.noreply.github.com>
Date: Mon Jul 31 08:04:41 2023 +0200

    Merge pull request #1 from ishimweClaude12/dev
    README Bundle 1 - Exercise 1

commit 35d1d1e9c1eacec303cb2707d3cb8620c96fb0b3 (origin/dev, dev)
Author: Claude Ishimwe <dpqb12haikuo@gmail.com>  
Date: Mon Jul 31 08:03:10 2023 +0200

    README Bundle 1 - Exercise 1

commit 0fd719ada67e036e6ca2db9e822298497d2caea2  
Author: Claude Ishimwe <dpqb12haikuo@gmail.com>  
Date: Mon Jul 31 07:58:33 2023 +0200

     Add README.md

commit 1c04b6c43dbf5e9bb24141929e4d269132c4e0ba  
Author: Claude Ishimwe <dpqb12haikuo@gmail.com>  
Date: Mon Jul 31 07:57:42 2023 +0200

    Add Home.html

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/contact-page)
$ git log --oneline
70b2703 (HEAD -> ft/contact-page, main) Add Terminal History - Bundle 2 - Exercise 2
f83c479 Change Services page
faa7498 (ft/bundle-2) Add README Changes on Bundle 2
382ca11 Merge pull request #2 from ishimweClaude12/ft/bundle-2
0a23864 (origin/ft/bundle-2) Add Services page  
8da8e87 Add: Terminal History
79b96ee Commit Current Changes
557abba Add Home.html
24b085a Merge pull request #1 from ishimweClaude12/dev
35d1d1e (origin/dev, dev) README Bundle 1 - Exercise 1
0fd719a Add README.md
1c04b6c Add Home.html

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/contact-page)
$ git branch
dev
ft/bundle-2

- ft/contact-page
  ft/service-redesign
  ft/team-page
  main

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/contact-page)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/team-page)
$ git log --oneline
0624abb (HEAD -> ft/team-page, origin/ft/team-page) Add Team page
70b2703 (main, ft/contact-page) Add Terminal History - Bundle 2 - Exercise 2
f83c479 Change Services page
faa7498 (ft/bundle-2) Add README Changes on Bundle 2
382ca11 Merge pull request #2 from ishimweClaude12/ft/bundle-2
0a23864 (origin/ft/bundle-2) Add Services page  
8da8e87 Add: Terminal History
79b96ee Commit Current Changes
557abba Add Home.html
24b085a Merge pull request #1 from ishimweClaude12/dev
35d1d1e (origin/dev, dev) README Bundle 1 - Exerci

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/team-page)
$ git checkout ft/contact-page
Switched to branch 'ft/contact-page'

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/contact-page)
$ git cherry-pick 0624abb
[ft/contact-page 9c02c84] Add Team page
Date: Wed Aug 2 10:56:28 2023 +0200
2 files changed, 18 insertions(+), 3 deletions(-) create mode 100644 team.html

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/contact-page)
$ git add .

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/contact-page)
$ git commit -m "Cherry pick changes from team page"
On branch ft/contact-page
nothing to commit, working tree clean

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/contact-page)
$ git push
fatal: The current branch ft/contact-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/contact-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help
config'.

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/contact-page)
$ git push --set-upstream origin ft/contact-page
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 12 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 642 bytes | 642.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote: https://github.com/ishimweClaude12/Gym-Git-Exercises/pull/new/ft/contact-page
remote:
To https://github.com/ishimweClaude12/Gym-Git-Exercises.git

- [new branch] ft/contact-page -> ft/contact-page
  branch 'ft/contact-page' set up to track 'origin/ft/contact-page'.

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/contact-page)
$ git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/faq-page)
$ git add .

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/faq-page)
$ git commit -m "Add faq page"
[ft/faq-page c53540b] Add faq page
1 file changed, 11 insertions(+)
create mode 100644 faq.html

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/faq-page)
$ git push
fatal: The current branch ft/faq-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/faq-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help
config'.

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/faq-page)
$ git push --set-upstream origin ft/faq-page  
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 473 bytes | 473.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote: https://github.com/ishimweClaude12/Gym-Git-Exercises/pull/new/ft/faq-page
remote:
To https://github.com/ishimweClaude12/Gym-Git-Exercises.git

- [new branch] ft/faq-page -> ft/faq-page  
  branch 'ft/faq-page' set up to track 'origin/ft/faq-page'.

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/faq-page)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/team-page)
$ git log --oneline
0624abb (HEAD -> ft/team-page, origin/ft/team-page) Add Team page
70b2703 (main) Add Terminal History - Bundle 2 - Exercise 2
f83c479 Change Services page
Revert "Add Team page"
faa7498 (ft/bundle-2) Add README Changes on Bundle 2
382ca11 Merge pull request #2 from ishimweClaude12/ft/bundle-2
0a23864 (origin/ft/bundle-2) Add Services page  
8da8e87 Add: Terminal History
79b96ee Commit Current Changes
557abba Add Home.html
24b085a Merge pull request #1 from ishimweClaude12/dev
35d1d1e (origin/dev, dev) README Bundle 1 - Exerci

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/team-page)
$ git revert 0624abb
hint: Waiting for your editor to close the file... Vim: Error reading input, exiting...
Vim: Finished.

error: There was a problem with the editor 'vi'.
Please supply the message using either -m or -F option.

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/team-page)
$ git revert 0624abb "Revert all changes back to team page"
fatal: bad revision 'Revert all changes back to team page'

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/team-page)
$ git checkout ft/faq-page
Switched to branch 'ft/faq-page'
M README.md
D team.html
Your branch is up to date with 'origin/ft/faq-page'.

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/faq-page)
$ git log
commit c53540b2fa449bcfdb0797cafac68e6a19d236cd (HEAD -> ft/faq-page, origin/ft/faq-page)
Author: Claude Ishimwe <dpqb12haikuo@gmail.com>  
Date: Wed Aug 2 11:21:00 2023 +0200

    Add faq page

commit 9c02c846f53242876a53821cd5e4d1e0eb6b16c8 (origin/ft/contact-page, ft/contact-page)
Author: Claude Ishimwe <dpqb12haikuo@gmail.com>  
Date: Wed Aug 2 10:56:28 2023 +0200

    Add Team page

commit 70b27039c706c9a6b8af0c4aa7d010ba0df59d11 (main)

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/faq-page)
$ git log
commit c53540b2fa449bcfdb0797cafac68e6a19d236cd (HEAD -> ft/faq-page, origin/ft/faq-page)
Author: Claude Ishimwe <dpqb12haikuo@gmail.com>  
Date: Wed Aug 2 11:21:00 2023 +0200

    Add faq page

commit 9c02c846f53242876a53821cd5e4d1e0eb6b16c8 (origin/ft/contact-page, ft/contact-page)
Author: Claude Ishimwe <dpqb12haikuo@gmail.com>  
Date: Wed Aug 2 10:56:28 2023 +0200

    Add Team page

commit 70b27039c706c9a6b8af0c4aa7d010ba0df59d11 (main)
Author: Claude Ishimwe <dpqb12haikuo@gmail.com>  
Date: Tue Aug 1 20:06:59 2023 +0200

    Add Terminal History - Bundle 2 - Exercise 2

commit f83c4792c3ab6b812522bcc6947721bf12c6c017  
Author: Claude Ishimwe <dpqb12haikuo@gmail.com>  
Date: Tue Aug 1 19:54:15 2023 +0200

    Change Services page

commit faa74986b2e0bea163fc29ff65fa66193fd5f2f8 (ft/bundle-2)
Author: Claude Ishimwe <dpqb12haikuo@gmail.com>  
Date: Tue Aug 1 16:46:45 2023 +0200

    Add README Changes on Bundle 2

commit 382ca111a1197fcc6c71db1e4090570a52e14af5  
Merge: 8da8e87 0a23864
Author: ishoborabyose <52440263+ishoborabyose@users.noreply.github.com>
Date: Tue Aug 1 16:18:07 2023 +0200

    Merge pull request #2 from ishimweClaude12/ft/bundle-2

    Bundle 2- Exercise 1  - Add Services page

commit 0a238648c72176ac7a13f7f665a5cc3257d95984 (origin/ft/bundle-2)
Author: Claude Ishimwe <dpqb12haikuo@gmail.com>

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/faq-page)
$ git revert 9c02c846f53242876a53821cd5e4d1e0eb6b16c81~
fatal: bad revision '9c02c846f53242876a53821cd5e4d1e0eb6b16c81~'

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/faq-page)
$ git log
commit c53540b2fa449bcfdb0797cafac68e6a19d236cd (HEAD -> ft/faq-page, origin/ft/faq-page)
Author: Claude Ishimwe <dpqb12haikuo@gmail.com>  
Date: Wed Aug 2 11:21:00 2023 +0200

    Add faq page

commit 9c02c846f53242876a53821cd5e4d1e0eb6b16c8 (origin/ft/contact-page, ft/contact-page)
Author: Claude Ishimwe <dpqb12haikuo@gmail.com>  
Date: Wed Aug 2 10:56:28 2023 +0200

    Add Team page

commit 70b27039c706c9a6b8af0c4aa7d010ba0df59d11 (main)
Author: Claude Ishimwe <dpqb12haikuo@gmail.com>  
Date: Tue Aug 1 20:06:59 2023 +0200

    Add Terminal History - Bundle 2 - Exercise 2

commit f83c4792c3ab6b812522bcc6947721bf12c6c017  
Author: Claude Ishimwe <dpqb12haikuo@gmail.com>  
Date: Tue Aug 1 19:54:15 2023 +0200

    Change Services page

commit faa74986b2e0bea163fc29ff65fa66193fd5f2f8 (ft/bundle-2)
Author: Claude Ishimwe <dpqb12haikuo@gmail.com>  
Date: Tue Aug 1 16:46:45 2023 +0200

    Add README Changes on Bundle 2

commit 382ca111a1197fcc6c71db1e4090570a52e14af5  
Merge: 8da8e87 0a23864
Author: ishoborabyose <52440263+ishoborabyose@users.noreply.github.com>
Date: Tue Aug 1 16:18:07 2023 +0200

    Merge pull request #2 from ishimweClaude12/ft/bundle-2

    Bundle 2- Exercise 1  - Add Services page

commit 0a238648c72176ac7a13f7f665a5cc3257d95984 (origin/ft/bundle-2)
Author: Claude Ishimwe <dpqb12haikuo@gmail.com>  
Date: Tue Aug 1 10:46:42 2023 +0200

    Add Services page

commit 8da8e8768df5763be9c414def195ce06f5724e99  
Author: Claude Ishimwe <dpqb12haikuo@gmail.com>  
Date: Mon Jul 31 08:58:19 2023 +0200

    Add: Terminal History

commit 79b96ee674217e28d7dfebff7724a86626da4371  
Author: Claude Ishimwe <dpqb12haikuo@gmail.com>  
Date: Mon Jul 31 08:34:41 2023 +0200

    Commit Current Changes

commit 557abba92ad303868d73ad8a25ffde8f295e2c4b  
Author: Claude Ishimwe <dpqb12haikuo@gmail.com>  
Date: Mon Jul 31 08:07:55 2023 +0200

    Add Home.html

commit 24b085a3660f8a63c9f9dc9a19b3b468450f234b  
Merge: 0fd719a 35d1d1e
Author: Claude <77576560+ishimweClaude12@users.noreply.github.com>
Date: Mon Jul 31 08:04:41 2023 +0200

    Merge pull request #1 from ishimweClaude12/dev
    README Bundle 1 - Exercise 1

commit 35d1d1e9c1eacec303cb2707d3cb8620c96fb0b3 (origin/dev, dev)
Author: Claude Ishimwe <dpqb12haikuo@gmail.com>  
Date: Mon Jul 31 08:03:10 2023 +0200

    README Bundle 1 - Exercise 1

commit 0fd719ada67e036e6ca2db9e822298497d2caea2  
Author: Claude Ishimwe <dpqb12haikuo@gmail.com>  
Date: Mon Jul 31 07:58:33 2023 +0200

     Add README.md

commit 1c04b6c43dbf5e9bb24141929e4d269132c4e0ba  
Author: Claude Ishimwe <dpqb12haikuo@gmail.com>  
Date: Mon Jul 31 07:57:42 2023 +0200

    Add Home.html

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/faq-page)ises (ft/faq-page)
$ git status
On branch ft/faq-page
Your branch is up to date with 'origin/ft/faq-page'.

Changes to be committed:
(use "git restore --staged <file>..." to unstage)  
 modified: README.md
deleted: team.html

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/faq-page)
$ git push
Everything up-to-date

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/faq-page)
$ git add .

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/faq-page)
$ git commit -m "Add everything after revert"
[ft/faq-page 98ba992] Add everything after revert
2 files changed, 3 insertions(+), 18 deletions(-)  
 delete mode 100644 team.html

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/faq-page)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 359 bytes | 359.00 KiB/s,
done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0  
remote: Resolving deltas: 100% (2/2), completed with 2
local objects.
To https://github.com/ishimweClaude12/Gym-Git-Exercises.git
c53540b..98ba992 ft/faq-page -> ft/faq-page

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/faq-page)
$

# Exercise 2

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/faq-page)
$ git checkout -b ft/home-page-redesign
Switched to a new branch 'ft/home-page-redesign'

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/home-page-redesign)
$ git switch main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git add .

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git commit -m "Add changes to the main Branch"
[main 373a98a] Add changes to the main Branch
1 file changed, 2 insertions(+)

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 351 bytes | 351.00 KiB/s,
done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0  
remote: Resolving deltas: 100% (2/2), completed with 2
local objects.
To https://github.com/ishimweClaude12/Gym-Git-Exercises.git
0c7712f..373a98a main -> main

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git switch ft/home-page-redesign
Switched to branch 'ft/home-page-redesign'

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/home-page-redesign)
$ git rebase main
Auto-merging README.md
CONFLICT (content): Merge conflict in README.md  
error: could not apply 9c02c84... Add Team page
hint: Resolve all conflicts manually, mark them as resolved with
hint: "git add/rm <conflicted_files>", then run "git rebase --continue".
hint: You can instead skip this commit: run "git rebase --skip".
hint: To abort and get back to the state before "git rebase", run "git rebase --abort".
Could not apply 9c02c84... Add Team page

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/home-page-redesign|REBASE 1/3)
$ git rebase --skip
Auto-merging README.md
CONFLICT (content): Merge conflict in README.md  
error: could not apply 98ba992... Add everything after
revert
hint: Resolve all conflicts manually, mark them as resolved with
hint: "git add/rm <conflicted_files>", then run "git rebase --continue".
hint: You can instead skip this commit: run "git rebase --skip".
hint: To abort and get back to the state before "git rebase", run "git rebase --abort".
Could not apply 98ba992... Add everything after revert

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/home-page-redesign|REBASE 3/3)
$ git rebase --continue
README.md: needs merge
You must edit all merge conflicts and then
mark them as resolved using git add

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/home-page-redesign|REBASE 3/3)
$ git rebase main
Current branch ft/home-page-redesign is up to date.

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/home-page-redesign)
$ git status
On branch ft/home-page-redesign
Changes not staged for commit:
(use "git add <file>..." to update what will be committed)
(use "git restore <file>..." to discard changes in working directory)
modified: README.md

no changes added to commit (use "git add" and/or "git commit -a")

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/home-page-redesign)
$ git add .

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/home-page-redesign)
$ git commit -m "Add Changes to the home page on ft/home-page-redesign branch"
[ft/home-page-redesign 0adf821] Add Changes to the home page on ft/home-page-redesign branch
2 files changed, 1 insertion(+), 6 deletions(-)

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/home-page-redesign)
$ git push
fatal: The current branch ft/home-page-redesign has no
upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/home-page-redesign

To have this happen automatically for branches without
a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/home-page-redesign)
$ git push --set-upstream origin ft/home-page-redesign
Enumerating objects: 13, done.
Counting objects: 100% (13/13), done.
Delta compression using up to 12 threads
Compressing objects: 100% (10/10), done.
Writing objects: 100% (10/10), 1.37 KiB | 700.00 KiB/s, done.
Total 10 (delta 4), reused 0 (delta 0), pack-reused 0  
remote: Resolving deltas: 100% (4/4), completed with 2
local objects.
remote:
remote: Create a pull request for 'ft/home-page-redesign' on GitHub by visiting:
remote: https://github.com/ishimweClaude12/Gym-Git-Exercises/pull/new/ft/home-page-redesign
remote:
To https://github.com/ishimweClaude12/Gym-Git-Exercises.git

- [new branch] ft/home-page-redesign -> ft/home-page-redesign
  branch 'ft/home-page-redesign' set up to track 'origin/ft/home-page-redesign'.

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/home-page-redesign)
$ git switch main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$

# Bundle 4

## Exercise 1

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git pull
Already up to date.

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git remote add git-copy https://github.com/ishimweClaude12/Gym-Git-Exercises-2.git

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git remote
git-copy
origin

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git add .

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git commit -m "Add Changes to the Home page"
[main 99cb169] Add Changes to the Home page
1 file changed, 1 insertion(+)

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git push git-copy
Enumerating objects: 51, done.
Counting objects: 100% (51/51), done.
Delta compression using up to 12 threads
Compressing objects: 100% (49/49), done.
Writing objects: 100% (51/51), 11.76 KiB | 2.94 MiB/s,
done.
Total 51 (delta 18), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (18/18), done.
To https://github.com/ishimweClaude12/Gym-Git-Exercises-2.git

- [new branch] main -> main

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git push origin
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 386 bytes | 386.00 KiB/s,
done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0  
remote: Resolving deltas: 100% (2/2), completed with 2
local objects.
To https://github.com/ishimweClaude12/Gym-Git-Exercises.git
69144c4..99cb169 main -> main

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$

## Exercise 2

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git checkout -b ft/footer
Switched to a new branch 'ft/footer'

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/footer)
$ git add .

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/footer)
$ git commit -m "Add Footer Features"
[ft/footer 9fe27bb] Add Footer Features
1 file changed, 10 insertions(+)  
 create mode 100644 footer.html

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/footer)
$ git commit -a -m "Add some more changes"
[ft/footer 2033a4e] Add some more changes
1 file changed, 5 insertions(+)

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/footer)
$ git push --set-upstream origin ft/footer1
error: src refspec ft/footer1 does not match any
error: failed to push some refs to 'https://github.com/ishimweClaude12/Gym-Git-Exercises.git'

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/footer)
$ git push --set-upstream origin ft/footer
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 12 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 782 bytes | 260.00 KiB/s,
done.
Total 6 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 1
local object.
remote:
remote: Create a pull request for 'ft/footer' on GitHub by visiting:
remote: https://github.com/ishimweClaude12/Gym-Git-Exercises/pull/new/ft/footer
remote:
To https://github.com/ishimweClaude12/Gym-Git-Exercises.git

- [new branch] ft/footer -> ft/footer
  branch 'ft/footer' set up to track 'origin/ft/footer'.

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/footer)
$ git switch main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (main)
$ git checkout -b ft/squashing
Switched to a new branch 'ft/squashing'

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/squashing)
$ git merge --squash ft/footer
Updating e44576c..2033a4e
Fast-forward
Squash commit -- not updating HEAD
footer.html | 15 +++++++++++++++
1 file changed, 15 insertions(+)
create mode 100644 footer.html

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/squashing)
$ git commit -m "footer changes squashing"
[ft/squashing 03a9d91] footer changes squashing
1 file changed, 15 insertions(+)
create mode 100644 footer.html

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/squashing)
$ git push --set-upstream origin ft/squashing
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 509 bytes | 254.00 KiB/s,
done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0  
remote: Resolving deltas: 100% (1/1), completed with 1
local object.
remote:
remote: Create a pull request for 'ft/squashing' on GitHub by visiting:
remote: https://github.com/ishimweClaude12/Gym-Git-Exercises/pull/new/ft/squashing
remote:
To https://github.com/ishimweClaude12/Gym-Git-Exercises.git

- [new branch] ft/squashing -> ft/squashing  
  branch 'ft/squashing' set up to track 'origin/ft/squashing'.

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/Git-Exercises (ft/squashing)
$

# Bundle 5

## Exercise 1

Unfortunately this exericise didn't require me to write so much in my termianl
But here is the link to the page I hosted using github pages.
https://ishimweclaude12.github.io/Gym-Git-Exercises/
You can check it out

## Exercise 2

Here is the link to my forked copy of the git-cafe-exercise repository
https://github.com/ishimweClaude12/git-cafe-exercise.git

# Bundle 6

## Exercise 1

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/git-cafe-exercise (main)
$ git add index.html

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/git-cafe-exercise (main)
$ git commit -m "Change Title to Welcome to our Restuarant"
[main 5ef7b9e] Change Title to Welcome to our Restuarant
1 file changed, 399 insertions(+), 239 deletions(-)

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/git-cafe-exercise (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 1.58 KiB | 1.58 MiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/ishimweClaude12/git-cafe-exercise.git
d1d3f9c..5ef7b9e main -> main

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/git-cafe-exercise (main)
$ git log
commit 5ef7b9e65786bfd1352bc47b37d50f71f286b267 (HEAD -> main, oricommit 5ef7b9e65786bfd1352bc47b37d50f71f286b267 (HEAD -> main, origin/main, origin/HEAD)
Author: Claude Ishimwe <dpqb12haikuo@gmail.com>
Date: Thu Jul 27 11:42:43 2023 +0200

    Change Title to Welcome to our Restuarant

commit d1d3f9cb39e96d536a439a0bcb1206f073305b9b

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/git-cafe-exercise (main)
$ git checkout -b ft/menu
Switched to a new branch 'ft/menu'

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/git-cafe-exercise (ft/menu)
$ git add index.html

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/git-cafe-exercise (ft/menu)
$ git commit -m "feat: Change Index.html Title"
[ft/menu 34d5727] feat: Change Index.html Title
1 file changed, 1 insertion(+), 1 deletion(-)

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/git-cafe-exercise (ft/menu)
$ git add .

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/git-cafe-exercise (ft/menu)
$ git commit -m "feat: Menu title"
[ft/menu e6c626f] feat: Menu title
1 file changed, 323 insertions(+)
create mode 100644 menu.html

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/git-cafe-exercise (ft/menu)
$ git push --set-upstream origin ft/menu
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 12 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 1.91 KiB | 325.00 KiB/s, done.
Total 6 (delta 4), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (4/4), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/menu' on GitHub by visiting:
remote: https://github.com/ishimweClaude12/git-cafe-exercise/pull/new/ft/menu
remote:
To https://github.com/ishimweClaude12/git-cafe-exercise.git

- [new branch] ft/menu -> ft/menu
  branch 'ft/menu' set up to track 'origin/ft/menu'.

## Exercise 2

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/git-cafe-exercise (ft/menu)
$ git checkout -b bug-fix
Switched to a new branch 'bug-fix'

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/git-cafe-exercise (bug-fix)
$ git add index-4.html

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/git-cafe-exercise (bug-fix)
$ git commit -m "feat: Change index-4.html | title to Contacts"
[bug-fix baba09a] feat: Change index-4.html | title to Contacts
1 file changed, 232 insertions(+), 164 deletions(-)

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/git-cafe-exercise (bug-fix)
$ git push --set-upstream origin bug-fix
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 1.44 KiB | 490.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote:
remote: Create a pull request for 'bug-fix' on GitHub by visiting:
remote: https://github.com/ishimweClaude12/git-cafe-exercise/pull/new/bug-fix
remote:
To https://github.com/ishimweClaude12/git-cafe-exercise.git

- [new branch] bug-fix -> bug-fix
  branch 'bug-fix' set up to track 'origin/bug-fix'.

## Exercise 3

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/git-cafe-exercise (bug-fix)
$ git checkout -b fot-fix
Switched to a new branch 'fot-fix'

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/git-cafe-exercise (fot-fix)
$ git add index-4.html

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/git-cafe-exercise (fot-fix)
$ git commit -m "feat: Hot-Fix, Change the telephone number"
[fot-fix 7884fa7] feat: Hot-Fix, Change the telephone number
1 file changed, 1 insertion(+), 1 deletion(-)

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/git-cafe-exercise (fot-fix)
$ git push --set-upstream origin fot-fix
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 325 bytes | 325.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote:
remote: Create a pull request for 'fot-fix' on GitHub by visiting:
remote: https://github.com/ishimweClaude12/git-cafe-exercise/pull/new/fot-fix
remote:
To https://github.com/ishimweClaude12/git-cafe-exercise.git

- [new branch] fot-fix -> fot-fix
  branch 'fot-fix' set up to track 'origin/fot-fix'.

User@DESKTOP-3M65OUK MINGW64 ~/Desktop/TheGym/git-cafe-exercise (fot-fix)
$

## Exercise 4

### Reviewing and Merging the Pull Requests from Peers.
