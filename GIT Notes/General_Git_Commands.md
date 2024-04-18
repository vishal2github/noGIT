# GENERAL COMMANDS OF GIT

### (These commands help in the manipulation of the file)

<br>

###### <ins>Help/Status/Clone/Touch Commands</ins>

+ **$ git** _(Shows the git manual. Alternative command: $git --help)_

+ **$ git status** _(Checks the state of the working directory)_

+ **$ git clone <span style="color:lightgray">_URL_ _repoName_</span>** _(Pulls the duplicated repository of an intended remote repository from the remote server's URL, and saves it as a local working directory with a custom repository name if written after the URL)_

+ **$ git touch .gitignore** _(Creates a blank file with the name '.gitignore'. After adding and thus track-starting this file, it will ignore any kind of directory, or files that are saved in it. It can be used in all kinds of directories and files with the same name or extension)_

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

+ **$ git add <span style="color:lightgray">_Filename_</span>** _(Adds the mentioned file)_

+ **$ git add --a** _(Initializes the directory's files tracking operation. Also, eveytime thereafter, adds all the newly created files or modified files to the staging area)_

<br>

###### <ins>Commit Commands</ins>

+ **$ git commit** _(Commits the files from the staging phase or area with a custom commit message by opening a configured text editor and algorithmic created unique commit id)_

+ **$ git commit -m "<span style="color:lightgray">_Commit-message_</span>"** _(Commits the files from the staging phase or area with a custom commit message and algorithmically created unique commit id)_

+ **$ git commit -a -m "<span style="color:lightgray">_Commit-message_</span>"** _(Directly commits the tracked, i.e., un-added modified, files, hence, skipping the staging step)_

+ **$ git commit --amend** _(Edits the commit's message)_

<br>

###### <ins>Branch Commands</ins>

+ **$ git branch** _(Displays all the available branches)_

+ **$ git branch -v** _(Displays all the branch's commit ID with their commit messages)_

+ **$ git branch -M** _(Renames the default branch name from 'master' to 'main')_

+ **$ git merge <span style="color:lightgray">_Branchname_</span>** _(Merges the other branch to the master branch)_

+ **$ git branch --merged** _(Displays all the merged branches)_

+ **$ git branch --no-merged** _(Displays all the non-merged branches)_

+ **$ git branch -d <span style="color:lightgray">_Branchname_</span>** _(Deletes the merged branch, shows the error for the non-merged branch)_

+ **$ git branch -D <span style="color:lightgray">_Branchname_</span>** _(Deletes the merged branch as well as the non-merged branch)_

<br>

###### <ins>Checkout Commands</ins>

+ **$ git checkout <span style="color:lightgray">_Filename_</span>** _(Un-modifies the file state and revert it to its previous state)_

+ **$ git checkout -f** _(Reverts all the files to thier previous state)_

+ **$ git checkout -b <span style="color:lightgray">_Branchname_</span>** _(Creates a new branch with the given branch name)_

+ **$ git checkout <span style="color:lightgray">_Branchname_</span>** _(Switches branch to given branch name)_

<br>

###### <ins>Difference Commands</ins>

+ **$ git diff** _(Shows the difference in the files between the staging area and the working area)_

+ **$ git diff --staged** _(Shows the difference between the staging area and the latest commit)_

<br>

###### <ins>Remove/Delete Commands</ins>

+ **$ git rm <span style="color:lightgray">_Filename_</span>** _(Deletes the intended files with the automatic staging of the the delete file)_

+ **$ rm <span style="color:lightgray">_Filename_</span>** _(Deletes the intended files without the automatic staging of the the delete file)_

+ **$ git rm --cached <span style="color:lightgray">_Filename_</span>** _(Untracks the intended file)_

<br>

###### <ins>Move Commands</ins>

+ **$ git mv <span style="color:lightgray">_Filename1 Filename2_</span>** _(Moves the file. Renames the file with automatic staging the renamed file)_

+ **$ mv <span style="color:lightgray">_Filename1 Filename2_</span>** _(Moves the file. Renames the file without automatically staging the renamed file)_

<br>

###### <ins>Restore Commands</ins>

+ **$ git restore --staged <span style="color:lightgray">_Filename_</span>** _(Un-stages the file from the staged state)_

+ **$ git restore <span style="color:lightgray">_Filename_</span>** _(Restores all the changes the the directory)_
