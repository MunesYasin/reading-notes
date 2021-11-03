# Data Modeling 

## Review, Research, and Discussion 

* **Name 3 advantages to Test Driven Development** 

* The software design becomes modular.

* The code is easier to maintain and Code refactoring goes more smoothly.

* Developers have less debugging to do and Project costs descrease.

* **In what case would you need to use beforeEach() or afterEach() in a test suite?** 

If you have some work you need to do repeatedly for many tests beforeEach() can be used before an event takes place so we could initialize a database. Followed by afterEach() which could clear out the results in a database.


* **What is one downside of Test Driven Development** 

The downside to TDD is that it is usually tightly associated with 'Agile' methodology, which places no importance on documentation of a system, rather the understanding behind why a test 'should' return one specific value rather than any other resides only in the developer's head.

* **What’s the primary difference between ES6 Classes and Constructor/Prototype Classes?**

A child of an ES6 class is another type definition which extends the parent with new properties and methods, which in turn can be instantiated at runtime. ... A class constructor creates an instance of the class. A constructor in JavaScript is just a plain old function that returns an object.

* **Why REST?**

they provide a great deal of flexibility. Data is not tied to resources or methods, so REST can handle multiple types of calls, return different data formats and even change structurally with the correct implementation of hypermedia


## Document the following Vocabulary Terms

Term | Def
------------ | -------------
functional programming |  a programming paradigm built on the concept of composing pure functions to build software.
object-oriented programming (OOP) | a programming paradigm built on the concept of objects that contain both data and code to modify the data.
class |a special function that encapsulates data and methods that manipulate data to create objects.
super | a keyword used to access the object's parent and call functions on it.
this | a keyword refers to the object it belongs to. It has different values depending on where it is used.
Test Driven Development (TDD) | a software development approach in which test cases are developed to specify and validate what the code will do.
Jest | a JavaScript testing framework used for creating, running, and structuring tests.
Continuous Integration (CI) | the practice of automating the integration of code changes from multiple contributors into a single software project.
REST |  architectural style for providing standards between computer systems (like clients or servers) on the web, making it easier for systems to communicate with each other.
Data Model | an abstract model that organizes elements of data and standardizes how they relate to one another and to the properties of real-world entities. 
