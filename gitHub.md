## Git Tools
- "Git Bash" is initially developed for Unix-based command line. This tool can be used on windows-based machine to utilize Git on Windows seamlessly. 

- Xcode can be used within terminal on Mac to utilize Git on Mac. this is shipped by Apple with Terminal

## Installation of Git

1. Open [Download Git for Windows](https://git-scm.com/) link.
2. Similar webpage will be displaied showing the version number of the latest source release and a download button, as in the image below.

<img width="1000" alt="" src="Images/git.jpg"> </br></br>

3. Click Download, and it automatically downloads the software package on your system.

4. Find the package and double-click to open the Git installer.

5. Follow the installation wizard and configure Git to suit your development needs. If you are new to version control systems, the best option would be to leave the default settings.

6. Click Install and type in your password if necessary.

7. Confirm once again by clicking Install Software.

## Configuring Git
It is essential to configure your git after the installation. Use the following commands to set up your identity:

```
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```
Using the below commands, varify the configuration
```
git config user.name
git config user.email
```

## Navigating within Git
Basic UNIX commands are used to navigate within Git. Here are some basic commands that can be used within Git bash

- ``` mkdir 'dirname'```: Creates a new directory.
- ```cd 'dirname'```: Changes the current directory (use cd .. to move up one level).
- ```ls```: Lists the contents of the directory (use ls -a to display hidden files).
- ```pwd```: Shows the present working directory.
- ```start .```: Opens the current working directory in a new window.
- ```touch 'filename'```: Creates a new file or multiple files (e.g., touch file1 file2 file3).
- ```rm 'filename'```: Deletes or removes a file.
- ```rm -rf 'foldername'```: Deletes or removes a directory.


## git Commands

- ```git init```: creates an empty Git repository or reinitializes an existing one.
- ```git status```: provides information on the current status of a Git repository and its contents.
```git --add or add .```: use this command to stage changes for commit. This tells Git to include the specified files or changes in the next commit. 
- ```git commit -m "message```: command creates a new commit with the changes that have been staged. It is good practice to include a descriptive commit message that explains the purpose of the changes.
- ```git push```: command to upload your local commits to the remote repository.
- ```git fetch```: get files from remote repository to local repository
- ```git pull```: get iteams from remote repository directly to working directory
- ```git fetch```: get files from remote repository to local repository
- ```git remote add origin <git url repository>```: To add remote repository

## Steps to upload to Git repository
- change to local repository
- git init
- git add .
- git commit -m "first commit"
- git branch -M main
- git remote add origin <remote url repository>
- git push -u origin main


## Git Ignore
This is a configuration file used by git. Thi is used to ignore specific files or directories in a Git repository. the format of the file name is ```.gitignore```. Place this file in the root of the repository and specify patterns to ignore certain files or directories.

## Dot git folder
The `.git` folcder is creadted when `git init` command is issued. This folder is required to log every commit history and every other information required for the remote repository, version control, commits etc. These things are saved in different folders within .git.  This is a hidden folder and can be seem with the following `ls` command: `ls -a`.  

The folder may have the following subfolders:

- Hooks
- Info
- Objects
- Config
- Description
- HEAD
<br>

#### Articles and Videos

- You can learn more about this folder in [this article](https://toolsqa.com/git/dot-git-folder/#:~:text=A%20.,the%20contents%20of%20the%20folder.)
- Inside the Hidden Git Folder [![YouTube Preview](./Images/youtube.png)](https://www.youtube.com/watch?v=bSA91XTzeuA&ab_channel=Computerphile)
- What makes a git repo a repo - .git folder [![YouTube Preview](./Images/youtube.png)](https://www.youtube.com/watch?v=w1DsVqRvdn4&ab_channel=BenKadel)

<br>
**Example patterns:**
- foldername/: Ignores the entire directory.
- *.log: Ignores files with the .log extension.

## Branching and Merging
Git’s branching and merging capabilities are powerful tools for managing parallel development efforts and integrating changes. Here are some commands that can be used 
- ```git branch```: shows all the branches
- ```git branch <new branch name>```: To create a new branch. 
- ```git checkout <branch name>```: Switch to the new branch
- ```git merge <from branch name```: Use git checkout to switch to branch to merge and then uissue this command

