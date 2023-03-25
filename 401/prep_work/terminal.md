## Bash Command Line Tutorials

### The Command Line

Remember to use up and down arrows, echo $SHELL will tell me which shell I am using

### Basic Navigation

pwd to print working directory to see the path
ls to see all the files
ls -l to see timestamp as in long listing
ls /etc lists directory contents
ls -l /etc

paths can be absolute or relative
file system is hierachial, at the top of the structure is the root
. references your current directory
~ short cut for your home directory
.. reference to the home directory
cd change directory

### More About Files

Everything is a file, even the monitor!
Linux doesn't care about extensions.
Linux is case senstive.
There are no spaces in Linux! But you can workaround this via quotes and escape characters.
I do know about the tab completion shortcut. 
Start a file with "." to hide it. 

### Manual Pages
<b>man <command to look up>, such as man ls </b>
man -k <search term>, I tried this with "reading"
long hand begins with --
short hand begins with -
n will select the next found item when searching in a manual page

### File Manipulation
awww mkdir! and greatest hits touch!
I need to remember rmdir, cp, and mv (can also use to rename)
-v confirmation message with abbrev path
-p confirmation message with full path
rm removes a directory with content
rm -r removes directory and all files and directories within
use i to make the above command interactive

### Cheat Sheet

[Cheat Sheet](https://ryanstutorials.net/linuxtutorial/cheatsheet.php)