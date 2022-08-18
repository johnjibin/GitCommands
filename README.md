#Unity3D

Important Commands to Setup Git on Mac OS and Solve Credential problems

Open Terminal and type following Commands

1. brew install git  
2. brew install --cask git-credential-manager-core

The Second Command Threw an error for me so used following two commands to setup
Error: Cask 'git-credential-manager-core' is unavailable: No Cask with this name exists.

3. brew tap microsoft/git      //The location of the files got changed as per documentation
4. brew install --cask git-credential-manager-core

--------------------------------------------------------------------------------------------

#Creating branch and pushing changes

1. create a branch named johnjibin-patch-1
2. In terminal add the command git checkout -b johnjibin-patch-1   
3. create any new file ( I created a .cpp file)
4. git status --> To know the changes
5. git add .  --> Adding all the changes
6. git commit -m "First commit from local repo to branch"
7. git push -u origin johnjibin-patch-1

----------------------------------------------------------------------------

#Switching Branch

1. git checkout <branch name>

----------------------------------------------------------------------------

#Fetch changes in remote repository

1. git fetch origin <remote repo name>
2. git merge origin/<branch name>                //name of the branch from action done

----------------------------------------------------------------------------

