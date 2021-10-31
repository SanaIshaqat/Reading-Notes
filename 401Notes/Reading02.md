# Code 401 Class 02 Reading notes:

## What’s the difference between PUT and PATCH?

- The main difference between the PUT and PATCH method is that the PUT method uses the request URI to supply a modified version of the requested resource which replaces the original version of the resource, whereas the PATCH method supplies a set of instructions to modify the resource.

- Unlike PUT, PATCH applies a partial update to the resource.


## Provide links to 3 services or tools that allow you to “mock” an API for development like json-server

1. https://www.npmjs.com/package/mockserver
2. https://www.mockable.io/
3. https://stoplight.io/mocking/

## Compare and contrast Swagger and APIDoc.js ?
**apiDocjs:** Inline Documentation for RESTful web APIs. It creates a documentation from API annotations in your source code. It includes a default template which uses handlebars, Bootstrap, RequireJS and jQuery for the output of the generated apidata.js and apiproject.js as a html-page.

 **Swagger Inspector**: Test and Document Your APIs With Ease. It is a free cloud-based API testing and documentation tool to simplify the validation of any API and generate its corresponding OpenAPI documentation.

*apiDocjs and Swagger Inspector can be primarily classified as "API" tools.*

## Which HTTP status codes should be sent with each type of (un)successful API call?

Client error responses (400–499)
Server error responses (500–599)
## Compare and contrast SOAP and ReST
The difference is: **SOAP** is a XML-based message protocol, while REST is an architectural style. SOAP uses WSDL for communication between consumer and provider, whereas **REST** just uses XML or JSON to send and receive data. **SOAP** invokes services by calling RPC method, **REST** just simply calls services via URL path.

## Document the following Vocabulary Terms


### Web Server:
A web server is software and hardware that uses HTTP (Hypertext Transfer Protocol) and other protocols to respond to client requests made over the World Wide Web.
### Express:
Express is a minimal and flexible Node.js web application framework that provides a robust set of features for web and mobile applications.
### Routing:
Routing refers to how an application's endpoints (URIs) respond to client requests.
### WRRC
Web Request Response Cycle.

## Preview


### Which 3 things had you heard about previously and now have better clarity on?
- NodeJs and how it's single threaded.
- What is NPM Exactly as well as details about express.
- Summary of WRRC and MiddleWare
### Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
- CI/CD
- Jest
- TDD
### What are you most excited about trying to implement or see how it works?
Implementing a proper testing unit for a realistic logical, complete project that makes sense, to see the full picture.



#### Want To Know More ? 
- [W3Schools](https://www.w3schools.com/js/)
- [Google](https://www.google.com)