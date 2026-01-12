# Git
Trying GIT
<br>
Author - RajMajhi

<pr>
//Git?
 Git is a Version Control System Popular, free & open source,  Fast & Scalable.
 // VCS is a tool that helps to track changes in code.

Ex : 
1. TO TRACK THE HISTORY 
 lets say we are working on a project like building a signup page, Here we added lot of things but now want to change those things as they were before, now we can do it manually as it is small scale project but what about large scale projects, In large scale project it's too risky to commit changes and on that if you do it manually it means you need to delete  files one by one which can be hectic, So here comes GIT which actually automates those works for you, with Git we can go back and forth i.e initial stage and updated stage./

2. COLLABORATE
 It's just as it sounds 'Collaborate', with the help of git we can collaborate with others to work on an project. Apart from sole projects, There are large projects from Companies where we need to work in a team, Which actually can messup if there is no proper co-ordination. 
 Like on such projects there are lot of developer are working so it is very difficult to find out who made the changes, shall we accept those changes?, And to prevent OverWrite too. So to avoid such issues we use git./

//Github?
 Is a Website that allows developers to store and manage their code using Git.
 https://github.com

 This code is then reviewed by other developers or HR for job purpose.

 We can say that Github is like instagram but it is specifically for developers, 
 Here, Developers post(PUSH) their folders(REPOSITORY), Even copy(CLONE) others Repository and perform changes(COMMIT)./

Let's dive into git and github

TO OPEN AN ACCOUNT ON GITHUB 
//Need email, Can be personal or college, while college email give lots of other features but generally we should prefer using our own personal email.
Password & Username...

AFTER LOGIN TO GITHUB
you'll see

Overview, Repositories, Projects, Packages, Stars.

//Task after GitHub Account - 
# Create a new repo : {name can be anything},
# make our first commit.
 git and github uses 2 step process before updation i.e,
  ADD then COMMIT
    When we perform some changes we ADD them here the changes are temperory but when we release it i.e COMMIT it is Permanent. 
    but on github the add step is geenerally skipped and we can directly Commit.

    Github saves the commits in the form of history.

//Commit message - here we need to write the change we made.    

//Initial commit - The first ever change we make after initial comes Update this are the secondary changes.

Repositories> New> Repositoryname{write here}> other options are optional.> Create repository.

//Readme? 
 Readme is a special type of file which include details about the project like name, what is the project about, and steps how to use the project, etc... 
 Generally adding readme is a good thing. 

 Readme.md <-- md stands for markdown.

//setting up Git
can be done in 
Visual studio code (VScode)
Windows (Git Bash)
Mac (Terminal)
website : git-scm.com

// To check git 
git --version {Git version}
ls - {list all the files.}
pwd - {to check working directory}

// Configuring Git
It is important step as here we'll connect git and github.

There are 2 types of configurations 
1. Global - The whole system.{Single user}
2. Local - Specific repo.{Multiple user}

git config --global user.name"My name"
git config --global user.email"someone@email.com" {use the same email & name that you used on github.}
git congig --list


# GIT BASIC COMMANDS
Remote {github}
Local {laptop / pc}

// Clone & Status 
Cloning a repository on our local machine.
 git clone <link>

 Go to github > Repo > Code > Clone > HTTPS {copy the link}.

Status
Displays the state of the code.
 git status

 There are 4 types of status
 1. untracked - new files that git doesn't yet track.
 2. modified - changed.
 3. staged - file is ready to be committed.
 4. unmodified - unchanged.

cd - {Change directory}
 cd directory name

There are two types of file {Directories}
 1. Hidden , ls -a
 2. Non-Hidden , ls

// Add & Commit
Add- adds new or changed files in your working directory to the Git staging area.
 git add<-filename-> for single file.
 git add . for all files

Unmodified - add (untracked) - commit

Commit- it is the record of change
 git commit -m "some message"

// Push Command
 push- upload local repo content to remote repo

 git push origin main 
  here the origin is the repo on github and the main is the branch.

// Init Command
 init- used to create a new git repo
cd .. {used to come out of and directory}
mkdir {It's used to make a new directory}
 
 git init
 git remote add origin<-link->
 git remote -v (To verify remote)
 
 git push -u origin main

// Git Branch 
 To understand branch let's say we have 3 teams
 1 Frontend team
 2 backend team
 3 bugfix team 
So all 3 teams are working on a same project and for a smooth working they all made a copy(BRANCH) of the real program. 
Just like a tree have lot of branch right. here all the branches comes from the main.

git branch (To check branch)

master branch is a default branch but on github it is changed to main.{I am talking about the name.}
So that's why we need to change to name of our branch to main from master before push.

git branch -M main (To rename branch)

git checkout <-branch name-> {To navigate}
git checkout -b <-new branch name-> {To create new branch}
git branch -d <-branch name-> {To delete branch}

// Workflow
Local Git
github repo
  |
clone
  |
changes
  |
add
  |
commit
  |
push

// Merging Code
way1
git diff <-branch name-> {to compare commits,branches,files&more}
git merge<-branch name-> {to merge2branches}

way2
create a PR

// PR- Pull Request
It lets you tell others about chnages you've pushed to a branch in a repository on GitHub.

// Pull Command
Used to fetch and download content froma remote repo and immediately update the local repo to match that content.
git pull origin main

// Resolving Merge Conflicts
An event that takes place when Git is unable to automatically resolve differences in code between two commits.

git merge <-branch name->
The error occur while merging is called conflict..
</p>
