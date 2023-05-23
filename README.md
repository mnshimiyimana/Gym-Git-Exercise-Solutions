# GIT Exercise
## Bundle 1
### Exercise 1


```bash
PS C:\Users\Lenovo\Desktop\work1\Coursera\Ojemba\Git_ba
sics\Git_basics> git init
Reinitialized existing Git repository in C:/Users/Lenov
o/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics/.
git/
PS C:\Users\Lenovo\Desktop\work1\Coursera\Ojemba\Git_ba
sics\Git_basics> git add .
PS C:\Users\Lenovo\Desktop\work1\Coursera\Ojemba\Git_ba
sics\Git_basics> git commit -m 'First commit'
[main (root-commit) fd7cb76] First commit
 1 file changed, 1 insertion(+)
 create mode 100644 README.md
PS C:\Users\Lenovo\Desktop\work1\Coursera\Ojemba\Git_ba
sics\Git_basics> git push
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 237 bytes | 118.00 KiB/s,
done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/mnshimiyimana/Git_basics.git
 * [new branch]      main -> main
PS C:\Users\Lenovo\Desktop\work1\Coursera\Ojemba\Git_ba
sics\Git_basics> git branch -m main master
PS C:\Users\Lenovo\Desktop\work1\Coursera\Ojemba\Git_basic
s\Git_basics> git branch dev
PS C:\Users\Lenovo\Desktop\work1\Coursera\Ojemba\Git_basic
s\Git_basics> git push origin dev
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'dev' on GitHub by visit
ing:
remote:      https://github.com/mnshimiyimana/Git_basics/p
ull/new/dev
remote:
To https://github.com/mnshimiyimana/Git_basics.git
 * [new branch]      dev -> dev
 PS C:\Users\Lenovo\Desktop\work1\Coursera\Ojemba\Git_basic
s\Git_basics> git branch test
PS C:\Users\Lenovo\Desktop\work1\Coursera\Ojemba\Git_basic
s\Git_basics> git push origin test
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'test' on GitHub by visi
ting:
remote:      https://github.com/mnshimiyimana/Git_basics/p
ull/new/test
remote:
To https://github.com/mnshimiyimana/Git_basics.git
 * [new branch]      test -> test
PS C:\Users\Lenovo\Desktop\work1\Coursera\Ojemba\Git_basic
s\Git_basics> git checkout dev
Switched to branch 'dev'
PS C:\Users\Lenovo\Desktop\work1\Coursera\Ojemba\Git_basic
s\Git_basics> git branch -d test
Deleted branch test (was d110e74).
PS C:\Users\Lenovo\Desktop\work1\Coursera\Ojemba\Git_basic
s\Git_basics> git push origin --delete test
To https://github.com/mnshimiyimana/Git_basics.git
 - [deleted]         test
```

### Exercise 2

