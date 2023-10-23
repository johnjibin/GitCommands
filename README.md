# Unity3D
<span style="color: green">This is a Green Header</span>


Important Commands to Setup Git on Mac OS and Solve Credential problems

Open Terminal and type following Commands

1. brew install git  
2. brew install --cask git-credential-manager-core

The Second Command Threw an error for me so used following two commands to setup
Error: Cask 'git-credential-manager-core' is unavailable: No Cask with this name exists.

3. brew tap microsoft/git      //The location of the files got changed as per documentation
4. brew install --cask git-credential-manager-core

--------------------------------------------------------------------------------------------

# configuring git user credentials

#Set username (local repository)
git config user.name "Your Name"

#Set username (global)
git config --global user.name "Your Name"

#Set email (local repository)
git config user.email "your@email.com"

#Set email (global)
git config --global user.email "your@email.com"





----------------------------------------------------------------------------------------------

# Creating branch and pushing changes

1. create a branch named johnjibin-patch-1
2. In terminal add the command git checkout -b johnjibin-patch-1   
3. create any new file ( I created a .cpp file)
4. git status --> To know the changes
5. git add .  --> Adding all the changes
6. git commit -m "First commit from local repo to branch"
7. git push -u origin johnjibin-patch-1

----------------------------------------------------------------------------

# Switching Branch

1. git checkout <"branch name">

----------------------------------------------------------------------------

# Fetch changes in remote repository

1. git fetch origin <remote repo name>
2. git merge origin / <"branch name">                //name of the branch from action done

----------------------------------------------------------------------------

# Uploading Large Files 

Reference - https://git-lfs.github.com/ 

1. git lfs install
2. Add .gitattribute file https://gist.github.com/nemotoo/b8a1c3a0f1225bb9231979f389fd4f3f
3. git config --system core.longpaths true  -> Some Unity files are with longer name tags
4. git lfs migrate info   -> To check larger files above 100mb
5. lfs migrate import --include="*.o,*.unity3d,*.bin,lld,dsymutil" -> the file types will get generate from 4th step
6. git status -u -> To display changes
7. git add .
8. git commit -m "comment"
9. git push origin


