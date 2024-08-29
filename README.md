# Simple Shell Team Project - 0x16. C

## Overview

The Simple Shell project involveD creating a basic UNIX command-line interpreter (shell) that simulates the behavior of a simple shell. The project enabled us to practice the basics  of UNIX processes, file systems, and command execution. The shell operates in both interactive and non-interactive modes.

## Tasks

1. **Task 0: Betty Would Be Proud**
   - Ensure code adheres to the Betty style guide.

2. **Task 1: Simple Shell 0.1**
   - Display a prompt and wait for user input.
   - Execute commands with no arguments.
   - Handle "command not found" errors.
   - Handle end-of-file (EOF) condition (Ctrl+D).

3. **Task 2: Simple Shell 0.2**
   - Process commands with arguments.

4. **Task 3: Simple Shell 0.3**
   - Search for executable commands in directories listed in PATH.
   - Avoid forking if the command does not exist.

5. **Task 4: Simple Shell 0.4**
   - Allow exiting the shell with the `exit` command.

6. **Task 5: Simple Shell 1.0**
   - Print the current environment variables with the `env` command.

7. **Task 6: Simple Shell 0.1.1 (Advanced)**
   - Implement a custom `getline` function to use a buffer and minimize system calls.

8. **Task 7: Simple Shell 0.2.1 (Advanced)**
   - Implement custom tokenization method to split command lines.

9. **Task 8: Simple Shell 0.4.1 (Advanced)**
   - Handle arguments for the `exit` built-in command.

10. **Task 9: Setenv and Unsetenv (Advanced)**
    - Implement `setenv` and `unsetenv` built-in commands to manage environment variables.

11. **Task 10: cd (Advanced)**
    - Implement the `cd` built-in command to change the current directory and manage directory history.

12. **Task 11: Command Separator ; (Advanced)**
    - Handle multiple commands on a single line, separated by `;`.

13. **Task 12: Logical Operators && and || (Advanced)**
    - Execute commands based on the success or failure of previous commands.

14. **Task 13: Alias (Advanced)**
    - Implement the `alias` built-in command to define, list, and manage command aliases.

15. **Task 14: Variables (Advanced)**
    - Support variable expansion with `$?` and `$$`.

16. **Task 15: Comments (Advanced)**
    - Ignore comments starting with `#`.

17. **Task 16: File as Input (Advanced)**
    - Read and execute commands from a file specified as a command-line argument.

## Compilation

To compile the shell, use the following command:

```bash
gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c -o hsh
```

## Testing
- Interactive Mode: Run the shell using ./hsh and interact with it by entering commands.

- Non-Interactive Mode: Test by entering commands or using command files specified as arguments.

## Files
- AUTHORS - List of authors.
- README.md - This file.
- shell.h - Header file containing function prototypes and definitions.
- shell_main.c - Main file for the shell implementation.
- shell_utils.c - Utility functions for the shell.
- builtin_.c
- initializer_.c - Functions for initializing the shell.
- non_interactive_.c - Functions for non-interactive mode.
- helperfunctions: help_0.c, help_1.c, help_2.c - Help functions for the shell.
- images - Image folder


## Process
- Creation of simple_shell repository
- Cloning of repo on local machine
- Creation of README.md file
- Update README.md with Simple Shell Flowchart
- Creation of header file
- Creation of c. files
- Compilation & Testing

## Collaborators - sirnicson & Abdulquadri


--------------------------------------------

## Simple Shell flow Chart

![Simple Shell Flowchart](images/Simple%20Shell%20Flowchart.png)
