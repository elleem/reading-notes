# Getting Git #

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
