# Git pull v.s git fetch
git pull=git fetch + git merge
  
# git remote  
show: origin  
what's origin?  
it means the repo you copied from the online repo  
=> git remote -v  
show:   
origin	git@github.com:github/git-reference.git (fetch)  
origin	git@github.com:github/git-reference.git (push)  

## git remote and local
if you cloned a the repo online  
git remote=>origin(aliases name of this repo is origin, set as default of clone)  
if you git init a local repo  
git remote=> nothing  
git remote add: add a new remote repository of your project  
=>git remote add [alias] [url]  
git remote=> nothing  
git remote add AAA https://github.com/THYao/EECS545_Lectures  
git remote -v =>  
AAA https://github.com/THYao/EECS545_Lectures(fetch)  
AAA https://github.com/THYao/EECS545_Lectures(pus)  
- Example  
$ git remote -v  
github	git@github.com:schacon/hw.git (fetch)  
github	git@github.com:schacon/hw.git (push)  
origin	git://github.com/github/git-reference.git (fetch)  
origin	git://github.com/github/git-reference.git (push)  
$ git remote set-url --push origin git://github.com/pjhyett/hw.git  
$ git remote -v  
github	git@github.com:schacon/hw.git (fetch)  
github	git@github.com:schacon/hw.git (push)  
origin	git://github.com/github/git-reference.git (fetch)  
origin	git://github.com/pjhyett/hw.git (push)  

# Good resources
http://gitref.org/remotes/#remote
