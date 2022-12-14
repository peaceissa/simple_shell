# Joseph and Peace's Shell

# simple_shell project repository

This repository contains the files for Holberton's **simple_shell**. It can be compiled using GCC and will execute a simple shell that can be used for some basic tasks and programs most commonly found in the /bin/ folder.

### Description

Joseph and Peace's Shell is a simple UNIX command line interpreter that replicates functionalities of the simple shell (sh). Additional functions are also included. This program was written in C programming as a Team project for AlX School.

### Installation

Clone this repository into your working directory. For best results, files should be compiled with GCC and the following flags:

```sh
gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c -o hsh
```

### Usage

After compilation, the resulting program can run stand-alone, either in interactive or non-interactive mode.

#### Interactive Mode

In interactive mode, simply run the program and wait for the prompt to appear. From there, you can type commands freely, exiting with either the "exit" command or ctrl-D.

```sh
$ ./hsh
($) /bin/ls
hsh main.c shell.c
($)
($) exit
$
```

#### Non-Interactive Mode

In non-interactive mode, echo your desired command and pipe it into the program like this:

```sh
$ echo "/bin/ls" | ./hsh
hsh main.c shell.c test_ls_2
$
```

In non-interactive mode, the program will exit after finishing your desired command(s).

#### Included Built-Ins


Our shell has support for the following built-in commands:



| Command             | Definition                                                                                |
| ------------------- | ----------------------------------------------------------------------------------------- |
| exit [n]            | Exit the shell, with an optional exit status, n.                                          |
| env                 | Print the environment.                                                                    |
| setenv [var][value] | Set an environment variable and value. If the variable exists, the value will be updated. |
| unsetenv [var]      | Remove an environment variable.                                                           |
| cd [dir]            | Change the directory.                                                                     |
| help [built-in]     | Read documentation for a built-in.                                                        |
| alias [name[='value']]|                                                                                         |

## Authors
* [Joseph Utuedeye](https://github.com/utuedey)
* [Peace Issa](https://github.com/peaceissa)
