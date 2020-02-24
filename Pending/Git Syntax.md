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

**Examples** <br>
[Example 1](#) <br>
[Example 2](#) <br>
[Example 3](#) <br>
[Example 4](#) <br>
[Example 5](#) <br>

**References**

[References](#References)
_______________________________________________________
## Git_Concepts
### A_Basic_Explanation
If you have ever worked on something with multiply revisions, you have probably found yourself with a folder filled with 10 versions of the same file, with the filenames being things like "Final", "Final 2", "Final Final", "Final Fo Real", and so on. 'Version Control' is a technical term that refers to managing all the different versions of a project, be it an essay, or a program. 'Git' is a piece of software that automates 'Version Control'. In 'Git' the initial state of a folder is stored in memory as the starting point, and all of the changes made to that folder are sequentially stored as discrete sets of changes. 

When done properly Git allows a user to have every version of a project, and even parallel versions. Starting from an empty folder, you will make 'commits' which is analagous to hitting the save button. But unlike the save button, your commits are strung together sequencially, and do not override one another. So if you want to see what your file looked like two commits ago, you can do that. The save button is like watching a movie in theaters, you can't go back to previous scenes. Git is like watching that movie at home with the ability to rewind back to any point. 

Additionally, you can string commits together along multiply branches. Imagine you are painting a picture of a mountain. You commit at the point where you've painted a basic mountain, then you start drawing trees on the mountain and make a couple of commits of that. Then you go back to befores the trees and start painting snow on the mountain. The painting will have a line of commits up too a point, but then it will fork into two paths. At the end of one is the mountain with snow and at the end of the other is the mountain with trees. Git lets you do that.

In Git there are repositories, often just called 'repos', which are the folders where the program saves the starting point and the commits. You can have repos on you computer that you commit to, but you can also have repos offsite, accessed over the internet. You can copy the commits you make to local repos and send them over the web somewhere else. That is what Github.com and other places like it are for. 
### Staged_Changes_vs._Committed_Changes
In Git, everything you change in a file is tracked against the last commit you made. However you have the choice to decide what changes will ultimately be saved into the next commit. Once changes are typed into a file, there are two things that need to happen before they end up stored in a commit. The first is they have to be moved to the 'staging area'. The staging area is just an intermediate place between uncommitted changes and committed changes. You may never end up thinking about it too much. It is just another level given to people who may need it for some reason. The `add` command moves changes into the staging area. Once there, the changes are described as'staged'. From there, you move changes into a commit with the `commit` command. Each commit will be required to have a short message attached to it describing the commit. Once changes are within a commit, they are described as 'committed'.

_______________________________________________________
## Initiate
The `Initiate` command wil create a local github repository in the working directory. This has to be done before changes can be added or committed. <br>
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
The `Status` command will show what where in the repo there are staged and unstaged changes. <br>
| Input | Return | 
|---|---|
|`git status`  |The Terminal will output a list of filenames in font colors indicative <br> of whether the changes in those files are staged or unstaged.| 
<br>

_______________________________________________________
## Commit
The `Commit` command will store the staged changes as a new commit in the repo. A description is required for every commit, indicated by the "-m" which is for "message". <br>
| Input | Return | 
|---|---|
|`git commit -m "description"`  |A commit will be saved to the repo with a description. | 
<br>

_______________________________________________________
## Log
The `Log` command will make the terminal output a list of all commits stored in the repo along with there descriptions and timestamps <br>
| Input | Return | 
|---|---|
|`git log`  |The terminal output a list of all commits stored in the repo. | 
<br>

_______________________________________________________
## Remote
The `Command` command wil... <br>
| Input | Return | 
|---|---|
|`command`  |description | 
<br>

_______________________________________________________
## Push
The `Push` command wil... <br>
| Input | Return | 
|---|---|
|`git push <remote> <branch>`  |description | 
<br>

_______________________________________________________

## Terms to Catalog



`git clone`

`git pull`

`git checkout`

`git merge`

`git reset`

_______________________________________________________

## Sequence_Catalog_Entry_Format

Description of sequence and result

```bash
command
#comment
return
```

Description of instance 1 <br>
![](/git_status.png)

Description of instance 2 <br>

_______________________________________________________
## Sequences to Catalog


```bash
mkdir NewFolder
git init
touch NewFile.txt
#open the file and adjust the content
git add
git commit
```


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



____________________________________________________________
## References

[Essential Git Commands](https://dev.to/dhruv/essential-git-commands-every-developer-should-know-2fl)

[Basic Git Commands](https://confluence.atlassian.com/bitbucketserver/basic-git-commands-776639767.html)

[joshnh Git Commands](https://raw.githubusercontent.com/joshnh/Git-Commands/master/READMEpt.md)


____________________________________________________________

[Top of Page](#Git_Syntax)