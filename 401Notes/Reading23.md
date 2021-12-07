# Code 401 Class 23 Reading notes:
## Reading: Advanced State with Reducers


## Review, Research, and Discussion


### How can we ensure that an effect hook runs only once?

If you want to run an effect and clean it up only once (on mount and unmount), you can pass an empty array ( [] ) as a second argument. This tells React that your effect doesn't depend on any values from props or state, so it never needs to re-run.

### Can useState() update more than one state variable at the same time?

You could combine the loading state and data state into one state object and then you could do one setState call and there will only be one render.

### Is useState() synchronous?

useState and setState both are asynchronous.,They do not update the state immediately but have queues that are used to update the state object.

## Document the following Vocabulary Terms

**State Hook**

A Hook is a special function that lets you “hook into” React features. For example, useState is a Hook that lets you add React state to function components. We'll learn other Hooks later.

**Component Lifecycle**

A component's lifecycle is broadly classified into four parts: initialization. mounting. updating, and. unmounting.

React components are created by being mounted onto the DOM, they change or grow through updates, and finally, they can be removed or unmounted from the DOM. These three milestones are referred to as the React component lifecycle.

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


### What is the useReducer hook?

The useReducer() hook in React lets you separate the state management from the rendering logic of the component. const [state, dispatch] = useReducer(reducer, initialState) accepts 2 argument: the reducer function and the initial state.

### When is the useReducer hook used?

The useReducer is a hook used sometimes to manage the state of the application. It is very similar to the useState hook, just more complex. It acts as an alternate hook to the useState hook to manage complex state in your application. The useReducer hook uses the same concept as the reducers in Redux.

### Does useReducer cause re render?

Quick summary ↬ In a React component, useState and useReducer can cause your component to re-render each time there is a call to the update functions. ... In React components, there are times when frequent changes have to be tracked without enforcing the re-rendering of the component.

#### Want To Know More ? 

[useReducer hook](https://reactjs.org/docs/hooks-reference.html#usereducer) 

[Ultimate Guide to useReducer](https://blog.logrocket.com/guide-to-react-usereducer-hook/) 