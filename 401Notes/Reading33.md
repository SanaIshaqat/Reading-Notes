# Code 401 Class 33 Reading notes:

## Readings: Redux - Additional Topics

## Review, Research, and Discussion


### What’s the best practice for “pre-loading” data into the store (on application start) in a Redux application?

- The most 'redux-like' way of handling the pre-loading of data would be to fire off the asynchronous action in the lifecycle method (probably componentWillMount ) of a Higher Order Component that wraps your app.

- To clean up the render by useEffect like willUnMount.
### When using a thunk/async action that dispatches the actual action, which do you export from your reducer?

- When you deal with side effects or async logic or complex sync logic.

- Still you export the state from your reducer as before without thunk.

## Document the following Vocabulary Terms

**middleware**

Middlewares in general are functions that run between two things in a certain process. Redux middleware provides a third-party extension point between dispatching an action, and the moment it reaches the reducer.

**thunk**

A thunk is a function that wraps an expression to delay its evaluation.

## Preview

### Which 3 things had you heard about previously and now have better clarity on?

- React
- Libraries
- Framework
### Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

- React Hooks
- React Native
- React Redux

### What are you most excited about trying to implement or see how it works?

Website and Mobile Application using the same js.
What are you most excited about trying to implement or see how it works?



## Preparation Materials


### Redux Toolkit (RTK)

- Redux Toolkit is a package that help you to use redux with easy and simple way by :

1. Built in things makes your code shorter.
2. Configure your store, reducers, middlewares, and DevTools easly.

- The core of RTK Query's functionality. It allows you to define a set of endpoints describe how to retrieve data from a series of endpoints, including configuration of how to fetch and transform that data. In most cases, you should use this once per app, with "one API slice per base URL" as a rule of thumb.


## Alternative State Managers

### MobX

- MobX is a library that mange the states in your appliaction.

- Main functionality in MobX is prevent producing an inconsistent state.

- MobX will make sure that all changes to the application state caused by your actions are automatically processed by all derivations and reactions. Synchronously and glitch-free.

- No boilerplate in MobX. Just some simple, declarative components that form our complete UI

### HookState

- HookState is laibrary based on React state hook, and it is a flexible state management tool.

- HookState is an ideal solution for huge states and very frequent updates.

### Features that provided by HookState :

- Global states
- Local states
- Asynchronously loaded states
- Partial state updates
- Deeply nested state updates



#### **Want To Know More ?** 

[Redux Toolkit (RTK)](https://redux-toolkit.js.org) 

[Tutorial](https://redux-toolkit.js.org/tutorials/overview) 


