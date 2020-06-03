---------------------------------------------------------------------------------------------------------------------------                   Creating a CLI internet chat interface
---------------------------------------------------------------------------------------------------------------------------
                   
Problem Statement:

Implement a websockets based chat server that can be used for exchanging text messages as well as running system commands on the other machine (linux). You need to devise a protocol to identify the type of incoming data and correspondingly treat it like a text message or an instruction to run a command.

The messages should be encrypted with RSA to ensure that the socket stream is secure.

Requirements:

1. Implement the chat server to serve multiple clients which should be emulated in the solution.
2. The chat server should have only one worker.
3. Multiple requests from different clients must be handled by implementing a priority message queue.
4. The messages should be encrypted using RSA.
5. The server should also respond to the client with the ACK message after each successful operation and NOACK for each failure[if the linux command throws up an error].
6. Your assignment pipeline should have 1 server with 20 clients, each sending messages to the server that are randomly selected from a message.txt files that should also be included along with the assignment.
7. The pipeline should have details logs for both the client and the server for each and every operation.

Requirements:
python3
`````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````
How to run this code:
pip install rsa //to to use RSA encryption and De-cryption 
on a linux terminal:

run commnand: python3 server.py

on another linux terminal
run commnad: python3 client*.py
(where * is the client no, eg client1.py)
`````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````


