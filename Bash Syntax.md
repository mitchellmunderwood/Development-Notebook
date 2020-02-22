# Bash Syntax
## Table of Contents 
[Change_Directory](#Change_Directory) <br>
[Print_Working_Directory](#Print_Working_Directory) <br>
...etc...
___
## Helpful Concepts to Understand
### **Directories vs. Folders** <br>
Most people only use the term folder to refer to 'that thing that files are grouped together in on my computer'. Folders can do other things than just store files and are not exclusively used that way. The folders that are used specifcally to store files have a specific name, and that is 'directory'.

[superuser.com reference](https://superuser.com/questions/187900/what-is-the-difference-between-a-directory-and-a-folder)

### **Directory Paths**

Directories are nested within each other. A 'Directory Path' is a sequence that listes the specific directories that connect the directory that you are in to another directory at a more nested level. It is represented as a sequence of directory names, seperated by a a forward slash `/`. Directory Paths output from the terminal will usually be the path from the highest level folder, known as the 'Home Directory', to the current folder you are in, known as the 'Working Directory'. Directory paths that start at the working directory and go elsewhere are uses in places such as hyperlinks within files.

[techterms.com reference](https://techterms.com/definition/path)
___

## Print_Working_Directory

The `Print Working Directory` command will return the directory path of the working directory relative to the home directory.

| Input | Return |
|---|---|
|`pwd`  |the terminal returns the address of the working directory <br> relative to the home directory | None |
<br>

___
## List
The `List Directories` command will return a list of all directories and files nested within the working directory <br>
| Input | Return | 
|---|---|
|`ls`  |the terminal returns a list of all files and folders nested within <br> the working directory | 
<br>

___

## Change_Directory

The `Change Directory` command is how you change the working directory to another directory, going up or down one level at a time, or returning to the home directory and navigating from there.
| Input  | Side Effect |
|-----------------|--------|
|`cd Name`  |The working directory transitions down a level to the folder <br> named Name |
|`cd .. `          |The working directory transitions up a level|
|`cd` |The work directory becomes the home directory
|`cd ~ `           |The working directory becomes the home directory. The <br> '~' represents the home directory when using the `cd` command.|
|`cd ~/Docs` |The working directory starts at the home directory and the <br> transitions down to the Docs folder. When navigating to a <br> folder from the home directory, the '~' is required.|
<br>

___

Reformatt what is below in above style

---

## Open
The `Open` command is used to open applications and files from the Terminal.
| Input  | Side Effect |
|-----------------|--------|
| `open`| Opens the working directory in the finder|
| `open -a AppName`| Opens the application with the name AppName|
<br>

___
## Make_Directory
The `Make Directory` command is used to create a directory from the terminal.
| Input  | Side Effect |
|-----------------|--------|
|`mkdir NewName` | Creates a new folder within the current folder with the name NewFolder |
<br>

___

## Move
The `Move Directory` command is used to move and rename files and directories.
| Input  | Side Effect |
|-----------------|--------|
|`mv Name NewName`|renames 'Name' to 'NewName'|
|`mv Name ~/Name`|Moves the Name file/folder from the current directory to <br> user's home directory.|
|`mv Name Subdir/Name`|Moves Name file/folder to 'Subdir/Name' relative to the <br> working directory |
|`mv Name Subdir`|Same as the previous command, Name is implied to be <br> the same.|
|`mv Name Subdir/NewName`|Moves 'Name' to 'Subdir' named  'NewName'|
<br>


___

## Remove
The `Remove` used for deleting files and folders from the directory tree. This type of deletion is permanent, as oppsed to placing a file inside the trash bin.
| Input  | Side Effect |
|-----------------|--------|
|`rm file.txt` | Deletes the file with name file.txt within working directory |
|`rm -R DirName` | Deletes the subdirectory with name DirName, utilizes the `-R` flag|
<br>

---

## Echo
The `Echo` command returns the string passed to it.
| Input  | Return |
|--------|--------|
| `echo String` | The terminal will return the given String |
<br>

---

## Say
The `Say` command causes the terminal to audible receite the string passed to it.
| Input  | Side Effect |
|-----------------|--------|
|`Say String` | The computer will audible recite the String, like in The Office episode|
<br>

---

## Touch
The `Touch` command is used to create a new file or directory
| Input  | Side Effect |
|-----------------|--------|
| `touch file.ext` | create a file in the working directory names file.ext |
| `touch NewName` | create a directory in the working directory with the name NewName|
<br>
 
---

<br>
<br>
<br>

# Under Construction

`man`

`grep`

`rmdir`

`locate`

`less`

`compgen`

https://www.cyberciti.biz/open-source/command-line-hacks/compgen-linux-command/

`cat`

`|`

`head`

`tail`

`exit`

`chmod`

`clear`

`copy`

`kill`

`sleep`

`alias`

# How to create your own custom Bash commands

https://www.educative.io/blog/bash-shell-command-cheat-sheet

Custom commands in Bash are known as “aliases”. Aliases are essentially an abbreviation, or a means to avoid typing a long command sequence. They can save a great deal of typing at the command line so you can avoid having to remember complex combinations of commands and options. There is one caveat to using aliases, and that is to be sure you don’t overwrite any keywords.

Syntax: `alias` alias_name = “command_to_run”

A very simple example would look like this:

`alias` c = “clear”

Now every time you want to clear the screen, instead of typing in “clear”, you can just type ‘c’ and you’ll be good to go.


---

## Bash Command Quick Reference Table

| Command Name | Terminal Input | Output| Output Description |
| --- | --- | --- | ---  
