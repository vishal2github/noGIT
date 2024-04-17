# GIT AND GITHUB COMMANDS

<br>

### 1. Git Configuration and Confirmation (Name, email, and editor)

Firstly, after installing the git software, we run the below commands to set up the user's name and email for the communication and file transfer purpose. The commands are as follows:

###### <ins>Git Configuration</ins>

+ **$ git config --global user.name "_your_name_"** *(Configures a name)*

+ **$ git config --global user.email "*_your_email_*"** *(Configures an email)*

+ **$ git config --global core.editor "*_editor_name_*"** *(Configures a file editor)*

<br>

###### <ins>Git Confirmation</ins>

+ **$ git config user.name** *(Displays the name)*

+ **$ git config user.email** *(Displays an email)*

+ **$ git config user.editor** *(Displays a file editor)*

+ **$ git config --list** *(Lists all the configured settings)*

<br>

###### <ins>Alias Configuration</ins>

+ **$ git config --global alias._desired_Name_ _command_Name_** *(Sets alias, second name for command)*

It can be used to shorten the long commands. Ex: $ git config --global alias.st status. Now 'status' command will turn in 'st' command name. For the commands with spaces, use quotes as usual.

<br>
<hr>
<br>

### 2. Git Initialization and deletion (Specific directory)

Before start syncing our files, we first need to create a specific custom directory, upon which the git feature
is to be implemented. That is first we create a directory, then we initialize the process of git in it to make it a
git-active directory. The commands are as follows:

###### <ins>Git Initialization</ins>

+ **$ mkdir _myDir_** _(Creates a directory)_

+ **$ cd _myDir_** _(Enters into a directory)_

+ **$ git init** _(Initialize the git into the current directory)_

<br>

###### <ins>Git Deletion and Index lock error</ins>

Similarly, a git-activated directory can be git-de-active by simply running the following command to withdraw
the git feature on the specified directory, hence completely removing the ‘.git’ folder from the directory.

+ **$ git -rf .git** _(Deletes the .git folder, hence deactivating the git from the current directory and reverting it back to a normal directory)_


+ **rm -f .git/index.lock** _(Removes the “index.lock” error, i.e., stops the already running git command simultaneously with the primary command hence eliminating the terminal git error)_

<br>
<hr>
<br>

### 3. Git-hub Remote Commands

**(I) Initial Process:** Create a new remote repository on git-hub after creating an account on git-hub.

+ **$ git remote add origin _Remote-Repo-URL_** _(To link the remote repository with local repository)_

+ **$ git remote** _(Displays the remote repository's remote name)_

+ **$ git remote -v** _(Displays the remote names and their respective URLs for fetch and push purpose)_

<br>

**(II) SSH Key Generation:** Before pushing the contents, one will need to configure the ssh-key for security purposes. Without generating the ssh-key, the following command won't work. There are several ways to generate the ssh-key using the terminal or simple GUI. While generation the key, the user may be asked for his/her password as a security measure. 

The steps have been mentioned on the github website itself.

+ **$ git push -u origin _main/master_** _(Pushes the current local repository modified content, i.e., snapshot, to the intended remote repository)_
