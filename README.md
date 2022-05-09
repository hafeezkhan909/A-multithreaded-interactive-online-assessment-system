# A-Multithreaded-Interactive-Online-Assessment-System

# Directions:
1) run the main server
2) run the sub servers
3) run the client after running all of 3 sub servers 

# Compile:
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
