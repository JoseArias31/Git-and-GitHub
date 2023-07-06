# Git

*After Installing Git, let's learn some Git concepts.

-Git Bash: It's the tool that will operate any commands with the file locally.

It is easy to open, just go to Windows search and type Git Bush.

Commands:

-cd: Change Directory
if a text has many spaces in between, instead of typing: cd Folder to Create a new project. we should try with "": "Folder to Create a new project" 
-cd ..: This command is useful to go back to the previous folder.
-cd: This command is to go  to the main root location

If I want to create a new folder:
-mkdir: Make Directory = mkdir new folder
-ls: I can use this command to see what files are in the current file.
-rmdir: remove Directory
-clear: It works to clear the tool.

*This section is to configure the user credentials where other programmers can see who made changes and from where (email address):

-git config --global user.name "Jose Arias": This is to operate all the changes in all the repositories in GitHub.
To see the name added: 
-git config user.name
output: Jose Arias

-git congig --global user.email "gojosearias@gmail.com"

*Create a new Repository with Git Bash

Inside the folder we are going to work on, we run the following command:

-git init

master is the name of the branch by default after running the previous command, if we want to get a new different branch name, we can run the following command:

-git config --global init.defaultBranch main
in  this case, the new branch name will be "main"

However, we need to delete the branch created with the git init command about, so the git folder or repository created is hidden, we need to enable hidden folders and remove it manually, after that, run git init with the new branch "main"


*3 ways in Git.

-Working Directory: Folder of the project in Windows
-Staging Area: Files or changes that will be added in the following commit.
-Repository: directory.git

*Commit:

-git commit -m "Testing"

after making the commit action, it is saved automatically, now, to check all the commits made, we can run the following command:

-git commit = running only this command, I will be able to add a text on my VSCode tool already set up. So basically I have to text in there, save and close it to save.

-git log.

Every time I want to add files to commit my files in case I have multiple files, I can run the following command:

-git add .   So, the "." means all the files.

*Modify a commit

git commit --amend: To make changes, this command is useful only "locally" It means, in my PC. However, it's strongly recommended for the last commit made.

*Reset commits: 

-git reset --soft HEAD~1 This command is used to remove the last commit made however, this command will not remove the changes in my VSCode.





