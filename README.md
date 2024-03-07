# File Transfer Application - Java
This Java application demonstrates a simple file transfer system 
between a client and a server using both traditional copy and zero copy techniques.
The project consists of two main components: ZClient (client-side) and ZServer (server-side).

# ZClient
 The ZClient program allows users to connect to a server, receive a list 
 of available files, choose a file for download, and perform the download 
 using either traditional or zero copy methods based on user input.
 
 # ZServer
 The ZServer program acts as a server, accepting client connections, 
 providing a list of available files, and handling file downloads using traditional or zero copy methods.

 # Implementation Details
The server listens on a specified port (SERVER_PORT) for client connections.
Upon connection, the server sends a list of available files to the client.
The server spawns a new thread (ClientHandler) for each connected client to handle file download requests.
File transfers can be performed in either traditional or zero copy mode.

# Important Notes
Ensure that the server is running before attempting to connect with the client.
Use consistent file paths between the client and server configurations.
This application is a basic demonstration and may require additional error handling and security measures for production use.
