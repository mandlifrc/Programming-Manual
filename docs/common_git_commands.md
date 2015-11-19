# Commonly Used Git Commands

## Clone the repository from GitHub to a local machine
* `git clone <repository URL>`

## Working with branches
* `git branch <new branch name>` to create a new branch
* `git checkout <branch name>` to then switch to the new branch OR
* `git checkout -b <new branch name>` to simultaneously create a new branch and switch to it

If a branch exists on GitHub that you want to sync onto the local machine, use the following from the master branch:
* `git pull`

## Adding files to be committed
Once you have made your code updates and are ready to commit them to the repository, add the files to be committed:

* `git add <file name>` to add a single file, OR
* `git add -u` to add any existing tracked files which have changed OR
* `git add .` to add all files in a folder

## Commiting changes and pushing commits to GitHub
* `git commit` to commit the changes
* `git push origin HEAD` to push the changes on the current branch to GitHub

## Syncing a local branch with the same one on GitHub
* `git pull` to sync your local topic branch with the same branch on GitHub
* `git mergetool` to manually merge if Git can't successfully merge on its own

## Perform a Pull Request
Must be performed on GitHub Desktop or on the GitHub website.

## Syncing a local branch with the master branch on Github
Required if the master has been updated since you started working on your branch (i.e. someone performed a pull request before you). From your local topic branch:

* `git pull origin master` to sync the changes on GitHub's master branch with your local topic branch
* `git mergetool` to manually merge if Git can't successfully merge on its own
