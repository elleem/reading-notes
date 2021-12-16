# reading-notes

## growth mindset

![check out this picture](http://1.bp.blogspot.com/-0eyqmM-se1Q/VjKADy4KmRI/AAAAAAAAADQ/fRpPpNQ44UU/s1600/Growth-v-Fixed.jpg)

- *when we're growing, we're more productive!*
- **Your fundamental abilities can be developed via hard work**
- Like ice hockey, celebrating incremental achievements and never giving up, are the keys to improvement. 

Some methods to troubleshoot:
1. break the problem down into the smallest steps
1. talk it through
1. stay focused
1. take breaks
1. ***you never regret a practice that you attend instead of staying at home***
1. look at the good, bad, and ugly parts of your day to learn
1. see others as your teammates and not your competition
1. ~~I love a strikethrough~~


<!--i can hide things using html?-->

## About Me: 

My name is Lauren. I live in Seattle and I am currently an analyst with King County government. I have two corgis! Thanks for taking the time to look at my page.  Here is my [github page](https://github.com/elleem).

## Different Types of Texts Editors
* the basic *plain* text editor that came with your computer
* third party options
> * NotePad
> * TextWranger
> * BB Edit
> * Visual Studio Code
> * Atom
> * Brackets
> * Sublime text

*An IDE is a suite of different software, such as a text editor, file manager, compiler, and a debugger (MS Outlook).*

## Cheat Sheet ##

### The Command Line ###

#### a text based interface to the system ####
- user@bash
- command line arguments
- options are used to modify the behaviour of the command, usu listed before other arguments and typically start with a dash (-)
- provides the information
- prompts us for the next command

#### the shell ####
- part of the system that defines how the terminal will behave

#### commands ####
- echo
- use up and down keys to navigate, don't re-enter
- pwd print working directory
- ls list
- pwd print working directory
- square brackets [] means that the command is optional
- "-l" is long listing

#### paths ####
1. absolute
2. relative
3. root directory "/"
4. relative paths do not start with "/"
5. ~ tilde
6. . (dot) hidden
7. ..(dotdot)
8. cd change directory
9. ">> " insert.html inserts into folder
10. look at /etc /var/log /bin /usr/bin

#### everything is a file ####
- file.exe
- file.text and so forth

#### be careful ####
 - spaces
 - case
 - use quotes to search for an item with a space in the title
 - use \ to negate the space 

### Version Control ###
- use VCS to allow you to save drafts
- allows you to save on your drive, or collaborative save CVCS, admin rights
- DVCS distributed as fail safe, spec mirror repositories

### Git ###
- allows snapshots, usu local, really effective at tracking changes, good at preventing loss of data
- 3 states: committed, modified, staged
- data stored locally, changed but not committed to db, flagged a file's changed version to be committed
- git config, set up email and username
- git config --global. user email will apply to all projects, you can specify user names, projects if needed
- to see all your settings git config --list
- could be using the default text editor, so you can config this as well git config --global core.editor emacs
- help:  git help command  git command --help  man git-command

### Switch to the project's directory ###
- cd test
- git init
- git add LICENSE
- git commit -m 'any message here'

### Cloning ###
git clone 

### Local repository structure ###
Working Directory: The actual files reside here.
Index: The area used for staging

### saving changes ###
files are tracked or untracked

### check file status ###
- git status
- git add filename (specify file)
- git add (tracks all) 

### committing a file ###
- commit changes and record what you did with the commit message
- git commit -m 'made change x,y,z'
- git commit -a will commit all changes
- git push origin master pushes changes to a remote repository, esp for cloned repositories
- git stash when you're not ready to commit changes, but don't want to lose them, also temp removes changes, hides, for a clean working directory
- git stash apply allows you to reapply stashed hidden changes

### seeing your remote ###
git remote view all specified remote handles
git remote -v, view all remote URLS next to their corresponding short names
Head: Points to the most recent commit
