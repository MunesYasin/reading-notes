# Functions
`Functions` are one of the fundamental building blocks in JavaScript. A function in JavaScript is similar to a procedure—a set of statements that performs a task or calculates a value, but for a procedure to qualify as a function, it should take some input and return an output where there is some obvious relationship between the input and the output. To use a function, you must define it somewhere in the scope from which you wish to call it.

## There are two ways to write the `Function` :

* **Function declarations**
* **Function expressions**

## Function declarations:
function declaration consist of :
* The name of the function.
* A list of parameters to the function, enclosed in parentheses and separated by commas.
* The JavaScript statements that define the function, enclosed in curly brackets, {...}.
### Example of `Function declaratin`:

`function` **square** (*number*) {

  `return number * number;`

}

## Function expression:
Such a function can be anonymous; it does not have to have a name. For example, the function square could have been defined as:

**const** `square` = **function**(*number*)

 {
   
`return number * number` 
    
  }

## Notice : 
The main diffrence between declaratin and expression is in function declaratin you can write the call the function before the function itself , but in expression function you must call the function after itself .

 ## How to call the Function :
 Defining a function does not execute it. Defining it names the function and specifies what to do when the function is called.

Calling the function actually performs the specified actions with the indicated parameters. For example, if you define the function **square**, you could call it as follows:


`square(5);`

About more datails you can visit [`This Link`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Functions#function_declarations).

![image](https://s3.ap-south-1.amazonaws.com/s3.studytonight.com/tutorials/uploads/pictures/1587882057-1.png)

