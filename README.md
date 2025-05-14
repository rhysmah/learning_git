# Learning Git

Things I've (re-)learned about Git.

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
- `rm -r <directory_name>` -- deletes the specified _directory_ and all its contents.