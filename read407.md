# Authentication


## Singleton
A singleton is a class that allows only a single instance of itself to be created and gives access to that created instance. It contains static variables that can accommodate unique and private instances of itself. It is used in scenarios when a user wants to restrict instantiation of a class to only one object. This is helpful usually when a single object is required to coordinate actions across a system.

The singleton pattern is used in programming languages such as Java and .NET to define a global variable. A single object used across systems remains constant and needs to be defined only once rather than many times.

## Router Middleware
Router is one of those middleware, what it does actualy is to take the original request, and forward it to a sub handler according to the path example : "/home" for a GET request is mapped to function getHome that handle it and eventually send a response to the client on the behalf of the original handler.

## Dynamic Module Loading
Dynamic code loading allows an app to pull content from beyond its codebase and execute it during operation, or runtime. This option can result in a smaller app size because a common practice is to store the code remotely instead of embedding it in the Android package kit (APK)

## CRUD -> REST Method Matches
The HTTP verbs comprise a major portion of our “uniform interface” constraint and provide us the action counterpart to the noun-based resource. The primary or most-commonly-used HTTP verbs (or methods, as they are properly called) are POST, GET, PUT, PATCH, and DELETE. These correspond to create, read, update, and delete (or CRUD) operations, respectively. There are a number of other verbs, too, but are utilized less frequently. Of those less-frequent methods, OPTIONS and HEAD are used more often than others.

## Mock Testing
Mocking means creating a fake version of an external or internal service that can stand in for the real one, helping your tests run more quickly and more reliably. When your implementation interacts with an object's properties, rather than its function or behavior, a mock can be used

Mocking is a process used in unit testing when the unit being tested has external dependencies. The purpose of mocking is to isolate and focus on the code being tested and not on the behavior or state of external dependencies

n object-oriented programming, mock objects are simulated objects that mimic the behavior of real objects in controlled ways, most often as part of a software testing initiative. ... The technique is also applicable in generic programming

Mocking is done when you invoke methods of a class that has external communication like database calls or rest calls. Through mocking you can explicitly define the return value of methods without actually executing the steps of the method

## Securing Passwords :
Passwords are the first line of defense against cyber criminals. It is the most vital secret of every activity we do over the internet and also a final check to get into any of your user account, whether it is your bank account, email account, shopping cart account or any other account you have.

* Cryptographic hash algorithms MD5, SHA1, SHA256, SHA512, SHA-3 are general purpose hash functions, designed to calculate a digest of huge amounts of data in as short a time as possible
* The benefit of hashing is that if someone steals the database with hashed passwords, they only make off with the hashes and not the actual plaintext passwords 

## Basic Auth 

* to provide a user name and password when making a request. In basic HTTP authentication, a request contains a header field in the form of Authorization: Basic , where credentials is the Base64 encoding of ID and password joined by a single colon

* is the simplest technique for enforcing access controls to web resources because it does not require cookies, session identifiers, or login pages; rather, HTTP Basic authentication uses standard fields in the HTTP header.

## OWASP auth Cheat Sheet

* Authentication is the process of verifying the identity of a user.
* Session Management is the process of maintaining a session between the client and the server.

* Authentication General Guidelines:
* User IDs
1. case-insensitive
2. must be unique
* Implement Proper Password Strength Controls
1. Password Length
* must be at least 8 characters long
2. usage of all characters
* must contain at least one upper case letter
* must contain at least one lower case letter
* must contain at least one number
* must contain at least one special character
* Password Recovery Mechanism
* Compare Password Hashes Using Safe Functions
1. set a maximum number of inputs
2. Explicitly sets the type of both variable
3. Returns in constant time
* Change Password Feature
* Transmit Passwords Only Over TLS or Other Strong Transport
* The login page and all subsequent authenticated pages must be exclusively accessed over TLS or other strong transport.

## bcrypt docs

A library to help you hash passwords, The bcrypt hashing function allows us to build a password security platform that scales with computation power and always hashes every password with a salt

## Preview
**Which 3 things had you heard about previously and now have better clarity on?**

* ES6 Classes
* Testing

**Which 3 things are you hoping to learn more about in the upcoming lecture/demo?**

* PostgreSQL
* Data Modeling

**What are you most excited about trying to implement or see how it works?**

* Data Structures
* Authentication
* SQL Databases

## Review, Research, and Discussion

**Explain what a “Singleton” is (in Computer Science terms)**

Is an object which can only be instantiated one time

**Explain how the Singleton pattern can be used with Node modules, specifically with classes**

Using ES6, you can represent a singleton using ES Modules

**If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?**
I will create a global Middleware to run on every HTTP request of the application and Routing Middleware to test a specific route