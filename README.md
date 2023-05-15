# GIT Exercise
## Bundle 1
### Exercise 1

'''bash

PS C:\Users\Lenovo\Desktop\work1\Coursera\Ojemba\Git_ba
sics\Git_basics> git init
Reinitialized existing Git repository in C:/Users/Lenov
o/Desktop/work1/Coursera/Ojemba/Git_basics/Git_basics/.
git/
PS C:\Users\Lenovo\Desktop\work1\Coursera\Ojemba\Git_ba
sics\Git_basics> git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be c
ommitted)
        README.md

nothing added to commit but untracked files present (us
e "git add" to track)
PS C:\Users\Lenovo\Desktop\work1\Coursera\Ojemba\Git_ba
sics\Git_basics> git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be c
ommitted)
        README.md

nothing added to commit but untracked files present (us
e "git add" to track)
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
s\Git_basics> git status
On branch main
Your branch is up to date with 'origin/main'.
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

'''