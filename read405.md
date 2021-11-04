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

## Preview

 * **Which 3 things had you heard about previously and now have better clarity on?**

* TDD
* Continuous Integration (CI)
* ES6 Classes

* **Which 3 things are you hoping to learn more about in the upcoming lecture/demo?**

* PostgreSQL
* Testing
* Data Modeling

* **What are you most excited about trying to implement or see how it works?**

* Data Structures
* Authentication
* SQL Databases

## SQL vs NoSQL Database 

*  SQL (Relational Databases): a good design (scheme and constraints defined correctly and transactions are used properly) allows the database engine to guarantee consistency based on that design.

*  NoSQL: lower consistency of information (it is a responsibility of the developer  to ensure consistency... some time this could be very difficult).

* **SQL Database Examples :**

* MySQL Community Edition
* MS-SQL Server Express Edition
* Oracle Express Edition
* **NoSQL Database Examples**

* MongoDB
* CouchDB
* Redis

![img](https://cdn-images-1.medium.com/fit/t/1600/480/0*xoC2DeugTHSh5yFV.jpg)

## sql modeling techniques :

There are many types of modeling software you can use to create models, such as MySql Workbench, which not only create smart looking diagrams

 **Model a relational database table that include :**

* The Table Name, which is located at the top of the table.
* The Primary Keys. Remember the primary keys uniquely identify each row in a table. A table typically has one primary key, but can have more. When the key has more than one column, it is called a compound key.
* Table Columns – There can be one or more table columns. To keep the diagrams simple, I don’t show the data types. I may introduce those later when we focus on more comprehensive modeling.
* Foreign Key – This is a column or set of columns which match a primary key in another table.

**Data Modeling – Table Relationships** 

* one-to-many relationship : an entry in one table can be related to more than one entry in another.
* many-to-one relationship: is similar to a one-to-many relationship, this difference is in the point-of-view you take when naming the relationship
* one-to-one
* zero or one-to-many