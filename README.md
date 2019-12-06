# git-basics
A page where I put everything that I have learned about git/GitHub, from syntax of the git language to its applications. 
### What is Git/GitHub
Git is a Version Control Software (VCS) that allows programmers to store code for projects remotely and allows for multiple people to work on coding projects, who are called contributors. Git simply checks for changes, additons, or deletions of files in certain directories, called repositories, and doesn't necessarily need to be for programmers and their code. One could use Git to track changes to a Word Document file, if they chose to do so.   

GitHub is a website and storage platform where programmers can push their Git repos to, in order to store them for later use or to collaborate with other programmers.  

Hence, Git is the tool and a language that allows you to track the modifications made to a project of yours and push it to GitHub, and GitHub is the place where the code is stored and can be accessed remotely. Furthermore, one must make an account in order to push code to GitHub, which opens the door for some cool features. Anyone can see what projects (repos) you have on your account, if you choose to make them public, and anyone can also see any code you contribute to other projects, and this activity is logged on your account page. Because of this, many programmers put links to their GitHub account on their resumes to show future employers and other people the extent of their skills by simply showing them what they are capable of creating.   

When using Git/GitHub, there are certain terms and concepts that one must accurately grasp in order to use the technology properly.
### Key Terms
| Term | Description |
|------|-------------|
| branch | A independent line of development, usually used to add features to an existing project before merging it with the main branch, which is uusally called Master. |
| fork | A personal copy of a repo that is owned by someone else. |
| remote | A repository on GitHub that all programmers in a certain project will communicate to push and pull code from. |
| pull request | When making contributions to a repo, you file a pull request which allows the original author to merge your changes with the main project. |
| clone | A local copy of a repo, including all commits and branches. |
| staging | A process where you determine what files/changes you are going to include in your next commit. |
| commit | Saving all marked changes to your local repo. |

### Config Commands 
| Command | Description |
|---------|-------------|
| git config --global user.name [name] | Set author name to be used for all commits. |
| git config --global user.email [email] | Set email to be used for all commits. |

### Core Commands
|Command | Description |
|--------|-------------|
| git status | Checks if the working directory of the terminal is a git repo. If it is, it prints all the tracked changes in the repo since the last commit. |
| git init [directory] | Makes the specified directory into a git repo. If no directory is specified, it uses the current working directory. |
| git clone [repo] | Creates a local copy of the remote repo specified. Also can be used with another local repo if given a directory path as input instead. |
| git add [file] | Adds the listed file to the staging area. |
| git add [directory] | Adds the directory to the staging area. |
| git add -A | Stages all modified files (NOT deleted or new files) |
| git add . | Stages all new and modified files. |
| git commit -m "[message]" | Commits everything that is staged. |


### Branch Mangement
| Command | Description |
|---------|-------------|
| git branch | Lists all branches in the current repo. |
| git branch [branch] | Creates a new branch with the given name. |
| git checkout [branch] | Switch to given branch. |
| git checkout -b [branch] | Create and switch to specified branch. |
| git merge [branch] | Merge given branch into current branch. |
| git branch -d [branch] | Deletes the given branch. |


### Comunicating with a Remote Repo
| Command | Description |
|---------|-------------|
| git remote add origin [url] | Link your local repo to a repo of yours on GitHub. |
| git push origin [branch] | Pushes the commited changes to the remote branch of your choice (usually master) e.g. `git push origin master`. |
| git fetch | Downloads all history from remote branches. |
| git merge | Merges remote branch with local branch |
| git pull | A combination of `git fetch` and `git merge`. Updates local branch with commits from same remote branch. |


### History Commands
| Command | Description |
|---------|-------------|
| git log | Lists version history for the currently selected branch. |
| git log --author=[name] | Lists only version history from a specific author. |
| git log --pretty=oneline | Shows version history for current branch, one commit and its stats all fits on one line. |
| git show [commit] | Output data about this commit. |
| git blame [file] | Shows list of changes to a specific file. |


### Undo Commands
| Command | Description |
|---------|-------------|
| git reset [file] | Removes a file from the staging area. |
| git revert [commit] | Creates a new commit that undoes changes made in [commit], and applies it. |
| git checkout -- [file] | Replaces file contents with the files contents from the last commit (HEAD). |
| git reset -- hard HEAD | Removes all local changes in working directory. |
| git reset -- hard [commit] | Reset HEAD pointer to [commit] and discard all changes since then. |
| git fetch origin, git reset --  head origin/master | Discards all local changes (and commits) and fetches the lastest history from the remote, and syncs your local master branch with the remote master branch. |


### Misc. Commands
| Command | Description |
|---------|-------------|
| tag | Mark certain commits, useful for software releases. e.g. `git tag 1.0.0 1b2e1d63ff`. The ending characters are called a commit id, and can be checked at GitHub or by checking the log using commands. 
### .gitignore file
A .gitignore file is a file that you place in the root of your repo that tells git to ignore changes and updates to certain files/directories within the repo's directory. 
Some files that are useful to ignore are system files, hidden files/folders, and compile/build files. 
Here is an example `.gitignore` file:
```
#This is a git ignore file
.DS_Store
a.out
.cache/
dist/
```