```bash
PS C:\Users\Lenovo\Desktop\work1\Coursera\Ojemba\Git_basics\Git_basics> git add home.html
PS C:\Users\Lenovo\Desktop\work1\Coursera\Ojemba\Git_basics\Git_basics> git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html
        team.html

PS C:\Users\Lenovo\Desktop\work1\Coursera\Ojemba\Git_basics\Git_basics> git stash
Saved working directory and index state WIP on main: de31fdb Submission
PS C:\Users\Lenovo\Desktop\work1\Coursera\Ojemba\Git_basics\Git_basics> git add about.html
PS C:\Users\Lenovo\Desktop\work1\Coursera\Ojemba\Git_basics\Git_basics> git stash
Saved working directory and index state WIP on main: de31fdb Submission
PS C:\Users\Lenovo\Desktop\work1\Coursera\Ojemba\Git_basics\Git_basics> git stash list
stash@{0}: WIP on main: de31fdb Submission
stash@{1}: WIP on main: de31fdb Submission
PS C:\Users\Lenovo\Desktop\work1\Coursera\Ojemba\Git_basics\Git_basics> git add team.html 
PS C:\Users\Lenovo\Desktop\work1\Coursera\Ojemba\Git_basics\Git_basics> git stash        
Saved working directory and index state WIP on main: de31fdb Submission
PS C:\Users\Lenovo\Desktop\work1\Coursera\Ojemba\Git_basics\Git_basics> git stash list   
stash@{0}: WIP on main: de31fdb Submission
stash@{1}: WIP on main: de31fdb Submission
stash@{2}: WIP on main: de31fdb Submission
//Switched to bash
Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (main)
$ git stash pop stash@{1}
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{1} (7a60211374ca0234c06a4699960eb326f6a09b3a)
Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (main)
$ git stash pop stash@{1}
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Dropped stash@{1} (a422b2e3f04d58795eb0df2b79feae6e37e69fcf)
Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (main)
$ git add .
Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (main)
$ git commit -m 'Files'
[main bcbe130] Files
 2 files changed, 10 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (4/4), 436 bytes | 436.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
remote: This repository moved. Please use the new location:
remote:   https://github.com/mnshimiyimana/Gym-Git-Exercise-Solutions.git
To https://github.com/mnshimiyimana/Git_basics.git
   de31fdb..bcbe130  main -> main

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (main)
$ git stash list
stash@{0}: WIP on main: de31fdb Submission

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (main)
$ git stash pop
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped refs/stash@{0} (05cc597b7c14223f372fd72fed6ad8bf387b16a4)

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (main)
$ git reset --hard
HEAD is now at bcbe130 Files

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
```

## Bundle 2
### Exercise 1

```bash
Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (main)
$ git checkout -b ft/bundle-2 
Switched to a new branch 'ft/bundle-2'

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/bundle-2)
$ git status
On branch ft/bundle-2
nothing to commit, working tree clean

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/bundle-2)
$ git add .

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/bundle-2)
$ git status
On branch ft/bundle-2
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   services.html


Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/bundle-2)
$ git commit -m 'Service page'
[ft/bundle-2 1790e78] Service page
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 services.html

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/bundle-2)
$ git push
fatal: The current branch ft/bundle-2 has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/bundle-2

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/bundle-2)
$ git push --set-upstream origin ft/bundle-2
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 269 bytes | 269.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: This repository moved. Please use the new location:
remote:   https://github.com/mnshimiyimana/Gym-Git-Exercise-Solutions.git
remote: 
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/mnshimiyimana/Gym-Git-Exercise-Solutions/pull/new/ft/bundle-2
remote:
To https://github.com/mnshimiyimana/Git_basics.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
branch 'ft/bundle-2' set up to track 'origin/ft/bundle-2'.

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/bundle-2)
$ git add .

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/bundle-2)
$ git status
On branch ft/bundle-2
Your branch is up to date with 'origin/ft/bundle-2'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   services.html


Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/bundle-2)
$ git commit -m 'Service page'
[ft/bundle-2 eb10390] Service page
 1 file changed, 12 insertions(+)

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/bundle-2)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 425 bytes | 425.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: This repository moved. Please use the new location:
remote:   https://github.com/mnshimiyimana/Gym-Git-Exercise-Solutions.git
To https://github.com/mnshimiyimana/Git_basics.git
   1790e78..eb10390  ft/bundle-2 -> ft/bundle-2

```

### Exercise 2

