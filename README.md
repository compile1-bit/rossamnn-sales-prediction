# OShell - Command Line Interpreter

### Group Information
- **Group Number:** G-1
- **Full Name:** [Group Member Name] | **ID:** [ID]
- **Full Name:** [Group Member Name] | **ID:** [ID]
- **Full Name:** [Group Member Name] | **ID:** [ID]

### Project Description
OShell is a custom Unix command-line interpreter implemented in C. It supports three modes of operation: interactive, non-interactive (piped), and batch mode. The shell handles standard command execution by searching through a configurable path, and it includes support for several advanced shell features like logical operators, parallel execution, and variable expansion.

### Implemented Features
- **Core Execution:** Supports absolute/relative paths and path searching.
- **Built-in Commands:** `exit`, `cd`, and `path`.
- **Operators:** - Sequential execution using `;`
  - Conditional AND using `&&`
  - Conditional OR using `||`
  - Parallel execution using `&`
- **Redirection:** Output redirection using `>` (overwrite mode).
- **Variable Expansion:** Supports `$$` (Process ID) and `$?` (Last Exit Status).
- **Comments:** Ignores any text following the `#` character.
- **Batch Mode:** Executes commands from a file passed as a single argument.
- **Signal Handling:** Ignores `Ctrl+C` (SIGINT) to prevent the shell from accidental termination.

### Compilation Instructions
The project uses a Makefile for compilation. To compile the project, navigate to the project directory and run:

```bash
make

##This will generate an executable named oshell using the required flags: -Wall -Wextra -Werror.

Execution Instructions
1. Interactive Mode
Start the shell normally to enter commands manually:
