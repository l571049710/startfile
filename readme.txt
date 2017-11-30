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
working directory: the file space in your pc
repository: .git file. it contains stage and branches. 

check the difference between file in work directoty and repository:
git diff HEAD -- FILENAME

discard changes in working directory:
git checkout -- FILENAME	#without being saved in stage
git reset HEAD FILENAME	#delete the file in stage

delete file:
git rm FILENAME

connect to github:
ssh-keygen -t rsa -C "EMAIL@EMAIL.COM"	#it will create two file. use the ssh in id_rsa.pub in github account setting

