# UDPServer
This repository contains a C program (server.c) implementing a reliable UDP server using Go-Back-N (GBN) protocol for basic functionality. The server establishes a connection, handles data transfer, and tears down the connection. The code includes packet structures, printing functions, and socket setup. It uses non-blocking sockets and provides timeout mechanisms. The server processes load instructions, prints events conforming to project specifications, and includes placeholders for additional features. 


# Running the Reliable UDP Server:
Compilation:
Ensure you have a C compiler installed (e.g., gcc).

gcc server.c -o server
Execution:
Run the compiled server executable with the following command:
./server <PORT> <ISN>
Replace <PORT> with the desired port number and <ISN> with the initial sequence number. For example:
./server 12345 1000
This command starts the server on port 12345 with an initial sequence number of 1000.
Observing Output:
The server will print events such as "RECV," "SEND," and "TIMEOUT" according to the protocol specifications. Additionally, it will create files (e.g., 1.file, 2.file) containing received data.
Termination:
Terminate the server manually (e.g., using Ctrl+C) after testing.

# Diagram
https://www.geeksforgeeks.org/sliding-window-protocol-set-2-receiver-side/

![Sliding_SET_2-4](https://github.com/Nikolair1/UDPServer/assets/93243326/0623d281-1266-4a8a-bd9b-bfdfccb71781)
