# git_exercise
First I opened my git account in my laptop using git config, then I started the exercise. 
~~~
git clone https://gitexercises.fracz.com/git/exercises.git
cd exercises
git config user.name "nandiniagrl"
git config user.email "nandini.agrawal.164@gmail.com"
./configure.sh
git start
~~~
## Commit-one-file
To commit only one file out of the two given files : A.txt and B.txt we add only one file to the staging area and then commit changes.
~~~
git add A.txt
git commit -m "one out of two files added"
~~~
## commit-one-file-staged
Then I added two files to staging area and commited only one out of those two as mentioned in the exercise.
~~~
git add --a
git commit -m ""
~~~
## ignore-them
Created a .gitignore file and added all the files in it that need to be ignored. ( * for extensions). Commited all the changes.
~~~
touch .gitignore
~~~
I added the following:
*.exe *.o *.jar libraries/
in the file
~~~
git add --a
git commit -m ""
~~~
## chase-branch
Merged the branch to chase-branch using git merge. This command merges the chase branch which is also head with escaped branch. So they point to same commit. git verify Next Level
               escaped
                  |
A <----- B <----- C
                  |
            chase-branch
                  |
                 HEAD
~~~
git branch checkout chase-branch
git merge escaped
git add --a
git commit -m "merged"
~~~
## merge-conflict
To solve the merge conflict, I edited the .txt file and then merged. i changed it to 2+3 = 5 and then run.
add equation.txt again, commit it and verify to move to next level.
~~~
git merge another-piece-of-work
open file.txt
git add equation.txt
git commit -m "changes"
~~~
## save-your-work
First I saved the current work using git stash.
<br>  fixed the big in bug.txt.
<br>  stash popped
<br>  added the new line
<br>  commited changes.
~~~
git stash
nano bug.txt 
THIS IS A BUG - remove the whole line to fix it.
git add bug.txt 
git commit -m "bug fix"
git stash pop
~~~
 added "Finally, finished it!" line to bug through
 ~~~
nano bug.txt
git add bug.txt program.txt 
git commit -m "final commit"
git verify
~~~
## remove-ignored
for next exercise, I simply removed ignored.txt using rm from repository
~~~
git rm --cached ignored.txt
git commit -m "remove ignored.txt"
git verify
~~~
## case-sensitive
Simply renamed the file.
~~~
rename File.txt file.txt
~~~
## fix-typo
first I changed the typo in the file using vim.
<br>Change wordl to world
~~~
vim file.txt
git add file.txt
git commit --ammend
git verify
~~~
Then I added and commited the previous file.
## change-branch-history
Rebased the branch 
~~~
git rebase hot-bugfix
git verify
~~~
## fix-old-typo
First i rebased in interactive environment so that I can edit any commit. 
<br>Then i edited my file, added , commited and continued rebase. 
<br>edited file to resolve conflict and added commits.
~~~
git rebase -i
nano.txt 
git add file.txt
git commit --amend 
git rebase --continue 
nano file.txt .
add file.txt
git verify
~~~
## forge-date
used git commit --amend
~~~
git commit --amend  --date="1987-08-03"
~~~
