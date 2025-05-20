# Chatroom using Socket Programming

A simple multi-user chatroom application built in **C** using **TCP sockets**. This project demonstrates how client-server communication can be implemented using low-level socket programming.

## 📌 Features

- Real-time messaging between multiple clients
- TCP socket-based communication
- Message broadcasting from server to all connected clients
- Simple command-line interface for both server and client

## 🗂️ File Structure

├── client.c # Client-side implementation
├── server.c # Server-side implementation
├── compile # Script to compile server and client


## 🛠️ Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/Vandanarangaswamy/chatroom-using-socketprogramming.git
cd chatroom-using-socketprogramming
```
### 2. Compile the Code
```bash
chmod +x compile
./compile
```
Or compile manually:
```bash
gcc server.c -o server
gcc client.c -o client
```

### 3. Run the Server

```bash
./server

```

The server will start listening on a port for incoming client connections.

### 4. Run Clients
Open multiple terminals and run:

```bash 
./client
```
You can run as many clients as needed to simulate a multi-user chatroom.

## 🧠 How It Works

- The server listens on a specified port for incoming TCP connections.
- Clients connect to the server using the server's IP and port.
- When a client sends a message, the server broadcasts it to all other connected clients.
- Ensures reliable message delivery using TCP.

## 📚 Concepts Demonstrated

- TCP socket programming in C
- Server-client architecture
- Handling multiple client connections (via threading or multiplexing)
- Real-time message broadcasting
- Graceful shutdown and error handling

## 📦 Requirements

- GCC compiler
- UNIX/Linux terminal environment
