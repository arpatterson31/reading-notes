#### Table of Content
[Git](#git)    
[Importing](#importing)   
[Cloning](#cloning)    
[Committing](#committing-a-file)  
[Command Key](#command-key)   
   
   

# Git
What is Git?  
*Git is a distributed version-control system that tracks changes, or commits, in files used by coders during software development.*  

### Perks 
+ All changes are tracked - easy to detect file corruption or loss of information
+ Minimize the loss of data
+ Operation benefit - stored on local disk and not a server

### States 
Files in Git fall under 3 main states:
+ Committed - data is stored to database
+ Modified - changed but not committed
+ Staged - flagged to be committed in next round


## Setting up a Git Repo

### Importing
1. `$ cd test (cd = change directory)` - Switch to target project directory
1. `$ git init` - creates a new subdir named .git that has the repo files - no tracking at this point
1. to start tracking
   + `$ git add *.c`
   + `$ git add LICENSE`
   + `$ git commit -m "any message here"`  


### Cloning
1. `$ git clone https://github.com/test` - creates copy by using repo's URL
1. `$ git clone https://github.com/test mydirectory` - clone repo into a directory with another name

### Committing a File
+ `$ git commit -m "made change blah blah blah"`
+ `$ git commit -a` - commits all changes


### Command Key

|**commands** | **action** | 
|-------------------|-----------------------|
|`git config --list` | check settings |
|`git help command` `git command --help` `man git-command`| getting help |
|`git status` | file state |
|`$ git commit -m "made change x,y,z"`| commits file |
|`$ git commit -a`| commits all changes |




##### Helpful Resources
[Git & GitHub Video Tutorial](https://www.youtube.com/watch?v=RGOj5yH7evk)
