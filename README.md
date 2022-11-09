# assignment2-300022472-300229069
Contents for Assignment 2.


(instructions for part 1 are below)
------------------------------------

<h1>Part 1:</h1>

This exercise will help you to become familiar with the internals of OCSF and Phase 1 of an instant messaging application we call SimpleChat. Modify the application to provide the following features (Remember: do not modify the OCSF framework):

<h2>Client Side</h2>
1. Currently, if the server shuts down while a client is connected, the client does not respond, and continues to wait for messages. Modify the client so that it responds to the shutdown of the server by printing a message saying the server has shut down, and quitting. Design hint: look at the methods called connectionClosed and connectionException.


2. The client currently always uses a default port. Modify the client so that it obtains the port number from the command line. Design hint: look at the way it obtains the host name from the command line. Test that this works by connecting a client to a server using a different port from the default. If the port is omitted from the command line, then the default value should still be used

<h2>Server Side</h2>
3. Currently the server ignores situations where clients connect or disconnect. Modify the server so that it prints out a nice message whenever a client connects or disconnects. Hint: you will simply have to write code in EchoServer that overrides certain methods found in AbstractServer – study the AbstractServer description above to determine which methods you have to override.
