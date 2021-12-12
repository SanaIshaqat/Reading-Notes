# Code 401 Class 26 Reading notes:
## Reading: Context API - Behaviors


## Review, Research, and Discussion


### When you have multiple contexts, what component type should you use (class/function) and why?


In class components, the render method will be called, whenever the state of the components changes. On the other hand, the Functional components render the UI based on the props. Class Components should be preferred whenever we have the requirement with the state of the component.

### What are some good use cases for using the Context API for global state?

Context is primarily used when some data needs to be accessible by many components at different nesting levels. Apply it sparingly because it makes component reuse more difficult. If you only want to avoid passing some props through many levels, component composition is often a simpler solution than context.

### How can you best test context?

The best way to test Context is to make our tests unaware of its existence and avoiding mocks. We want to test our components in the same way that developers would use them (behavioral testing) and mimic the way they would run in our applications (integration testing).

## Document the following Vocabulary Terms

**context**

 It provides a way to pass data through the component tree without having to pass props down manually at every level. Context is primarily used when some data needs to be accessible by many components at different nesting levels. Context is designed to share data that can be considered global for a tree of React components, such as the current authenticated user, theme, or preferred language.

**useContext()**

useContext hook allows passing data to children elements without using redux. useContext hook is used to create common data that can be accessed throughout the component hierarchy without passing the props down manually to each level. Context defined will be available to all the child components without involving “props”.


**static context**

A static method or, block belongs to the class and these will be loaded into the memory along with the class. You can invoke static methods without creating an object.

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

- **Dynamic** context defines items that are unique to each invocation of an executable, items such as the values for external variables, external function implementations, and resolvers to external inputs or results. These items might change across invocations.

- **Context provides** a way to pass data through the component tree without having to pass props down manually at every level. Context is primarily used when some data needs to be accessible by many components at different nesting levels.

- **Context** is designed to share data that can be considered global for a tree of React components, such as the current authenticated user, theme, or preferred language.

- **Caveats** Because context uses reference identity to determine when to re-render, there are some gotchas that could trigger unintentional renders in consumers when a provider’s parent re-renders. To get around this, lift the value into the parent’s state .

#### Want To Know More ? 

[context api](https://reactjs.org/docs/context.html) 

[hooks and context example](https://medium.com/swlh/snackbars-in-react-an-exercise-in-hooks-and-context-299b43fd2a2b) 

[react context links](https://github.com/diegohaz/awesome-react-context) 

