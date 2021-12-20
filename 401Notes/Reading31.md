# Code 401 Class 31 Reading notes:
## Readings: Redux - Combined Reducers

## Review, Research, and Discussion


### Why choose Redux instead of the Context API for global state?

Redux works around the idea of having a central state called a store. To change the state, a component has to dispatch an action. The action is then passed on to the reducer, which changes the state of our application.

When using Redux with React, states will no longer need to be lifted up. This makes it easier for you to trace which action causes any change.

### What is the purpose of a reducer?

A reducer is a function that determines changes to an application's state. It uses the action it receives to determine this change. We have tools, like Redux, that help manage an application's state changes in a single store so that they behave consistently.
### What does an action contain?

Actions are the only source of information for the store as per Redux official documentation. It carries a payload of information from your application to store. It is recommended to keep your action object as light as possible and pass only the necessary information. 
### Why do we need to copy the state in a reducer?

If the new state is different, the reducer must create new object, and making a copy is a way to describe the unchanged part.

## Document the following Vocabulary Terms

**immutable state**

Immutable state means its value cannot be changed once it's created. Where mutable state allows us to modify already created data structures and change them whichever way we want.

**time travel in redux**

Redux refers to the process of logging actions and state during an app's execution. Since it represents the entire state of an application at a given moment, it is often used in web development for time-travel debugging and to view Redux actions.

**action creator**

An action creator is merely a function that returns an action object. Redux includes a utility function called bindActionCreators for binding one or more action creators to the store's dispatch() function.

**reducer**

In Redux, a reducer is a pure function that takes an action and the previous state of the application and returns the new state. The action describes what happened and it is the reducer's job to return the new state based on that action.

**dispatch**

Dispatch is a function of the Redux store. You call store. dispatch to dispatch an action. This is the only way to trigger a state change. With React Redux, your components never access the store directly - connect does it for you.

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

### combineReducers

- As your app grows more complex, you'll want to split your reducing function into separate functions, each managing independent parts of the state. The combineReducers helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore.

- The resulting reducer calls every child reducer, and gathers their results into a single state object. The state produced by combineReducers() namespaces the states of each reducer under their keys as passed to combineReducers().

- You may call combineReducers at any level of the reducer hierarchy. It doesn't have to happen at the top. In fact you may use it again to split the child reducers that get too complicated into independent grandchildren, and so on.

### There are several important ideas to be aware of when using combineReducers :

1. First and foremost, combineReducers is simply a utility function to simplify the most common use case when writing Redux reducers. You are not required to use it in your own application, and it does not handle every possible scenario.

2. While Redux itself is not opinionated about how your state is organized, combineReducers enforces several rules to help users avoid common errors.

3. One frequently asked question is whether Redux "calls all reducers" when dispatching an action. Since there really is only one root reducer function, the default answer is "no, it does not". However, combineReducers has specific behavior that does work that way.

4. You can use it at all levels of your reducer structure, not just to create the root reducer. It's very common to have multiple combined reducers in various places, which are composed together to create the root reducer.

#### **Want To Know More ?** 

[Multiple Reducers Example](https://www.youtube.com/watch?v=gBER4Or86hE) 

[Redux Docs: Using Combined Reducers](https://redux.js.org/usage/structuring-reducers/using-combinereducers/) 

[Redux Docs: Combined Reducer Syntax](https://redux.js.org/api/combinereducers/) 

