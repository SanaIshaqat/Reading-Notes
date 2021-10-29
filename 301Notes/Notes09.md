# Code 301 Class 09 Reading notes:


## Functional Programming Concepts
### What is functional programming?
Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data 

### What is a pure function and how do we know if something is a pure function?
The first fundamental concept we learn when we want to understand functional programming is pure functions. But what does that really mean? What makes a function pure?
So how do we know if a function is pure or not? Here is a very strict definition of purity:
- It returns the same result if given the same arguments (it is also referred as deterministic)
- It does not cause any observable side effects.

### What are the benefits of a pure function?
ne of the major benefits of using pure functions is they are immediately testable. They will always produce the same result if you pass in the same arguments. They also makes maintaining and refactoring code much easier.
### What is immutability?
Unchanging over time or unable to be changed.
When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.
In Javascript we commonly use the for loop. This next for statement has some mutable variables.

### What is Referential transparency?
Referential Transparency emphasizes that an expression in a JavaScript program may be replaced by its value or any other variable having the same value without changing the result of the program. As a result, methods should always return the same value for the given argument without any side effects.
## Node JS Modules and require()

### What is a module?
Module pattern. The Module pattern is used to mimic the concept of classes (since JavaScript doesn't natively support classes) so that we can store both public and private methods and variables inside a single object 
### What does the word ‘require’ do?
The require() method is used to load and cache JavaScript modules. So, if you want to load a local, relative JavaScript module into a Node. js application, you can simply use the require() method.


### What do we have to do to make a module available?

The first thing you do to get access to module features is export them. This is done using the export statement. You can export functions, var , let , const , and — as we'll see later — classes. They need to be top-level items; you can't use export inside a function, for example.


## Things I want to know more about
How RegExr works  

#### Want To Know More ? 

[Concepts of Functional Programming in Javascript](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)