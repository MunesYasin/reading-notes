# Context API - Behaviors 

## Review, Research, and Discussion 

* When you have multiple contexts, what component type should you use (class/function) and why?

- Function

* What are some good use cases for using the Context API for global state?

- Authentication

* How can you best test context?

- The best way to test Context is to make our tests unaware of its existence and avoiding mocks.

## Terms

* context : Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language. For example, in the code below we manually thread through a “theme” prop in order to style the Button component: class App extends React.

* useContext() : “useContext” hook is used to create common data that can be accessed throughout the component hierarchy without passing the props down manually to each level. Context defined will be available to all the child components without involving “props”.

* static context : This rule applies when the static contextType property of a React component is not properly specified. The contextType property is used to consume a context created with React. ... When the property is specified for a React component, you can access the current value of the context using this.

## Preview 

* Which 3 things had you heard about previously and now have better clarity on?

JSX, events, class component

* Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

AWS, useEffect hook, useReducer hook

* What are you most excited about trying to implement or see how it works?

reducer hook & Redux

## Preparation Materials 

**Context api** 

Context provides a way to pass data through the component tree without having to pass props down manually at every level.

In a typical React application, data is passed top-down (parent to child) via props, but such usage can be cumbersome for certain types of props (e.g. locale preference, UI theme) that are required by many components within an application. Context provides a way to share values like these between components without having to explicitly pass a prop through every level of the tree.

* When to Use Context
- Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language.

Before You Use Context Context is primarily used when some data needs to be accessible by many components at different nesting levels. Apply it sparingly because it makes component reuse more difficult.

If you only want to avoid passing some props through many levels, component composition is often a simpler solution than context.

Hooks and context example After performing an audit on how we communicate with our users, we landed with a simple system of three classes of communication, and snackbars fit perfectly on the ‘low priority’ end of that spectrum. They are small notifications that show up on the screen when a user performs an action. They are not intrusive at all and appear for just a brief moment.

From an engineering standpoint, our snackbar system must easy to use and generally be very lightweight. We want to be able to place one on the screen with just a couple of lines of code. Anything more and it’s overkill.

This means forget render props and higher order components. We don’t want to deal with a messy React tree and wrappers. We don’t want action creators, reducers*, or any of that stuff.