```bash
Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/bundle-2)
$ git checkout main
Switched to branch 'main'
Your branch is behind 'origin/main' by 4 commits, and can be fast-forwarded.
  (use "git pull" to update your local branch)

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (main)
$ git pull
Updating bcbe130..559928c
Fast-forward
 services.html | 12 ++++++++++++
 1 file changed, 12 insertions(+)
 create mode 100644 services.html

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (main)
$ git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/service-redesign)
$ git add .

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/service-redesign)
$ git status
On branch ft/service-redesign
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   services.html


Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/service-redesign)
$ git commit -m 'changes'
[ft/service-redesign 5b753d2] changes
 1 file changed, 3 insertions(+)

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/service-redesign)
$ git push
fatal: The current branch ft/service-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/service-redesign

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/service-redesign)
$ git push --set-upstream origin ft/service-redesign
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 395 bytes | 395.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote: This repository moved. Please use the new location:
remote:   https://github.com/mnshimiyimana/Gym-Git-Exercise-Solutions.git
remote: 
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/mnshimiyimana/Gym-Git-Exercise-Solutions/pull/new/ft/service-redesign
remote:
To https://github.com/mnshimiyimana/Git_basics.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (main)
$ git add .

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (main)
$ git commit -m 'changes'
[main afe34bc] changes
 1 file changed, 2 insertions(+)

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 363 bytes | 363.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote: This repository moved. Please use the new location:
remote:   https://github.com/mnshimiyimana/Gym-Git-Exercise-Solutions.git
To https://github.com/mnshimiyimana/Git_basics.git
   559928c..afe34bc  main -> main
Merge branch 'main' into ft/service-redesign

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (main)
$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/service-redesign)
$ git merge main
Auto-merging services.html
CONFLICT (content): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/service-redesign|MERGING)
$ git add .

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/service-redesign|MERGING)
$ git commit
[ft/service-redesign 37c6d1f] Merge branch 'main' into ft/service-redesign

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/service-redesign)
$ git push
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 441 bytes | 441.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote: This repository moved. Please use the new location:
remote:   https://github.com/mnshimiyimana/Gym-Git-Exercise-Solutions.git
To https://github.com/mnshimiyimana/Git_basics.git
   5b753d2..37c6d1f  ft/service-redesign -> ft/service-redesign

```

## Bundle 3
### Exercise 1

