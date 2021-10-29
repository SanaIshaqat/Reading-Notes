# Code 301 Class 02 Reading notes:

## React lifecycle
![](https://miro.medium.com/max/2000/0*0saPKFiTUk6W3FYp)

### Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?

'render' happens first according to the diagram.

### What is the very first thing to happen in the lifecycle of React?

**Mounting**


When an instance of a component is being created and inserted into the DOM it occurs during the mounting phase. Constructor, static getDerivedStateFromProps, render, componentDidMount, and UNSAFE_componentWillMount all occur in this order during mounting.



### Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates

render
componentDidMount
constructor
React Updates
componentWillUnmount 


### What does componentDidMount do?

This method is invoked immediately after a component is mounted. If you need to load anything using a network request or initialize the DOM, it should go here. This method is a good place to set up any subscriptions. If you do that, don’t forget to unsubscribe in componentWillUnmount().
setState() can be called here, but it should be used sparingly, because it will cause a rerender, which can lead to perfomance issues.
Here we use componentDidMount() to connect to the YouTube API and get videos when the components is rendered.

## React State Vs Props


### What types of things can you pass in the props?

Props (aka "properties") in React allows us to pass values from a parent component down to a child component. The values can be any data type, from strings to functions, objects, etc.

### What is the big difference between props and state?

The key difference between props and state is that state is internal and controlled by the component itself while props are external and controlled by whatever renders the component.

props get passed to the component (similar to function parameters) whereas state is managed within the component (similar to variables declared within a function).

### When do we re-render our application?

React components automatically re-render whenever there is a change in their state or props. A simple update of the state, from anywhere in the code, causes all the User Interface (UI) elements to be re-rendered automatically.

### What are some examples of things that we could store in state?
State allows us to manage changing data in an application. It's defined as an object where we define key-value pairs specifying various data we want to track in the application.
counter and anything that changes.
## Things I want to know more about


#### Want To Know More ? 

[Visit our Resources website](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)