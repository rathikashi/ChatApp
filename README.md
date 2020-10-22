# RAKSHA-FORGE

Fast Online Runtime for Garbled-circuit Execution

This project aims to implement fast online runtime for Garbled-circuit Execution in JavaScript. The idea is as follows:
We use the CBMC-GC compiler hosted on our server, to convert the program to a circuit. 
The Circuit is garbled in Javascript and sent by the protocol initiator to the other. 
The two engage in oblivious transfer to exchange the relevant information. 
Both parties receive the output of their function. 

In order to establish the P2P connection, we use PeerJS, a JavaScript library framework. The server initiates a connection between the two peers, following which
all communication is carried out by the peers with no involvement of the server. 
