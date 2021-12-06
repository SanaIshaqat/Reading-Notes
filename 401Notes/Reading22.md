# Code 401 Class 22 Reading notes:
## Reading: Component Lifecycle / useEffect() Hook

## Review, Research, and Discussion



### Why do we not need more .html pages in a multi-page React app?

React apps are single page app ,A React app consists of a single HTML file index.html. The views are coded in JSX format as components.

### If we wanted a component to show up on every page, where would we put it and why?

Inside the < BrowserRouter/ >, outside a < Route/ >, to have it always no matter what the current route is .

### What does routing do with the components that were rendered when a new route is requested

It goes to the new componetnt and remove the old one _cleans up _

### What does props.children contain?

Children is a special property of React components which contains any child elements defined within the component, e.g. the divs inside Example above. {this.props.children} includes those children in the rendered result.

### How do useState() and this.setState() differ?

- The setState function is used to handle the state object in a React class component.
setState is merging the previous state with the new one, it means that you dont have to pass the full state object every time you want to change some part of the state. React will update given properties and won’t touch the rest. 

- The useState’s updater rewrites a previous state with a new one and it does not perform any merging. Its just replacement instead of merging.

## Document the following Vocabulary Terms

**State Hook**

State Hook The useState() is a Hook that allows you to have state variables in functional components , it takes the initial state as an argument and returns an array of two entries.

**Mounting and Un-Mounting**

Mounting and Un-Mounting The main job of React is to figure out how to modify the DOM to match what the components want to be rendered on the screen. React does so by mounting (adding nodes to the DOM), unmounting (removing them from the DOM), and updating (making changes to nodes already in the DOM).


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

## What is useEffect Hook?

useEffect is a hook for encapsulating code that has 'side effects,' and is like a combination of componentDidMount , componentDidUpdate , and componentWillUnmount . Previously, functional components didn't have access to the component life cycle, but with useEffect you can tap into it.
 
## What is a React effect?

When you call useEffect , you're telling React to run your “effect” function after flushing changes to the DOM. Effects are declared inside the component so they have access to its props and state. By default, React runs the effects after every render — including the first render.

#### Want To Know More ? 

[effects hook](https://reactjs.org/docs/hooks-effect.html) 