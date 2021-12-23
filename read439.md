# Redux - Additional Topics 

## Review, Research, and Discussion
* What’s the best practice for “pre-loading” data into the store (on application start) in a Redux application?

* The most 'redux-like' way of handling the pre-loading of data would be to fire off the asynchronous action in the lifecycle method (probably componentWillMount) of a Higher Order Component that wraps your app. However, you will not use the results of the API call directly in that component - it needs to be handled with a reducer that puts it into your app store. This will require you to use some sort of a thunk middleware to handle the asynchronous action. Then you will use mapStateToProps to simply pass it down to the component that renders the data.

* When using a thunk/async action that dispatches the actual action, which do you export from your reducer?

* The first solution suggested by the documentation is Redux Thunk. This middleware allows you to create Actions as more than plain objects. These new Actions can dispatch other Actions, other Thunks and also perform async operations inside them.

## Document the following Vocabulary Terms
* middleware: anything you put in the middle of one layer of the software and another to do a specific thing.

* thunk: the Redux's official version of async function middleware. The thunk middleware allows us to write functions that get dispatch and getState as arguments.

## Preview

* Which 3 things had you heard about previously and now have better clarity on?

middleware,thunk

* Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

middleware,thunk

* What are you most excited about trying to implement or see how it works?

middleware,thunk