# Code 401 Class 13 Reading notes:

## Message Queues


## Review, Research, and Discussion

### What does it mean that web sockets are bidirectional? Why is this useful?

- It means communication flows both ways between a server and client.

- This is useful because a conversation can be kept going between a server and client.

- It enables the server to send real-time updates asynchronously, without requiring the client to submit a request each time. In the context of networked AV and control systems, this allows devices to send and receive continuous streams of data to and from any point on the network.

### Does socket.io use HTTP? Why?

A socket.io server will attach to an HTTP server so it can serve its own client code through /socket.io/socket.io.js to communication with clients.

### What happens when a client emits an event?

The client emits an event and then the server handles the event using the on method.it would go the event handler.

### What happens when a server emits an event?

Server emits the event and it is handled by the client side(The server emits an event and then the client that the event was emitted to handles the event.)

### What happens if a client “misses” an event?

Unhandled messages are just ignored. It's just like when an event occurs and there are no event listeners for that event. The socket receives the msg and doesn't find a handler for it so nothing happens with it (Nothing. The event will be ignored if it is missed.)

### How can we mitigate this?

We could assign unique IDs to events in order to track them, log events, and make sure the client recieved the event.(You could avoid missing messages by always having the handlers installed and then deciding in the handlers (based on other state) whether to do anything with the message or not.)

## Document the following Vocabulary Terms

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

## Preview

### Which 3 things had you heard about previously and now have better clarity on?
- Emitting Events. 
- Socket.io
- Jest

### Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

- TCP
- OSI model
- web sockets

### What are you most excited about trying to implement or see how it works?
A real-time chatroom or messaging queue with loginlogout autherization system.



#### Want To Know More ? 
[Socket.io Chat Example](https://canvas.instructure.com/courses/3671271/discussion_topics/12904444)

[Socket.io Emit Cheatsheet](https://socket.io/docs/v4/emit-cheatsheet)