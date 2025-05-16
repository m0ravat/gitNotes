# gitNotes
## misc commands
git log (--oneline) - check log of commits history  
git status - view current branch, files to be committed etc   

## Basics
cd into your directory you wanna create into a repo.       
git init - Intiailise empty git repo  
touch index.html - create file  
git add index.html - adds file into staging area  
git rm --cached index.html - takes it out of staging area  
git add . - add all modified files  
git commit -m "Message" (or just git commit) - Might need shift colon then wq  

## Reviewing History
git checkout #ere334 - Seeing code in the state of a previous commit. Changes are read only, wont be committed.  
git checkout master - check out master branch (origin before checking out another commit)  
git revert #dsfeef - revert code to a previous state and commit it, full history still available.   
git reset #efwfe434 - Reverts repo to previous state and removes the commits after it from the log, your code changes are still there but unstaged.   
git reset --hard #fwesef3r - Reverts repo and removes code you produced after the point, you will lose uncommitted code.   

## Branches
git branch featureName - create branch  
git branch -a - show all branches  
git checkout branch1 - switch branches  
git branch -d (-D if unmerged) - delete a branch  
git checkout -b featureName - Creates branch and switches to it.   

## Merging & conflicts
git checkout master  
git merge featureName - merge branch to master  
If conflict adjust the file as needed and git commit.   

## GitHub
git push https://url.com master - Push master branch to an empty git repo.   
git remote add origin https://url.com - adds origin alias to repo:   
git push origin master - pushes commits to github  

git clone https://url.com - intiailise an empty project to repo.   
You don't need to add origin alias when cloning, can go straight to push.   

### Collabaration
git pull origin master - taking in teammates' code.   
git checkout -b myBranch - make your own branch to avoid conflicts.  
Compare and pull request after making changes via github repo site, explain what you did.   
Can add reviewers, add comments to it or merge if no conflicts.   

### Forking
Press fork button on repo from another account and it will go on your account. After making changes if you want to contribute changes to main repo create pull request to be merged by original creator. 
