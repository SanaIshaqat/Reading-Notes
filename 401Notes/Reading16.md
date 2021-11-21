# Code 401 Class 16 Reading notes:

## AWS: Cloud Servers


## Review, Research, and Discussion

### Describe the Web-Request-Response-Cycle
The request/response cycle traces how a user's request flows through the app.

1. A user opens his browser, types in a URL, and presses Enter.
2. When a user presses Enter, the browser makes a request for that URL.
3. The request hits the Rails router (config/routes.rb). The router maps the URL to the correct controller and action to handle the request.
4. The action receives the request and passes it on to the view.
5. The view renders the page as HTML.
6. The controller sends the HTML back to the browser. The page loads and the user sees it.

### Explain what a “server” is, as it relates to the WRRC

A client is a piece of computer hardware or software that accesses a service made available by a **server**. Generally, clients are web browsers (like Chrome or Firefox), but clients can also be API’s making requests to another **server** or the command line (when making cURL requests).

### What does it mean to “deploy” an application?

- The Software Deployment Process Defined
Software deployment refers to the process of running an application on a server or device. 

- Software deployment refers to the process of making the application work on a target device, whether it be a test server, production environment or a user's computer or mobile device.

## Document the following Vocabulary Terms

**Server**
In computing, a server is a piece of computer hardware or software (computer program) that provides functionality for other programs or devices, called "clients".

**Pub/Sub**

Pub/Sub, which stands for Publisher/Subscriber, allows services to communicate asynchronously, with latencies on the order of 100 milliseconds.

**WRRC**
Web-Request-Response-Cycle

- The request/response cycle traces how a user's request flows through the app.

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

### Virtual Machines

A virtual machine, commonly shortened to just VM, is no different than any other physical computer like a laptop, smart phone, or server. It has a CPU, memory, disks to store your files, and can connect to the internet if needed.

### AWS EC2

- Amazon Elastic Compute Cloud (Amazon EC2) provides scalable computing capacity in the Amazon Web Services (AWS) Cloud.

- You can use Amazon EC2 to launch as many or as few virtual servers as you need, configure security and networking, and manage storage.

### Elastic Beanstalk

What is Elastic Beanstalk used for?
AWS Elastic Beanstalk is an easy-to-use service for deploying and scaling web applications and services developed with Java, . NET, PHP, Node. js, Python, Ruby, Go, and Docker on familiar servers such as Apache, Nginx, Passenger, and IIS.


#### Want To Know More ? 
[Virtual Machines](https://www.youtube.com/watch?v=yIVXjl4SwVo) 

[VMS and the Cloud ](https://www.youtube.com/watch?v=l0DfHUWMjsU)

[AWS EC2](https://aws.amazon.com/ec2/?ec2-whats-new.sort-by=item.additionalFields.postDateTime&ec2-whats-new.sort-order=desc)

[EC2 For Humans](https://www.youtube.com/watch?v=lZMkgOMYYIg)

[Elastic Beanstalk](https://www.youtube.com/watch?v=SrwxAScdyT0)