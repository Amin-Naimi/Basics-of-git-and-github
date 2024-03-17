# Introduction to Git & Github
## Git Basics:
Git is a free and open-source version control system that helps developers manage and track changes in their projects over time. Here are some key terms to get you started:

- Directory: Think of it as a folder where your project files are stored.
- Repository: Often referred to as a project, or the place where your project is kept. It contains all the files and revision history of your project.
- GitHub: A popular website used to host Git repositories online.

## Common Git Commands
Let's familiarize ourselves with some essential Git commands:

- "Clone": Copies a repository hosted somewhere (like GitHub) onto your local machine.
- "Add": Tracks changes in your files and prepares them to be committed to Git.
- "Commit": Saves your changes to the Git repository.
- "Push": Uploads Git commits from your local machine to a remote repository, such as GitHub.
- "Pull": Downloads changes from a remote repository to your local machine.
- "Init": Initializes a new Git repository.
- "Remote": Manages connections to remote repositories.
- "Branch": Lists, creates, or deletes branches in your Git repository.
- "Checkout": Switches between branches.
- "Merge": Combines changes from different branches into one.
- "Diff": Shows the differences between files or commits.

## Examples
### Example 1: 
  Clone a repository from GitHub:
  
    git clone https://github.com/Amin-Naimi/demo-repo.git
  List all files (including hidden ones):
  
    ls -a
  Check the current status of the repository:

    git status
  Add files for tracking:

    git add .
  Commit changes with a message:
  
    git commit -m "added index.html"
  Upload commits to GitHub:
              
    git push origin main

### Example 2:
Create a new folder and navigate to it.
Initialize a new Git repository:

    git init
Add files to the repository:

    git add .
Commit changes:

    git commit -m "created a new file"
Connect your local repository to a remote one on GitHub:

    git remote add origin https://github.com/Amin-Naimi/demo-repo-2.git
Push changes to the remote repository:

    git push -u origin master
    
## Branching
Git allows you to work on different features or versions of your project simultaneously using branches:

View existing branches:

    git branch
Create a new branch and switch to it:

    git checkout -b newbranche

. Make changes to your files.
. Add and commit changes.

Merge changes from the feature branch to the master branch:

    git checkout master
    git merge feature
    
Push changes to GitHub:

    git push origin master

### Additional Tips
To check out a specific commit, use:

 Find the commit hash
 
    git log
    git checkout <commit-hash>
Keep in mind that this puts you in a "detached HEAD" state. Meaning you won't be on any branch. If you want to make changes or continue from that specific commit, 
you might want to create a new branch from that commit using:

    git checkout -b <new-branch-name> <commit-hash>

Remember to replace <commit-hash> with the actual hash of the commit you want to check out.

With these basic Git commands and concepts, you're ready to start collaborating on projects and tracking your changes effectively!
    
