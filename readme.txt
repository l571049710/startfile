This is a tutoral file for git in Windows.

add file and add commit:
git add FILENAME
git commit -m"COMMIT"	#you can add multiple files and commit them with one commit command.

check out changes of files in repository:
git status	#check status of repository
git diff FILENAME

update file:
#same as add file and add commit

get history record:
git log
git log --pretty=oneline	#clear view of history record with commit id number
git reflog	#this will record every command with commit id number

reset file to last version and undo reset operation:
git reset --hard HEAD^
git reset --hard COMMIT_ID_NUMBER	#you need remembering COMMIT_ID_NUMBER for deleted version

explanations of git words:
working directory: the file space in your PC
repository: .git file. it contains stage and branches. 

check the difference between file in work directoty and repository:
git diff HEAD -- FILENAME

discard changes in working directory:
git checkout -- FILENAME	#without being saved in stage
git reset HEAD FILENAME	#delete the file in stage

delete file:
git rm FILENAME

connect to GitHub:
ssh-keygen -t rsa -C "EMAIL@EMAIL.COM"	#it will create two file. use the ssh in id_rsa.pub in github account setting

push changes in repository to GitHub:
git push origin master

clone repository on GitHub to PC:
git clone git@github.com:GITHUB_USER_NAME/REPOSITORY_NAME.git	#this command can only clone master branch
git checkout -b BRANCH_NAME REMOTE_NAME/BRANCH_NAME	#this command will create branch and clone branch from GitHub repository 

create new branch and switch to it:
git checkout -b BRANCH_NAME	#-b means create and switch to new branch
git branch BRANCH_NAME
git checkout BRANCH_NAME	#those two commands equals to the first one

check branches:
git branch

switch back to old branch:
git checkout master

bring changes in new branch to old branch:
git merge BRANCH_NAME

delete branch:
git branch -d BRANCH_NAME

hide changes in working directory:
git stash

checkout changes in stash:
git stash list

bring changes in stash back:
git stash pop stash@{NUM}
git stash apply stash@{NUM}
git stash drop stash@{NUM}	#those two commands equal to the first command

checkout information of GitHub repository:
git remote -v

push branch to GitHub repository:
git push REMOTE_NAME BRANCH_NAME