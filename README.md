# Learn-Git
This repository is created for learning Git

List of useful git commands
===========================

git status : 
    View current status of the directory

git add <filepath> : 
    Stage a file

git add <directory path> : 
    Stage all files in a directory

git add -A : 
    Add all files

git add -p : 
    Choose and select changed files

git commit -m "message" : 
    Commit with a message

git commit --amend 'new commit message' : 
    Merge with last commit

git reset : 
    Unstage all the staged files
	
------------------------------------------

git checkout -- <path to file> : 
    Undo files in the path

git diff : 
    View the difference between changed and respective pristine files

git stash : 
    Stash local changed files

git stash save "message" : 
    Stash local changed files with a message

git stash apply : 
    Pop last stashed local changes

git stash list : 
    List all stashed changes

--------------------------------------------

git checkout - <branch name> : 
    create and checkout a new branch

git checkout - : 
    switch between 2 branches

git branch : 
    view local git branches

git branch -d <branch name>: 
    delete branch (will NOT DELETE if the branch is not merged with parent)

git branch -D <branch name>:  
    delete branch (will DELETE even if the branch is not merged with parent)

git push origin :<branch name> :
    delete remote branch

git branch -m <oldname> <newname> : 
    rename local branch
	
---------------------------------------------

git log : 
    log current commits in the local branch in a simple way

git log --oneline : 
    log current commits in <hash>:<commit message> way

git log --oneline --pretty : 
    log current with descriptive way with auther name and date

git log -S 'something' :
    log commits with the keyword you are looking for

git log --author 'Author Name' :
    log commits by the author name

git reflog :
    audit your git command history

git shortlog -s --author 'Author Name' :
    log number of commits by an author
	
--------------------------------------------------

git reset --soft HEAD~<number of commits>: 
    reset your LOCAL commit history , but keep the changes staged

git reset --hard HEAD~<number of commits> : 
    reset your LOCAL commit history (WARNING! changes will erased from local history)

git cherry-pick <commit-hash> : 
    pick commits from your local history and append to the current branch

git cherry-pick --abort :
    abort current cherry-picking process

git merge --abort :
    abort merging current process