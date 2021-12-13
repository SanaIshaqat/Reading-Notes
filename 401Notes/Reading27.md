# Code 401 Class 27 Reading notes:
## Reading: < Login /> and < Auth />


## Review, Research, and Discussion


### Why is the Context API useful?

React's context allows you to share information to any component, by storing it in a central place and allowing access to any component that requests it (usually you are only able to pass data from parent to child via props).

### Can a component outside of a provider get its context?
React context gets injected into the component render stack. It's a state management which u can use over your whole react app. U can also access the state outside of react (if necessary) and it has a connector to react (react-redux).

### What are some common use cases for using the Context API?

- Theming — Pass down app theme.
- i18n — Pass down translation messages.
- Authentication — Pass down current authenticated user.

### Describe “Context Hell”

Like the callback hell, usual when jQuery was used for everything, the React Context hell is the nasty code you get taking advantage of the React Context API.

## Document the following Vocabulary Terms

**global state**

Global state is the data that is shared between all the components within a React application. When the state is changed, or let's say a filter is added, the components re-render accordingly.

**global context**

Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language.

**provider**

The < Provider> component makes the Redux store available to any nested components that need to access the Redux store. Since any React component in a React Redux app can be connected to the store, most applications will render a < Provider> at the top level, with the entire app's component tree inside of it.

**consumer**

A React component that subscribes to context changes. Using this component lets you subscribe to a context within a function component. Requires a function as a child. The function receives the current context value and returns a React node.

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

### What is Role-Based Access Control (RBAC)?

"Role-based access control (RBAC) restricts network access based on a person's role within an organization and has become one of the main methods for advanced access control. The roles in RBAC refer to the levels of access that employees have to the network".

### Some of the designations in an RBAC tool can include:

- Management role scope : it limits what objects the role group is allowed to manage.
- Management role group : you can add and remove members.
- Management role : these are the types of tasks that can be performed by a specific role group.
- Management role assignment : this links a role to a role group.

### BENEFITS OF RBAC :
Reducing administrative work and IT support
Maximizing operational efficiency
Improving compliance

### React-cookies :

- "Cookies are the data stored in the form of key-value pairs that are used to store information about the user on their computer by the websites that the users browse and use it to verify them".

- To set or remove the cookies, we are using a third-party dependency of react-cookie

- Install : npm i react-cookies
"To be able to access user cookies while doing server-rendering, you can use plugToRequest or setRawCookie".




#### Want To Know More ? 

[what is role based access control?](https://digitalguardian.com/blog/what-role-based-access-control-rbac-examples-benefits-and-more) 

[react-cookies component](https://www.npmjs.com/package/react-cookies) 

[react-cookie library](https://www.npmjs.com/package/react-cookie) 
