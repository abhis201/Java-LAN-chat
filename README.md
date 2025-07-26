
# Java LAN Chat Application

Java LAN Chat is a UI-based chat application built with Java (NetBeans IDE) for local area networks. It consists of two main modules:

- **JServer**: The server application that manages user authentication, message routing, and file transfers.
- **JMessenger**: The client application that allows users to connect, chat, and send files over LAN.

## Features

- User authentication (login/signup) using XML-based storage
- Real-time chat between multiple users on the same network
- View online users
- File transfer between clients (no internet required)
- Simple, intuitive UI

## Architecture

### JServer
- Hosts the chat server on the local machine
- Authenticates users using credentials stored in an XML file (`Data.xml`)
- Handles multiple client connections
- Routes messages and files between clients

### JMessenger
- Connects to the server using its IP address
- Provides login and signup functionality
- Displays online users
- Supports one-to-one chat and file transfer

## Setup & Build Instructions

1. **Requirements:**
   - Java JDK 8 or higher
   - NetBeans IDE (recommended for building and running)

2. **Build the Server:**
   - Open the `jServer` project in NetBeans
   - Build the project (`build.xml` is provided)
   - Run the server: The server window will display its IP address

3. **Build the Client:**
   - Open the `jMessenger` project in NetBeans
   - Build the project
   - Run the client: Enter the server's IP address to connect

## Usage

1. **Start the Server:**
   - Run `jServer`. The server will listen for incoming connections and manage user authentication.

2. **Connect a Client:**
   - Run `jMessenger` on any machine in the same LAN
   - Enter the server's IP address
   - Login with existing credentials or sign up as a new user

3. **Chat & File Transfer:**
   - After login, view online users
   - Select a user to start chatting
   - Use the file send feature to transfer files directly over LAN

## XML-Based Authentication

- User credentials are stored in `Data.xml` (server side)
- Note: This method is not highly secure and is intended for demonstration/educational purposes

## Security Notes

- The application is designed for LAN use and does not implement strong encryption or secure authentication
- For production use, consider upgrading to a database and adding encryption

## Contributing

Pull requests and suggestions are welcome! Please open an issue for major changes.

## License

This project is for educational purposes.
