# Forms

**HTML form** elements work a bit differently from other DOM elements in React, because form elements naturally keep some internal state. For example, this form in plain HTML accepts a single name:

`<form>`

  `<label>`

`Name:`

`<input type="text" name="name" />`

 ` </label>`

  `<input type="submit" value="Submit" />`

`</form>`

## Controlled Components

In HTML, form elements such as `<input>`, `<textarea>`, and `<select>` typically maintain their own state and update it based on user input. In React, mutable state is typically kept in the state property of components, and only updated with `setState()`.

## The Conditional (Ternary) Operator 

`condition ? value if true : value if false`

Here’s what you need to know:

1. The `condition` is what you’re actually testing. The result of your `condition` should be true or false or at least coerce to either boolean value.

2. A `?` separates our conditional from our true value. Anything between the `?` and the `:` is what is executed if the `condition` evaluates to true.

3. Finally a `:` colon. If your `condition` evaluates to false, any code after the colon is executed.

![img](https://media.geeksforgeeks.org/wp-content/uploads/20190920110229/Conditional-or-Ternary-Operator-__-in-C_C.jpg)
