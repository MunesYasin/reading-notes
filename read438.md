# Redux - Asynchronous Actions 

## How granular should your reducers be?
* Generally, as granular as possible. This allows for easier organizing, debugging, and testing. It also allows you to more easily add new features or remove features in the future.

## Pro or Con – multiple reducers can “fire” when a commonly named action is dispatched
* PRO! Having multiple reducers fire on a shared action is a great way to handle complex state changes in a predicable, reliable, and modular way, as long as it is intended.
## Name a strategy for preventing the above
* Use explicit names for each action to prevent unintended firing (i.e. don’t use ‘RESET’ for every reducer… unless you want them all to reset at the same time

* store: the object created by redux that stores all states for a given application. This is the single source of truth for our application.
* combined reducers: a way redux allows us to ‘export’ many reducer files from a single source to our store, so that they are all available in different parts of an app.

## Asynchronous Actions
introduction

* By default, Redux’s actions are dispatched synchronously, which is a problem for any non-trivial app that needs to communicate with an external API or perform side effects. Redux also allows for middleware that sits between an action being dispatched and the action reaching the reducers.

* There are two very popular middleware libraries that allow for side effects and asynchronous actions: Redux Thunk and Redux Saga. In this post, you will explore Redux Thunk.

* Thunk is a programming concept where a function is used to delay the evaluation/calculation of an operation.

* Redux Thunk is a middleware that lets you call action creators that return a function instead of an action object. That function receives the store’s dispatch method, which is then used to dispatch regular synchronous actions inside the function’s body once the asynchronous operations have been completed.

Using Redux Thunk in a Sample Application

* The most common use case for Redux Thunk is for communicating asynchronously with an external API to retrieve or save data. Redux Thunk makes it easy to dispatch actions that follow the lifecycle of a request to an external API.