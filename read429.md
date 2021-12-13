# Advanced State with Reducers

## Review, Research, and Discussion

* How can we ensure that an effect hook runs only once?

By passing an empty array ( [] ) as a second argument. This way React will run the code inside it only once on mount/unmount, and React will know that the effect doesn’t depend on any values from props or state, so it never needs to re-run

* Can useState() update more than one state variable at the same time?

Yes, useState() can be used multiple times to declare multiple state variable pairs

A single instance can’t but creating multiple state variables can.

* Is useState() synchronous?

No, its asynchronous

##  Terms

* State Hook : A Hook is a special function that lets you “hook into” React features. For example, useState is a Hook that lets you add React state to function components. We’ll learn other Hooks later

* Component Lifecycle : Components are created (mounted on the DOM), grow by updating, and then die (unmount on DOM). This is referred to as a component lifecycle. There are different lifecycle methods that React provides at different phases of a component’s life.At present, we know what lifecycle methods are and why they are important.

# Preview 

* Which 3 things had you heard about previously and now have better clarity on?

useState() Hook Component Lifecycle

* Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

useState() Hook Component Lifecycle

* What are you most excited about trying to implement or see how it works?

all feature for this week that we take

## Preparation Materials 

* What is the useReducer hook?

The useReducer() hook in React lets you separate the state management from the rendering logic of the component. const [state, dispatch] = useReducer(reducer, initialState) accepts 2 argument: the reducer function and the initial state.

* When is the useReducer hook used?

The useReducer is a hook used sometimes to manage the state of the application. It is very similar to the useState hook, just more complex. It acts as an alternate hook to the useState hook to manage complex state in your application. The useReducer hook uses the same concept as the reducers in Redux.

* Does useReducer cause re render?

Quick summary ↬ In a React component, useState and useReducer can cause your component to re-render each time there is a call to the update functions. … In React components, there are times when frequent changes have to be tracked without enforcing the re-rendering of the component.