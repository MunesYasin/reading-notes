# Application State with Redux


## Review, Research, and Discussion 

What are the advantages of storing tokens in “Cookies” vs “Local Storage”

t’s just less convenient for the attacker because they can’t read the content of the token although they rarely have to. It might also be more advantageous for the attacker to attack using victim’s browser (by just sending that HTTP Request) rather than using the attacker’s machine.

Explain 3rd party cookies.

Third-party cookies are cookies that are set by a website other than the one you are currently on. For example, you can have a “Like” button on your website which will store a cookie on a visitor’s computer, that cookie can later be accessed by Facebook to identify visitors and see which websites they visited.

How do pixel tags work?

tracking pixel (also called 1x1 pixel or pixel tag) is a graphic with dimensions of 1x1 pixels that is loaded when a user visits a webpage or opens an email. … The tracking pixel URL is the memory location on the server. When the user visits a website, the image with the tag is loaded from this server

## Preview 

1.Which 3 things had you heard about previously and now have better clarity on?

JSX, context api, class component

2.Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

AWS, useEffect hook, useReducer hook

3.What are you most excited about trying to implement or see how it works?

reducer hook & Redux

## Preparation Materials 
Fundamentals of Redux Course from Dan Abramov (Links to an external site.)
Redux is a predictable state container for JavaScript apps.

State management is absolutely critical in providing users with a well-crafted experience with minimal bugs.

Redux helps organizing React code, to make it easier to read and functions.

Redux Advantages: (Links to an external site.)
Predictable:
Redux helps you write applications that behave consistently, run in different environments (client, server, and native), and are easy to test.

Centralized:
Centralizing your application’s state and logic enables powerful capabilities like undo/redo, state persistence, and much more.

Debuggable:
The Redux DevTools make it easy to trace when, where, why, and how your application’s state changed. Redux’s architecture lets you log changes, use “time-travel debugging”, and even send complete error reports to a server.

Flexible:
Redux works with any UI layer, and has a large ecosystem of addons to fit your needs.