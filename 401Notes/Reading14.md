# Code 401 Class 14 Reading notes:

## Event Driven Architecture

## Review, Research, and Discussion


### What’s the difference between a FIFO and a standard queue?

**Standard queues** guarantee that a message is delivered at least once and duplicates can be introduced into the queue. 
**FIFO** queues ensure a message is delivered exactly once and remains available until a consumer processes and deletes it; duplicates are not introduced into the queue.

### How can the server be assured a message was properly received?

By adding a message queue into our server that will be listening to received event for example from the client side, and when that event emitted from the client it will delete the request from the queue in the server.

Message Queues are so useful to store the data and make sure nothing is lost in case any other server went down.

### What classic design pattern is best represented by event driven programming?

Behavioral (Observer) design pattern.

An Event-Driven Architecture for data and applications is a modern design approach centered around data that describes “events” (i.e., something that just happened). Examples of events include the taking of a measurement, the pressing of a button, or the swiping of a credit card.

### How do you test an event driven system?

Start the application under test. Send some input events to the server. in the server try to console log each event data. Wait until the application has listened to the events been send. Assert that the data is logged and as you want.

## Document the following Vocabulary Terms

**FIFO Queue**

The first-in-first-out (FIFO) queue is the type of AWS SQS queue that guarantees order and provides exactly once delivery of messages. That sounds great, but there are some other important features to understand to avoid unexpected queue behaviour.

**Pub/Sub**

The Publish/Subscribe pattern, also known as pub/sub, is an architectural design pattern that provides a framework for exchanging messages between publishers and subscribers. This pattern involves the publisher and the subscriber relying on a message broker that relays messages from the publisher to the subscribers.

## Preview

### Which 3 things had you heard about previously and now have better clarity on?
- Emitting Events. 
- Socket.io
- Jwt

### Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

- TCP
- OSI model
- AWS

### What are you most excited about trying to implement or see how it works?
A real-time chatroom or messaging queue with login logout authorization system.


## Preparation Materials

### SNS vs SQS

**SNS** is a distributed publish-subscribe service.

**SQS** is distributed queuing service.

- You can have **SNS** send messages to email, sms or http end point apart from SQS. 

- There are advantages to coupling **SNS** with **SQS**. You may not want an external service to make connections to your hosts (firewall may block all incoming connections to your host from outside).

- **SNS** is a fast, flexible, fully managed push notification service that lets you send individual messages or to bulk messages to large numbers of recipients.


#### Want To Know More ? 
[AWS SNS and SQS](https://www.youtube.com/watch?v=mXk0MNjlO7A)
