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

git commit --amend: To make changes, this command is useful only "locally" It means, in my PC. However, it's strongly recommended for the last commitment made.

*Reset commits: 

-git reset --soft HEAD~1 This command is used to remove the last commit made however, this command will not remove the changes in my VSCode.

*Make a new branch and modify branches. 

-git branch javascript = so basically I add the name after the git branch command
-git branch = it shows all the branches created.
-git checkout javascript = I can switch branches with this command, from master to javascript
-git checkout -b python = This command is to create a new branch and switches it to the new one.
-git branch -m "version-js" = We need to stay on the branch we want to change the name and run this command with the new branch name.
-git branch -m python version-python = This is a way to change the branch name, after the -m line we type the current branch name and the new one, we can still be in our main or master branch.

*Remove a branch
-git branch -d version-py

*Make a commit with a branch that is not the main (master) one.

Basically, we need to switch branches and make the change, after adding the change to be committed, we run the command git add . and the new changes are in the new branches, not in the main (master) one.

While we are in the branch we just created and made changes, we can see all the commitments made with git log, however, we can use the following command to see them clearly.

-git log --oneline

-git log -p = we can see the changes made on Visual Studio Code

*Merging Branches=

To merge branches, we need to stay in the main (master) one before continuing.
-git merge expanded-text

*Issues with branches after being merged.

Once branches are merged, we can delete the branch we used to modify and add to the main (master) one. git branch -d

--In case we have a "conflict" we need to accept all the changes on my code editor before continuing, once the changes are accepted on VSCode, we should run the command:

*git  merge --continue


# GitHub

After creating a GitHub account and setting up all the settings properly. 

Let's clone a repository:

On git bash, we type:

-git clone GitHub Link.

-git remote = This command run the name of the remote repository.

-git remote -v = Here we can see the ways we can push our changes.
Fetch = Finds the changes
push = Send the changes

*Send changes from local repository to remote repository with git push

*Before pushing the changes, we need to protect our email address, this is the way to change the current personal emaail address to a Github Email:

-Click on my photo on GitHub
-Settings
-Emails
-Copy GitHub Email
-Open Git Bash
-git config --global user.email 115059715+JoseArias31@users.noreply.github.com


*Tokens with HTTPS

Every time I use git with GitHub, I have to authenticate my account and synchronized both tools, there is an easy way to do it:

1-Clasic sign in with the GitHub credentials.
2-By using tokens(This is only for personal security access):

-On GitHub click on settings
-<>Developer settings
-Personal Access Token
-Tokens (Classic)
-Click on Generate a personal access token
-Type a note
-Set an expiration time
-Select a scope
-Finally click on Generate Token
-On the sign-in option, instead of clicking on sign-in, we can select the Token option instead.

*To Pull documents from GitHub to our local repository:

-git pull origin main = Keep in mind we need to be on the branch we want to pull from.

*Git fetch works to validate the changes made without changing anything from our repositories if so, we can git pull the changes.

-git fetch origin =works as a command to check the commit made so far.

*Now, to push files to a remote repository from a local repository, we need to make sure that we have created a folder and have done the setup to start a new local repository with a git init.

A good way to see if the repository is not ready to pull documents, we should run:
-git remote -v = This will display no messages which means the local repository is not connected with the remote one.

-Let's create a new repository on GitHub to see the lines commands to connect both repositories.

-git remote add origin https://github.com/JoseArias31/Testing-Local-Remote-Repositories.git

*Pull Request

This section is very interesting, the best way to start doing a pull request is by forking a repository and cloning it locally, once it is done, we should make the changes and go to our forked repository and click on:
-Contribute
-Click on Open Pull request
-Add notes or a message about your pull request.
-Finally, click on "Create a pull Request"
-Wait until the owner accepts the pull request.

Short Cut to open VS Code from git bash
-code .

*Adding a new branch and pushing files from a new branch, first of all, we should create a new branch, on its branch, we can run the following command:
-git push origin new-text = So the new branch will be added to the remote repository
-git branch -a : This command shows the remote branches.
-git push origin -d name of the branch : This command deletes a branch locally.



