bash-aux
================

Auxiliary functions to be used in bash

# Core functions

## Dependency checks

### check_dependencies

Checks whether an array of commands, e.q. `("jq" "perl")`, are available
in bash

### check_dependency

Checks whether a command, e.q. `"perl"`, is available in bash

## Folders & Files

### current_file

Determine the current file path, using `"${BASH_SOURCE}"` in bash and
`"${(%):-%x}"` in zsh

### make_file_path

Create file from path, create path if it does not exist

### normalize_path

Normalize a folder / file path

### read_from_file

Read a file. Like `cat`, but returns empty string if file does not exist

## Misc

### read_non_blocking

Read input from stdin / pipe / user input, but don’t wait for the input