```bash
Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/service-redesign)
$ git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/team-page)
$ git add .

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/team-page)
$ git status
On branch ft/team-page
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html


Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/team-page)
$ git commit -m 'Team page'
[ft/team-page c60ffcb] Team page
 1 file changed, 10 insertions(+)
 create mode 100644 team.html

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/team-page)
$ git push
fatal: The current branch ft/team-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/team-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/team-page)
$ git push --set-upstream origin ft/team-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 409 bytes | 409.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: This repository moved. Please use the new location:
remote:   https://github.com/mnshimiyimana/Gym-Git-Exercise-Solutions.git
remote: 
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/mnshimiyimana/Gym-Git-Exercise-Solutions/pull/new/ft/team-page
remote:
To https://github.com/mnshimiyimana/Git_basics.git
 * [new branch]      ft/team-page -> ft/team-page
branch 'ft/team-page' set up to track 'origin/ft/team-page'.

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/team-page)
$ git checkout main
Switched to branch 'main'
Your branch is behind 'origin/main' by 3 commits, and can be fast-forwarded.
  (use "git pull" to update your local branch)

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (main)
$ git pull
Updating afe34bc..0bad156
Fast-forward
 services.html | 6 ++++++
 1 file changed, 6 insertions(+)

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (main)
$ git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/contact-page)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/team-page)
$ git log
commit c60ffcbb06ef47bb5d1ac6b086030e02dee2a122 (HEAD -> ft/team-page, origin/ft/team-page)
commit c60ffcbb06ef47bb5d1ac6b086030e02dee2a122 (HEAD -> ft/team-page, origin/ft/team-page)
commit c60ffcbb06ef47bb5d1ac6b086030e02dee2a122 (HEAD -> ft/team-page, origin/ft/team-page)
Author: mnshimiyimana <m.nshimiyim@alustudent.com>
Date:   Tue May 16 15:04:29 2023 +0200

    Team page

commit 37c6d1f45974dc32d9f1e247bce8c10437cfb924 (origin/ft/service-redesign, ft/service-redesign)
Merge: 5b753d2 afe34bc
Author: mnshimiyimana <m.nshimiyim@alustudent.com>
Date:   Tue May 16 14:54:51 2023 +0200

    Merge branch 'main' into ft/service-redesign

commit afe34bcb2b0c1c6b123063d09e1a82ebb2cc42ef
Author: mnshimiyimana <m.nshimiyim@alustudent.com>
Date:   Tue May 16 14:33:30 2023 +0200


Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/team-page)
$ git checkout ft/contact-page 
Switched to branch 'ft/contact-page'

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/contact-page)
$ git cherry-pick c60ffcbb06ef47bb5d1ac6b086030e02dee2a122
[ft/contact-page bcc3f9d] Team page
 Date: Tue May 16 15:04:29 2023 +0200
 1 file changed, 10 insertions(+)
 create mode 100644 team.html

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/contact-page)
$ git add .

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/contact-page)
$ git status
On branch ft/contact-page
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   contact.html


Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/contact-page)
$ git commit -m 'Contact page'
[ft/contact-page dac080e] Contact page
 1 file changed, 11 insertions(+)
 create mode 100644 contact.html

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/contact-page)
$ git push
fatal: The current branch ft/contact-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/contact-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/contact-page)
$ git push --set-upstream origin ft/contact-page
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 8 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 777 bytes | 777.00 KiB/s, done.
Total 6 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 1 local object.
remote: This repository moved. Please use the new location:
remote:   https://github.com/mnshimiyimana/Gym-Git-Exercise-Solutions.git
remote: 
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/mnshimiyimana/Gym-Git-Exercise-Solutions/pull/new/ft/contact-page
remote:
To https://github.com/mnshimiyimana/Git_basics.git
 * [new branch]      ft/contact-page -> ft/contact-page
branch 'ft/contact-page' set up to track 'origin/ft/contact-page'.
Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/contact-page)
$ git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/faq-page)
$ git add .

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/faq-page)
$ git status
On branch ft/faq-page
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   faq.html


Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/faq-page)
$ git commit -m 'Faq page'
[ft/faq-page 6947f13] Faq page
 1 file changed, 9 insertions(+)
 create mode 100644 faq.html

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/faq-page)
$ git push
fatal: The current branch ft/faq-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/faq-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/faq-page)
$ git push --set-upstream origin ft/faq-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Revert "Team page"
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 339 bytes | 339.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: This repository moved. Please use the new location:
remote:   https://github.com/mnshimiyimana/Gym-Git-Exercise-Solutions.git
remote:
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/mnshimiyimana/Gym-Git-Exercise-Solutions/pull/new/ft/faq-page
remote:
To https://github.com/mnshimiyimana/Git_basics.git
 * [new branch]      ft/faq-page -> ft/faq-page
branch 'ft/faq-page' set up to track 'origin/ft/faq-page'.

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/faq-page)
$ git revert c60ffcbb06ef47bb5d1ac6b086030e02dee2a122
[ft/faq-page 4b3d2b2] Revert "Team page"
 1 file changed, 10 deletions(-)
 delete mode 100644 team.html

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/faq-page)
$ git log
commit 4b3d2b2d76b8a3206f8f1afdc8b81a10ee064d70 (HEAD -> ft/faq-page)
Author: mnshimiyimana <m.nshimiyim@alustudent.com>
Date:   Tue May 16 15:31:45 2023 +0200

    Revert "Team page"

    This reverts commit c60ffcbb06ef47bb5d1ac6b086030e02dee2a122.

commit 6947f13fe88c9a640ed9608224aaa695cb25c5c9 (origin/ft/faq-page)
Author: mnshimiyimana <m.nshimiyim@alustudent.com>
Date:   Tue May 16 15:28:38 2023 +0200

    Faq page

commit dac080e13b25644f5ad01a5ef154e7c69c2d16ce (origin/ft/contact-page, ft/contact-page)
Author: mnshimiyimana <m.nshimiyim@alustudent.com>
Date:   Tue May 16 15:17:02 2023 +0200

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/faq-page)
$ git push
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 271 bytes | 271.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: This repository moved. Please use the new location:
remote:   https://github.com/mnshimiyimana/Gym-Git-Exercise-Solutions.git
To https://github.com/mnshimiyimana/Git_basics.git
   6947f13..4b3d2b2  ft/faq-page -> ft/faq-page

```

### Exercise 2

