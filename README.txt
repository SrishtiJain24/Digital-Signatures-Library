# Digital-Signatures-Library
A Digital Signatures Library (RSA)preceded with a hashing(SHA-1) library in C language

Requirement: gcc 6.2 or above

How to execute the entire project on system:

Download all files except server.c on client side.
Download server.c, sha1.c, sha1.h files on server side.

Change the IP address of Server in client.c file on line number 30.

Run following commands in terminal:
First, on server side
  gcc -c server.c -o server.o
  gcc -c sha1.c -o sha1.o
  gcc server.o sha1.o -o server
  ./server

Then, on client side
  gcc -c client.c -o client.o
  gcc -c sha1.c -o sha1.o
  gcc -c rsa.c -o rsa.o
  gcc client.o sha1.o rsa.o -o client
  ./client
