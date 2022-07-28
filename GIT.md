# Git Stuff


## Basic
- git init 
- git config 
- git status
- adding ".gitignore"
- git diff
- git add ... stop using "." 
- git commit 
- git pull & git merge ... before, why?  
- git remote 
- git push 
- git clone
- diff between ... ssh / http 
- sudo or no-sudo 

## Branches / Flow

- master/main (prod) -> develop (staging) -> recycle-branch (sprint-1:version-1.0) -> sui-10-login-fix
- git checkout 
- git merge 
- create "pull-request" (bitbucket / github)


inorder to put conflict responsibility to the brnch coder: 
master -> develop -> 

version-1.0 <- fix.login.module

git checkout version-1.0
git pull origin version-1.0
git checkout fix.login.module
git merge version-1.0  
- resolve conflicts 
    git add ...
    git commit "resolved conflict" 
git push origin fix.login
PR 

