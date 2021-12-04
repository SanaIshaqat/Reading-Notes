# Code 401 Class 20 Reading notes:

## Component Based UI


### Name 5 Javascript UI Frameworks (other than React)

1. Angular
2. Mithril
3. Vue.js
4. Ember.js
5. Meteor


### What’s the difference between a framework and a library?
- A library is essentially a set of functions that you can call, these days usually organized into classes. Each call does some work and returns control to the client. 

- A framework embodies some abstract design, with more behavior built in.

When you import a library, you have to call the specific methods or functions of your choice so, and it's up to you when and where to call the Library. Here, you are in charge of flow. On the other hand, Framework itself makes a call to your code and provide you with some space to write down details.


## Document the following Vocabulary Terms

**Rendering**

Rendering is a process used in web development that turns website code into the interactive pages users see when they visit a website. The term generally refers to the use of HTML, CSS, and JavaScript codes. The process is completed by a rendering engine, the software used by a web browser to render a web page.

**Templates**

A website template is a predesigned resource that shows the structure for the comprehensive layout and display features of any website. It is provided by various suppliers to help make Web design a lot easier for designers. A website template is also known as a Web page template or page template.

**State**

State is how something is; its configuration, attributes, condition or information content. We will use the term component to include software and hardware "things". Virtually all components have state, from applications to operating systems to network layers.

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

### React
A JavaScript library for building user interfaces.

### A Simple Component

React components implement a render() method that takes input data and returns what to display. This example uses an XML-like syntax called JSX. Input data that is passed into the component can be accessed by render() via this.props.

### A Stateful Component
In addition to taking input data (accessed via this.props), a component can maintain internal state data (accessed via this.state). When a component’s state data changes, the rendered markup will be updated by re-invoking render().

### A Component Using External Plugins
React allows you to interface with other libraries and frameworks. This example uses remarkable, an external Markdown library, to convert the < textarea >’s value in real time.


### What is JSX? 

JSX stands for JavaScript XML. JSX allows us to write HTML in React. JSX makes it easier to write and add HTML in React.


### How does React JSX work? 

It is a JavaScript extension that allows us to describe React's object tree using a syntax that resembles that of an HTML template. It is just an XML-like extension that allows us to write JavaScript that looks like markup and have it returned from a component.


### Rendering Elements
Elements are the smallest building blocks of React apps.

An element describes what you want to see on the screen:

const element = < h1>Hello, world< /h1>;
Unlike browser DOM elements, React elements are plain objects, and are cheap to create. React DOM takes care of updating the DOM to match the React elements.


### Rendering an Element into the DOM
Let’s say there is a < div> somewhere in your HTML file:

< div id="root">< /div>
We call this a “root” DOM node because everything inside it will be managed by React DOM.

Applications built with just React usually have a single root DOM node. If you are integrating React into an existing app, you may have as many isolated root DOM nodes as you like.

To render a React element into a root DOM node, pass both to ReactDOM.render():

const element = < h1>Hello, world</ h1>;
ReactDOM.render(element, document.getElementById('root'));
Try it on CodePen

It displays “Hello, world” on the page.




#### Want To Know More ? 

[react hello world](https://reactjs.org/docs/hello-world.html) 

[introducing JSX](https://reactjs.org/docs/introducing-jsx.html)

[rendering elements](https://reactjs.org/docs/rendering-elements.html)

[sass cheatsheet](https://devhints.io/sass)

[react cheatsheet](https://devhints.io/react)

[another react cheatsheet](https://reactcheatsheet.com)


