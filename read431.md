# Context API

## Review, Research, and Discussion

* Describe use cases useState() vs useReducer()

- Next state depends on the previous: It is always better to use this method when the state depends on the previous one.
- Complex state shape: When the state consists of more than primitive values, like nested object or arrays
- Easy to test: Reducers are pure functions, and this means they have no side effects and must return the same outcome given the same arguments.

* Why do custom hooks need the use prefix?

T- his convention is very important. Without it, we wouldn’t be able to automatically check for violations of rules of Hooks because we couldn’t tell if a certain function contains calls to Hooks inside of it.

* What do custom hooks usually do?

- Custom hooks allow us to have cleaner functional components, remove logic from the UI layer, and prevent code duplication by bringing common use cases to reusable hooks.
- Using any list of custom hooks, research and name one that you think will be useful in your applications

- useReducer

* Describe how a hook that fetches API data might work

- create an asynchronous function to fetch our data.
- Put the fetchData function above in the useEffect hook and call it
- Once we get a response, we are parsing it using the .json() function, meaning that we are transforming the response into JSON data that we can easily read

## Terms

* **reducer**: is a pure function that takes an action and the previous state of the application and returns the new state. The action describes what happened and it is the reducer's job to return the new state based on that action.

## Preview 

* Which 3 things had you heard about previously and now have better clarity on?

- API fetching ,conetxt api ,useContext

* Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

- API fetching ,conetxt api ,useContext

* What are you most excited about trying to implement or see how it works?

- API fetching ,conetxt api ,useContext


## Preparation Materials:

**Context API**
* Context provides a way to pass data through the component tree without having to pass props down manually at every level.

* Before You Use Context :Context is primarily used when some data needs to be accessible by many components at different nesting levels. Apply it sparingly because it makes component reuse more difficult.

* If you only want to avoid passing some props through many levels, component composition is often a simpler solution than context.

* Creates a Context object. When React renders a component that subscribes to this Context object it will read the current context value from the closest matching Provider above it in the tree.

* The defaultValue argument is only used when a component does not have a matching Provider above it in the tree. This can be helpful for testing components in isolation without wrapping them. Note: passing undefined as a Provider value does not cause consuming components to use defaultValue.

* Creates a Context object. When React renders a component that subscribes to this Context object it will read the current context value from the closest matching Provider above it in the tree.

* The defaultValue argument is only used when a component does not have a matching Provider above it in the tree. This can be helpful for testing components in isolation without wrapping them. Note: passing undefined as a Provider value does not cause consuming components to use defaultValue.

