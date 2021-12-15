# Code 401 Class 29 Reading notes:

## Reading: Implementation: Graphs

## Document the Vocabulary Terms




**role based access control**

Role-based access control (RBAC) restricts network access based on a person's role within an organization and has become one of the main methods for advanced access control. The roles in RBAC refer to the levels of access that employees have to the network.

**http cookies**

HTTP cookies, or internet cookies, are built specifically for Internet web browsers to track, personalize, and save information about each user's session. A “session” just refers to the time you spend on a site. Cookies are created to identify you when you visit a new website.

**global state**

Global state is the data that is shared between all the components within a React application. When the state is changed, or let's say a filter is added, the components re-render accordingly.

**global context**

Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language.

**provider**

The < Provider> component makes the Redux store available to any nested components that need to access the Redux store. Since any React component in a React Redux app can be connected to the store, most applications will render a < Provider> at the top level, with the entire app's component tree inside of it.

**consumer**

A React component that subscribes to context changes. Using this component lets you subscribe to a context within a function component. Requires a function as a child. The function receives the current context value and returns a React node.

**context**

 It provides a way to pass data through the component tree without having to pass props down manually at every level. Context is primarily used when some data needs to be accessible by many components at different nesting levels. Context is designed to share data that can be considered global for a tree of React components, such as the current authenticated user, theme, or preferred language.

**useContext()**

useContext hook allows passing data to children elements without using redux. useContext hook is used to create common data that can be accessed throughout the component hierarchy without passing the props down manually to each level. Context defined will be available to all the child components without involving “props”.


**static context**

A static method or, block belongs to the class and these will be loaded into the memory along with the class. You can invoke static methods without creating an object.

**reducer**

- reducer useReducer is one of the additional Hooks , An alternative to the useState Hook, it helps you manage complex state logic in React applications. When combined with other Hooks like useContext, useReducer can be a good alternative to Redux or MobX .

- useReducer is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one.so reducers are responsible for handling transitions from one state to the next state in your application. Reducer functions handle these transitions by determining which actions to handle based on the action's type.

## Graphs

A graph is a non-linear data structure that can be looked at as a collection of vertices (or nodes) potentially connected by line segments named edges.

* Vertex - A vertex, also called a “node”, is a data object that can have zero or more adjacent vertices.
* Edge - An edge is a connection between two nodes.
* Neighbor - The neighbors of a node are its adjacent nodes, i.e., are connected via an edge.
* Degree - The degree of a vertex is the number of edges connected to that vertex.

## Undirected Graphs

**Undirected Graph is a graph where each edge is undirected or bi-directional. This means that the undirected graph does not move in any direction**

Vertices/Nodes = {a,b,c,d,e,f}

Edges = {(a,c),(a,d),(b,c),(b,f),(c,e),(d,e),(e,f)}

![img](https://camo.githubusercontent.com/37e2586bc43bb7faa1ac026202b570d8b11020596be0965af8ba454a14c2fdb7/68747470733a2f2f636f646566656c6c6f77732e6769746875622e696f2f636f6d6d6f6e5f637572726963756c756d2f646174615f737472756374757265735f616e645f616c676f726974686d732f436f64655f3430312f636c6173732d33352f7265736f75726365732f6173736574732f556e646972656374656447726170682e504e47)

## Directed Graphs (Digraph)

**A _Directed Graph _ also called a Digraph is a graph where every edge is directed.**

Unlike an undirected graph, a Digraph has direction. Each node is directed at another node with a specific requirement of what node should be referenced next.

![img](https://camo.githubusercontent.com/80304cdda39f1fa9973941747e8c27cce073c3f23a2e613ca347e55818409cfa/68747470733a2f2f636f646566656c6c6f77732e6769746875622e696f2f636f6d6d6f6e5f637572726963756c756d2f646174615f737472756374757265735f616e645f616c676f726974686d732f436f64655f3430312f636c6173732d33352f7265736f75726365732f6173736574732f446972656374656447726170682e504e47)

Vertices = {a,b,c,d,e,f}

Edges = {(a,c),(b,c),(b,f),(c,e),(d,a),(d,e)(e,c)(e,f)}

## Complete vs Connected vs Disconnected
This depends on how connected the graphs are to other node/vertices.

* **_Complete Graphs _** A complete graph is when all nodes are connected to all other nodes.

* **A connected graph** is graph that has all of vertices/nodes have at least one edge.

* **A disconnected graph** is a graph where some vertices may not have edges.

## Acyclic vs Cyclic

* **Acyclic Graph** An acyclic graph is a directed graph without cycles.
A cycle is when a node can be traversed through and potentially end up back at it

* **A Cyclic graph** is a graph that has cycles.
A cycle is defined as a path of a positive length that starts and ends at the same vertex.

## Graph Representation
We represent graphs through:

* **Adjacency Matrix** An Adjacency matrix is represented through a 2-dimensional array. If there are n vertices, then we are looking at an n x n Boolean matrix

* **Adjacency List** An adjacency list is the most common way to represent graphs.An adjacency list is a collection of linked lists or array that lists all of the other vertices that are connected.Adjacency lists make it easy to view if one vertices connects to another.

## Real World Uses of Graphs

Graphs are extremely popular when it comes to it’s uses. Here are just a few examples of graphs in use:

* GPS and Mapping
* Driving Directions
* Social Networks
* Airline Traffic
* Netflix uses graphs for suggestions of products




#### Want To Know More ? 

[Graphs](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/graphs.html) 