```bash
Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/faq-page)
$ git checkout -b ft/home-page-redesign
Switched to a new branch 'ft/home-page-redesign'

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/home-page-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (main)
$ git add .

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (main)
$ git commit -m 'Changes'
[main 0e9e8db] Changes
 1 file changed, 10 insertions(+)

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 390 bytes | 390.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: This repository moved. Please use the new location:
remote:   https://github.com/mnshimiyimana/Gym-Git-Exercise-Solutions.git
To https://github.com/mnshimiyimana/Git_basics.git
   0bad156..0e9e8db  main -> main

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (main)
$ git checkout ft/
ft/bundle-2             ft/contact-page         ft/faq-page             ft/home-page-redesign   ft/service-redesign     ft/team-page

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (main)
$ git checkout ft/home-page-redesign 
Switched to branch 'ft/home-page-redesign'

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/home-page-redesign)
$ git rebase main
Successfully rebased and updated refs/heads/ft/home-page-redesign.

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/home-page-redesign)
$ git status
On branch ft/home-page-redesign
nothing to commit, working tree clean

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/home-page-redesign)
$ git log
commit 1f25f3c12b1e9cd90872d7858e1d24376866029b (HEAD -> ft/home-page-redesign)
commit 1f25f3c12b1e9cd90872d7858e1d24376866029b (HEAD -> ft/home-page-redesign)
Author: mnshimiyimana <m.nshimiyim@alustudent.com>
Date:   Tue May 16 15:31:45 2023 +0200

    Revert "Team page"

    This reverts commit c60ffcbb06ef47bb5d1ac6b086030e02dee2a122.

commit 2385719f48eba2a64d9600ccbf55866f81837392
Author: mnshimiyimana <m.nshimiyim@alustudent.com>
Date:   Tue May 16 15:28:38 2023 +0200

    Faq page

commit 650475af7cbd4f38a52e587f5436a825579ea6f1
Author: mnshimiyimana <m.nshimiyim@alustudent.com>
Date:   Tue May 16 15:17:02 2023 +0200
Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/home-page-redesign)
$ git add .
Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/home-page-redesign)
$ git commit -m 'Changes'
[ft/home-page-redesign a4fde3f] Changes
 1 file changed, 6 insertions(+), 1 deletion(-)
Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/home-page-redesign)
$ git push
fatal: The current branch ft/home-page-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/home-page-redesign

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics (ft/home-page-redesign)
$ git push --set-upstream origin ft/home-page-redesign
Enumerating objects: 16, done.
Counting objects: 100% (16/16), done.
Delta compression using up to 8 threads
Compressing objects: 100% (14/14), done.
Writing objects: 100% (14/14), 1.71 KiB | 1.71 MiB/s, done.
Total 14 (delta 4), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (4/4), done.
remote: This repository moved. Please use the new location:
remote:   https://github.com/mnshimiyimana/Gym-Git-Exercise-Solutions.git
remote: 
remote: Create a pull request for 'ft/home-page-redesign' on GitHub by visiting:
remote:      https://github.com/mnshimiyimana/Gym-Git-Exercise-Solutions/pull/new/ft/home-page-redesign
remote:
To https://github.com/mnshimiyimana/Git_basics.git
 * [new branch]      ft/home-page-redesign -> ft/home-page-redesign
branch 'ft/home-page-redesign' set up to track 'origin/ft/home-page-redesign'.
```
## Bundle 4
### Exercise 1

