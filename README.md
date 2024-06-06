# connect via ssh
## Create an empty github repository
add repository name, description, public/private
get ssh directory
##
local folder
mkdir ~/github/repo-folder
cd ~/github/repo-folder

# part 1

## initialize git
~~~
git init
~~~
## show global config
~~~
git config --global --list
~~~
## set user.email and user.name for git
~~~
git config --global user.email "email@domain.com"
git config --global user.name "Name"
~~~
## set default branchname to <main> for github
~~~
git config --global init.defaultbranch main
~~~



# part 2

## git remote
~~~
git remote -v
git remote add origin git@github.com:mohawkey/tst.git

~~~
~~~
git remote show origin
~~~
git config --global push.autoSetupRemote true
git pull origin main

git add .
git commit -m "info"
git push

