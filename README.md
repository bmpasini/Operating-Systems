Assignment 1 - Shared Memory
=============

Write two simple C programs that communicate with each other via shared memory. The first program receiver.c  runs in an infinite loop receiving alpha numeric strings as input from the user one line at a time. After reading one line from the standard input, this program sends this information to the other program. The sharing of data between the two processes should take place via shared memory. The second program processor.c creates an output file digits.out and waits for user input to be sent by the receiver program. As soon as one line is received from the receiver, it counts the number of digits in that line and dumps the digit count along with the original line in the digits.out file. This program also runs in an infinite loop.

Assignment 2 - Multithreading
=============

Study the example program in the attached file. This program creates a new thread. Both the main thread and the new thread then increment the variable counter infinitely. After incrementing the value of counter, each thread prints a message showing the value of the variable. One of the threads exits when it finds that the counter value has exceeded 25. Run the program and explain the output. Why do the print statements stop appearing after a certain point in the program ? Explain.

1. Compile and run the program on a Linux system. Find out what results it produces and explain the results.
Compile as follows:
$ gcc assignment_multithreading.c -o assignment_mt -lpthread 

Run using the following command
$ ./assignment_mt

2. Modify the program and write a correct version that fixes the problem that you just discovered. Explain how you fixed the program.

Assignment 3 - Sockets Programming
=============

Modify the program described in Assignment 1 in such a way that the two programs can be run on different machines. The program receiver.c will now be the client program that will interact with the user. Call it client.c. The processor.c will be the backend program – call it server.c. The client and server programs have the same functionality as described in Assignment 1 except that they should use a different communication mechanism that will allow them to be run on different machines. Find out which communication mechanism can be used and use that in your program.  

Assignment 4 - Shell Program
=============

Implement a simple command line shell program in C that interacts with the user in the following way. By default, the shell gives a prompt to the user. When the user types in a command (in response to its prompt) and hits Enter, the shell creates a child process that executes the command he entered and displays the results if any. It then prompts for more user input by displaying the prompt again. 

The shell can be limited to handling basic commands that do not involve piping and redirection.