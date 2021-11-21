# Event Driven Applications

## Review, Research, and Discussion
**Why is access control important?**

Access controls limit access to information and information processing systems. because it is a valuable security technique that can be used to regulate who or what can view or use any given resource

**Describe an application that would need access control.**

* Login credentials
* PINs and one-time passwords
* Virtual private network (VPN) access to internal networks.
**What is a role used for?**

A role is a collection of privileges that can be granted to one or more users or other roles

**Why is role based access control more scalable than discretionary or mandatory access control?**

it provides for defining and maintaining roles

## Vocabulary Terms
* Authorization :Authorization is the process of giving someone permission to do or have something.
* Role Based Access Control: is an approach that uses the job functions performed by individual users within the organization to determine their appropriate access levels
* Capabilities: capabilities is what a person has the ability or knowledge to do

 ## Preview
1. Which 3 things had you heard about previously and now have better clarity on?

SQL and Role Based Access Control.
2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

 Event Driven Programming
3. What are you most excited about trying to implement or see how it works? 

Events.

## Preparation Materials

### Event Driven Programming

**Event-Driven Programming is a logical pattern that we can choose to confine our programming within to avoid issues of complexity and collision .**

* Event-Driven Programming makes use of the following concepts:
 	 
An Event Handler is a callback function that will be called when an event is triggered.	

A Main Loop listens for event triggers and calls the associated event handler for that event.

* The Object Oriented approach promotes the idea that all behavior of an individual unit (or object) be handled from code within that unit. Using this approach, applications are built with many different units that all speak to and interact with each other.

” Much of the Node.js core API is built around an idiomatic asynchronous event-driven architecture in which certain kinds of objects (called “emitters”) emit named events that cause Function objects (“listeners”) to be called.

For instance: a net.Server object emits an event each time a peer connects to it; a fs.ReadStream emits an event when the file is opened; a stream emits an event whenever data is available to be read.

All objects that emit events are instances of the EventEmitter class. These objects expose an eventEmitter.on() function that allows one or more functions to be attached to named events emitted by the object. Typically, event names are camel-cased strings but any valid JavaScript property key can be used.

When the EventEmitter object emits an event, all of the functions attached to that specific event are called synchronously. Any values returned by the called listeners are ignored and discarded.”