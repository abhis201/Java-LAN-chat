# Java-Chatting-Application
This is a UI based Java Chatting App made on Netbeans having 2 mains directory

JServer
1. This file starts a server on the host's pc where many other clients on the same network can login using the server's IP address.
2. This file also runs an xml file which is used to store user authentication information(although not so secured).

JMessenger
1. This file is used to connect to the server just by using the IP address of the server where it is hosted.
2. After connecting to the server the user enters their username and password if they are old user and that data is authenticated by the server.
3. A new user can also signup by clicking the singup button.
4. The user after logging in can now see other users connected to the server and can chat with them.
5. JMessenger also supports file sending via LAN(without using the internet) which is very handy in a network.
