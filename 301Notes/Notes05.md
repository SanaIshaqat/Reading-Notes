# Code 301 Class 05 Reading notes:


## React Docs - thinking in React

### How would you break a mock into a component heirarchy?

The first thing you’ll want to do is to draw boxes around every component (and subcomponent) in the mock and give them all names. If you’re working with a designer, they may have already done this, so go talk to them! Their Photoshop layer names may end up being the names of your React components!

But how do you know what should be its own component? Use the same techniques for deciding if you should create a new function or object. One such technique is the single responsibility principle, that is, a component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents.

Since you’re often displaying a JSON data model to a user, you’ll find that if your model was built correctly, your UI (and therefore your component structure) will map nicely. That’s because UI and data models tend to adhere to the same information architecture. Separate your UI into components, where each component matches one piece of your data model.


![](https://reactjs.org/static/9381f09e609723a8bb6e4ba1a7713b46/90cbd/thinking-in-react-components.png)



1. **FilterableProductTable (orange):** contains the entirety of the example
2. **SearchBar (blue):** receives all user input
3. **ProductTable (green):** displays and filters the data collection based on user input
4. **ProductCategoryRow (turquoise):** displays a heading for each category
5. **ProductRow (red):** displays a row for each product


Now that we’ve identified the components in our mock, let’s arrange them into a hierarchy. Components that appear within another component in the mock should appear as a child in the hierarchy:

**FilterableProductTable**

**SearchBar**
**ProductTable**

**ProductCategoryRow**

**ProductRow**


### What is the single responsibility principle and how does it apply to components?

One such technique is the single responsibility principle, that is, a component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents.

### What does it mean to build a ‘static’ version of your application?

- Static applications and websites render in the user’s browser without the need for server side processing, this means that all the rendering of HTML, CSS, and JavaScript is done on the client side, rather then relying on server side technologies.


### Once you have a static application, what do you need to add?
Add React.
You’ll have a library of reusable components that render your data model. The components will only have render() methods since this is a static version of your app. The component at the top of the hierarchy (FilterableProductTable) will take your data model as a prop. If you make a change to your underlying data model and call ReactDOM.render() again, the UI will be updated. You can see how your UI is updated and where to make changes. React’s one-way data flow (also called one-way binding) keeps everything modular and fast.

### What are the three questions you can ask to determine if something is state?

1. Is it passed in from a parent via props? If so, it probably isn’t state.

2. Does it remain unchanged over time? If so, it probably isn’t state.

3. Can you compute it based on any other state or props in your component? If so, it isn’t state.

### How can you identify where state needs to live?

For each piece of **state** in your application:

- Identify every component that renders something based on that state.

- Find a common owner component (a single component above all the components that need the state in the hierarchy).

- Either the common owner or another component higher up in the hierarchy should own the state.

- If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.


## Things I want to know more about


#### Want To Know More ? 

[React Docs](https://reactjs.org/docs/thinking-in-react.html)

