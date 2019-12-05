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



### Core Commands
|Command | Description |
|--------|-------------|
| git status | Checks if the working directory of the terminal is a git repo. If it is, it prints all the tracked changes in the repo since the last commit. |
| git init [directory] | Makes the specified directory into a git repo. If no directory is specified, it uses the current working directory. |
| git clone [repo] | Creates a local copy of the remote repo specified. |
| git add [file] | Adds the listed file to the staging area. |
| git add [directory] | Adds the directory to the staging area. |
| git add -A | Stages all modified files (NOT deleted or new files) |
| git add . | Stages all new and modified files. |
| git commit -m "[message]" | Commits everything that is staged. |



### Branch Mangement
git branch lists all branches 
### Comunicating with a Remote Repo

### History Commands

### Undo Commands

### .gitignore file
