# Component Lifecycle / useEffect() Hook 

## Review, Research, and Discussion

* Why do we not need more .html pages in a multi-page React app? 

Using the react-router-dom package, we can implement multiple routes in a React application. A user browsing this app feels each route is on each page. So in React, multiple routes are considered as multiple pages.

* If we wanted a component to show up on every page, where would we put it and why?

- Outside the
- Inside the , outside a
- Inside a
- Inside BrowserRouter and inside a Route 

* What does routing do with the components that were rendered when a new route is requested ?

- One way to do would be to pass the component prop an inline function. When you use component, the router uses React. createElement to create a new React element from the given component. That means if you provide an inline function to the component prop, you would create a new component every render.

* What does props.children contain?

- props. children does is that it is used to display whatever you include between the opening and closing tags when invoking a component. This component contains an  that is receiving some props and then it is displaying {props. children}

* How do useState() and this.setState() differ?

- setState() does not immediately mutate this. state but creates a pending state transition. Accessing this. state after calling this method can potentially return the existing value.

## Terms 

* State Hook : The state is an instance of React Component can be defined as an object of a set of observable properties that control the behavior of the component. In other words, the State of a component is an object that holds some information that may change over the lifetime of the component. 

* Mounting and Un-Mounting: Mounting: is the process of outputting the virtual representation of a component into the final UI representation (e.g. DOM or Native Components).

Un-Mounting: This method is called just before the component gets destroyed. Any clean up statements should be executed inside this method.

## Preparation Materials

**Using the Effect Hook**

* The Effect Hook lets you perform side effects in function components, Data fetching, setting up a subscription, and manually changing the DOM in React components are all examples of side effects.

* useEffect Hook as componentDidMount, componentDidUpdate, and componentWillUnmount combined.

* In React class components, the render method itself shouldn’t cause side effects. It would be too early — we typically want to perform our effects after React has updated the DOM.

* Placing useEffect inside the component lets us access the count state variable (or any props) right from the effect.

* By default, it runs both after the first render and after every update. (We will later talk about how to customize this.) Instead of thinking in terms of “mounting” and “updating”, you might find it easier to think that effects happen “after render”.

* Every effect may return a function that cleans up after it. This lets us keep the logic for adding and removing subscriptions close to each other.

* The Effect Hook unifies both use cases with a single API.

* Tips for Using Effects :

- Use Multiple Effects to Separate Concerns
- Optimizing Performance by Skipping Effect