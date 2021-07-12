# Class 13 Summary:

### Message Queues :

#### What does it mean that web sockets are bidirectional? Why is this useful?
  * " Client and server are connected by two ways (from client to server and from server to client). it is useful in increasing speed and realtime capability on the web and also in keeping track of clients".

#### Does socket.io use HTTP? Why?
  * Yes it is , " a socket.io server will attach to an HTTP server so it can serve its own client code through /socket.io/socket.io.js".

#### What happens when a client emits an event?
  * " The event gets passed to the server through websockets. Its a tcp connection from the browser to the server. The connection is full duplex meaning the server can send real time data to the client and vise versa".

#### What happens when a server emits an event?
  * "All listening client will execute the handeler for that event".

#### What happens if a client “misses” an event?
  * The Event Handler will be excuted.

#### How can we mitigate this?
  * By using message queue.

#### Document the following Vocabulary Terms

| Term      |                                                          |
| -----------  | ----------------------------------------------------------------|
|Socket  | one endpoint of a two-way communication link between two programs running on the network   |
| Web Socket |provides the API for creating and managing a WebSocket connection to a server, as well as for sending and receiving data on the connection.    |
| Socket.io  |Socket.IO enables real-time, bidirectional and event-based communication. It works on every platform, browser or device, focusing equally on reliability and speed. |
| Client  |piece of computer hardware or software that accesses a service made available by a server as part of the client–server model of computer networks|
| Server  | piece of computer hardware or software (computer program) that provides functionality for other programs or devices, called "clients"   |
| OSI Model  | (Open Systems Interconnection Model) is a conceptual framework used to describe the functions of a networking system.    |
| TCP Model | a concise version of the OSI model. It contains four layers, unlike seven layers in the OSI model. The layers are:Process/Application Layer, Host-to-Host/Transport Layer,Internet Layer and Network Access/Link Layer   |
|TCP  | is one of the main protocols of the Internet protocol suite. It originated in the initial network implementation in which it complemented the Internet Protocol (IP).  |
|UDP  |  is one of the core members of the Internet protocol suite. With UDP, computer applications can send messages, in this case referred to as datagrams, to other hosts on an Internet Protocol (IP) network.   |
|Packets |  basic units of communication over a TCP/IP network. Devices on a TCP/IP network divide data into small pieces, allowing the network to accommodate various bandwidths, to allow for multiple routes to a destination, and to retransmit the pieces of data which are interrupted or lost|


### Socket.io :
  * Rooms : "A room is an arbitrary channel that sockets can join and leave. It can be used to broadcast events to a subset of clients":

  ![image1](https://socket.io/images/rooms.png)

  * "Each Socket in Socket.IO is identified by a random, unguessable, unique identifier Socket#id. For your convenience, each socket automatically joins a room identified by its own id".

  * multiple Socket.IO servers :

  ![image2](https://socket.io/images/rooms-redis.png)

  * "The “room” feature is implemented by what we call an Adapter". This Adapter is a server-side component which is responsible for:
   1. storing the relationships between the Socket instances and the rooms
   2. broadcasting events to all (or a subset of) clients.
  
  * Reserved events : "On each side, the following events are reserved and should not be used as event names by your application":

   1. connect
   2. connect_error
   3. disconnect
   4. disconnecting
   5. newListener
   6. removeListener


#### Sources:
[source1](https://stackoverflow.com/questions/37836130/socket-io-why-does-it-need-an-http-server)
[source2](https://stackoverflow.com/questions/48332454/how-does-socket-io-on-the-client-listen-to-events-emitted-from-server)
[source3](https://developer.mozilla.org/en-US/docs/Web/API/WebSocket)
[source4](https://kb.iu.edu/d/anyq)
[source5](https://socket.io/docs/v3/rooms/index.html)
[source6](https://socket.io/docs/v3/emit-cheatsheet/index.html)



