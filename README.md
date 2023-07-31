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
