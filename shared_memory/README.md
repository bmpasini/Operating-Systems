Assignment 1 - Shared Memory
=============

Write two simple C programs that communicate with each other via shared memory. The first program receiver.c  runs in an infinite loop receiving alpha numeric strings as input from the user one line at a time. After reading one line from the standard input, this program sends this information to the other program. The sharing of data between the two processes should take place via shared memory. The second program processor.c creates an output file digits.out and waits for user input to be sent by the receiver program. As soon as one line is received from the receiver, it counts the number of digits in that line and dumps the digit count along with the original line in the digits.out file. This program also runs in an infinite loop.
