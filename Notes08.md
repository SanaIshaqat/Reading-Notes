# Code 301 Class 08 Reading notes:


## API Design Best Practices



### What does REST stand for?
Representational State Transfer
### REST APIs are designed around a 
REST APIs are designed around resources, which are any kind of object, data, or service that can be accessed by the client.

### What is an identifer of a resource? Give an example.

A resource has an identifier, which is a URI that uniquely identifies that resource. For example, the URI for a particular customer order might be:

HTTP

Copy
https://adventure-works.com/orders/1

### What are the most common HTTP verbs?
The most common operations are GET, POST, PUT, PATCH, and DELETE.
### What should the URIs be based on?

 Resource URIs should be based on nouns (the resource) and not verbs (the operations on the resource).

### Give an example of a good URI.
Adopt a consistent naming convention in URIs. In general, it helps to use plural nouns for URIs that reference collections. It's a good practice to organize URIs for collections and items into a hierarchy. For example, **/customers** is the path to the customers collection, and **/customers/5** is the path to the customer with **ID** equal to **5**. This approach helps to keep the web API intuitive. Also, many web API frameworks can route requests based on parameterized URI paths, so you could define a route for the path **/customers/{id}**.

### What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?

The more requests, the bigger the load. Which makes  **"chatty"** web APIs that expose a large number of small resources. Such an API may require a client application to send multiple requests to find all of the data that it requires. Instead, you might want to denormalize the data and combine related information into bigger resources that can be retrieved with a single request.

### What status code does a successful GET request return?
A successful GET method typically returns HTTP status code 200 (OK). 
### What status code does an unsuccessful GET request return?
If the resource cannot be found, the method should return 404 (Not Found).

### What status code does a successful POST request return?
If a POST method creates a new resource, it returns HTTP status code 201 (Created). The URI of the new resource is included in the Location header of the response. The response body contains a representation of the resource.
### What status code does a successful DELETE request return?

If the delete operation is successful, the web server should respond with HTTP status code 204 (No Content), indicating that the process has been successfully handled, but that the response body contains no further information. If the resource doesn't exist, the web server can return HTTP 404 (Not Found).










## Things I want to know more about
How RegExr works  

#### Want To Know More ? 

[REST](https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design#what-is-rest)
