# Bash Syntax
## Table of Contents 
[Change_Directory](#Change_Directory) <br>
[Print_Working_Directory](#Print_Working_Directory) <br>
...etc...
___
## *Change_Directory*
**cd** +stuff
```
cd FolderName   descend from the current folder into the subfolder with the name of FolderName
cd ..           Takes you to the directory one level about your current level
cd ~            Takes you to your root directory
cd ~/Desktop    Changes to the root directory and then to the Desktop folder one level down
```
___

## *Print_Working_Directory*
**pwd**

| pwd  | causes the terminal to output the folder address of the current folder |
| ---- | ------------------------------------------------------------ |


___
## *List_Contents*
**ls**

```
ls              The Terminal will output a all files and folders within the current folder 
```
___
## *Open_a_File,_Folder,_or_Application*
**open** +stuff
```
open                          Opens the current folder in the finder
open -a ApplicationName       Opens the application with the specied ApplicationName
```
___
## *Make_a_Directory*
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