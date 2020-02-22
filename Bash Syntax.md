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

| Input | Return | Side Effect |
|---|---|---|
|`pwd`  |the terminal returns the address of the working directory relative to the home directory | None |
<br>

___
## List_Directories
The `List Directories` command will return a list of all directories and files nested within the working directory <br>
| Input | Return | Side Effect |
|---|---|---|
|`ls`  |the terminal returns a list of all files and folders nested within the working directory | None |
<br>

___

## Change_Directory

The `Change Directory` command is how you change the working directory to another directory, going up or down one level at a time, or returning to the home directory and navigating from there.
| Input | Return | Side Effect |
|---|---|---|
|`cd Name`  | nil|The working directory transitions down a level to the folder named Name |
|`cd .. `          | nil|The working directory transitions up a level|
|`cd`| nil |The work directory becomes the home directory
|`cd ~ `            | nil|The working directory becomes the home directory. The '~' represents the home directory when using the `cd` command.|
|`cd ~/Docs`    | nil|The working directory starts at the home directory and the transitions down to the Docs folder. When navigating to a folder from the home directory, the '~' is required.|
<br>

___

Reformatt what is below in above style

---

## *Open_a_File,_Folder,_or_Application*
**open** +stuff
```
open                          Opens the current folder in the finder
open -a ApplicationName       Opens the application with the specied ApplicationName
```
___
## *Make_Directory*
**mkdir** + FolderName

```
mkdir FolderName              Creates a new folder within the current folder with the name NewFolder 
```
___




`mkdir`   make directory

> `mkdir NewFolder` creates a new folder within the current folder with the name NewFolder 

`mv`         move

`rm` 	    remove: used for deleting files and folders from the directory tree. This type of deletion is permanent, as oppsed to placing a file inside the trash bin     

>`rm new_file.txt` deletes a file
>
>`rm -R new_directory` deletes a directory, utilizes the `-R` flag in conjuction with the `rm` command

`echo`

> `echo String` causes the computer to return the string in the terminal

`say`

> `say Sting` causes the computer to speak the given string aloud

`touch`   touch: command that creates files and can also be used to adjust file timestamps

> `touch NewFile.txt` creates a file of type text `txt` with the name `NewFile`
 
<br>
<br>
<br>

# TO BE FORMATTED

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

| Command Name | Terminal Input | Return | Side Effect |
| --- | --- | --- | ---| 
