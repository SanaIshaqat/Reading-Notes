# Code 401 Class 06 Reading notes:

## Review, Research, and Discussion

### Explain what a “Singleton” is (in Computer Science terms)

A singleton is a class that allows only a single instance of itself to be created and gives access to that created instance. It contains static variables that can accommodate unique and private instances of itself.

### Explain how the Singleton pattern can be used with Node modules, specifically with classes
A singleton represents a single instance of an object. Only one can be created, no matter how many times the object is instantiated. If there's already an instance, the singleton will create a new one.
### What is Singleton Pattern?
Singleton pattern is a design pattern that allows us to use a single instance of a class everywhere.


### Example:
class MyClass {
  ...
}

const Singleton = (function () {
  var instance;

  function createInstance() {
    var classObj = new MyClass();
    return classObj;
  }

  return {
    getInstance: function () {
        if (!instance) {
            instance = createInstance();
        }
        return instance;
    },
  };
})();

module.exports = Singleton;

The Singleton object is implemented as an IIFE.

An IIFE (Immediately Invoked Function Expression) is a JavaScript function that runs as soon as it is defined.

The createInstance function is responsible for creating the instance of MyClass.

The getInstance method will be invoked via the Singleton object. If the instance of MyClass is not present it will be created and returned, if already present it will return directly without creating a new instance.

So this pattern allows us to access and manipulate the members of a class instance from any file or function.

### If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?

Requirements to Write Express Middleware
There are a few things you will need installed to create, use, and test Express middleware. First, you will need Node and NPM. To ensure you have them installed, you can run:

- npm -v && node -v

- Create a new project and npm init
- Create server.js 
- Run the server via node server.js, access http://localhost:3000, and you should see “Welcome Home” printed in your browser.

The app.get() function is Application-level Middleware. You’ll notice the parameters passed to the method are req, res, and next. These are the incoming request, the response being written, and a method to call to pass the call to the next middleware function once the current middleware is finished. In this case, once the response is sent, the function exits. You could also chain other middleware here by calling the next() method.

Let’s take a look at a few more examples of the different types of middleware.
### Document the following Vocabulary Terms

**Router Middleware**
The term is composed of 2 words router and middleware. Middleware. It is a piece of code that comes in the middle of request and response . It kind of hijacks your request so that you can do anything that you want with your request or response eg: Modify the data or call the next middleware.
**Dynamic Module Loading**
Dynamic loading is a mechanism by which a computer program can, at run time, load a library (or other binary) into memory, retrieve the addresses of functions and variables contained in the library, execute those functions or access those variables, and unload the library from memory.
**Singleton Pattern**
Use the Singleton pattern when a class in your program should have just a single instance available to all clients; for example, a single database object shared by different parts of the program. The Singleton pattern disables all other means of creating objects of a class except for the special creation method.
**CRUD -> REST Method Matches**
Which GET HTTP method is equivalent to which the CRUD operation?
HTTP GET - SELECT/Request. HTTP PUT - UPDATE. HTTP POST - INSERT/Create. HTTP DELETE - DELETE.
**Mock Testing**
Mocking is done when you invoke methods of a class that has external communication like database calls or rest calls. Through mocking you can explicitly define the return value of methods without actually executing the steps of the method.

## Preview

### Which 3 things had you heard about previously and now have better clarity on?
- CRUD/REST Methods
- Mocking 
- postgresql

### Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
- Data Structuring
- sequelize 
- creating nodes.
### What are you most excited about trying to implement or see how it works?
A project that combines most/all concepts we learned, to see how everything is connect in the full picture.

## Preparation Materials

### Securing Passwords
Cryptographic hash algorithms MD5, SHA1, SHA256, SHA512, SHA-3 are general purpose hash functions, designed to calculate a digest of huge amounts of data in as short a time as possible. Hashing is the greatest way for protecting passwords and considered to be pretty safe for ensuring the integrity of data or password. 

### Basic Auth
In the context of an HTTP transaction, basic access authentication is a method for an HTTP user agent (e.g. a web browser) to provide a user name and password when making a request

### bcrypt docs
A library to help you hash passwords.
#### Want To Know More ? 
- [Securing Passwords](https://thehackernews.com/2014/04/securing-passwords-with-bcrypt-hashing.html)
- [Basic Auth](https://en.wikipedia.org/wiki/Basic_access_authentication)
- [OWASP auth cheatsheet](https://cheatsheetseries.owasp.org/cheatsheets/Authentication_Cheat_Sheet.html)
- [bcrypt docs](https://www.npmjs.com/package/bcrypt)