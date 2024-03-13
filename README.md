# gitexercise
First I opened my git account in my laptop using git config, then I started the exercise. 
~~~
git clone https://gitexercises.fracz.com/git/exercises.git
cd exercises
git config user.name "nandiniagrl"
git config user.email "nandini.agrawal.164@gmail.com"
./configure.sh
git start
~~~
## Commit one file
## commit one file from staging area
Then I added two files to staging area and commited only one out of those two as mentioned in the exercise.
~~~
git add --a
git commit -m ""
~~~
## ignore them
Created a .gitignore file and added all the files in it that need to be ignored. ( * for extensions). Commited all the changes.
~~~
touch .gitignore
git add --a
git commit -m ""
~~~
## chase branch
Merged the branch to chase-branch using git merge.
~~~
git merge
git add
git commit
~~~
## merge conflict
To solve the merge conflict, I edited the .txt file and then merged.
~~~
git merge
open file.txt
git add
git commit
~~~
## save your work
First I saved the current work using git stash, fixed the big in bug.txt, stash popped, added the new line, commited changes.
~~~
git stash
git stash pop
~~~
## remove ignored
for next exercise, I simply removed ignored.txt using rm from repository
~~~
rm ignored.txt
~~~
## case sensitive
Simply renamed the file (I have mac)
~~~
rename File.txt file.txt
~~~
## fix typo
first I changed the typo in the file using vim 
~~~
vim file
~~~
Then I added and commited the previous file.
## change branch history
Rebased the branch 
~~~
git rebase
~~~
## fix old typo
First i rebased in interactive environment so that I can edit any commit. Then i edited my file, added , commited and continued rebase. edited file to resolve conflict and added commits.
~~~
git rebase -i
~~~
## forge date
used git commit --amend
~~~
git commit --amend  --date="1987-08-03"
~~~
