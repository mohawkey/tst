# using git to connect with github via ssh key
## Create an empty github repository
- add repository name
- description
- public/private

get ssh directory
## create a local folder
mkdir ~/github/repo-folder
cd ~/github/repo-folder
## create a ssh key
~~~
ssh-keygen -t ed25519 -C "email@example.com"
~~~
## add sshkey to github
Username > Settings > SSH and GPG keys > New SSH key
~~~
cat ~/.ssh/id_ed25519.pub
~~~
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
git config --global user.email "email@example.com"
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


https://ubc-library-rc.github.io/intro-git/content/03_sync.html
https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account?tool=cli

