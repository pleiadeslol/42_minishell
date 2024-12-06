# Minishell 🐚✨

## Project Overview 

Minishell is a custom implementation of a Unix shell, designed to provide a deep understanding of process management, system calls, and command-line interactions. 🖥️👩‍💻

## 🎯 Project Goals

Build a functional shell that mimics basic bash functionality, offering insights into:
- Process creation and management
- File descriptor manipulation
- Command parsing and execution
- Environment variable handling
- Signal management

## ✨ Features

### Core Shell Capabilities
- 🖥️ Interactive command-line interface
- 📜 Command history support
- 🔍 Executable search and launch mechanisms
- 🔀 Input/Output redirection
- 📊 Pipeline processing
- 🌍 Environment variable expansion

### Built-in Commands
- `echo` (with `-n` option support)
- `cd` (relative/absolute path)
- `pwd`
- `export`
- `unset`
- `env`
- `exit`

## 🛠️ Technical Requirements

### Execution Parameters
- Written in C
- Follows project Norm guidelines
- Memory leak prevention
- Robust error handling

### Supported Operations
- Command execution via PATH or direct paths
- Input/Output redirections (`<`, `>`, `<<`, `>>`)
- Pipe (`|`) support
- Environment variable parsing
- Special variable `$?` for exit status

## 🎮 Interactive Mode Behavior

### Signal Handling
- `Ctrl-C`: Display new prompt
- `Ctrl-D`: Exit shell
- `Ctrl-\`: No action

## 🚀 Compilation

Use the provided Makefile:
```bash
make        # Compile project
make clean  # Remove object files
make fclean # Remove executable
make re     # Recompile
```

### 🛡️ Compilation Flags
- `-Wall`
- `-Wextra`
- `-Werror`

## 📋 System Requirements
- Unix-like operating system
- GCC compiler
- Readline library

## 🧠 Learning Objectives
- Unix process management
- System programming
- Command parsing
- Memory management
- Signal handling
- Shell mechanics

## 🚧 Potential Challenges
- Handling complex command scenarios
- Implementing robust parsing
- Managing child processes
- Efficient memory usage
- Accurate signal management

## 💡 Development Tips
- Test incrementally
- Use valgrind for memory leak detection
- Reference bash behavior for edge cases
- Implement modular, clean code
- Create comprehensive test scenarios

## 🔍 Readline Consideration
The `readline()` function may introduce memory leaks. Focus on managing memory in your own code.