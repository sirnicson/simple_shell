# Simple Shell Team Project

## Overview

The Simple Shell project is a key part of our systems programming work using C. 
Our team is building a basic UNIX command-line interpreter, similar to a simple shell. 
This project helps us learn important C programming skills and understand how UNIX processes, file systems, and commands work. 
Our shell will work in both interactive and non-interactive modes, covering essential UNIX functions.

## Features

- **Interactive Mode**: The shell operates in an interactive mode, where it
  waits for user input, processes commands, and returns the output. This mode
  continues to run until the user exits the shell.

- **Non-Interactive Mode**: The shell supports non-interactive mode, where it
  reads commands from a file or standard input, executes them, and exits upon
  completion.

- **Command Execution**: The shell executes standard UNIX commands by forking a
  child process and using the `execve` system call. It supports the execution
  of commands with arguments, handling both relative and absolute paths.

- **Built-in Commands**: The shell includes a set of built-in commands such as
  `exit`, `cd`, and `env`, which are handled internally without invoking
  external programs.

- **Error Handling**: The shell provides basic error handling, ensuring that
  users are notified of invalid commands or incorrect usage.

## Requirements

- C programming language
- GCC compiler
- UNIX-based operating system (e.g., Linux)

## Project Structure

- The project is structured into multiple tasks.
- Each building upon the previous one to gradually develop a fully functioning shell

## Tasks

### BASIC TASKS

0. Betty Would Be Proud
	Objective: Ensure that your code adheres to the Betty coding style.
	Details: Write a well-documented, and structured code that passes Betty checks.

1. Simple Shell 0.1
	Objective: Create a basic UNIX command-line interpreter.
	Features:
	Display a prompt and wait for user input.
	Execute single-word commands without arguments.
	Handle errors gracefully.
	Manage end-of-file (Ctrl+D) condition.
- Limitations:
	No use of PATH.
	No built-in commands or special character handling.

2. Simple Shell 0.2
	Objective: Enhance the shell to handle commands with arguments.
	Features: Allow command execution with arguments passed.

3. Simple Shell 0.3
	Objective: Implement PATH handling.
	Features:
	Search and execute commands using the PATH environment variable.
	Avoid calling fork if the command doesn’t exist.

4. Simple Shell 0.4
	Objective: Implement built-in commands.
	Features:
	Implement the exit built-in command to exit the shell.

5. Simple Shell 1.0
	Objective: Add environment management capabilities.
	Features:
	Implement the env built-in command to print the current environment.


### ADVANCED TASKS

    These tasks further extend the shell’s functionality, 
    including custom implementations of standard functions and advanced shell features.

6. Simple Shell 0.1.1
	Objective: Implement a custom getline function.
	Features:
	Use a buffer to optimize reading from input.
	Avoid using the standard getline.

7. Simple Shell 0.2.1
	Objective: Refine argument handling and environment management.
	Features:
	Implement custom argument parsing without strtok.
	Handle arguments for exit.
	Implement setenv and unsetenv commands.

10. cd
	Objective: Implement the cd command.
	Features:
	Change the current working directory.
	Handle special cases like cd - and update the PWD environment variable.

11. Command Separator ;
	Objective: Handle command chaining using the ; separator.

12. Logical Operators && and ||
	Objective: Implement support for logical operators to control command execution flow.

13. Alias
	Objective: Implement the alias command to define and manage command shortcuts.

14. Variables
	Objective: Implement variable replacement.
	Features:
	Handle special variables like $$ and $?.

15. Comments
	Objective: Implement support for comments (lines starting with #).

16. File as Input
	Objective: Enable the shell to execute commands from a file.
	Features:
	Accept a filename as a command-line argument.
Execute commands in the file without displaying a prompt.


### Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/simple_shell.git
    ```

2. Navigate to the project directory:
    ```bash
    cd simple_shell
    ```

3. Compile the shell:
    ```bash
    gcc -Wall -Werror -Wextra -pedantic *.c -o hsh
    ```

### Compilation

    Compiled, using the gcc command:

    gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c -o hsh



### Interactive Mode

To start the shell in interactive mode, run the compiled `hsh` program:
```bash
./hsh
```


### Non-Interactive Mode 

Tested by entering commands to the shell or using command files



## Simple Shell Flow Chart

![Simple Shell Flowchart](images/Simple%20Shell%20Flowchart.png)

-----------------------------------------------------------------------

Collaborators - sirnicson & Abdulquadri
