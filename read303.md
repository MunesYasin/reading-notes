# Lists and Keys 

Given the code below, we use the map() function to take an array of numbers and double their values. We assign the new array returned by map() to the variable doubled and log it: 

`const numbers = [1, 2, 3, 4, 5];`
`const doubled = numbers.map((number) => number * 2);`
`console.log(doubled);` 

This code logs [2, 4, 6, 8, 10] to the console.

In React, transforming arrays into lists of elements is nearly identical.

**Basic List Component**

Usually you would render lists inside a component.

We can refactor the previous example into a component that accepts an array of numbers and outputs a list of elements.

`function NumberList(props) {`

  `const numbers = props.numbers;`

 ` const listItems = numbers.map((number) =>`

   ` <li>{number}</li>`

  `);`

 ` return (`

   ` <ul>{listItems}</ul>`

 ` );`

`}`

`const numbers = [1, 2, 3, 4, 5];`


`ReactDOM.render(`

 ` <NumberList numbers={numbers} />,`

 ` document.getElementById('root')`

`);`

**Keys**

Keys help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside the array to give the elements a stable identity:

**Extracting Components with Keys**

Keys only make sense in the context of the surrounding array.

For example, if you extract a ListItem component, you should keep the key on the <ListItem /> elements in the array rather than on the <li> element in the ListItem itself.

![img](https://i.morioh.com/200626/ec9a9e94.jpg)

# spread operator 

## What is the spread operator? 

InJavaScript, spread syntax refers to the use of an ellipsis of three dots (…) to expand an iterable object into the list of arguments.
“When ...arr is used in the function call, it ‘expands’ an iterable object arr into the list of arguments.” — JavaScript.info
The spread operator was added to JavaScript in ES6 (ES2015), just like the rest parameters, which have the same syntax: three magic dots ….

## What is ... used for?
“Spread operator to the rescue! It looks similar to rest parameters, also using ..., but does quite the opposite.” — JavaScript.info

## What else can … do? 

The … spread operator is useful for many different routine tasks in JavaScript, including the following: 

* Copying an array
* Concatenating or combining arrays
* Using Math functions
* Using an array as arguments
* Adding an item to a list
* Adding to state in React
* Combining objects
* Converting NodeList to an array