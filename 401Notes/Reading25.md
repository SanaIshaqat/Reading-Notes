# Code 401 Class 25 Reading notes:
## Reading: Context API

## Review, Research, and Discussion

### Describe use cases useState() vs useReducer()

- useState is a Basic Hook for managing simple state transformation and useReducer is an Additional Hook for managing more complex state logic, it is worth noting that useState uses the useReducer internally. This implies that you could use useReducer for everything you can do with useState.

- useReducer is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one. useReducer also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks.

### Why do custom hooks need the use prefix?
Custom Hooks
This is mainly to have an extra option for sharing state and logic between components. Custom hooks are normal JS functions, named with the prefix 'use', that can use hooks inside of it and contain a common stateful logic to be reused in other components.

### What do custom hooks usually do?

Custom hooks allow us to have cleaner functional components, remove logic from the UI layer, and prevent code duplication by bringing common use cases to reusable hooks.

### Using any list of custom hooks, research and name one that you think will be useful in your applications

useScript React hook to dynamically load an external script and know when its loaded , useScript is a hook for loading (and notifying when they’re loaded) external scripts, dynamically.

use-mouse-action :A library with three React hooks for listening to mouse events on an element or JSX element. useMouseAction: This is used to register mouse actions on an element. useMouseDown: This is used to register a mouse down event on an element. useMouseUp: This registers a mouse up event on an element.

### Describe how a hook that fetches API data might work

The hook might take in a url, a method, and a body. Using axios or something similar, useState and possibly useEffect, an API call can be made based on and using the parameters passed in and then an objects state could be ‘set’ based on the results of the API call

Put the fetchData function above in the useEffect hook and call it, like so: useEffect(() => { const url = "https://api.adviceslip.com/advice"; const fetchData = async () => { try { const response = await fetch(url); const json = await response. json(); console. log(json); } catch (error) { console.

## Document the following Vocabulary Terms

**reducer**

- reducer useReducer is one of the additional Hooks , An alternative to the useState Hook, it helps you manage complex state logic in React applications. When combined with other Hooks like useContext, useReducer can be a good alternative to Redux or MobX .

- useReducer is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one.so reducers are responsible for handling transitions from one state to the next state in your application. Reducer functions handle these transitions by determining which actions to handle based on the action's type.

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

### Context :
#### When to Use Context :
Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language.


#### Before You Use Context :
Context is primarily used when some data needs to be accessible by many components at different nesting levels. Apply it sparingly because it makes component reuse more difficult.

If you only want to avoid passing some props through many levels, component composition is often a simpler solution than context.

#### React.createContext :
Creates a Context object. When React renders a component that subscribes to this Context object it will read the current context value from the closest matching Provider above it in the tree".

#### Context.Provider:
Every Context object comes with a Provider React component that allows consuming components to subscribe to context changes.
The Provider component accepts a value prop to be passed to consuming components that are descendants of this Provider. One Provider can be connected to many consumers. Providers can be nested to override values deeper within the tree.

#### Class.contextType :
The contextType property on a class can be assigned a Context object created by React.createContext().

#### Context.Consumer :
A React component that subscribes to context changes. Using this component lets you subscribe to a context within a function component.

#### Caveats:
Because context uses reference identity to determine when to re-render, there are some gotchas that could trigger unintentional renders in consumers when a provider’s parent re-renders.




#### Want To Know More ? 

[context api](https://reactjs.org/docs/context.html) 

[hooks and context example](https://medium.com/swlh/snackbars-in-react-an-exercise-in-hooks-and-context-299b43fd2a2b) 

[react context links](https://github.com/diegohaz/awesome-react-context) 


