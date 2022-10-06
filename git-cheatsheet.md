# Git commands

## Committing CLI & remote

After installing Git on your machine, you can create repositories and commits locally. You can also synchronize your local repository with a <strong>remote</strong> repository (i.e. on GitHub).

### Committing in a local repository

We recommend executing the following git commands for every completed task.

- git status : List all files that have changed nd their state
- git add <filename> : Add a file to the stage
- git commit -m 'Commit message' : Creat a commit including all staged files
- git log -oneline : Show the commit history

### Using commits as backups

- git restore . : Return to the last committed state of the entire project
- git restore <file name> : Restore individual files

### Connecting to a remote repository

This enables teams to work on the same remote repository and clone it locally. The remote repository also serves as a backup.

#### Connecting your local repository to a new remote repository

- git remote add origin git@github.com:GitHubUsername/repository-name.git
- git branch -M main
- git push -u origin main

#### Cloning a remote repository

- git clone <url>

#### Synchronizing local & remote repositories

- git push : Upload content to the remote repository
- git pull : Download content from the remote repository

## Git branch commands

- git switch -c <branchname> : create a new branch and switch to it
- git switch <branchname> : switch branches
- git branch : list your branches
- git branch -a : list all branches (local and remote)
- git branch -de <branchname>
