0x15. C - File I/O
C Syscall By: Julien Barbier Weight: 1 Ongoing second chance project - started Oct 2, 2023 6:00 AM, must end by Oct 7, 2023 6:00 AM An auto review will be launched at the deadline

In a nutshell…
Auto QA review: 0.0/43 mandatory & 0.0/9 optional Altogether: 0.0% Mandatory: 0.0% Optional: 0.0% Calculation: 0.0% + (0.0% * 0.0%) == 0.0%

Resources
Read or watch:
File descriptors C Programming in Linux Tutorial #024 - open() read() write() Functions

man or help:
open close read write dprintf

Learning Objectives
At the end of this project, you are expected to be able to explain to anyone, without the help of Google:

General
Look for the right source of information online How to create, open, close, read and write files What are file descriptors What are the 3 standard file descriptors, what are their purpose and what are their POSIX names How to use the I/O system calls open, close, read and write What are and how to use the flags O_RDONLY, O_WRONLY, O_RDWR What are file permissions, and how to set them when creating a file with the open system call What is a system call What is the difference between a function and a system call

Copyright - Plagiarism
You are tasked to come up with solutions for the tasks below yourself to meet with the above learning objectives. You will not be able to meet the objectives of this or any following project by copying and pasting someone else’s work. You are not allowed to publish any content of this project. Any form of plagiarism is strictly forbidden and will result in removal from the program.

Requirements
General
Allowed editors: vi, vim, emacs All your files will be compiled on Ubuntu 20.04 LTS using gcc, using the options -Wall -Werror -Wextra -pedantic -std=gnu89 All your files should end with a new line A README.md file, at the root of the folder of the project is mandatory Your code should use the Betty style. It will be checked using betty-style.pl and betty-doc.pl You are not allowed to use global variables No more than 5 functions per file The only C standard library functions allowed are malloc, free and exit. Any use of functions like printf, puts, calloc, realloc etc… is forbidden Allowed syscalls: read, write, open, close You are allowed to use _putchar You don’t have to push _putchar.c, we will use our file. If you do it won’t be taken into account In the following examples, the main.c files are shown as examples. You can use them to test your functions, but you don’t have to push them to your repo (if you do we won’t take them into account). We will use our own main.c files at compilation. Our main.c files might be different from the one shown in the examples The prototypes of all your functions and the prototype of the function _putchar should be included in your header file called main.h Don’t forget to push your header file All your header files should be include guarded Tip: always prefer using symbolic constants (POSIX) vs numbers when it makes sense. For instance read(STDIN_FILENO, ... vs read(0, ...

Quiz questions
Great! You've completed the quiz successfully! Keep going! (Show quiz)

Tasks
Tread lightly, she is near mandatory Score: 0.0% (Checks completed: 0.0%) Write a function that reads a text file and prints it to the POSIX standard output.
Prototype: ssize_t read_textfile(const char *filename, size_t letters); where letters is the number of letters it should read and print returns the actual number of letters it could read and print if the file can not be opened or read, return 0 if filename is NULL return 0 if write fails or does not write the expected amount of bytes, return 0
