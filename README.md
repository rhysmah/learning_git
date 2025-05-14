# Learning Git

Things I've (re-)learned about Git.

## Git Config

These are local and global configuration settings for Git. Local settings apply to the current repository; global settings apply to _all_ repositories.

Users are required to set their name and email. These are assoicated with all commits, allowing others to too who made what changes.

- `git config --global --list` -- lists all global configuration settings.
- `git config --global user.name "<name>"` -- sets the global username.
- `git config --global user.email "<email>"` -- sets the global email address.

## Commands & Options

#### Options
An _option_, which follows a single dash (`-`) or double dash (`--`), changes the behavior of a command. For example, in `git commit -m "message"`, `-m` is an option.

#### Arguments
An _argument_ is a value that the command acts on. For example, in `git commit -m "message"`, `"message"` is an argument for the `-m` option.
 
## Useful Command Line Commands

#### The Bare Basics
- `pwd` -- prints the current working directory.
- `ls` -- lists all visible files and directories in the current directory.
- `ls -a` -- lists all files and directories, including hidden ones.

- `cd` -- returns to the home directory.
- `cd ..` -- moves up one directory level ("up" meaning closer to the home directory).
- `cd -` -- returns to the previous directory.
- `cd <path_to_directory>` -- changes the current directory to the specified one. 

- `mkdir <directory_name>` -- creates a new directory (folder) with the specified name.
- `touch <file_name>` -- creates a new file with the specified name.
- `rm <file_name>` -- deletes the specified file; does not work on directories.
- `rm -r <directory_name>` -- deletes the specified _directory_ and all its conˆtents.

## Repositories

### Local Repositories

### Some Commands
- `git init` -- initializes a new Git repository in the current directory. This creates a hidden `.git` directory that contains all the information about the repository.
- `git init -b <branch_name>` -- initializes a new Git repository in the current directory and creates a new branch with the specified name. This is useful for starting a new project with a specific branch structure.

### Areas of Git

#### Working Directory
The Working Directory is contains the files and directories in the project directory. These are files and directories on your local machine that you work on; they're not part of the Git repo.

#### Local Repository
The Local Repository is the Git repository on your local machine. It contains all the information about the project (stored in the `.git` directory). The local repository is where you make changes to your project and commit them to the version control system.

#### Staging Area
The Staging Area acts as a buffer between your Working Directory and the Local Repository. You can make changes to your files, which can then be added to the Staging Area (`git add`) but aren't yet committed to the Local Repository. Here, you can review and select which changes you want to commit, i.e., which changes are added to the official history of the project.


The Staging Area is a _temporary_ area where you can add files before committing them. You can make changes to local files that aren't automatically committed; instead, they're stored in the staging area until you're ready to commit them.

#### Commit History
