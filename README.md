# Simple Shell

## Overview

**Simple Shell** is a basic UNIX command line interpreter developed as a collaborative project. This project involves implementing essential features of a shell in C, adhering to the requirements and constraints typical of a UNIX environment.

### Contributors

- Name: Paschal Ugwu
- Email: ugwupaschal@gmail.com

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Usage](#usage)
- [Compilation](#compilation)
- [Tasks](#tasks)
  - [Task 0: Betty would be proud](#task-0-betty-would-be-proud)
  - [Task 1: Simple shell 0.1](#task-1-simple-shell-01)
  - [Task 2: Simple shell 0.2](#task-2-simple-shell-02)
  - [Task 3: Simple shell 0.3](#task-3-simple-shell-03)
  - [Task 4: Simple shell 0.4](#task-4-simple-shell-04)
  - [Task 5: Simple shell 1.0](#task-5-simple-shell-10)
  - [Advanced Tasks](#advanced-tasks)
- [Resources](#resources)
- [Testing](#testing)
- [Acknowledgments](#acknowledgments)

## Introduction

This project implements a simple UNIX command interpreter, commonly known as a shell. It covers fundamental aspects of shell functionality, including command execution, environment management, and built-in commands.

## Features

- **Interactive Mode**: Prompts the user for commands and executes them.
- **Non-Interactive Mode**: Executes commands from a file or standard input.
- **Command Execution**: Executes commands located in directories specified by the PATH environment variable.
- **Built-in Commands**: Supports built-in commands like `exit` and `env`.

## Usage

### Interactive Mode

```bash
$ ./hsh
($) /bin/ls
($) exit
```

### Non-Interactive Mode

```bash
$ echo "/bin/ls" | ./hsh
$ cat commands.txt | ./hsh
```

## Compilation

Compile the shell with:

```bash
gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c -o hsh
```

Ensure to use `gcc` with the provided options to meet project requirements.

## Tasks

### Task 0: Betty would be proud

- **Objective**: Ensure all code adheres to the Betty style guide.
- **Implementation**: Verify code style using `betty-style.pl` and `betty-doc.pl`.

### Task 1: Simple shell 0.1

- **Objective**: Implement a basic shell that:
  - Displays a prompt and waits for user input.
  - Executes simple commands without arguments.
  - Handles "end of file" (Ctrl+D) and errors.
- **Limitations**: No support for advanced features like pipes, redirections, or multiple commands.

### Task 2: Simple shell 0.2

- **Objective**: Extend the shell to handle command lines with arguments.
- **Enhancements**: Parse and execute commands with arguments.

### Task 3: Simple shell 0.3

- **Objective**: Integrate PATH handling.
- **Enhancements**: Search for commands in directories specified by the PATH environment variable.

### Task 4: Simple shell 0.4

- **Objective**: Implement the `exit` built-in command.
- **Enhancements**: Support exiting the shell using the `exit` command.

### Task 5: Simple shell 1.0

- **Objective**: Implement the `env` built-in command.
- **Enhancements**: Display the current environment variables.

### Advanced Tasks

1. **Simple shell 0.1.1**: Implement a custom `getline` function using a buffer.
2. **Simple shell 0.2.1**: Implement custom tokenization without `strtok`.
3. **Simple shell 0.4.1**: Handle arguments for the `exit` built-in command.
4. **setenv, unsetenv**: Implement `setenv` and `unsetenv` built-ins for environment variable management.
5. **cd**: Implement the `cd` built-in command.
6. **;**: Handle command separator `;`.
7. **&& and ||**: Implement logical operators `&&` and `||`.

## Resources

- **Unix shell**: [Wikipedia](https://en.wikipedia.org/wiki/Unix_shell)
- **Thompson shell**: [Wikipedia](https://en.wikipedia.org/wiki/Thompson_shell)
- **Ken Thompson**: [Wikipedia](https://en.wikipedia.org/wiki/Ken_Thompson)
- **Shell Programming Guide**: [Everything you need to know to start coding your own shell](https://intranet.alxswe.com/concepts/64)

## Testing

Test the shell in both interactive and non-interactive modes. Ensure it handles common edge cases and adheres to expected behavior as outlined in the tasks.

## Acknowledgments

This project was developed as part of the ALX Software Engineering curriculum. Special thanks to the ALX community for their guidance and support.
