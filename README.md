# HowToGit

Notes:
A bunch of usefuly gitcommands
All of the words <> must be replaced and do not include <>


Git workflow 

(1) git clone or git pull --> (2) (making changes) git add, git mv, git rm, etc 
-->(3) git commit -->(4) git pull, git merge ->(5) git push


#Usefull Git commands

$ git log                             //shows all the commits that have been made to repo
$ git status                          //shows any pending changing in the repo waiting to be commited
$ git checkout -f                     //Go back to the last working branch and the -f flag force overwrites 
$ git push origin <NAMEOFBRANCH>      //push your commited code to branch
$ git pull                            //pull the most up to date branch from github
$ git checkout <BranchName>           //Change to <BranchName>
$ git checkout -b <BranchName>        //create a new branch with the name <BranchName> and-b command flag means new  
$ git branch                          //check what branch you are on and what other branches are avaible 
$ git mv OldFile.rdoc NewFile.md      //change the name of a file
$ git commit -a -m "Improve the README file" //commit with -a add flag shortcut but DO NOT USE if you added new files
$ git branch -d <BranchName>          //delete a branch with the name <BranchName>        


#Setup up your config settings
$ git config --global user.name "Your Name"                  //Setup Name
$ git config --global user.email your.email@example.com      //Setup email
$ git config --global push.default matching                  //ensure forward-compatibility with an upcoming releases
$ git config --global alias.co checkout                      //Short cut to make checkout to co



#Starting a new repo
In this case you created a repo online and you want to clone it to your workspace.

$ git clone https://<USERNAME>:<PASSWORD>@github.com/<OWNER>/<REPO_NAME>.git <workspace>
  <USERNAME> with your GitHub username;
  <PASSWORD> with your GitHub password;
  <OWNER> with the username of the person who owns the repository;
  <REPO_NAME> with the name of your project’s repository; and
  <workspace> with the name for your workspace directory. Although optional, we will specify it here to create the     <workspace> directory.



#Starting a local Repo
Go to the home folder of the project on the terminal

$ git init
$ git add -A                               //Adds all files to be commited
$ git commit -m "Initialize repository"    //Commits all files with -m flag to write a comment

To push the local Repo to a github repo

$ git remote add origin https://github.com/<USERNAME>/<NAMEOFREPO>.git
$ git push -u origin master

