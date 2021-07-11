# Class 12 Summary :

###  Socket.io :

#### What is the benefit of transforming data into packets?

  * "Transfer the file data fast and efficient manner over the network and minimize the transmission latency, the data broken into peices of variable length".

#### UDP is often refereed to as a connectionless protocol. Why is this?

  * "because it is analogous to sending a letter where you don't acknowledge receipt. no connection neeeds to be established between the source and destination before transmit data. UPD does not have a mechanism to make sure that the payload is not corrupted".

#### Can a socket server application have multiple socket connections?
  
  * "Ports are a way to multiplex IP addresses so that different applications can listen on the same IP address/protocol pair. Unless an application defines its own higher-level protocol, there is no way to multiplex a port. If two connections using the same protocol have identical source and destination IPs and identical source and destination ports, they must be the same connection. Thus multiple client using same protocol may use same socket of server seemingly multi-threading".

#### Can a socket connection application be connected to multiple socket servers?

  * yes it is posiible if we make a lot of connections in a short time.

#### Can an application be both a socket server and a socket connection?

  * Yes we can , if we are willing to use two different ports. or if the sockets won't be using the same port at the same time.

#### Document the following Vocabulary Terms :

| Term      |                                                          |
| -----------  | ----------------------------------------------------------------|
|Observer Pattern  | software design pattern in which an object, named the subject, maintains a list of its dependents, called observers, and notifies them automatically of any state changes, usually by calling one of their methods.  |
|Listener  | procedure or function in a computer program that waits for an event to occur.  |  
| Event Handler |handle and verify user input, user actions, and browser actions   |
| Event Driven Programming |  programming paradigm in which the flow of the program is determined by events such as user actions (mouse clicks, key presses), sensor outputs, or message passing from other programs or threads.   |
|Event Loop  | programming construct or design pattern that waits for and dispatches events or messages in a program.  |  
|Event Queue  | repository where events from an application are held prior to being processed by a receiving program or system.  |
|Call Stack  | stack data structure that stores information about the active subroutines of a computer program.    |
| Emit/Raise/Trigger |in event-driven programming, emit sends a message to trigger a response and raise an event   |  
|Subscribe  |subscribe dom events in browser or node.js events.   |
|database  |  an organized collection of structured information, or data, typically stored electronically in a computer system   |


#### Web Socket :

   * WebSocket :"is a library that enables real-time, bidirectional and event-based communication between the browser and the server".
     *  "is a computer communications protocol, providing full-duplex communication channels over a single TCP connection".

   * Consists of :
     1. a Node.js server : Source & API
     2. a javascript client library for the browser.

#### Socket.IO :

  * "enables real-time bidirectional event-based communication. It works on every platform, browser or device, focusing equally on reliability and speed. Socket.IO is built on top of the WebSockets API (Client side) and Node.js. It is one of the most depended upon library on npm (Node Package Manager)".

#### Web Sockets VS Socket.io

![image1](https://cdn.educba.com/academy/wp-content/uploads/2018/11/WebSockets-vs-Socket-1.jpg.webp)






### Sources:

[source1](https://docs.oracle.com/cd/E19620-01/805-4041/6j3r8iu2f/index.html)

[source2](https://www.quora.com/Can-a-socket-of-a-server-be-used-by-multiple-clients-simultaneously)

[source3](https://www.quora.com/Can-you-make-a-client-socket-and-a-server-socket-in-one)

[source4](https://socket.io/docs/v4/index.html)

[source5](https://en.wikipedia.org/wiki/WebSocket)

[source6](https://www.educba.com/websocket-vs-socket-io/)





