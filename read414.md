# Message Queues 

## Review, Research, and Discussion 
* **What does it mean that web sockets are bidirectional? Why is this useful?**
* bidirectional because it allows you to send and receive data from the same computer

* **Does socket.io use HTTP? Why?**

* socket.io isn’t a pure Websocket server/implementation, it depends on HTTP for its initial connection setup.

* **What happens when a client emits an event?**
* the server receives the event

* **What happens when a server emits an event?**

* the client receives the event

* **What happens if a client “misses” an event?**

* the server receives the event

* **How can we mitigate this?**

* we can use a “heartbeat” to keep the connection alive

## Document the following Vocabulary Terms

* Socket :

 A socket is one endpoint of a two-way communication link between two programs running on the network. A socket is bound to a port number so that the TCP layer can identify the application that data is destined to be sent to. ... Every TCP connection can be uniquely identified by its two endpoints

* Web Socket

WebSocket is a computer communications protocol, providing full-duplex communication channels over a single TCP connection. The WebSocket protocol was standardized by the IETF as RFC 6455 in 2011, and the WebSocket API in Web IDL is being standardized by the W3C. WebSocket is distinct from HTTP

* Socket.io :

Socket.IO  is a JavaScript library for realtime web applications. It enables realtime, bi-directional communication between web clients and servers. It has two parts: a client-side library that runs in the browser, and a server-side library for Node.js. Both components have a nearly identical AP

* Client:

it is the library that runs inside the browser(Accesses services or functionality from server)

* Server : It is the library for Node.js(Provides services and functionality for clients)

* OSI Model :

(Open Systems Interconnection Model) is a conceptual framework used to describe the functions of a networking system. The OSI model characterizes computing functions into a universal set of rules and requirements in order to support interoperability between different products and software.

* TCP Model:

specifications for translating the network addressing methods used in the Internet Protocol to link-layer addresses, such as media access control (MAC) addresses.

* TCP:

Transmission control protocol. TCP provides reliable, ordered, and error-checked delivery of a stream of octets (bytes) between applications running on hosts communicating via an IP network. (Transmission Control Protocol - a connection-based communication protocol used for the transmission of data within a network.)

* UDP :

(User Datagram Protocol) is a communications protocol that is primarily used for establishing low-latency and loss-tolerating connections between applications on the internet. It speeds up transmissions by enabling the transfer of data before an agreement is provided by the receiving party.(a connectionless communication protocol used for time-sensitive transmission of data.)

* Packets :

a formatted unit of data carried by a packet-switched network. A packet consists of control information and user data; the latter is also known as the payload. Control information provides data for delivering the payload

## Preview
* **Which 3 things had you heard about previously and now have better clarity on?**

* Socket
* authentication & authorization
* ACL

* **Which 3 things are you hoping to learn more about in the upcoming lecture/demo?**

* Socket
* Socket.io (Links to an external site.)
* OSI Model

## Preparation Materials
**Rooms and Namespaces**

* **What is Room?**

* A room is an arbitrary channel that sockets can join and leave. It can be used to broadcast events to a subset of clients.
* rooms are a server-only concept.(i.e. the client does not have access to the list of rooms it has joined)
* Each Socket in Socket.IO is identified by a random, unguessable, unique identifier Socket#id.
* We can call join to subscribe the socket to a given channel.
* use to or in (they are the same) when broadcasting or emitting.
* You can emit to several rooms at the same time.
* **What are Namespaces?**
* Socket.IO allows you to Namespace your sockets, which essentially means assigning different endpoints or paths.
* This is a useful feature to minimize the number of resources (TCP connections) and at the same time separate concerns within your application by introducing separation between communication channels.
* Multiple namespaces actually share the same WebSockets connection thus saving us socket ports on the server.
* Namespaces are created on the server side. But they are joined by clients by sending a request to the server.