```bash
Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Gym-Git-Exercise-Solutions/Gym-Git-Exercise-Solutions-1 (main)
$ git checkout main
Already on 'main'
Your branch is up to date with 'origin/main'.
Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Gym-Git-Exercise-Solutions/Gym-Git-Exercise-Solutions-1 (main)
$ git remote add git-copy https://github.com/mnshimiyimana/git-exercise-clone.git

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Gym-Git-Exercise-Solutions/Gym-Git-Exercise-Solutions-1 (main)
$ git remote
git-copy
origin
Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Gym-Git-Exercise-Solutions/Gym-Git-Exercise-Solutions-1 (main)
$ git status 
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   home.html

no changes added to commit (use "git add" and/or "git commit -a")

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Gym-Git-Exercise-Solutions/Gym-Git-Exercise-Solutions-1 (main)
$ git add .

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Gym-Git-Exercise-Solutions/Gym-Git-Exercise-Solutions-1 (main)
$ git commit -m 'Changes'
[main d45d9a6] Changes
 1 file changed, 1 insertion(+)

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Gym-Git-Exercise-Solutions/Gym-Git-Exercise-Solutions-1 (main)
$ git push origin
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 301 bytes | 301.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/mnshimiyimana/Gym-Git-Exercise-Solutions.git
   f6adde5..d45d9a6  main -> main
Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Gym-Git-Exercise-Solutions/Gym-Git-Exercise-Solutions-1 (main)
$ git push git-copy
Enumerating objects: 60, done.
Counting objects: 100% (60/60), done.
Delta compression using up to 8 threads
Compressing objects: 100% (32/32), done.
Writing objects: 100% (60/60), 10.67 KiB | 10.67 MiB/s, done.
Total 60 (delta 21), reused 53 (delta 18), pack-reused 0
remote: Resolving deltas: 100% (21/21), done.
To https://github.com/mnshimiyimana/git-exercise-clone.git
 * [new branch]      main -> main
 ```
### Exercise 2

```bash
Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Gym-Git-Exercise-Solutions/Gym-Git-Exercise-Solutions-1 (main)
$ git checkout -b ft/footer
Switched to a new branch 'ft/footer'

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Gym-Git-Exercise-Solutions/Gym-Git-Exercise-Solutions-1 (ft/footer)       
$ git add .

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Gym-Git-Exercise-Solutions/Gym-Git-Exercise-Solutions-1 (ft/footer)       
$ git commit -m 'New file'
[ft/footer 31a9883] New file
 1 file changed, 6 insertions(+)
 create mode 100644 footer.html

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Gym-Git-Exercise-Solutions/Gym-Git-Exercise-Solutions-1 (ft/footer)       
$ git status
On branch ft/footer
nothing to commit, working tree clean

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Gym-Git-Exercise-Solutions/Gym-Git-Exercise-Solutions-1 (ft/footer)       
$ git status
On branch ft/footer
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   footer.html

no changes added to commit (use "git add" and/or "git commit -a")

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Gym-Git-Exercise-Solutions/Gym-Git-Exercise-Solutions-1 (ft/footer)       
$ git add .

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Gym-Git-Exercise-Solutions/Gym-Git-Exercise-Solutions-1 (ft/footer)       
$ git commit -m 'Changes'
[ft/footer 32fe01c] Changes
 1 file changed, 2 insertions(+)

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Gym-Git-Exercise-Solutions/Gym-Git-Exercise-Solutions-1 (ft/footer)       
$ git push
fatal: The current branch ft/footer has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/footer

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Gym-Git-Exercise-Solutions/Gym-Git-Exercise-Solutions-1 (ft/footer)       
$  git push --set-upstream origin ft/footer
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 8 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 593 bytes | 296.00 KiB/s, done.
Total 6 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/footer' on GitHub by visiting:
remote:      https://github.com/mnshimiyimana/Gym-Git-Exercise-Solutions/pull/new/ft/footer
remote:
To https://github.com/mnshimiyimana/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/footer -> ft/footer
branch 'ft/footer' set up to track 'origin/ft/footer'.

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Gym-Git-Exercise-Solutions/Gym-Git-Exercise-Solutions-1 (ft/footer)       
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Gym-Git-Exercise-Solutions/Gym-Git-Exercise-Solutions-1 (main)
$ git checkout -b ft/squashing
Switched to a new branch 'ft/squashing'

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Gym-Git-Exercise-Solutions/Gym-Git-Exercise-Solutions-1 (ft/squashing)    
$ git merge --squash ft/footer
Updating d45d9a6..32fe01c
Fast-forward
Squash commit -- not updating HEAD
 footer.html | 8 ++++++++
 1 file changed, 8 insertions(+)
 create mode 100644 footer.html

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Gym-Git-Exercise-Solutions/Gym-Git-Exercise-Solutions-1 (ft/squashing)    
$ git status
On branch ft/squashing
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   footer.html


Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Gym-Git-Exercise-Solutions/Gym-Git-Exercise-Solutions-1 (ft/squashing)    
$ git commit -m 'footer changes squashing'
[ft/squashing 9c2ba90] footer changes squashing
 1 file changed, 8 insertions(+)
 create mode 100644 footer.html

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Gym-Git-Exercise-Solutions/Gym-Git-Exercise-Solutions-1 (ft/squashing)    
$ git push origin ft/squashing
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 352 bytes | 117.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/squashing' on GitHub by visiting:
remote:      https://github.com/mnshimiyimana/Gym-Git-Exercise-Solutions/pull/new/ft/squashing
remote:
To https://github.com/mnshimiyimana/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/squashing -> ft/squashing
 ```

 ## Bundle 5
 ### Exercise 2

 ```bash
 Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git-cafe-exercise (main)
$ cd git-cafe-exercise/

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git-cafe-exercise/git-cafe-exercise (main)
$ ls
bat/  css/  images/  index.html  index-1.html  index-2.html  index-3.html  index-4.html  js/  README.md

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git-cafe-exercise/git-cafe-exercise (main)
$ git add .

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git-cafe-exercise/git-cafe-exercise (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   index.html


Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git-cafe-exercise/git-cafe-exercise (main)
$ git commit -m 'Changes'
[main 177c7b4] Changes
 1 file changed, 1 insertion(+), 1 deletion(-)

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git-cafe-exercise/git-cafe-exercise (main)
$ git push 
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 317 bytes | 105.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/mnshimiyimana/git-cafe-exercise.git
   d1d3f9c..177c7b4  main -> main
   ```
   ## Bundle 6
