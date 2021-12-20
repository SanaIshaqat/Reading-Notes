# Code 401 Class 32 Reading notes:

## Readings: Redux - Asynchronous Actions

## Review, Research, and Discussion

### How granular should your reducers be?

It’s easy to go full-warp with very specific events, dedicated for every change that occurs when a user is editing forms such as CHANGE_NAME, CHANGE_STREET, CHANGE_AGE, etc… But it is not actually necessary if the logic behind the update is not different for all those fields. For those parts which require different handling in various reducers; dedicated action is the best solution. For others, sometimes a general action might be good enough.

### Pro or Con – multiple reducers can “fire” when a commonly named action is dispatched

Whether this is good or bad depends on your app. having many stores (or Redux reducers) handling the same action is actually very convenient because it divides responsibilities, and also lets people work on feature branches without colliding with the rest of the team.

### Name a strategy for preventing the above

Redux thunk 
## Document the following Vocabulary Terms


**store**

A store is an immutable object tree in Redux. A store is a state container which holds the application's state. Redux can have only a single store in your application. Whenever a store is created in Redux, you need to specify the reducer. Let us see how we can create a store using the createStore method from Redux.

**combined reducers**

The combineReducers helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore . The resulting reducer calls every child reducer, and gathers their results into a single state object.

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

## Preparation Materials

### Redux Fundamentals:

use the React-Redux library to let our React components interact with a Redux store, including calling useSelector to read Redux state, calling useDispatch to give us access to the dispatch function, and wrapping our app in a Provider component to give those hooks access to the store.

### Redux Middleware and Side Effects:

Redux reducers must never contain "side effects". A "side effect" is any change to state or behavior that can be seen outside of returning a value from a function. Some common kinds of side effects are things like:

1. Logging a value to the console
2. Saving a file
3. Setting an async timer
4. Making an AJAX HTTP request
5. Modifying some state that exists outside of a function, or mutating arguments to a function
6. Generating random numbers or unique random IDs (such as Math.random() or Date.now())

Redux middleware were designed to enable writing logic that has side effects.
img

### Using Middleware to Enable Async Logic :

We could have our middleware check to see if the "action" is actually a function instead, and if it's a function, call the function right away. That would let us write async logic in separate functions, outside of the middleware definition.

### Understanding Asynchronous Redux Actions with Redux Thunk :

- There are two very popular middleware libraries that allow for side effects and asynchronous actions: Redux Thunk and Redux Saga.

- Thunk is a programming concept where a function is used to delay the evaluation/calculation of an operation".

- Redux Thunk is a middleware that lets you call action creators that return a function instead of an action object. That function receives the store’s dispatch method, which is then used to dispatch regular synchronous actions inside the function’s body once the asynchronous operations have been completed".

#### **Want To Know More ?** 

[async actions](https://redux.js.org/tutorials/fundamentals/part-6-async-logic) 

[thunk middleware](https://github.com/reduxjs/redux-thunk) 

[redux thunk](https://www.digitalocean.com/community/tutorials/redux-redux-thunk) 

