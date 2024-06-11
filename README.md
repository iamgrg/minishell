# Minishell

## Overview

Minishell is a project that involves creating a simple shell, similar to bash. This project allows you to understand how a shell interprets and executes commands, handles environment variables, and manages processes and file descriptors.

## Objectify

- Build a basic command-line interface.
- Implement several bash features like command history, environment variables, and basic shell commands.
- Understand and implement the functionality of pipes and redirections.

## Build Instructions

Compile the project using the provided Makefile:
```bash
make all
```

## Usage
Run the shell by simply executing:

```bash
./minishell
```

The shell will display a prompt and wait for command input.

## Features

- Command Parsing and Execution: Processes commands entered by the user, searching for the executable based on the PATH variable or using a relative/absolute path.
- Redirections and Pipes: Handles input (<), output (>), append (>>), and heredoc (<<) redirections, as well as piping between commands (|).
- Signal Handling: Implements signal handling for ctrl-C (interrupt), ctrl-D (EOF), and ctrl-\ (quit), similar to bash.
- Environment Variables: Supports expansion of environment variables ($VAR) and the last command exit status ($?).
- Built-in Commands: Includes built-ins like echo, cd, pwd, export, unset, env, and exit.

## Built-in Commands

- echo: Implement echo with the -n option to not output the trailing newline.
- cd: Change the working directory.
- pwd: Print the current working directory.
- export: Set environment variables.
- unset: Remove environment variables.
- env: List all environment variables.
- exit: Exit the shell.

## Contributors

- @iamgrg
- @yass-mhl

## License

![MIT License](https://img.shields.io/badge/license-MIT-green)
Distributed under the MIT License.
