# Code 401 Class 18 Reading notes:


# AWS: API, Dynamo and Lambda

## Review, Research, and Discussion

### What are serverless functions?

Single-purpose, programmatic functions that are hosted on managed infrastructure. These functions, which are invoked through the Internet, are hosted and maintained by cloud computing companies.

### If you were to create a system that emulated Lambda functions, how would you do it?

You can use serverless functions or you could create a CL tool to locally run and remotely deploy your node.js applications.

### Describe how a CDN works

- CDNs work through servers nearest to the website visitor respond to the request. The content delivery network copies the pages of a website to a network of servers that are spread out at geographically different locations, caching the contents of the page.

- When a user requests a webpage that is part of a content delivery network, the CDN will redirect the request from the originating site’s server to a server in the CDN that is closest to the user and deliver the cached content.


## Document the following Vocabulary Terms

**Serverless Functions**

- Single-purpose, programmatic functions that are hosted on managed infrastructure. 

- These functions, which are invoked through the Internet, are hosted and maintained by cloud computing companies. 

**Cloud Storage**

Cloud storage is a cloud computing model that stores data on the Internet through a cloud computing provider who manages and operates data storage as a service.

**CDN**

- Content Delivery Network
A content delivery network (CDN) is a group of geographically distributed servers that speed up the delivery of web content by bringing it closer to where users are.

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



### AWS API Gateway

#### What is the AWS API gateway?

- Amazon API Gateway is a fully managed service that makes it easy for developers to create, publish, maintain, monitor, and secure APIs at any scale. 

- Using API Gateway, you can create RESTful APIs and WebSocket APIs that enable real-time two-way communication applications.

#### Why do we need AWS API gateway?

API Gateway provides WebSocket API management functionality such as the following: Monitoring and throttling of connections and messages.

### AWS DynamoDB

**DynamoDB** is an Amazon Web Services database system that supports data structures and key-valued cloud services. It allows users the benefit of auto-scaling, in-memory caching, backup and restore options for all their internet-scale applications using DynamoDB.

### Dynamoose

**Dynamoose** is a modeling tool for Amazon's DynamoDB. Dynamoose is heavily inspired by Mongoose, which means if you are coming from Mongoose the syntax will be very familar.

#### Want To Know More ? 

[AWS API Gateway](https://aws.amazon.com/api-gateway/) 

[AWS DynamoDB](https://aws.amazon.com/dynamodb/)

[Dynamoose](https://dynamoosejs.com/getting_started/Introduction/)