### Exercise 1
```bash
Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git-Cafe-Exercise (main)
$ git checkout -b ft/menu
Switched to a new branch 'ft/menu'

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git-Cafe-Exercise (ft/menu)
$ git add .

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git-Cafe-Exercise (ft/menu)
$ git commit -m 'Menu page'
[main 177c7b4] Changes
 1 file changed, 1 insertion(+), 1 deletion(-)

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git-Cafe-Exercise (ft/menu)
$ git push
fatal: The current branch ft/menu has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/menu

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git-Cafe-Exercise (ft/menu)
$ git push origin ft/menu
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 352 bytes | 117.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/menu' on GitHub by visiting:
remote:      https://github.com/mnshimiyimana/Git-Cafe-Exercise/pull/new/ft/menu
remote:
To https://github.com/mnshimiyimana/Git-Cafe-Exercise.git
 * [new branch]      ft/menu -> ft/menu
 ```

 ### Exercise 2

```bash
Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git-Cafe-Exercise (ft/menu)
$ git checkout -b bug-fix
Switched to a new branch 'bug-fix'

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git-Cafe-Exercise (bug-fix)
$ git add .

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git-Cafe-Exercise (bug-fix)
$ git commit -m 'Title change'
[main 177c7b4] Title change
 1 file changed, 1 insertion(+), 1 deletion(-)

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git-Cafe-Exercise (bug-fix)
$ git push
fatal: The current branch ft/menu has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin bug-fix

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git-Cafe-Exercise (bug-fix)
$ git push origin bug-fix
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 352 bytes | 117.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/menu' on GitHub by visiting:
remote:      https://github.com/mnshimiyimana/Git-Cafe-Exercise/pull/new/bug-fix
remote:
To https://github.com/mnshimiyimana/Git-Cafe-exercise.git
 * [new branch]      bug-fix -> bug-fix
 ```

### Exercise 3

```bash
Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git-Cafe-exercise (bug-fix)
$ git checkout main
Switched to a new branch 'main'

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git-Cafe-exercise (main)
$ git add .

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git-Cafe-exercise (main)
$ git commit -m 'Changes'
[main 177c7b4] Changes
 1 file changed, 1 insertion(+), 1 deletion(-)

Lenovo@DESKTOP-7E3EPVK MINGW64 ~/Desktop/work1/Coursera/Ojemba/Git_basics/Git-Cafe-exercise (main)
$ git push 
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 317 bytes | 105.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/mnshimiyimana/git-cafe-exercise.git
   d1d3f9c..177c7b4  main -> main