# Event Driven Architecture 

## Review, Research, and Discussion 

* **What’s the difference between a FIFO and a standard queue?**

* Standard queues provide at-least-once delivery, which means that each message is delivered at least once. FIFO queues provide exactly-once processing, which means that each message is delivered once and remains available until a consumer processes it and deletes it
* **How can the server be assured a message was properly received?**

* because of the process of the Message queue architecture
* **What classic design pattern is best represented by event driven programming?**

* An event-driven architecture enables applications to act on these events as they occur. This is in contrast to traditional architectures, which largely dealt with data as batches of information to be inserted and updated at some defined interval, and responded to user-initiated requests rather than new information.
* **How do you test an event driven system?**

    * There are multiple levels of tests you will typically write for your system. In the most canonical case, you will write unit tests, service tests, and end-to-end tests. In each of these cases, your System Under Test (SUT, what is actually being tested) comprises a different part of your application

   ## Terms 
* FIFO Queue:

The operations of a queue make it a first-in-first-out (FIFO) data structure. In a FIFO data structure, the first element added to the queue will be the first one to be removed. … A queue is an example of a linear data structure, or more abstractly a sequential collection.

* Pub/Sub
an asynchronous messaging service that decouples services that produce events from services.

## Preview
* **Which 3 things had you heard about previously and now have better clarity on?**

* Queues, FIFO vs standard Queues, AWS

* **Which 3 things are you hoping to learn more about in the upcoming lecture/demo?**

* AWS, SNS, SQS

* **What are you most excited about trying to implement or see how it works?**

* AWS, SNS, SQS

## Preparation Materials

**SNS vs SQS**

**SNS** is a distributed publish-subscribe service.

**SQS** is distributed queuing service.

* You can have SNS send messages to email, sms or http end point apart from SQS.

* There are advantages to coupling SNS with SQS. You may not want an external service to make connections to your hosts (firewall may block all incoming connections to your host from outside).

* **SNS** is a fast, flexible, fully managed push notification service that lets you send individual messages or to bulk messages to large numbers of recipients.

