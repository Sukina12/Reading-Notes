# Class 03 Summary :

### Name 3 real world use cases where you’d want to change the request with custom middleware :
1. parameters validation.
2. Authentication
3. Error Handling

### True or false: The route handler is middleware? :

* false, middleware used to change the shape of the request and response . the route handler can take the request and get the response without middleware.

### In what ways can a middleware function end the process and send data to the browser?

* send the data to the browser using next() function , and end the process by get an error such as 500 error and send the error message.

### At what point in the request lifecycle can you “inject” middleware?

* Access to the request object, the answer object and the next function for the middleware. The request is applied when the server receives the request.

### What can cause express to error with “Request headers sent twice, cannot start a second response” ?

* This happens when you have more than one response being sent to your client.


### Document the following Vocabulary Terms :

| Term      |                                                          |
| -----------  | ----------------------------------------------------------------|
| Middleware   |  is a type of computer software that provides services to software applications beyond those available from the operating system.  |
| Request Object    |   the main entry point for an application to issue a request to the Library - all operations on a URL must use a Request object. The request object is application independent in that both servers and clients use the same Request class.  |
| Response Object     |    It is the object which communicates between the server and the output which is sent to the client.    |
| Application Middleware    |  a middleware that is bound to an instance of express, using app.use() and app.VERB(). |
| Routing Middleware    |     a middleware that bound to an instance of express.Router().   |
| TDD    |   a style of programming in  three activities: coding, testing (in the form of writing unit tests) and design (in the form of refactoring)       |
| Behavioral Testing    |   a testing of the external behaviour of the program, also known as black box testing. It is usually a functional testing.    |


### ES6 Classes :

* "Classes are a template for creating objects. They encapsulate data with code to work on that data. Classes in JS are built on prototypes but also have some syntax and semantics that are not shared with ES5 class-like semantics".

* "Classes are in fact "special functions", and just as you can define function expressions and function declarations, the class syntax has two components: class expressions and class declarations".

### Using Express Routing :

* "define routing using methods of the Express app object that correspond to HTTP methods; for example, app.get() to handle GET requests and app.post to handle POST requests. For a full list, see app.METHOD. You can also use app.all() to handle all HTTP methods and app.use() to specify middleware as the callback function"

### Express Routing :

* "Routing refers to determining how an application responds to a client request to a particular endpoint, which is a URI (or path) and a specific HTTP request method (GET, POST, and so on)".

* "outing methods specify a callback function (sometimes called “handler functions”) called when the application receives a request to the specified route (endpoint) and HTTP method. In other words, the application “listens” for requests that match the specified route(s) and method(s), and when it detects a match, it calls the specified callback function".

### Sources:

[source1](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes)
[source2](https://expressjs.com/en/guide/routing.html)
[source3](https://expressjs.com/en/starter/basic-routing.html)

