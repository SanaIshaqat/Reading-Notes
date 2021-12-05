# Code 401 Class 21 Reading notes:

## useState() Hook


## Review, Research, and Discussion


### How does React differ from vanilla JS/HTML/CSS?


**What is React?** 

A JavaScript library for building user interfaces. Lots of people use React as the V in MVC. Since React makes no assumptions about the rest of your technology stack, it's easy to try it out on a small feature in an existing project.

**What is Vanilla.JS?**

A fast, lightweight and cross-platform framework. It is a fast and cross-platform framework for building incredible, powerful JavaScript applications. it is the most lightweight framework available anywhere.

React and Vanilla.JS belong to "Javascript UI Libraries" category of the tech stack.

Plain JS apps usually start with the initial UI created on the server (as HTML), whereas React apps start with a blank HTML page, and dynamically create the initial state in JavaScript. React requires you to break your UI into components, but plain JS apps can be structured in any way you see fit.

### What is the primary difference between a function component and a class component?

A functional component is just a plain JavaScript function that accepts props as an argument and returns a React element. A class component requires you to extend from React. Component and create a render function which returns a React element. There is no render method used in functional components.

## Document the following Vocabulary Terms

**Functional Components**

Functional components are basic JavaScript functions. These are typically arrow functions but can also be created with the regular function keyword. Sometimes referred to as “dumb” or “stateless” components as they simply accept data and display them in some form; that is they are mainly responsible for rendering UI.

**Children / Child Components**

Children allow you to pass components as data to other components, just like any other prop you use. The special thing about children is that React provides support through its ReactElement API and JSX. XML children translate perfectly to React children!

## Preview

### Which 3 things had you heard about previously and now have better clarity on?

- React
- Libraries
- Framework
### Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

- React Hooks
- React Native
- Type Script

### What are you most excited about trying to implement or see how it works?

Website and Mobile Application.

## Preparation Materials

### Hooks React Js 

Hooks are the new feature introduced in the React 16.8 version. It allows you to use state and other React features without writing a class. Hooks are the functions which "hook into" React state and lifecycle features from function components. It does not work inside classes.

### Why we need Hooks in React JS?

If the React community embraces [ hooks], it will reduce the number of concepts you need to juggle when writing React applications. Hooks let you always use functions instead of having to constantly switch between functions, classes, higher-order components, and render props. 

### What is State Hook?

A Hook is a special function that lets you “hook into” React features. For example, useState is a Hook that lets you add React state to function components. 

### What does a state Hook return?

useState is a Hook (function) that allows you to have state variables in functional components. You pass the initial state to this function and it returns a variable with the current state value (not necessarily the initial state) and another function to update this value.


[making sense of hooks](https://medium.com/@dan_abramov/making-sense-of-react-hooks-fdbde8803889)
[the state hook](https://reactjs.org/docs/hooks-state.html)
[hooks api](https://reactjs.org/docs/hooks-overview.html)
[hooks api reference](https://reactjs.org/docs/hooks-reference.html)