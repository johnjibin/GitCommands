#Unity3D

Important Commands to Setup Git on Mac OS and Solve Credential problems

Open Terminal and type following Commands

1. brew install git  
2. brew install --cask git-credential-manager-core

The Second Command Threw an error for me so used following two commands to setup
Error: Cask 'git-credential-manager-core' is unavailable: No Cask with this name exists.

3. brew tap microsoft/git      //The location of the files got changed as per documentation
4. brew install --cask git-credential-manager-core

----------------------------------------------------------------------------

#Switching Branch

1. git checkout <branch name>

----------------------------------------------------------------------------

#Fetch changes in remote repository

1. git fet <remote repo name>
2. git merge origin/<branch name>

----------------------------------------------------------------------------
