# HowToGit

Notes:
A bunch of usefuly gitcommands



Git workflow 

(1) git clone or git pull --> (2) (making changes) git add, git mv, git rm, etc 
-->(3) git commit -->(4) git pull, git merge -->(5) git push


#Usefull Git commands

**$ git log** &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; //shows all the commits that have been made to repo   
**$ git status** &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; //shows any pending changing in the repo waiting to be commited  
**$ git checkout -f** &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; //Go back to the last working branch and the -f flag force overwrites   
**$ git push origin NameOfBranch** &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; //push your commited code to branch  
**$ git pull** &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; //pull the most up to date branch from github  
**$ git checkout BranchName** &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; //Change to BranchName  
**$ git checkout -b BranchName** &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; //create a new branch with the name BranchName and-b command flag means new    
**$ git branch** &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; //check what branch you are on and what other branches are avaible   
**$ git mv OldFile.rdoc NewFile.md** &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; //change the name of a file  
**$ git commit -a -m "Improve the README file"** &nbsp;&nbsp; //shortcut add, DO NOT USE if you added new files  
**$ git branch -d BranchName** &nbsp;&nbsp;&nbsp;&nbsp; //delete a branch with the name BranchName          


#Setup up your config settings
**$ git config --global user.name "Your Name"** &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; //Setup Name  
**$ git config --global user.email your.email@example.com** &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; //Setup email  
**$ git config --global push.default matching** &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; //ensure forward-compatibility with an upcoming releases  
**$ git config --global alias.co checkout** &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; //Short cut to make checkout to co  



#Starting a new repo
In this case you created a repo online and you want to clone it to your workspace.  

**$ git clone https://USERNAME:PASSWORD@github.com/OWNER/REPO_NAME.git workspace** </br>     
  USERNAME with your GitHub username;  
  PASSWORD with your GitHub password;  
  OWNER with the username of the person who owns the repository;  
  REPO_NAME with the name of your project’s repository; and  
  workspace with the name for your workspace directory. Although optional, we will specify it here to create the       workspace directory.  



#Starting a local Repo
Go to the home folder of the project on the terminal  

**$ git init**  
**$ git add -A** &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; //Adds all files to be commited  
**$ git commit -m "Initialize repository"** &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; //Commits all files with -m flag to write a comment  

To push the local Repo to a github repo  

**$ git remote add origin https://github.com/USERNAME/NAMEOFREPO.git**  
**$ git push -u origin master**  

