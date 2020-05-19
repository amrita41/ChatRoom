TITLE:
A server-client console based Chat Application using Multithreading and Socket programming.

ABOUT:
A multithreaded client/server Chat Application based on console which uses Java Socket programming.
A Server listens for connection requests from Clients across network or even from the same machine.
Clients know how to connect to the server via an IP address and port number.
After connecting to Server, a Client gets to choose his/her username for the Chat room.
The Client sends message, the message is sent to the Server using ObjectOutputStream in JAVA.
After receiving message from Client, the server broadcasts the message if it is not a private message.
And if it is a private message which is detected using ‘@’ followed by a valid username, message is sent only to that user.
JAVA object serialization is used to transfer messages.

INSTRUCTIONS:
Client 

To start Client in console mode, use one of the following commands:-

*java Client
*java Client username
*java Client username portNumber
*java Client username portNumber serverAddress
At the console prompt, if the portNumber is not specified, 1500 is used. If the serverAddress is not specified "localHost" is used. If the username is not specified "Anonymous" is used.

Server

To start Client in console mode, use one of the following commands:-

*java Server
*java Server portNumber 
If the portNumber is not specified 1500 is used.

Chat

While in client console:-

Simply type the message to send broadcast to all active clients.
Type '@usernameyourmessage' without quotes to send message to desired client.
Type 'WHOISIN' without quotes to see list of active clients.
Type 'LOGOUT' without quotes to logoff from server.
