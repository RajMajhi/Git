# Complete Git & GitHub Guide (All-in-One)

**Author:** Raj Majhi  

This repository is a complete beginner-to-intermediate reference for **Git and GitHub**.  
It explains what Git/GitHub are, how they work, and includes **well-commented commands** with their uses.

---

# 📌 What is Git?

Git is a **free and open-source Version Control System (VCS)** used to track changes in source code.

### ✅ Uses of Git
- Track project history  
- Revert to older versions  
- Work safely on large projects  
- Collaborate with multiple developers  

---

#  What is GitHub?

GitHub is a **web platform** that hosts Git repositories and helps developers collaborate, review code, and manage projects online.

It is like a **social platform for developers**, where repositories can be pushed, cloned, reviewed, and improved.

---

# 🧾 What is a README?

A `README.md` file describes:
- What the project does  
- How to install and use it  
- Commands and documentation  

Markdown (`.md`) helps format content on GitHub.

---

# ⚙️ Installing & Checking Git

```bash
git --version        # Checks whether Git is installed and shows the version

git config --global user.name "Your Name"        
# Sets your name for all repositories (global configuration)

git config --global user.email "youremail@example.com"  
# Sets your email (use the same one as GitHub)

git config --list    
# Displays all configured Git settings

Basic system Commands (Used in Git)
ls            # Lists files and folders
ls -a         # Lists all files including hidden ones
pwd           # Shows current working directory
cd folder     # Moves into a folder
cd ..         # Moves one step back
mkdir name    # Creates a new directory
clear         # Clears the terminal screen


Creating a New Repository
git init      
# Initializes a new Git repository (creates hidden .git folder)

git status    
# Shows current state of files (tracked, untracked, modified, staged)

Cloning a Repository 
git clone <repo-link>   
### Creates a copy of an existing GitHub repository on your system ###


File states in git
Untracked → New file (Git doesn’t track yet)
Modified → File changed
Staged → Ready to commit
Unmodified → No changes

Adding Files to Staging Area # Staging means preparing files for commit.
git add file.txt    
# Adds a specific file to staging

git add .           
# Adds all changed and new files to staging

Committing Changes # Commit = record of change
git commit -m "Your message" # Saves a permanent snapshot of staged changes with a message

Connecting local repo to github
git remote add origin <repo-link>  
# Connects local repository to GitHub

git remote -v  
# Shows connected remote URLs

Pushing Code to Github
git push origin main  
# Uploads commits from local system to GitHub

git push -u origin main  
# Sets upstream so future pushes need only: git push

Pulling Code from Github
git pull origin main  
# Downloads changes from GitHub and updates local repository

Branching (Working in Parallel) # Branches are used for features, fixes, and experiments.
git branch                 
# Lists all branches

git branch new-branch      
# Creates a new branch

git checkout new-branch    
# Switches to that branch

git checkout -b feature    
# Creates and switches to a new branch

git branch -d branch-name  
# Deletes a branch

git branch -M main         
# Renames current branch to main


Merging Branches 
git diff branch-name       
# Shows differences before merging

git merge branch-name      
# Merges specified branch into current branch

Resolving Merge Conflicts
Open conflicted file
Fix code manually
Add file again
Commit changes

git add .
git commit -m "Resolved merge conflict"


🧲 Pull Requests (PR)
A Pull Request lets you:
Propose changes
Get reviews
Merge branches safely on GitHub

Used heavily in team projects.

Viewing History
git log           
# Shows detailed commit history

git log --oneline 
# Shows short commit history

⏪ Undoing Changes
git restore file.txt       
# Discards changes in a file (not staged)

git reset file.txt         
# Unstages a staged file

git revert <commit-id>     
# Safely undo a commit by creating a new commit

git reset --hard <id>      
# Deletes commits and changes permanently (use carefully)

📦 Temporary Save (Stash)
git stash        
# Temporarily saves uncommitted changes

git stash pop    
# Restores stashed changes

🔍 Inspecting & Comparing
git show <id>      
# Shows details of a specific commit

git diff          
# Shows unstaged changes

git diff --staged 
# Shows staged changes

🔄 Workflow
Create / Clone Repo
        ↓
  Make Changes
        ↓
     git add
        ↓
    git commit
        ↓
     git push
        ↓
      GitHub

#This repository is created for learning, practicing, and revising Git & GitHub.
It connects all major concepts in one place with clear commands and uses.

If someone want they can PR me for an Edit...
Happy Learning & Building
@RajMajhi 

