# Digital-Signatures-Library
A Digital Signatures Library (RSA)preceded with a hashing(SHA-1) library in C language 


How to execute the entire project on system. (Linux)

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
