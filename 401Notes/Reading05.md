# Code 401 Class 05 Reading notes:

## Linked Lists
Linked list is a sequence of Nodes that are connected/linked to each other. The defining feature of a linked list is tat Node references the next Node in the link.

**There are two types of Linked list - Singly and Doubly**

### Singly: 
Singly refers to the number of references the node has. A singly linked list means that there is only one reference, and the reference points to the next node.

### Doubly: Doubly refers to there being two (double) references within the node. A doubly linked list means that there is a reference to both the next and additionally the previous node.


### Traversing
As you traverse a linked list, you cannot use a **forEach** or a **for** loop. We are relying on the Next value to guide the node to the next reference point. A next property is exceptionally important because it will lead us to the next node and allows us to extract data appropriately.

### So what can you use to traverse?? 

The best approach is to use a **while()** loop. This will allow us to continually check that the next node is the list is not null.
Example
ALGORITHM Includes (value) // INPUT <– integer value // OUTPUT <– boolean

Current <– Head

WHILE Current is not NULL IF Current.Value is equal to value return TRUE

Current <– Current.Next return FALSE

### How the process looks like?

1. We first create Current at the Head to guarantee we are starting from the beginning.
2. We create the while loop and this will only run is the node that Current is pointing too is not null.
3. Once we are in the while loop, we are checking if the value of the current node is equal to the value that we were looking for.
4. If the Current node does not contain the value we are looking for, we must move the current to the next node that is being referenced.
5. At this point, the while loop is run again and steps 3 & 4 will continue until Current reaches the end of the LinkedList.

### Adding a Node
Order of operations is extremely important when it comes to working with a Linked list. Each of your links and nodes should be properly assigned.
Prerequisites
When constructing your code, keep in mind that a Node class will be passed in to each node that has a value,
When making a Linked List, you may want to require that at least one node gets passed in upon instantiation. This first node is what your Head and Current will point too.

## The Big O:

Big O(oh) notation is used to describe the efficiency of an algorithm or function. This efficiency is evaluated based on 2 factors:

### Running Time (also known as time efficiency / complexity)
The amount of time a function needs to complete.

### Memory Space (also known as space efficiency / complexity)
The amount of memory resources a function uses to store data and instructions.

### Overview
Big O’s role in algorithm efficiency is to describe the Worst Case of efficiency an algorithm can have in performing it’s job. It specifically looks at the factors mentioned above, which we often refer to as Space and Time. In order to analyze these limiting factors, we should consider 4 Key Areas for analysis:

- Input Size
- Units of Measurement
- Orders of Growth
- Best Case, Worst Case, and Average Case


## General summaries of what I learned this week :

### How to Solve Programming Problems
Common mistakes Programmers make
When most programmers are given a programming problem in an interview, they make several key mistakes.

The most severe of those is the improper allocation of time.

The most common mistake I see when conducting interviews or watching someone try to solve a programming problem is they try to start writing code as soon as possible.

### A simple set of steps to handle programming problems:

- Read the problem completely twice. Solve the problem manually with 3 sets of sample data.
- Optimize the manual steps.
- Write the manual steps as comments or pseudo-code.
- Replace the comments or pseudo-code with real code.
- Optimize the real code.
- As much as 70% of our time should be spent in steps 1-3.

## Documented Vocabulary Terms

**Web Server:**
A web server is software and hardware that uses HTTP (Hypertext Transfer Protocol) and other protocols to respond to client requests made over the World Wide Web.

**Express:**
Express is a minimal and flexible Node.js web application framework that provides a robust set of features for web and mobile applications.

**Routing:**
Routing refers to how an application’s endpoints (URIs) respond to client requests.

**WRRC**
Web Request Response Cycle.

**Middleware:**
middleware is basically a piece of code that may be used to process a request. Middleware functions are usually chained together and it’s up to them to decide whether to invoke the next one in the chain.

**Request Object:**
The request object represents the HTTP request and has properties for the request query string, parameters, body, HTTP headers, and so on.

**Response Object:**
The res object represents the HTTP response that an Express app sends when it gets an HTTP request.

**Application Middleware:**
Middleware is software that lies between an operating system and the applications running on it.

**Routing Middleware:**
Routing defines the way in which the client requests are handled by the application endpoints. And when you make some routers in separate file, you can use them by using middleware.

**Test Driven Development:**
Test-driven development” refers to a style of programming in which three activities are tightly interwoven: coding, testing (in the form of writing unit tests) and design (in the form of refactoring)

**Behavioral Testing:**
Unit testing is a methodology where units of code are tested in isolation from the rest of the application. A unit test might test a particular function, object, class, or module.

**Functional programming:**
In computer science, functional programming is a programming paradigm where programs are constructed by applying and composing functions.

This allows programs to be written in a declarative and composable style, where small functions are combined in a modular manner.

**Object-oriented programming (OOP)**
Object-oriented programming (OOP) is a computer programming model that organizes software design around data, or objects, rather than functions and logic. An object can be defined as a data field that has unique attributes and behavior.

**Class**
A JavaScript class is a blueprint for creating objects. A class encapsulates data and functions that manipulate data. Unlike other programming languages such as Java and C#, JavaScript classes are syntactic sugar over the prototypal inheritance.

**Super**
What is super () in JavaScript? The super keyword is used to access and call functions on an object’s parent. The super. prop and super[expr] expressions are valid in any method definition in both classes and object literals.

**This**
The value that this stores is the current execution context of the JavaScript program. Thus, when used inside a function this’s value will change depending on how that function is defined, how it is invoked and the default execution context.

**Test Driven Development (TDD)**
Test Driven Development (TDD) is software development approach in which test cases are developed to specify and validate what the code will do.

**Jest**
Jest is a JavaScript testing framework designed to ensure correctness of any JavaScript codebase. It allows you to write tests with an approachable, familiar and feature-rich API that gives you results quickly.

**Continuous Integration (CI)**
CI and CD stand for continuous integration and continuous delivery/continuous deployment. In very simple terms, CI is a modern software development practice in which incremental code changes are made frequently and reliably.

**REST**
The rest parameter syntax allows a function to accept an indefinite number of arguments as an array, providing a way to represent variadic functions in JavaScript.

**Data Model**
JSON objects and arrays in the ABL are based on the objects and arrays of the JavaScript data model. JavaScript objects are associative arrays. Object property names can be any Unicode string. Properties and their values can be added, changed, or deleted at runtime.