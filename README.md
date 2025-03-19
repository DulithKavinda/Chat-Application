# Chat-Application

 
This group chat application is designed using socket programming in the C programming 
language. It operates on a client-server model where a single server manages multiple clients. 
It is compatible with Ubuntu, Linux, and MacOS and can be executed both locally or across 
separate computers. 
¨ Let’s execute the program Linux terminal with GCC compiler. 
 
 
Execution Guide>> 
 
1. Opening Terminals 
• Open separate terminals for the server and individual clients. If executing on 
separate computers, you can run a server on one computer and clients on another 
computer. The computer that runs the server can also run clients. 
2. Compiling Server Code 
• In the server terminal, compile the server code using the following command: 
gcc server.c -o server.out -pthread 
 
3. Compiling Client Code 
• In each client's terminal, compile the client code using the following command: 
gcc client.c -o client.out -pthread 
 
4. Running the Server 
• Execute the server using the following command, ensuring the specified port 
number: 
./server.out <port_number> 
Example:    ./server.out 8080 
 
5. Running Clients 
Note:- Ensure uniqueness of usernames for each client. 
 
• For local execution (same computer): 
./client.out <username> <local_server_IP_address> <port_number> 
Example: ./client.out Nimal 127.0.0.1 8080 
 
• For separate computer execution: 
./client.out <username> <server_IP_address> <port_number> 
Example: ./client.out Kamal 172.20.10.2 8080

Type messages in the client terminal to have them displayed in other clients' 
terminals along with the sender's name.
