# Redux - Combined Reducers

## Why choose Redux instead of the Context API for global state?
Context API is easy to is use as it has a short learning curve. It requires less code, and because there's no need of extra libraries, bundle sizes are reduced. Redux on the other hand requires adding more libraries to the application bundle. The syntax is complex and extensive creating unnecessary work and complexity

## What is the purpose of a reducer?
A reducer is a function that determines changes to an application's state. It uses the action it receives to determine this change. We have tools, like Redux, that help manage an application's state changes in a single store so that they behave consistently.

## What does an action contain?
Redux data flow. Actions: Actions are a plain JavaScript object that contains information. Actions are the only source of information for the store. Actions have a type field that tells what kind of action to perform and all other fields contain information or data.

## Why do we need to copy the state in a reducer?
If the new state is different, the reducer must create new object, and making a copy is a way to describe the unchanged part.

## Document the following Vocabulary Terms
* immutable state Immutable state means its value cannot be changed once it's created. ... A mutable state allows us to modify already created data structures and change them whichever way we want.

* time travel in redux The Redux DevTools records dispatched actions and the state of the Redux store at every point in time. This makes it possible to inspect the state and travel back in time to a previous application state without reloading the page or restarting the app.

* reducer The concept of a Reducer became popular in JavaScript with the rise of Redux as state management solution for React. But no worries, you don't need to learn Redux to understand Reducers. Basically reducers are there to manage state in an application. For instance, if a user writes something in an HTML input field, the application has to manage this UI state (e.g. controlled components).

* dispatch Redux doesn't have a Dispatcher or support many stores. Instead, there is just a single store with a single root reducing function. As your app grow