This is a test file in Windows.

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
git log --pretty=online	#clear view of history record with commit id number

reset file to last version and undo reset operation:
git reset --hard HEAD^
git reset --hard COMMIT_ID_NUMBER	#you need remembering COMMIT_ID_NUMBER for deleted version

