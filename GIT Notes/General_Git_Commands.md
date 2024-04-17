# GENERAL COMMANDS OF GIT

### (These commands help in the manipulation of the file)

<br>

###### <ins>Help/Status/Clone/Touch Commands</ins>

**$ git** _(Shows the git manual. Alternative command: $git --help)_

**$ git status** _(Checks the state of the working directory)_

**$ git clone <mark>_URL repoName_</mark>** _(Pulls the duplicated repository of an intended remote repository from the remote server's URL, and saves it as a local working directory with a custom repository name if written after the URL)_

**$ git touch .gitignore** _(Creates a blank file with the name '.gitignore'. After adding and thus track-starting this file, it will ignore any kind of directory, or files that are saved in it. It can be used in all kinds of directories and files with the same name or extension)_

<br>

###### <ins>Log Commands</ins>

+ **$ git log** _(Shows the log of every commit performed)_

+ **$ git log -p** _(Shows the log with all the changes)_

+ **$ git log -p -1/-2/etc..** _(Shows the specific number of logs with all the changes)_

+ **$ git log --stat** _(Shows a summary of the log)_

+ **$ git log --pretty=oneline** _(Shows the log with all-in-one lines)_

+ **$ git log --short=oneline** _(Shows the log with all-in-one lines)_

+ **$ git -pretty=format:"%h --%an"** _(Shows the log with all-in-one lines)_

<br>

###### <ins>Add Commands</ins>

+ **$ git add .** _(Adds all the files simultanously)_

+ **$ git add <mark>_Filename_</mark>** _(Adds the mentioned file)_

+ **$ git add --a** _(Initializes the directory's files tracking operation. Also, eveytime thereafter, adds all the newly created files or modified files to the staging area)_

<br>

###### <ins>Commit Commands</ins>

+ **$ git commit** _(Commits the files from the staging phase or area with a custom commit message by opening a configured text editor and algorithmic created unique commit id)_

+ **$ git commit -m "<mark>_Commit message_</mark>"** _(Commits the files from the staging phase or area with a custom commit message and algorithmically created unique commit id)_

+ **$ git commit -a -m "<mark>_Commit message_</mark>"** _(Directly commits the tracked, i.e., un-added modified, files, hence, skipping the staging step)_

+ **$ git commit --amend** _(Edits the commit's message)_

<br>

###### <ins>Branch Commands</ins>

+ **$ git branch** _(Displays all the available branches)_

+ **$ git branch -v** _(Displays all the branch's commit ID with their commit messages)_

+ **$ git branch -M** _(Renames the default branch name from 'master' to 'main')_

+ **$ git merge <mark>_branchName_</mark>** _(Merges the other branch to the master branch)_

+ **$ git branch --merged** _(Displays all the merged branches)_

+ **$ git branch --no-merged** _(Displays all the non-merged branches)_

+ **$ git branch -d <mark>_branchName_</mark>** _(Deletes the merged branch, shows the error for the non-merged branch)_

+ **$ git branch -D <mark>_branchName_</mark>** _(Deletes the merged branch as well as the non-merged branch)_

<br>

###### <ins>Checkout Commands</ins>

+ **$ git checkout <mark>_filename_</mark>** _(Un-modifies the file state and revert it to its previous state)_

+ **$ git checkout -f** _(Reverts all the files to thier previous state)_

+ **$ git checkout -b <mark>_branchName_</mark>** _(Creates a new branch with the given branch name)_

+ **$ git checkout <mark>_branchName_</mark>** _(Switches branch to given branch name)_

<br>

###### <ins>Difference Commands</ins>

+ **$ git diff** _(Shows the difference in the files between the staging area and the working area)_

+ **$ git diff --staged** _(Shows the difference between the staging area and the latest commit)_

<br>

###### <ins>Remove/Delete Commands</ins>

+ **$ git rm <mark>_fileName_</mark>** _(Deletes the intended files with the automatic staging of the the delete file)_

+ **$ rm <mark>_fileName_</mark>** _(Deletes the intended files without the automatic staging of the the delete file)_

+ **$ git rm --cached <mark>_fileName_</mark>** _(Untracks the intended file)_

<br>

###### <ins>Move Commands</ins>

+ **$ git mv <mark>_filename1 filename2_</mark>** _(Moves the file. Renames the file with automatic staging the renamed file)_

+ **$ mv <mark>_filename1 filename2_</mark>** _(Moves the file. Renames the file without automatically staging the renamed file)_

<br>

###### <ins>Restore Commands</ins>

+ **$ git restore --staged <mark>_filename_</mark>** _(Un-stages the file from the staged state)_

+ **$ git restore <mark>_filename_</mark>** _(Restores all the changes the the directory)_
