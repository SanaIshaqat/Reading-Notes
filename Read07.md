# 102 Lecture05 Class Notes:


## Functions:  

**Functions** are one of the fundamental building blocks in JavaScript. A function in JavaScript is similar to a procedure—a set of statements that performs a task or calculates a value, but for a procedure to qualify as a function, it should take some input and return an output where there is some obvious relationship between the input and the output. To use a function, you must define it somewhere in the scope from which you wish to call it.


### Defining functions:

A function definition (also called a function declaration, or function statement) consists of the function keyword, followed by:

- The name of the function.
- A list of parameters to the function, enclosed in parentheses and separated by commas.
- The JavaScript statements that define the function, enclosed in curly brackets, {...}.
For example, the following code defines a simple function named square:

**Example**:  
function square(number) {
  return number * number;
}

The function square takes one parameter, called number. The function consists of one statement that says to return the parameter of the function (that is, number) multiplied by itself. The statement return specifies the value returned by the function:

**Example**:
return number * number;

Primitive parameters (such as a number) are passed to functions by value; the value is passed to the function, but if the function changes the value of the parameter, this change is not reflected globally or in the calling function.


### Function expressions:
Function expressions are convenient when passing a function as an argument to another function.

**Example**: 
const square = function(number) { return number * number }
var x = square(4)


### Calling functions:
Defining a function does not execute it. Defining it names the function and specifies what to do when the function is called.

Calling the function actually performs the specified actions with the indicated parameters. For example, if you define the function square, you could call it as follows:

**Example**: 

square(5);


#### Want To Know More ? 
[Visit our Resources website](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Functions)