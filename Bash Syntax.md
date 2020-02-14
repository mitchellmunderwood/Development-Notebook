# Bash Syntax

`cd`		 change directory 

> `cd ..` ascend one node up in the file directory tree
>
> `cd ~` changes to the home directory of the user
>
> `cd ~/Desktop` changes to the home folder and then to the Desktop folder one level down
>
> `cd FolderName` decend from the current folder into the subfolder with the specficied FolderName

`pwd`	   print working directory

> `pwd` causes the terminal to output the folder address of the current node

`ls`		 list 

> `ls` causes the terminal to output a list of the files and folders contained within the current folder 

`open` 	open

> `open .` opens the current folder in the finder
>
> `open -a ApplicationName` opens the application with the specied ApplicationName

`mkdir`   make directory

> `mkdir NewFolder` creates a new folder within the current folder with the name NewFolder 

`mv`         move

`rm` 	    remove: used for deleting files and folders from the directory tree. This type of deletion is permanent, as oppsed to placing a file inside the trash bin     

>

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