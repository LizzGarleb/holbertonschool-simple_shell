# Simple Shell
Releade date December 9, 2022.

## Table of Contents
1. Introduction
2. Prokect Information
    - Task
    - General Requirements
    - Allowed functions & system calls
3. Documentation
    - Instalation
    - Usage
    - Files Description
    - Flowchart
4. Authors
    
Introduction (Question from task)
- What is Shell?
  Shell is an enviorment in which we can run our commands, programs and shell scripts.

- What is a pid and a ppid?
  PID (Process Id) & PPID (Process PW) are two important Linux system identifiers. PID is the process id, and PPID is the process pointer. When a process start up, it assigns a PID to itself.

- What is the difference between a function & a system call?
  The main difference between system call and function call is that a system call is a reques for the kernel to access a resource while a function call is a request made by a program to perform a specific task. System call s are used when a program needs to communicate wirh the kernel while function call are to call a specific functio within the program.

- How does the shell use the PATH to find the programs?
  The PATH variable is basicaly a list of firectories your computer looks through to fing a requested executable.

- How to suspend the execution of a process until one of its children terminates?
  We can suspend the execution of a process until one of its children terminates using the wait function. A call to wait() blocks the calling process until one of its child processes exits or a signal is received. After child process terminates, parent continues its execution after wait system call instruction.

## Project Information

### Tasks

    Task 0 - Write a README, Write a man for your shell & AUTHOR file.

    Task 1 - Write a beautiful code that passed the Betty checks

    Task 2
     Write a UNIX command line interpreter.

    Usage: simple_shell

Your Shell should:

    Display a prompt and wait for the user to type a command. A command line always ends with a new line.
    The prompt is displayed again each time a command has been executed.
    The command lines are simple, no semicolons, no pipes, no redirections or any other advanced features.
    The command lines are made only of one word. No arguments will be passed to programs.
    If an executable cannot be found, print an error message and display the prompt again.
    Handle errors.
    You have to handle the “end of file” condition (Ctrl+D)

You don’t have to:

    use the PATH
    implement built-ins
    handle special characters : ", ', `, \, *, &, #
    be able to move the cursor
    handle commands with arguments

    Task 3 - Handle command lines with arguments

    Task 4 - Handle the PATH, fork must not be called if the command doesnt exist

    Task 5 - Implement the exit built-in, that exits the shell

    Task 6 - Implement the env built-in, that prints the current enviorment


### General requirements

    Allowed editors:
    All our files were compiled on Ubuntu 20.04 LTS using `gcc`, using the options `-Wall -Werror -Wextra -pedantic -std=gnu89`

### Allowed functions & system calls

    - access (man 2 access)
    - chdir (man 2 chdir)
    - close (man 2 close)
    - closedir (man 3 closedir)
    - execve (man 2 execve)
    - exit (man 3 exit)
    - _exit (man 2 _exit)
    - fflush (man 3 fflush)
    - fork (man 2 fork)
    - free (man 3 free)
    - getcwd (man 3 getcwd)
    - getline (man 3 getline)
    - getpid (man 2 getpid)
    - isatty (man 3 isatty)
    - kill (man 2 kill)
    - malloc (man 3 malloc)
    - open (man 2 open)
    - opendir (man 3 opendir)
    - perror (man 3 perror)
    - read (man 2 read)
    - readdir (man 3 readdir)
    - signal (man 2 signal)
    - stat (__xstat) (man 2 stat)
    - lstat (__lxstat) (man 2 lstat)
    - fstat (__fxstat) (man 2 fstat)
    - strtok (man 3 strtok)
    - wait (man 2 wait)
    - waitpid (man 2 waitpid)
    - wait3 (man 2 wait3)
    - wait4 (man 2 wait4)
    - write (man 2 write)

## Documentation
### Instalation

### Usage (Interactive & Non-Interactive, Built-In)

  Interactive
  
  An interactive shell is defined as the shell that simply takes commands as input from the user and acknowledges the output to the user. This shell also reads startup files that occurred during activation and display a prompt.

  Non-Interactive
  
  As the name inplies, a non-interactive shell is a type of shell that doesnt interact with the user. We can run it through a script or similat. Also, it can be run through some automated process. The non-interactive shell influence the PATH variables. It is higly recommended to use the full path for a command in non-interactive shells. Non-interactive scripts can smoothly run in the background easily.

  Built-In
  
  A built-in is a command or functio that is part of the shell itself. The command is "built-in" to the shell program - no external program is necessary to run the command, and a new process does not need to be created.

### Files (Table of content detailing every file and function)

### Flowchart

### Authors

![Lizbeth Garcia](https://github.com/Lizz3108)
![Yahdiel Saldana](https://github.com/yahdielo)
