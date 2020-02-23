# Bash_Syntax

[Development Notebook](Table%20of%20Contents.md)

___

## Table_of_Contents 
### Basic Concepts
[Helpful_Concepts_to_Understand](#Helpful_Concepts_to_Understand) <br>

### Directory_Navigation

[Print_Working_Directory](#Print_Working_Directory) <br>
[List](#List) <br>
[Change_Directory](#Change_Directory) <br>

### Directory_Adjustments

[Make_Directory](#Make_Directory) <br>
[Touch](#Touch) <br>
[Copy](#Copy)<br>
[Move](#Move) <br>
[Remove](#Remove) <br>

### Opening_and_Viewing

[Open](#Open) <br>
[Less](#Less) <br>
[Head](#Head) <br>
[Tail](#Tail)<br>

### Using_the_Terminal

[Manual](#Manual) <br>
[Exit](#Exit)<br>
[History](#History)<br>
[Clear](#Clear)<br>
[Echo](#Echo) <br>
[Say](#Say) <br>

### Reference

[References](#References) <br>

___
## Helpful_Concepts_to_Understand
### **Directories vs. Folders** <br>
Most people only use the term folder to refer to 'that thing that files are grouped together in on my computer'. Folders can do other things than just store files and are not exclusively used that way. The folders that are used specifcally to store files have a specific name, and that is 'directory'.

[superuser.com reference](https://superuser.com/questions/187900/what-is-the-difference-between-a-directory-and-a-folder)

### **Directory Paths**

Directories are nested within each other. A 'Directory Path' is a sequence that listes the specific directories that connect the directory that you are in to another directory at a more nested level. It is represented as a sequence of directory names, seperated by a forward slash `/`. Directory Paths output from the terminal will usually be the path from the highest level folder, known as the 'Home Directory', to the current folder you are in, known as the 'Working Directory'. Directory paths that start at the working directory and go elsewhere are uses in places such as hyperlinks within files.

[techterms.com reference](https://techterms.com/definition/path)
___

## Print_Working_Directory

The `Print Working Directory` command will return the directory path of the working directory relative to the home directory.

| Input | Return |
|---|---|
|`pwd`  |the terminal returns the address of the working directory <br> relative to the home directory | 
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
## Make_Directory
The `Make Directory` command is used to create a directory from the terminal.
| Input  | Side Effect |
|-----------------|--------|
|`mkdir NewName` | Creates a new folder within the current folder with the name NewFolder |
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

## Copy

The `Copy` command is used to create copies of files and folders.

| Input  | Side Effect |
|-----------------|--------|
|`cp Name NewName` | The terminal will create a copy of the Name file <br> and save it as NewName|
<br>

___

## Move
The `Move` command is used to move and rename files and directories.
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
## Open
The `Open` command is used to open applications and files from the Terminal.
| Input  | Side Effect |
|-----------------|--------|
| `open`| Opens the working directory in the finder|
| `open -a AppName`| Opens the application with the name AppName|
<br>

---

## Less

The `Less` command is used to view the contents of a text file without opening an editor.

| Input  | Return |
|-----------------|--------|
|`less file.txt` | The terminal will show the contents of the file.|

<br>

___

## Head

The `Head` command will cause the terminal to return the first 10 lines of the file. This command is useful to analyze logs or text files that change frequently.

| Input  | Return |
|-----------------|--------|
|`head file.txt` | The terminal will show the first ten lines of file.txt|
<br> 

---

## Tail

The `Tail` command will cause the terminal to return the last 10 lines of the file. This command is useful to analyze logs or text files that change frequently.

| Input  | Return |
|-----------------|--------|
|`tail file.txt` | The terminal will show the last ten lines of file.txt|
<br>

---



## Manual

The `Manual` command is used to look up the the specifications of commands within the terminal documentation for the specific command that is looked up.

| Input  | Return |
|-----------------|--------|
| `man rm` | Returns a documentation entry for the `Remove` command from the terminal <br> documentation.  |
<br>



---
## Exit

The `Exit` command will close a terminal window, end the execution of a shell script, or log you out of an SSH remote access session.

| Input  | Side Effect |
|-----------------|--------|
|`exit` | The terminal window will close|
<br>

---

## History 

The `History` command outputs a list of previous commands.

| Input  | Return |
|-----------------|--------|
|`history` | The terminal window will output a list of all previous commands|
<br>


---
## Clear 

The `Clear` command clears all previous commands and output from consoles and terminal windows.

| Input  | Side Effect |
|-----------------|--------|
|`clear` | The terminal window will be cleared of all previous commands|
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
|`Say String` | The computer will audible recite the String, <br> like in The Office episode|
<br>

____

## References

[Top 25 Commands and Creating Custom Commands](https://www.educative.io/blog/bash-shell-command-cheat-sheet)

[Command Line Hacks](https://www.cyberciti.biz/open-source/command-line-hacks/compgen-linux-command/)

---
[Top of Page](#Bash_Syntax)



