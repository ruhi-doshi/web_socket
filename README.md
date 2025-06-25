🔌 Python Socket Chat Server

This is a simple multi-client chat server written in Python using the socket and select modules. It allows multiple clients to connect, send messages, and receive messages from other connected clients in real-time.

🚀 Features

Accepts multiple client connections

Uses non-blocking I/O with select for efficient client handling

Simple custom protocol with fixed-size headers

Broadcasts messages to all other connected clients

Graceful handling of client disconnections

🛠️ How It Works

The server starts and listens for connections on a specified IP and port.

When a new client connects, they send a username.

Messages sent by clients are received with a fixed-size header indicating the message length.

The server forwards incoming messages to all other connected clients.

📌 Notes
This is only the server-side implementation. You’ll need a client script to connect and communicate.

The server uses a fixed-length header (HEADER_LENGTH = 10) to parse incoming messages correctly.
