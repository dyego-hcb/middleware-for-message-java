# Simple Java Middleware for Message Passing

This is a basic Java middleware project that allows multiple clients to send and receive messages through a central server. It provides a simple way for clients to communicate with each other via a server acting as a message relay.

## Features

- Clients can connect to the server and send messages.
- The server relays messages from one client to all other connected clients.
- Clients can disconnect by sending an "exit" message.

## Folder Structure

- The **[Source Code](./source_code/)** folder contains Java code related to the mentioned project.
- In the **[Output Test](./output_testes/)** folder, you will find some images of the server and client output, where we tested the application to verify if it was working correctly.

## Usage

### Server

1. Compile the `MiddlewareServer.java` file using `javac MiddlewareServer.java`.
2. Run the server with `java MiddlewareServer`.

The server will listen for incoming connections on port 12345 by default. You can modify the port in the source code if needed.

### Client

1. Compile the `Client.java` file using `javac Client.java`.
2. Run a client with `java Client`.

Clients will connect to the server and can start sending and receiving messages. To exit a client, simply send "exit."

## Dependencies

This project does not require any external dependencies. It uses Java's built-in `java.net` package for socket communication.