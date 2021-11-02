
# Code 401 Class 03 Reading notes:
## Review, Research, and Discussion

### Name 3 real world use cases where you’d want to change the request with custom middleware

### True or false: The route handler is middleware?

‏They are not middleware functions by definition. If such function is used on routing methods then they are only handler functions. We use such a handler function which is not a middleware when it is the only one callback function.

### In what ways can a middleware function end the process and send data to the browser?

If the current middleware function does not end the request-response cycle, it must call next() to pass control to the next middleware function. Otherwise, the request will be left hanging.


### At what point in the request lifecycle can you “inject” middleware?

Session Provider
If one of the middleware has instructed the request object to redirect, the view that is ready to execute, will not execute.
For example, if the user is planned on going to the dashboard view, but middleware has told the request to redirect to the login page instead then the dashboard view, and therefore the controller, will not execute at all. It will be skipped over. Masonite checks if the request is redirecting before executing a view.
Also, the request object can be injected into middleware by passing the Request parameter into the constructor.

### What can cause express to error with “Request headers sent twice, cannot start a second response”

The error happens in this workflow:
1.- nunjucks render template and send.
2.- if any async errors happends latter express tries to render the error template and send (here is the error)

### Document the following Vocabulary Terms

**Middleware:** 

middleware is basically a piece of code that may be used to process a request. Middleware functions are usually chained together and it’s up to them to decide whether to invoke the next one in the chain.

**Request Object:** 

The req object represents the HTTP request and has properties for the request query string, parameters, body, HTTP headers, and so on.

**Response Object:** 
The res object represents the HTTP response that an Express app sends when it gets an HTTP request.

**Application Middleware:**  
Middleware is software that lies between an operating system and the applications running on it. 

**Routing Middleware:**

 Routing defines the way in which the client requests are handled by the application endpoints. And when you make some routers in separate file, you can use them by using middleware.


**Test Driven Development:**
 Test-driven development” refers to a style of programming in which three activities are tightly 
 interwoven: coding, testing (in the form of writing unit tests) and design (in the form of refactoring)

**Behavioral Testing:**
Unit testing is a methodology where units of code are tested in isolation from the rest of the application. A unit test might test a particular function, object, class, or module. 

### Which 3 things had you heard about previously and now have better clarity on?
Express framework 
Dev-dependencies 
Errors handlers 

### Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
Jest 
Express routing 
TDD


### What are you most excited about trying to implement or see how it works?
 Complete testing of all features of a backend project .