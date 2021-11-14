# Code 401 Class 12 Reading notes:

## Review, Research, and Discussion


### What is the benefit of transforming data into packets?

Packets are intended to transfer data reliably and efficiently. Instead of transferring a large file as a single block of data, sending smaller packets helps ensure each section is transmitted successfully.

### UDP is often refereed to as a connectionless protocol. Why is this?

No connection needs to be established between the source and destination before you transmit data.

### Can a socket server application have multiple socket connections?

By default, a single server can handle 65,536 socket connections, but we can definitely say that number of WebSocket connections is also limited.

### Can a socket connection application be connected to multiple socket servers?

You can only have one application listening on the same port at one time. Now if you had 2 network cards.

### Can an application be both a socket server and a socket connection?

However, if you want to use a client socket and a server socket within a single application, then yes! You can do that if you're willing to use two different ports. Or if the sockets won't be using the same port at the same time.

## Document the following Vocabulary Terms

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

## Preview

### Which 3 things had you heard about previously and now have better clarity on?
- Emitting Events. 
- Authorization
- Jest
### Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
- Socket-io
- EDA
- AWS
### What are you most excited about trying to implement or see how it works?

Authorising user to access certain data only after signing in, allowing user to change/password, then allow for inserting real data to events to track delivering an order.

## Preparation Materials

### Websocket 

- **WebSocket** is a computer communications protocol, providing full-duplex communication channels over a single TCP connection. 

- **WebSocket** remains open all the time, so they allow real-time data transfer. 
When clients trigger the request to the server, it does not close the connection on receiving the response; it rather persists and waits for the Client or server to terminate the request.

### Socket.IO?

Is a library that enables real-time and full-duplex communication between the Client and the Web servers. It uses the WebSocket protocol to provide the interface. Generally, it is divided into two parts .

- Client-Side : it is the library that runs inside the browser.

- Server Side : It is the library for Node.js.

### Key features of Socket.IO
It helps in broadcasting to multiple sockets at a time and handles the connection transparently.

It works on all platform, server or device, ensuring equality, reliability, and speed.

### Difference Between WebSocket and Socket.io


- WebSocket provides the Connection over TCP, while Socket.io is a library to abstract the WebSocket connections. 

- WebSocket doesn't have fallback options, while Socket.io supports fallback. 

- WebSocket is the technology, while Socket.io is a library for WebSockets.



#### Want To Know More ? 
[WebSocket](https://en.wikipedia.org/wiki/WebSocket)

[Websocket vs Socket-io](https://www.educba.com/websocket-vs-socket-io/)