# Git Syntax

`git init` 

> ```bash
> mkdir NewFolder
> git init
> Initialized empty Git repository in /Users/mitchellunderwood/Desktop/NewFolder/.git/
> ```

`git add`

> 

`git clone`

>

`git commit`

>

`git pull`

>

`git push`

`git checkout`

`git merge`

`git reset`

`git remote`

`git log`

Example of committing changes and pushing to the address of a remote repository

```bash
mkdir NewFolder
git init
touch NewFile.txt
~open the file and adjust the content~
git add
git commit
```



## References

https://dev.to/dhruv/essential-git-commands-every-developer-should-know-2fl

https://confluence.atlassian.com/bitbucketserver/basic-git-commands-776639767.html

https://raw.githubusercontent.com/joshnh/Git-Commands/master/READMEpt.md

### To Create a folder, commit changes, and push to a remote repo

``` bash
cd ~/Desktop
mkdir NewFolder
git init
git add -A
git status
git commit -m "This is my message"
git log
*create remote github repo on github.com, copy the repo address to the clickboard
git remote add origin https://github.address
git push origin master
*username: sassypigeon
*password: ***********
```

### To Change the Remote Repo setting of a local Repo

``` bash
*to view the current url attached to the push command of the repo
git remote -v
*alternatively you can also use `git remote show origin`
*to change the url 
git remote set-url <remote_name> <remote_url>

```

### To create multiple remotes 

``` bash
*git remote add <remote 1 name> <remote 1 url>
*git remote add <remote 2 name> <remote 2 url>

mkdir NewFolder
git init
git remote add origin <origin url>
git remote add upstream <upstream url>
git remote -v
```



