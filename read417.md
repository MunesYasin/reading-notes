# AWS: Cloud Servers 

## Review, Research, and Discussion 

* **Describe the Web-Request-Response-Cycle**

All backend technologies and web APIs are based on one system that is The Request-Response Cycle. The system is responsible for data interchange between client and servers. ... Request/Response objects are transmitted over the web. Content like images, HTML, CSS, JavaScript is all Response Objects.


* **Explain what a “server” is, as it relates to the WRRC**

The client (usually a browser) opens a connection to the server and sends a request. The server processes the request, generates a response, and closes the connection if it finds a Connection: Close header. ... Headers may provide various information about the request or the client body data.


* **What does it mean to “deploy” an application?**

Application Deployment (also referred to as Software Deployment) is the process of installing, configuring, and enabling a specific application or set of applications, usually through an application manager (app manager) or software management system, to a specific URL on a server.

## Document the following Vocabulary Terms

* **Server:**is a computer on a network that manages network resources. Servers are referred to as “dedicated” meaning they are designed to perform a specific task.
* **Pub/Sub :**Publish/subscribe messaging, or pub/sub messaging, is a form of asynchronous service-to-service communication used in serverless and microservices architectures.
* **WRRC:** a cycle of requests and responses that flow between clients and servers.

## Preview 

* **Which 3 things had you heard about previously and now have better clarity on?**

* ROUTES, ENDPOINT , SOCKET

* **Which 3 things are you hoping to learn more about in the upcoming lecture/demo?**

* queue Message,

* Tree data structure,

* UDP

## Preparation Materials

### Virtual Machine
**Operating system:**

It is a software that control the hardware of a computer.
**Virtual Machine Manager:**
It is a software that allows us to run an operating system within another operating system.
Examples:
1. VirtualBox
2. vmware

* An operating system created by Virtual Machine Manager is called a Virtual Machine.

**Reasons to use Virtual Machines:**

* Trying a new operating system.
* Testing an application.
* Running old applications.

**Virtualization and Cloud Computing**
* **Virtualization** allows us to better utilize the resources we have available in out machine.
Virtualization is when many Virtualization Machines are controlled and operate inside one single machine. This gives us the following advantages:

* Fewer machines.
* Lower capital investment.
* Centralized management.
* Lower operation cost.

* **Cloud Computing** is when someone is using a computer that is in another location.

**AWS EC2**

It’s a service provided by Amazon. The term AWS EC2 stands for “Amazon Elastic Compute Cloud”. it is a web service that provides secure, resizable compute capacity in the cloud.

Amazon claims It is designed to make web-scale cloud computing easier for developers and it’s simple web service interface allows you to obtain and configure capacity with minimal friction. Also, It provides you with complete control of your computing resources and lets you run on Amazon’s proven computing environment.

**EC2 For Humans**

EC2 is a service, where clients can rent a like server (not physical machine) or in other words virtual machine, that is independent form other virtual machines that are on aws server.

Throw amazon site you can create an instance , where you can choose the type of operating system, memory size, number of CPUs, storage capacity and more.

This virtual machine can be used for storing data, web application, machine learning and more.

There are different settings that fit each usage, related to access and privacy.

**Elastic Beanstalk**
Elastic Beanstalk is a service that deploys, manages and scales web apps and services on behave of the developer.

Elastic Beanstalk uses managed containers like:

* java.net
* PHP
* Node.js
* Python
* Ruby
* docker
It also works on familiar servers such as :

* apache HTTP
* apache tomcat
* engin x
* passenger
* IIS
Elastic Beanstalk leverages familiar AWS services such as :

* Amazon EC2
* Amazon S3
* Amazon simple notification service
* Amazon elastic load balancing
* Amazon auto scaling
To start with Elastic Beanstalk you can use, AWS management console, the command line interface or the API. choose your platform and amazon EC2 instance type, then select additional resources to use such as Amazon relational database service, then upload yor code.

Elastic Beanstalk will handle Load Balancing, Provisioning, Auto Scaling and Application Health Monitoring.