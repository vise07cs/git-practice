link --> https://github.com/ashokitschool/Ultimate_GitHub_Tutorial



# Git & GitHub Class Notes
-------------------------
Git is a version control software.
GitHub is a platform used to store all developers' project source code in one place.
On GitHub, we can create repositories to store project code.
All developers can connect to the GitHub repository for code integration (making code integration very easy).
GitHub allows tracking of all code changes:
Who modified
When modified
What was modified
Why modified


# Environment Setup
Create an account at github.com (free of cost).
Download & install Git client software: https://git-scm.com/downloads
Open Git Bash and configure your name and email:
git config --global user.name "your-name"
git config --global user.email "your-email"


# What is a GitHub Repository?
----------------------------------
A repository is a place to store project source code/files.
For each project, one GitHub repository is created.
Two types of repositories:
Public Repo: Anybody can see & you choose who can commit.
Private Repo: You choose who can see & who can commit.
Example:
Project Git Repo URL: https://github.com/ashokitschool/sbi_loans_app.git

Project team members use the repo URL to connect.

# Git Architecture
-----------------------------------------
Working Tree
Staging Area
Local Repository
Central Repository (Remote)


# Git Bash Commands
---------------------
git init              # Initialize working tree
git status            # Show working tree status
git add <file-name>   # Add file to staging area
git add .             # Add all files to staging area
git commit -m "msg"   # Commit staged files to local repo
git push              # Push local commits to remote/central repo
git restore <file>    # Unstage or discard changes
git log               # Show commit history
git rm <file-name>    # Remove a file
git clone <repo-url>  # Download remote repo to local
git pull              # Get latest changes from remote repo



session 2
============

git push              # Push local commits to remote repo
git restore       --> 2 purposes --> (1) if code is in staged area (git add) then git restore will bring that file back to unstaged area 
                                     (2) if code is in unstaged area , then git restore will unmodify/discard the changes made in file and roll it back to previous (latest staged ) version  .      

git log            --> display the commit history 
git rm              --> to remove the file locally(working tree)
* To delete the file from central repo (already pushed ) --> After git rm , you need to execute git commit and git push 
To delete the file from central repo  --> git rm <filename>  + git commit + git push 

git clone     --> to take the copy of the repository locally (from central to local )
        git clone <repo url >

cd project-directory    (Always cd to the directory which has .git)



git pull --> to download the latest changes made in the project from central repo to local repo 

(Q) --> Difference between git clone and git pull ?

git clone     --> to take the copy of the entire repository locally (from central to local )(to doenload the whole repo locally)
clone is genereally done only 1 time . (Suppose , You joined a company ,  you will be assigned a project to work on , now few develpers might be already working on  a project , So  only The 1st time you need to clone the entire repo locally )  

git pull     ---> to download only the latest changes made in the project from central repo to local repo 
It is done everyday , before starting the day to take the latest changes made in the central repository  by other developers 

At the end of day , you push the latest changes to the central repo (git push )


.gitignore -->Specifies files/folders to skip in Git operations

gitignore File
Example:
.settings
.classpath
.project
target/ 

(Q) --> what is .gitignore ?





# Session 3
===========

Branches in git 