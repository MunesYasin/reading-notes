# Socket.io

## Review, Research, and Discussion

* What is the benefit of transforming data into packets?

  to meet the demands of pervasive data-centric applications and services
* UDP is often referred to as a connectionless protocol. Why is this?

  No connection needs to be established between the source and destination before you transmit data.
* Can a socket server application have multiple socket connections?, Can a socket connection application be connected to multiple socket servers?

  Multiple connections on the same server can share the same server-side IP/Port pair as long as they are associated with different client-side IP/Port pairs, and the server would be able to handle as many clients as available system resources allow it to

* Can an application be both a socket server and a socket connection?

    You can not combine server and client sockets into one, because a TCP/IP connection goes from a source port to a destination port

   ##  Document the following Vocabulary Terms

* Observer Pattern: The observer pattern is a software design pattern in which an object, named the subject, maintains a list of its dependents, called observers, and notifies them automatically of any state changes, usually by calling one of their methods.

* Listener: a procedure in JavaScript that waits for an event to occur.

* Event Handler: It is the function that will handle a particular proccess when an event occurred.

* Event Driven Programming: Event-driven programming is a programming paradigm in which the flow of program execution is determined by events - for example a user action such as a mouse click, key press, or a message from the operating system or another program.

* Event Loop: is a programming construct or design pattern that waits for and dispatches events or messages in a program.

* Event Queue: is a repository where events from an application are held prior to being processed by a receiving program or system.

* Call Stack: is a mechanism for an interpreter (like the JavaScript interpreter in a web browser) to keep track of its place in a script that calls multiple functions — what function is currently being run and what functions are called from within that function, etc.

* Emit/Raise/Trigger: these are terminologies to discribe some functionality in Event Driven Programming.

* Subscribe: This is a JavaScript object that defines the handlers for the notifications you receive.

* database: It is the palce that we are saving the data into.

## Preview 

**Which 3 things had you heard about previously and now have better clarity on?**

* User Role
* authentication & authorization
* ACL

**Which 3 things are you hoping to learn more about in the upcoming lecture/demo?**

* setting the role
* JWT.
* Bearer Authorization
 
 ## Preparation Materials 

 **Socket.io**

Socket.IO is a library that enables real-time and full-duplex communication between the Client and the Web servers. It uses the WebSocket protocol to provide the interface

**features of Socket.IO**

* It helps in broadcasting to multiple sockets at a time and handles the connection transparently.
* It works on all platform, server or device, ensuring equality, reliability, and speed.
* It automatically upgrades the requirement to WebSocket if needed.
* It is a custom real-time transport protocol implementation on top of other protocols.
* It requires both libraries to be used Client side as well as a server-side library.
* IO works on work-based events. there are some reserved events that can be accessed using the Socket on the server side like Connect, message, Disconnect, Ping and Reconnect.

**Why do we need Socket.IO:**

* It handle all the degradation of your technical alternatives to get full-duplex communication in real-time.
* It also handles the various support level and the inconsistencies from the browser.
* It also gives the additional feature room support for basic publish infrastructure and thinks like automatic reconnect.

