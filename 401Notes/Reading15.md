# Code 401 Class 15 Reading notes:

## Trees

# Trees

## Why
### Using trees is a way to create a data structure that mimics a "yes/no" decision making process. resource

## What
### "Trees can have any number of children per node, but Binary Trees restrict the number of children to two (hence our left and right children)."

### K-ary Trees: If nodes have more than 2 child nodes, then it is a K-ary Tree.

## Terms

### Node: A component that may contain it's own value and references to the other node.
### Root: The node at the beginning of the tree
### K: The number that specifies the maximum number of children any node may have in a k-ary tree. K=2 for a binary tree
### Left: Reference to one child node in a binary tree
### Right: Reference to the other child node in a binary tree
### Edge: The link between a parent and child node
### Leaf: A node that does not have any children
### Height: The number of edges from root to the furthest leaf.


## How

### Traversals
### **Depth First** Prioritizes going through the height of the tree first. The most common way to traverse through a tree is to use recursion.

 * Pre-order root > left > right
 * In-order left > root > right
 * Post-order left > right >root
 * Pre-order Pre-order

**Pre-order :**


![img](https://camo.githubusercontent.com/5ff2f562db620315f3824fdeb39bafcc15302b5cd3c79f17aabb19afd22755c2/68747470733a2f2f636f646566656c6c6f77732e6769746875622e696f2f636f6d6d6f6e5f637572726963756c756d2f646174615f737472756374757265735f616e645f616c676f726974686d732f436f64655f3430312f636c6173732d31352f7265736f75726365732f696d616765732f446570746854726176657273616c31312e504e47)

  1. Root, A, is the output value
  2. We will then look to the left, B
  3. Look to the left of that last node which is a leaf, D. D would then get popped off
  4. We look at the next leaf, E
  5. Pop off B
  6. Back to the root of A
  7. Look at C
  8. Look to the F
  9. Pop off F
  10. Pop off C
  11. Back to the root of A

**Breadth First** Iterates through the tree going through each level of the tree node by node. Traversal uses a queue.

  1. Root, A, is in the queue and needs to be dequeued.
  2. Enqueue left, B, and right, C, child.
  3. You then dequeue the front nodes (B then C).
  4. Continue the enqueue and dequeue process on with the leafs

#### Want To Know More ? 
[Trees](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/Trees.html)



  ## General summaries of what I learned this week :

  **FIFO Queue**

The first-in-first-out (FIFO) queue is the type of AWS SQS queue that guarantees order and provides exactly once delivery of messages. That sounds great, but there are some other important features to understand to avoid unexpected queue behaviour.

**Pub/Sub**

The Publish/Subscribe pattern, also known as pub/sub, is an architectural design pattern that provides a framework for exchanging messages between publishers and subscribers. This pattern involves the publisher and the subscriber relying on a message broker that relays messages from the publisher to the subscribers.

**Socket**

A socket is one endpoint of a two-way communication link between two programs running on the network. A socket is bound to a port number so that the TCP layer can identify the application that data is destined to be sent to.

**Web Socket**

WebSocket is the communication Protocol that provides bidirectional communication between the Client and the Server over a TCP connection; WebSocket remains open all the time, so they allow real-time data transfer.

**Socket.io**

 Library that enables real-time and full-duplex communication between the Client and the Web servers. 

**Client**

It is the library that runs inside the browser(Accesses services or functionality from server)

**Server**

It is the library for Node.js(Provides services and functionality for clients).

**OSI Model**

Open Systems Interconnection Model is a conceptual framework used to describe the functions of a networking system. The OSI model characterizes computing functions into a universal set of rules and requirements in order to support interoperability between different products and software.

**TCP Model**

Specifications for translating the network addressing methods used in the Internet Protocol to link-layer addresses, such as media access control (MAC) addresses.

**TCP**

Transmission control protocol. TCP provides reliable, ordered, and error-checked delivery of a stream of octets (bytes) between applications running on hosts communicating via an IP network. 

**UDP**

(User Datagram Protocol) is a communications protocol that is primarily used for establishing low-latency and loss-tolerating connections between applications on the internet.

**Packets**

A formatted unit of data carried by a packet-switched network. A packet consists of control information and user data; the latter is also known as the payload. 

**Observer Pattern**

The Observer pattern offers a subscription model in which objects subscribe to an event and get notified when the event occurs. This pattern is the cornerstone of event driven programming, including JavaScript. 

The Observer pattern facilitates good object-oriented design and promotes loose coupling.

**Listener**

An event listener is a procedure in JavaScript that waits for an event to occur. The simple example of an event is a user clicking the mouse or pressing a key on the keyboard.

**Event Handler**

Event handlers are the JavaScript code that invokes a specific piece of code when a particular action happens on an HTML element. The event handler can either invoke the direct JavaScript code or a function.

**Event Driven Programming**

JavaScript in the browser uses an event-driven programming model. Everything starts by following an event. The event could be the DOM is loaded, or an asynchronous request that finishes fetching, or a user clicking an element or scrolling the page, or the user types on the keyboard.

**Event Loop**

The event loop is the secret behind JavaScript's asynchronous programming. JS executes all operations on a single thread, but using a few smart data structures, it gives us the illusion of multi-threading.

**Event Queue**

The event queue is responsible for sending new functions to the track for processing. It follows the queue data structure to maintain the correct sequence in which all operations should be sent for execution. Whenever an async function is called, it is sent to a browser API. These are APIs built into the browser.

**Call Stack**

The call stack is used by JavaScript to keep track of multiple function calls. It is like a real stack in data structures where data can be pushed and popped and follows the Last In First Out (LIFO) principle. We use call stack for memorizing which function is running right now.

**Emit/Raise/Trigger**

The emit method (the publish method), on the other hand, allows you to "emit" an event, which causes all callbacks registered to the event to 'fire', (get called). Short: Emit's job is to trigger named event(s) which in turn cause functions called listeners to be called.


**Subscribe**

What is subscribe in JavaScript?
This is the function that is executed when a consumer calls the subscribe() method. ... To execute the observable you have created and begin receiving notifications, you call its subscribe() method, passing an observer. This is a JavaScript object that defines the handlers for the notifications you receive.

**database**

js is a javascript SQL database. It allows you to create a relational database and query it entirely in the browser. js can be used like any traditional JavaScript library. If you are building a native application in JavaScript (using Electron for instance), or are working in node.

**Authorization**
Authorization is the process of giving someone the ability to access a resource.

**Role Based Access Control**
Approach to restricting system access to authorized users.

**Capabilities**
The process the user is allowed to have access on based on his role.


