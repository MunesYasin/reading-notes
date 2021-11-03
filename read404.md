# Express REST API 

## Review, Research, and Discussion 

* **Name 3 real world use cases where you’d want to change the request with custom middleware** 

1. Login authentication 
2. Async Actions 
3. Data streaming

* **True or false: The route handler is middleware?**

true 

* **In what ways can a middleware function end the process and send data to the browser?** 

Through the use of the next() Or 500 errors. If an error is triggered, it will end the WRRC and send the 500 message to the user through the broswer. 

* **At what point in the request lifecycle can you “inject” middleware?**

Middleware can be injected to shape the way the request object 

* **What can cause express to error with “Request headers sent twice, cannot start a second response”** 

When a server tries to send several responses for one request 

## Document the following Vocabulary Terms

Term | Def
------------ | -------------
Middleware | Middleware functions are functions that have access to the request object ( req ), the response object ( res ), and the next middleware function in the application’s request-response cycle. The next middleware function is commonly denoted by a variable named next . 
Request Object | The req object represents the HTTP request and has properties for the request query string, parameters, body, HTTP headers, and so on. 
Response Objec | The res object represents the HTTP response that an Express app sends when it gets an HTTP request. 
Application Middleware | Application level middleware are bound to an instance of express, using app. use() and app. VERB(). Router level middleware work just like application level middleware except they are bound to an instance of express 
Routing Middleware | the way in which the client requests are handled by the application endpoints. And when you make some routers in separate file, you can use them by using middleware. 
Test Driven Development | an iterate process that begins with writing a test code for an application or function before starting out to write the application. … The next steps entails writing and refactoring the application until it passes the test code 
Behavioral Testing | Unit testing is a methodology where units of code are tested in isolation from the rest of the application. A unit test might test a particular function, object, class, or module. Unit tests are great to learn whether or not individual parts of an application work. NASA had better know whether or not a heat shield will work before they launch the rocket into space. 

