# Login  and Auth 

## Review, Research, and Discussion 

1. Why is the Context API useful?

The Context API is a React structure that enables you to exchange unique details and assists in solving prop-drilling from all levels of your application.

2. Can a component outside of a provider get its context?

To access a React context outside of the render function, we can use the useContext hook. We create the UserContext by calling the React. createContext method with a default context value. Then in the Users component, we call the useContext hook with UserContext to accxess the current value of UserContext.

3. What are some common use cases for using the Context API?

Some sample use cases where the Context API proves helpful are: Theming — Pass down app theme. i18n — Pass down translation messages. Authentication — Pass down current authenticated user.

Context is primarily used when some data needs to be accessible by many components at different nesting levels. Apply it sparingly because it makes component reuse more difficult. If you only want to avoid passing some props through many levels, component composition is often a simpler solution than context.

4. Describe “Context Hell”

the React Context hell is the nasty code you get taking advantage of the React Context API.

## Terms 

* global state:
This is the state of the entire React application that located in the context.

* global context :
This is context that affects the entire application, and it will share data to everything in the React component tree.

* provider:
The context provider accepts a value that will be passed to its children. All children components will re-render when the value changes.

* consumer :
This is a React component that subscribes to context changes in value of the Provider.

## Preparation Materials 

* we will combine Authentication (valid user is logged in) and Authorization (what permissions does the user have) to create a UI that ensures that users only have access to content and functionality that they’re granted access to.

* What is Role-Based Access Control (RBAC) ?

In computer systems security, role-based access control or role-based security is an approach to restricting system access to authorized users. It is used by the majority of enterprises with more than 500 employees, and can implement mandatory access control or discretionary access control.

BENEFITS OF RBAC

  - Reducing administrative work and IT support
  - Maximizing operational efficiency
  - Improving compliance


* React-cookies

Cookies are the data stored in the form of key-value pairs that are used to store information about the user on their computer by the websites that the users browse and use it to verify them.

To set or remove the cookies, we are using a third-party dependency of react-cookie
