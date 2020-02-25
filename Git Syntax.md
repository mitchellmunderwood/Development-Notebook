# Git_Syntax
[Developement Notebook](Table%20of%20Contents.md)
_______________________________________________________

## Table of Contents
**Git_Concepts** <br>
[A_Basic_Explanation](#A_Basic_Explanation) <br>
[Staged_Changes_vs._Committed_Changes](#Staged_Changes_vs._Committed_Changes)


**Commands** <br>
[Initiate](#Initiate) <br>
[Add](#ADD) <br>
[Status](#Status) <br>
[Commit](#Commit) <br>
[Log](#Log) <br>
[Remote](#Remote) <br>
[Push](#Push) <br>
[Clone](#Clone) <br>
[Pull](#Pull) <br>
[Branch](#Branch) <br>
[Checkout](#Checkout) <br>
[Merge](#Merge) <br>

**Examples** <br>
[Initializing_a_Repo_and_Commiting_Changes](#Initializing_a_Repo_and_Commiting_Changes) <br>
[Add_and_Push_to_a_Remote_Repo](#Add_and_Push_to_a_Remote_Repo) <br>
[Change_Remote_Repo](#Change_Remote_Repo) <br>
[Clone_a_Repo](#Clone_a_Repo) <br>
[Delete_a_Local_Repo](#Delete_a_Local_Repo) <br>

**References**

[References](#References)
_______________________________________________________
## Git_Concepts
### A_Basic_Explanation
If you have ever worked on something with multiply revisions, you have probably found yourself with a folder of 10 versions of the same file, named things like "Final", "Final 2", "Final Final", and "Final For Real". 'Version Control' is a technical term that refers to managing all the different versions of a project, be it an essay, or a program. 'Git' is a piece of software that automates 'Version Control'. In 'Git' the initial state of a folder is stored in memory as the starting point, and all of the changes made are sequentially stored as discrete sets, called 'commits', that don't override one another. 

The saving technique you are probably use too is this: you have a file, you open that file, you make changes to that file, then you hit 'save'. The entire file is updated to whatever you currently have typed. Everything that was in the file before is completely replaced. But Git never overrides anything, it only adds to a string of existing commits. Therefore, nothing is ever lost.

Imagine you are walking through a city and have an app that tells you your current gps location. The is what the 'save' function is like. Now imagine you have another app that does two things, it saves the gps of where you started walking and then it keeps track of the turns you made in the city. Using the info from that app, you could go back to every point in the city that you went too. Git is the second app. It can recreate every version of your product because it has a list of all the changes that were made between one version and the next version. To get too any version of the project, git will just take the starting point and add all the commits that were done up too that point. 

You can also string commits together along multiply branches. Imagine you are painting a picture of a mountain. You commit at the point where you've painted a basic mountain, then you start drawing trees on the mountain and make a couple of commits of that. Then you go back to before the trees were painted and start painting snow on the mountain instead but save those commits along a different 'branch'. The painting will have a line of commits up too a point, but then it will fork into two paths. At the end of one is the mountain with snow and at the end of the other is the mountain with trees. Using Git you can have parallel versions of the same project. 

In Git there are repositories, often just called 'repos', which are the folders where the program saves the starting point and the commits. You can have repos on you computer that you commit to, but you can also have repos offsite, accessed over the internet. You can copy the commits you make to local repos and send them over the web somewhere else. That is what Github.com and other places like it are for. 

### Staged_Changes_vs._Committed_Changes
In Git, everything you change in a file is tracked against the last commit you made. However you have the choice to decide what changes will ultimately be saved into the next commit. Once changes are typed into a file, there are two things that need to happen before they end up stored in a commit. The first is they have to be moved to the 'staging area'. The staging area is just an intermediate place between uncommitted changes and committed changes. You may never end up thinking about it too much. It is just another level given to people who may need it for some reason. The `add` command moves changes into the staging area. Once there, the changes are described as 'staged'. From there, you move changes into a commit with the `commit` command. Each commit will be required to have a short message attached to it describing the commit. Once changes are within a commit, they are described as 'committed'.

_______________________________________________________
## Initiate
The `Initiate` command wil create a local git repository in the working directory. This has to be done before changes can be added or committed. <br>
| Input | Return | 
|---|---|
|`git init`  | A git repo will be created in the working directory| 
<br>

_______________________________________________________
## Add
The `Add` command wil move any changes to the staging area.  <br>
| Input | Return | 
|---|---|
|`git add +stuff`  |Changes will be moved to the staging area.| 
|`git add -A`  |All Changes will be moved to the staging area.| 
<br>

_______________________________________________________
## Status
The `Status` command will show where in the repo there are staged and unstaged changes. <br>
| Input | Return | 
|---|---|
|`git status`  |The Terminal will output a list of filenames, and the names will be <br> in font colors indicative of whether the changes in those files are <br> staged or unstaged.| 
<br>

_______________________________________________________
## Commit
The `Commit` command will store the staged changes as a new commit in the repo. A description is required for every commit, indicated by the "-m" flag, which is for "message". <br>
| Input | Return | 
|---|---|
|`git commit -m "description"`  |A commit will be saved to the repo with a description. | 
<br>

_______________________________________________________
## Log
The `Log` command will make the terminal output a list of all commits stored in the repo along with there descriptions and timestamps. <br>
| Input | Return | 
|---|---|
|`git log`  |The terminal output a list of all commits stored in the repo. | 
<br>

_______________________________________________________
## Remote
The `Command` command is used to store the online address of a remote repository. Once changes are commited to a local repository, these commits can be sent to the location of the remote repo using the `Push` command detailed later. <br>
| Input | Return | 
|---|---|
|`git remote`  |The terminal will output the list of remote repos.|
|`git remote -v`  |The terminal will output the list of remote repos <br> with URL addresses listed.|
|`git remote add <name> <address>`  |The remote repo name `<name>` will be recorded <br> and addressed to `<address>`. | 
|`git remote rename <old> <new>`|The name of the selected remote will be changed.|
|`git remote remove <name>` |The remote will be removed from the local repo.|
|`git remote set-url <name> <newurl>` |The address of the selected remote will be changed.|
<br>

_______________________________________________________
## Push
The `Push` command send all commits in the local repo to the designated remote repo. <br>
| Input | Return | 
|---|---|
|`git push <remote> <branch>`  |All commits from `<branch>` will be pushed <br> to the listed `<remove>` repo.| 
<br>

_______________________________________________________
## Clone
The `Clone` command will copy a remote repository to the working directory <br>
| Input | Return | 
|---|---|
|`git clone <url>`  |The remote repo at <url> will be copied to the working directory | 
<br>

_______________________________________________________
## Pull
The `Pull` command will fetch content from a remote repo and update the local repo to match the content. <br>
| Input | Return | 
|---|---|
|`git pull remote`  |The remote content will be merged into the local repo| 
<br>

_______________________________________________________
## Branch
The `Branch` command will make the terminal output the list of branches in the repo and show which branch you are currently on. <br>
| Input | Return | 
|---|---|
|`git branch`  |The Terminal will output the list of branches and the current branch.| 
<br>

_______________________________________________________
## Checkout
The `Checkout` command will provide details on the selected branch. <br>
| Input | Return | 
|---|---|
|`git checkout <branch>`  |The terminal will output details about the selected `<branch>`.| 
<br>

_______________________________________________________
## Merge
The `Merge` command will merge all commits from the selected branch into the master branch . <br>
| Input | Return | 
|---|---|
|`git merge <branch>`  |All commits in the `<branch>` will be moved into the master branch. | 
<br>

_______________________________________________________
## Initializing_a_Repo_and_Commiting_Changes
```bash
mkdir NewFolder #creates a new folder
cd NewFolder #make NewFolder the working directory
git init #creates a local repo in the new folder
touch NewFile.txt #create a new file
git add -A #the -A flag stages all changes
git status #to see the state of the staged changes
git commit -m "added a new file to the repo"
git log #should see the commit made"
```
_______________________________________________________
## Add_and_Push_to_a_Remote_Repo

``` bash
git commit -m "added a new file to the repo"
#create remote github repo on github.com, copy the repo address to the clipboard
git remote add origin https://github.address #adds a remote name 'origin' with the given address
git push origin master #pushes all commits from the master banch to the address of the 'origin' remote.
```
_______________________________________________________

## Change_Remote_Repo

``` bash
git remote -v #to view the current url attached to the remote repo
git remote set-url origin https://www.otheraddress.com #to change the url of the chose remote
```
____________________________________________________________

## Clone_a_Repo

```bash
mkdir NewFolder #create the folder to house the clone
cd NewFolder #make NewFolder the working directory
git pull https://github.com/sassypigeon/readmetest.git #clones the repo from the given address
```
____________________________________________________________

## Delete_a_Local_Repo
```bash
mkdir NewFolder
cd NewFolder
git init 
rm -rf .git #remove all git files within Newfolder
cd .. #go up a level
rm -R NewFolder #delete the folder
```
____________________________________________________________
## References

[Essential Git Commands](https://dev.to/dhruv/essential-git-commands-every-developer-should-know-2fl)

[Basic Git Commands](https://confluence.atlassian.com/bitbucketserver/basic-git-commands-776639767.html)

[joshnh Git Commands](https://raw.githubusercontent.com/joshnh/Git-Commands/master/READMEpt.md)

[Atlassian Git Tutorials](https://www.atlassian.com/git/tutorials)

[Atlassian Git Cheatsheet](Atlassian%20Git%20Cheatsheet.pdf)

____________________________________________________________

[Top of Page](#Git_Syntax)



