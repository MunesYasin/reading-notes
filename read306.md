# What Is Node.js? 

Node.js is an event-based, non-blocking, asynchronous I/O runtime that uses Google’s V8 JavaScript engine and libuv library. 

**OR**

Node.js® is a JavaScript runtime built on Chrome’s V8 JavaScript engine. 

# How Do I Install Node.js? 

In this next section, we’ll install Node and write a couple of simple programs. We’ll also look at **npm**, a package manager that comes bundled with Node.

# Node Binaries vs Version Manager 

Many websites will recommend that you head to the official Node download page and grab the Node binaries for your system. While that works, I would suggest that you use a version manager instead. This is a program that allows you to install multiple versions of Node and switch between them at will. There are various advantages to using a version manager. For example, it negates potential permission issues when using Node with npm and lets you set a Node version on a per-project basis.

# Node.js Has Excellent Support for Modern JavaScript 

As can be seen on this compatibility table, Node has excellent support for ECMAScript 2015 (ES6) and beyond. As you’re only targeting one runtime (a specific version of the V8 engine), this means that you can write your JavaScript using the latest and most modern syntax. It also means that you don’t generally have to worry about compatibility issues — as you would if you were writing JavaScript that would run in different browsers. 

# What Is Node.js Used For? 

Now that we know what Node and npm are and how to install them, we can turn our attention to the first of their common uses: installing (via npm) and running (via Node) various build tools — designed to automate the process of developing a modern JavaScript application.

These build tools come in all shapes and sizes, and you won’t get far in a modern JavaScript landscape without bumping into them. They can be used for anything from bundling your JavaScript files and dependencies into static assets, to running tests, or automatic code linting and style checking.

We have a wide range of articles covering build tooling on SitePoint. Here’s a short selection of my favorites:

* A Beginner’s Guide to Webpack
* Up and Running with ESLint — the Pluggable JavaScript Linter
* An Introduction to Gulp.js
* Unit Test Your JavaScript Using Mocha and Chai

# The Node.js Execution Model 

Node.js, however, is single-threaded. It’s also event-driven, which means that everything that happens in Node is in reaction to an event. For example, when a new request comes in (one kind of event) the server will start processing it. If it then encounters a blocking I/O operation, instead of waiting for this to complete, it will register a callback before continuing to process the next event. When the I/O operation has finished (another kind of event), the server will execute the callback and continue working on the original request. Under the hood, Node uses the libuv library to implement this asynchronous (that is, non-blocking) behavior.

Node’s execution model causes the server very little overhead, and consequently it’s capable of handling a large number of simultaneous connections. The traditional approach to scaling a Node app is to clone it and have the cloned instances share the workload. Node.js even has a built-in module to help you implement a cloning strategy on a single server.

The following image depicts Node’s execution model:

![img](https://uploads.sitepoint.com/wp-content/uploads/2012/10/1516152673node_event_loop.png)

# 6 Reasons for Pair Programming 

1. Greater efficiency 

2. Engaged collaboration 

3. Learning from fellow students 

4. Social skills 

5. Job interview readiness 

6. Work environment readiness 