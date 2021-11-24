# Code 401 Class 18 Reading notes:

## AWS: Events


## Review, Research, and Discussion


### Describe the similarities between AWS API Gateway + Lambda functions and an ExpressJS Server

They are both ways you can implement an API. Within an Express Server you define your routes and write the logic for them. With AWS API Gateway, you set up your routes and then implement the functionality using lamda functions

### List the AWS Database offerings and talk about the pros and cons of each

They are each comparable to different db services. RDS is similar to oracle SQL, DynamoDB is similar to MongoDB, Aurora is MySQL, postrgeSQL compatible, etc.


**Pros**: They are scalable, managed, secure, easy to work with, and scalable


**Cons**: The only major con I can see is the cost.

**AWS Database offerings**

- AWS database offerings include:

- RDS

- DynamoDB

- ElastiCache

- Neptune

- Amazon QLDB

- Amazon DocumentDB

- Amazon Keyspaces

- Amazon Timestream

### What’s the difference between a FIFO and a standard queue?

A FIFO queue is first in first out and a standard queue provides at least once delivery and isn’t neccessarily ordered.


### How can the server be assured a message was properly received?

Logging and using timestamps and checking whether it was delivered based on the response sent from the endpoint.


## Document the following Vocabulary Terms

**Serverless API**

An API that lives in the cloud and is created using cloud services.

**Triggers**

Essentially a connection between resources. When something happens to a resource, it triggers an action to be taken.

**Dynamo vs Mongo**

Dynamo is like the AWS version of Mongo. Mongo is open source and uses JSON objects, whereas Dynamo uses tables. MongoDB is less restrictive of data types and size.

**Dynamoose vs Mongoose**

Dynamoose is a modeling tool used for dynamo and mongoose is used for mongo.

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

A real-time chatroom or messaging queue with login logout authorization system, with different chatting channels.



## Preparation Materials

### SQS and SNS
![](https://miro.medium.com/max/875/1*DRrTtdyah9NHwR0VCm6MWA.png)

SQS and SNS are important components for scalable, large scale, distributed, cloud-based applications:

**SNS**

(Simple Notification Service)
 is a distributed publish-subscribe service.

![SNS](https://miro.medium.com/max/628/1*mdUPKzrfJFuXa4d43KhKUQ.png)

Amazon SNS is a fast, flexible, fully managed push notification service that lets you send individual messages or to bulk messages to large numbers of recipients. Amazon SNS makes it simple and cost effective to send push notifications to mobile device users, email recipients or even send messages to other distributed services.

**SQS**
(Simple Queue Service)
is distributed queuing service.

![SQS](https://miro.medium.com/max/875/1*7eL3udb6Cto4I9Ly1sN8oA.jpeg)

Amazon SQS is a fully managed message queuing service that enables you to decouple and scale microservices, distributed systems, and serverless applications.
SQS is distributed queuing system. Messages are not pushed to receivers. Receivers have to poll SQS to receive messages. Messages can be stored in SQS for short duration of time (max 14 days).


### AWS — Difference between SNS and SQS

**Entity Type**


SQS : Queue (similar to JMS, MSMQ).
SNS : Topic-Subscriber (Pub/Sub system).



**Message consumption**


- SQS : Pull Mechanism — Consumers poll messages from SQS.

- SNS : Push Mechanism — SNS pushes messages to consumers.


**Persistence**


- SQS : Messages are persisted for some duration is no consumer available. The retention period value is from 1 minute to 14 days. The default is 4 days.

- SNS : No persistence. Whichever consumer is present at the time of message arrival, get the message and the message is deleted. If no consumers available then the message is lost.
In SQS the message delivery is guaranteed but in SNS it is not.

**Consumer Type**


- SQS : All the consumers are supposed to be identical and hence process the messages in exact same way.

- SNS : All the consumers are (supposed to be) processing the messages in different ways.


#### Want To Know More ? 

[SQS and SNS Basics](https://www.youtube.com/watch?v=UesxWuZMZqI) 

[AWS SQS vs SNS](https://medium.com/awesome-cloud/aws-difference-between-sqs-and-sns-61a397bf76c5)

[SNS Javascript SDK](https://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/SNS.html)

[SQS Javascript SDK](https://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/SQS.html)