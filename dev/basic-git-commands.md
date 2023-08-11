# Basic Git Commands
List of basic Git commands.

This is based on Ubuntu 22.04.

## Install Git

See [Install and configure Git](../dev/install-and-configure-git.md)

## Initialise a folder for Git

Within the folder you want to initialise, run:

```bash
git init
```

## Connect to a remote repository

To connect a local repository to a remote repository:

```bash
git remote add origin <remote repository URL>
```

For example:

```bash
git remote add origin https://github.com/username/repository-name.git
```

To confirm the remote repository:

```bash
git remote -v
```

## Status

Check the status of the current folder:

```bash
git status
```
## Add / Remove files to staging area

To add a file to the staging area:

```bash
git add <file>
```

To add all files to the staging area:

```bash
git add .
```

To remove a file from the staging area:

```bash
git rm --cached <file>
```

## Commit

To commit the files in the staging area:

```bash 
git commit -m "Commit message"
```

## Push

To push a new branch to the remote repository (i.e. Github, etc):

```bash
git push -u origin <branch>
```

To perform ongoing pushes to an existing branch once the upstream info is set:

```bash
git push origin
```

## Clone

To clone a remote repository:

```bash
git clone <remote repository URL>
```

This will create a folder with the same name as the repository in the current folder.

## Branches

To list all local branches:

```bash
git branch
```

To list all remote branches:

```bash
git fetch origin # to update the list of remote branches
git branch -r
```

To create a new local branch:

```bash
git branch <branch>
```

To switch to a branch:

```bash
git checkout <branch>
```

To create a new branch and switch to it:

```bash     
git checkout -b <branch>
```

To create a new local branch from a remote branch, set the local to track the remote and switch to it:

```bash
git checkout -b <branch> origin/<remote branch>
```

To delete a local branch:

```bash
git branch -d <branch>
```

To delete a remote branch:

```bash
git push origin --delete <branch>
```

## Pull

To pull changes from a remote repository:

```bash
git pull origin <branch>
```

## Merge

To merge a branch into the current branch:

```bash
git merge <branch>
```

Note: This merges the changes in the named branch into the current branch.

## View Git Logs

To view the Git logs:

```bash
git log
```

To view the Git logs in a single line:

```bash
git log --oneline
```

To customise the output, use the pretty=format command:

```bash
git log --pretty=format:"%h - %an, %ar : %s"
```

To view the commits that changed the number of occurances of a string (useful to find the commit that introduced a bug):

```bash
git log -S <string>
```

## Examples

Add a new local project to Git and push to GitHub:

```bash
git init
git add .
git commit -m "Initial commit"
git remote add origin https://github.com/username/repository-name.git
git push -u origin main
```

Clone a remote repository from GitHub:

```bash
git clone https://github.com/username/repository-name.git
cd repository-name
```

## References
- (Git - Book)[https://git-scm.com/book/en/v2]
- (Git Tutorial:W3 Scools)[https://www.w3schools.com/git/]
- (Master Git in 7 Minutes)[https://dev.to/valeriavg/master-git-in-7-minutes-gai]
