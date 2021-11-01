# What’s the difference between PUT and PATCH? 

PUT: Is a method of modifying resource where the client sends data that updates the entire resource. It is used to set an entity’s information completely

PATCH: Applies a partial update to the resource. This means that you are only required to send the data that you want to update, and it won’t affect or change anything else.

# Provide links to 3 services or tools that allow you to “mock” an API for development like json-server 

* https://www.npmjs.com/package/mockserver
* https://www.mockable.io/
* https://stoplight.io/mocking 

#  Which HTTP status codes should be sent with each type of (un)successful API call? 

Client error responses (400–499)

Server error responses (500–599)

# Document the following Vocabulary Terms

Web Server - a computing system that stores, processes, and delivers resources for the web.

Express - a backend web application framework for Node.js, designed for building web apps and APIs.

Routing - a mechanism where HTTP requests are being sent to the code that handles them.

WRRC - Web Request/Response Cycle, the cycle describes how web apps actually works: server contain all the required resources, clients need some of them to show web pages, so clients requests resources from the servers and the servers process those requests and send responses.


# Compare and contrast SOAP and ReST

SOAP stands for Simple Object Access Protocol whereas REST stands for Representational State * Transfer.

SOAP is a protocol whereas REST is an architectural pattern.

SOAP uses service interfaces to expose its functionality to client applications while REST uses Uniform Service locators to access to the components on the hardware device.

SOAP needs more bandwidth for its usage whereas REST doesn’t need much bandwidth.

SOAP only works with XML formats whereas REST work with plain text, XML, HTML and JSON.

SOAP cannot make use of REST whereas REST can make use of SOAP.