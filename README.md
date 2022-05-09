# A-Multithreaded-Interactive-Online-Assessment-System

Details:

There will be a main server and three sub-servers (for three different tests). The main server does not want to overburden itself by communicating with all the incoming clients and handle the tests, so it only stores the info about which sub-server contains what sort of test (Three subservers each of which contains one type of test i.e., Science, Math or English). When a sub-server connects to the main server it sends the main server a string containing the Test Name which it can carry out along with its IP and Port number (e.g. Mathematics, Sub-server IP, Sub-server Port). Whenever a client connects to the main server, it will display three kinds of tests (Science, Mathematics and English) to the client. The client will then choose the type of test (e.g., Math). The main server will then send the information of corresponding sub-server to the client. The client will then connect to the corresponding sub-server. The sub-server will then show different types of the corresponding test (e.g, Geometry, Algebra and IQ for Math Sub-server) to the client. The client will select the test type and complete the test (You don’t need any test. Just make the sub-server to assign random marks to the client from 1 to 100). Then sub-server will send the information related to client (Client IP, Client Port, Test Name, Test Type, Marks) back to main server and also to the client. The client will then terminate. The main server will store the information within a file for all the clients.

Directions:
```bash
1) run the main server
2) run the sub servers
3) run the client after running all of 3 sub servers 
```

Compile:
```bash
gcc -std=c11 main_server.c -o main_server
gcc -std=c11 sub_server_1.c -o sub_server_1
gcc -std=c11 sub_server_2.c -o sub_server_2
gcc -std=c11 sub_server_3.c -o sub_server_3
gcc -std=c11 client.c -o client
```

Commands to execute:
```bash
./main_server
./sub_server_1
./sub_server_2
./sub_server_3
./client
```
