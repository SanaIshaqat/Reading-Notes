# Code 401 Class 04 Reading notes:

## Review, Research, and Discussion

### Name 3 advantages to Test Driven Development
- You are able to identify the errors and problems quickly.
- Writing the tests first requires you to really consider what do you want from the code.
- TDD creates code that is maintainable, flexible, and easily extensible.

### In what case would you need to use beforeEach() or afterEach() in a test suite?
The difference is beforeEach()/afterEach() automatically run before and after each tests, which 1. removes the explicit calls from the tests themselves, and 2. invites inexperienced users to share state between tests.
### What is one downside of Test Driven Development
No silver bullet – Tests help to seek out bugs, but they can not find bugs that you simply introduce within the test code and in implementation code.
### What’s the primary difference between ES6 Classes and Constructor/Prototype Classes?
 The most important difference between class- and prototype-based inheritance is that a class defines a type which can be instantiated at runtime, whereas a prototype is itself an object instance.
### Why REST?
One of the key advantages of REST APIs is that they provide a great deal of flexibility. Data is not tied to resources or methods, so REST can handle multiple types of calls, return different data formats and even change structurally with the correct implementation of hypermedia.
## Document the following Vocabulary Terms


**functional programming**
In computer science, functional programming is a programming paradigm where programs are constructed by applying and composing functions.

This allows programs to be written in a declarative and composable style, where small functions are combined in a modular manner.

**object-oriented programming (OOP)**
Object-oriented programming (OOP) is a computer programming model that organizes software design around data, or objects, rather than functions and logic. An object can be defined as a data field that has unique attributes and behavior.

**class**
A JavaScript class is a blueprint for creating objects. A class encapsulates data and functions that manipulate data. Unlike other programming languages such as Java and C#, JavaScript classes are syntactic sugar over the prototypal inheritance.

**super**
What is super () in JavaScript?
The super keyword is used to access and call functions on an object's parent. The super. prop and super[expr] expressions are valid in any method definition in both classes and object literals.

**this**
The value that this stores is the current execution context of the JavaScript program. Thus, when used inside a function this's value will change depending on how that function is defined, how it is invoked and the default execution context.

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

## Preview


### Which 3 things had you heard about previously and now have better clarity on?
- Mocking
- Jest
- REST
### Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
- object-oriented programming (OOP)
- psql
-postgres
### What are you most excited about trying to implement or see how it works?
Link Database that has all types of info on postgres and have different ways to access it.
