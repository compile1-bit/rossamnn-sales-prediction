# OShell - Command Line Interpreter

### Group Information
- **Group Number:** G-10
- **Full Name:** Abine Mekonen  | **ID:** 1134/16
- **Full Name:** Firdos Abduresak | **ID:** 2156/16
- **Full Name:** Eleni Yisfalem | **ID:** 0338/15
- **Full Name:** Elbetel Alem | **ID:** 1908/16
- **Full Name:** Vittoria Tamire | **ID:** 3739/16
- **Full Name:** Esmael Yasin | **ID:** 1996/16
- **Full Name:** Biniam Mesfin | **ID:** 1598/16

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

This will generate an executable named oshell using the required flags: -Wall -Wextra -Werror.

Execution Instructions
1. Interactive Mode
Start the shell normally to enter commands manually:

./oshell

2. Batch Mode
Run the shell with a single file argument to execute a script:

./oshell tests.txt

3. Piped Mode
Pipe commands into the shell:

echo "ls -l; echo done" | ./oshell

Cleaning Up
To remove compiled object files and the executable, run:

make clean
